# Comparing `tmp/gundi_client-0.2.2.tar.gz` & `tmp/gundi_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_client-0.2.2.tar", max compression
+gzip compressed data, was "gundi_client-1.0.0.tar", max compression
```

## Comparing `gundi_client-0.2.2.tar` & `gundi_client-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      895 2023-02-07 15:42:42.967307 gundi_client-0.2.2/README.md
--rw-r--r--   0        0        0       30 2023-02-07 15:29:11.456509 gundi_client-0.2.2/gundi_client/__init__.py
--rw-r--r--   0        0        0     9161 2023-02-07 15:03:49.298771 gundi_client-0.2.2/gundi_client/client.py
--rw-r--r--   0        0        0    13842 2023-02-07 15:03:49.350773 gundi_client-0.2.2/gundi_client/schemas.py
--rw-r--r--   0        0        0      890 2023-02-07 15:17:02.449046 gundi_client-0.2.2/gundi_client/settings.py
--rw-r--r--   0        0        0      725 2023-02-07 15:05:12.717970 gundi_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 gundi_client-0.2.2/setup.py
--rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 gundi_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1681 2023-06-06 07:27:28.357433 gundi_client-1.0.0/README.md
+-rw-r--r--   0        0        0      358 2023-05-09 15:53:31.705675 gundi_client-1.0.0/gundi_client/.env.local
+-rw-r--r--   0        0        0       30 2023-05-24 04:47:28.211754 gundi_client-1.0.0/gundi_client/__init__.py
+-rw-r--r--   0        0        0     9887 2023-06-06 07:27:28.358366 gundi_client-1.0.0/gundi_client/client.py
+-rw-r--r--   0        0        0    13842 2023-05-24 04:47:28.212310 gundi_client-1.0.0/gundi_client/schemas.py
+-rw-r--r--   0        0        0      890 2023-05-24 04:47:28.212516 gundi_client-1.0.0/gundi_client/settings.py
+-rw-r--r--   0        0        0      560 2023-05-24 06:06:40.882965 gundi_client-1.0.0/gundi_client/test.py
+-rw-r--r--   0        0        0      767 2023-06-06 07:27:28.359914 gundi_client-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2442 1970-01-01 00:00:00.000000 gundi_client-1.0.0/PKG-INFO
```

### Comparing `gundi_client-0.2.2/README.md` & `gundi_client-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,26 +7,51 @@
 ```
 pip install gundi-client
 ```
 
 ## Usage
 
 ```
-import aiohttp
 from gundi_client import PortalApi
+import httpx
 
-async with aiohttp.ClientSession() as session:
-    try:
-        response = await portal.get_outbound_integration_list(
-            session=session, inbound_id=str(inbound_id), device_id=str(device_id)
-        )
-    except aiohttp.ServerTimeoutError as e:
-        logger.error("Read Timeout")              
+# You can use it as an async context-managed client
+async with PortalApi() as portal:
+   try:
+    response = await portal.get_outbound_integration_list(
+        session=session, inbound_id=str(inbound_id), device_id=str(device_id)
+    )
+    except httpx.RequestError as e:
+        logger.exception("Request Error")   
         ...
-    except aiohttp.ClientResponseError as e:
-        logger.exception("Failed to get outbound integrations for inbound_id")
-        ..
+    except httpx.TimeoutException as e:
+        logger.exception("Request timed out")
+        ...
+    except httpx.HTTPStatusError as e:
+        logger.exception("Response returned error")
+    else:
+        # response contains a list configs as dicts
+        for integration in response:  
+            ...
+   ...
+
+# Or create an instance and close the client explicitly later
+portal = PortalApi()
+try:
+    response = await portal.get_outbound_integration_list(
+        session=session, inbound_id=str(inbound_id), device_id=str(device_id)
+    )
+    except httpx.RequestError as e:
+        logger.exception("Request Error")   
+        ...
+    except httpx.TimeoutException as e:
+        logger.exception("Request timed out")
+        ...
+    except httpx.HTTPStatusError as e:
+        logger.exception("Response returned error")
     else:
         # response contains a list configs as dicts
         for integration in response:  
-            .. 
+            ...
+   ...
+   await portal.close()  # Close the session used to send requests to ER API
 ```
```

### Comparing `gundi_client-0.2.2/gundi_client/client.py` & `gundi_client-1.0.0/gundi_client/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,76 @@
 import logging
 from datetime import datetime, timedelta, timezone
 from typing import List, Dict, Any
 from uuid import UUID
-from aiohttp import ClientSession, ClientResponseError, ClientTimeout
 from pydantic import parse_obj_as
 from . import settings
 from .schemas import (
     IntegrationInformation,
     OAuthToken,
     TIntegrationInformation,
     DeviceState,
     OutboundConfiguration,
 )
+from httpx import (
+    AsyncClient,
+    AsyncHTTPTransport,
+    RequestError,
+    Timeout,
+    TimeoutException,
+    HTTPStatusError
+)
 
 logger = logging.getLogger(__name__)
 logger.setLevel(settings.LOG_LEVEL)
 
 
 class PortalApi:
-    def __init__(self):
-        self.client_id = settings.KEYCLOAK_CLIENT_ID
-        self.client_secret = settings.KEYCLOAK_CLIENT_SECRET
+
+    DEFAULT_CONNECT_TIMEOUT_SECONDS = 3.1
+    DEFAULT_DATA_TIMEOUT_SECONDS = 20
+    DEFAULT_CONNECTION_RETRIES = 5
+
+    def __init__(self, **kwargs):
+        self.client_id = kwargs.get("KEYCLOAK_CLIENT_ID", settings.KEYCLOAK_CLIENT_ID)
+        self.client_secret = kwargs.get("KEYCLOAK_CLIENT_SECRET", settings.KEYCLOAK_CLIENT_SECRET)
         self.integrations_endpoint = (
-            f"{settings.PORTAL_API_ENDPOINT}/integrations/inbound/configurations"
+            f'{kwargs.get("PORTAL_API_ENDPOINT", settings.PORTAL_API_ENDPOINT)}/integrations/inbound/configurations'
         )
-        self.device_states_endpoint = f"{settings.PORTAL_API_ENDPOINT}/devices/states"
-        self.devices_endpoint = f"{settings.PORTAL_API_ENDPOINT}/devices"
+        self.device_states_endpoint = f'{kwargs.get("PORTAL_API_ENDPOINT", settings.PORTAL_API_ENDPOINT)}/devices/states'
+        self.devices_endpoint = f'{kwargs.get("PORTAL_API_ENDPOINT", settings.PORTAL_API_ENDPOINT)}/devices'
 
-        self.oauth_token_url = settings.OAUTH_TOKEN_URL
-        self.audience = settings.KEYCLOAK_AUDIENCE
-        self.portal_api_endpoint = settings.PORTAL_API_ENDPOINT
+        self.oauth_token_url = kwargs.get("OAUTH_TOKEN_URL", settings.OAUTH_TOKEN_URL)
+        self.audience = kwargs.get("KEYCLOAK_AUDIENCE", settings.KEYCLOAK_AUDIENCE)
+        self.portal_api_endpoint = kwargs.get("PORTAL_API_ENDPOINT", settings.PORTAL_API_ENDPOINT)
 
         self.cached_token = None
         self.cached_token_expires_at = datetime.min.replace(tzinfo=timezone.utc)
 
-    async def get_access_token(self, session: ClientSession) -> OAuthToken:
+        self.max_retries = kwargs.get('max_http_retries', self.DEFAULT_CONNECTION_RETRIES)
+        transport = AsyncHTTPTransport(retries=self.max_retries)
+
+        connect_timeout = kwargs.get('connect_timeout', self.DEFAULT_CONNECT_TIMEOUT_SECONDS)
+        data_timeout = kwargs.get('data_timeout', self.DEFAULT_DATA_TIMEOUT_SECONDS)
+        timeout = Timeout(data_timeout, connect=connect_timeout, pool=connect_timeout)
+
+        self._session = AsyncClient(transport=transport, timeout=timeout, verify=settings.CDIP_ADMIN_SSL_VERIFY)
+
+    async def close(self):
+        await self._session.aclose()
+
+    # Support using this client as an async context manager.
+    async def __aenter__(self):
+        await self._session.__aenter__()
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        await self._session.__aexit__()
+
+    async def get_access_token(self) -> OAuthToken:
         if self.cached_token and self.cached_token_expires_at > datetime.now(
             tz=timezone.utc
         ):
             return self.cached_token
 
         logger.debug(
             f"get_access_token from {self.oauth_token_url} using client_id: {self.client_id}"
@@ -47,200 +79,195 @@
             "client_id": self.client_id,
             "client_secret": self.client_secret,
             "audience": self.audience,
             "grant_type": "urn:ietf:params:oauth:grant-type:uma-ticket",
             "scope": "openid",
         }
 
-        response = await session.post(
-            self.oauth_token_url, data=payload, ssl=settings.CDIP_ADMIN_SSL_VERIFY
+        response = await self._session.post(
+            self.oauth_token_url, data=payload
         )
 
         response.raise_for_status()
-        token = await response.json()
+        token = response.json()
         token = OAuthToken.parse_obj(token)
         self.cached_token_expires_at = datetime.now(tz=timezone.utc) + timedelta(
             seconds=token.expires_in - 15
         )  # fudge factor
         self.cached_token = token
         return token
 
-    async def get_auth_header(self, session: ClientSession) -> dict:
-        token_object = await self.get_access_token(session)
+    async def get_auth_header(self) -> dict:
+        token_object = await self.get_access_token()
         return {
             "authorization": f"{token_object.token_type} {token_object.access_token}"
         }
 
     async def get_destinations(
         self, *args, integration_id: str = None, device_id: str = None
     ):
-        async with ClientSession() as session:
-            headers = await self.get_auth_header(session)
+        headers = await self.get_auth_header()
 
-            url = f"{self.portal_api_endpoint}/integrations/outbound/configurations"
-            response = await session.get(
-                url,
-                params={"inbound_id": integration_id, "device_id": device_id},
-                headers=headers,
-            )
-
-            if response.ok:
-                data = await response.json()
+        url = f"{self.portal_api_endpoint}/integrations/outbound/configurations"
+        response = await self._session.get(
+            url,
+            params={"inbound_id": integration_id, "device_id": device_id},
+            headers=headers,
+        )
 
-                return [OutboundConfiguration.parse_obj(item) for item in data]
+        response.raise_for_status()
+        data = response.json()
 
-            return []
+        return [OutboundConfiguration.parse_obj(item) for item in data]
 
     async def get_authorized_integrations(
         self,
-        session: ClientSession,
         t_int_info: TIntegrationInformation = IntegrationInformation,
     ) -> List[IntegrationInformation]:
         logger.debug(f"get_authorized_integrations for : {settings.KEYCLOAK_CLIENT_ID}")
-        headers = await self.get_auth_header(session)
+        headers = await self.get_auth_header()
 
         logger.debug(f"url: {self.integrations_endpoint}")
-        response = await session.get(
+        response = await self._session.get(
             url=self.integrations_endpoint,
             headers=headers,
-            ssl=settings.CDIP_ADMIN_SSL_VERIFY,
         )
         response.raise_for_status()
-        json_response = await response.json()
+        json_response = response.json()
 
         if isinstance(json_response, dict):
             json_response = [json_response]
 
         logger.debug(
             f"Got {len(json_response)} integrations for {settings.KEYCLOAK_CLIENT_ID}"
         )
         return [t_int_info.parse_obj(r) for r in json_response]
 
     async def update_state(
-        self, session: ClientSession, integration_info: IntegrationInformation
+        self, integration_info: IntegrationInformation
     ):
-        async with ClientSession() as sess:
-            headers = await self.get_auth_header(sess)
+        headers = await self.get_auth_header()
 
-            response = await sess.put(
-                url=f"{self.integrations_endpoint}/{integration_info.id}",
-                headers=headers,
-                json=dict(state=integration_info.state),
-                ssl=settings.CDIP_ADMIN_SSL_VERIFY,
-            )
-            logger.info(f"update integration state resp: {response.status}")
-            response.raise_for_status()
+        response = await self._session.put(
+            url=f"{self.integrations_endpoint}/{integration_info.id}",
+            headers=headers,
+            json=dict(state=integration_info.state),
+        )
+        logger.info(f"update integration state resp: {response.json()}")
+        response.raise_for_status()
 
-            return await self.update_states_with_dict(
-                sess, integration_info.id, integration_info.device_states
-            )
+        return await self.update_states_with_dict(
+            integration_info.id, integration_info.device_states
+        )
 
-    async def fetch_device_states(self, session: ClientSession, inbound_id: UUID):
+    async def fetch_device_states(self, inbound_id: UUID):
         try:
-            headers = await self.get_auth_header(session)
+            headers = await self.get_auth_header()
 
             # This ought to be quick so just do it straight away.
-            response = await session.get(
+            response = await self._session.get(
                 url=f"{self.device_states_endpoint}/",
                 params={"inbound_config_id": str(inbound_id)},
                 headers=headers,
-                timeout=ClientTimeout(sock_connect=3.1, sock_read=10),
-                verify=settings.CDIP_ADMIN_SSL_VERIFY,
             )
-            if response.status == 200:
-                result = response.json()
-        except ClientResponseError as ex:
-            logger.exception("Failed to get devices for iic: {inbound_id}")
+            response.raise_for_status()
+            result = response.json()
+        except (RequestError, TimeoutException, HTTPStatusError):
+            logger.exception(f"Failed to get devices for iic: {inbound_id}")
         else:
             states_received = parse_obj_as(List[DeviceState], result)
             # todo: cleanup after all functions have their device state migrated over
             states_asdict = {}
             for s in states_received:
                 if isinstance(s.state, dict) and "value" in s.state:
                     states_asdict[s.device_external_id] = s.state.get("value")
                 else:
                     states_asdict[s.device_external_id] = s.state
             return states_asdict
             # return {s.device_external_id: s.state for s in states_received}
 
     async def ensure_device(
-        self, session: ClientSession, inbound_id: UUID, external_id: str
+        self, inbound_id: UUID, external_id: str
     ):
-        # Post device ID and Integration ID combination to ensure it exists
-        # in the Portal's database and is also in the Integration's default
-        # device group.
-        headers = await self.get_auth_header(session)
-        payload = {"external_id": external_id, "inbound_configuration": inbound_id}
-        response = await session.post(
-            url=self.devices_endpoint,
-            json=payload,
-            headers=headers,
-            ssl=settings.CDIP_ADMIN_SSL_VERIFY,
-        )
-        resp = await response.json()
-        # print(resp)
-        if response.ok:
+        try:
+            # Post device ID and Integration ID combination to ensure it exists
+            # in the Portal's database and is also in the Integration's default
+            # device group.
+            headers = await self.get_auth_header()
+            payload = {"external_id": external_id, "inbound_configuration": inbound_id}
+            response = await self._session.post(
+                url=self.devices_endpoint,
+                json=payload,
+                headers=headers,
+            )
+            # print(resp)
+            response.raise_for_status()
+            resp = response.json()
             return resp
-        else:
-            logger.error(
-                "Failed to post device to portal.",
-                extra={**payload, "response": str(response)},
+        except RequestError:
+            logger.exception(
+                "Failed to post device to portal (request failed).",
+                extra={**payload},
+            )
+        except TimeoutException:
+            logger.exception(
+                "Failed to post device to portal (timeout).",
+                extra={**payload},
+            )
+        except HTTPStatusError:
+            logger.exception(
+                "Failed to post device to portal (HTTP returned error).",
+                extra={**payload},
             )
 
         return None
 
     async def update_states_with_dict(
-        self, session: ClientSession, inbound_id: UUID, states_dict: Dict[str, Any]
+        self, inbound_id: UUID, states_dict: Dict[str, Any]
     ):
-        headers = await self.get_auth_header(session)
-        response = await session.post(
+        headers = await self.get_auth_header()
+        response = await self._session.post(
             url=f"{self.device_states_endpoint}/update/{inbound_id}",
             headers=headers,
             json=states_dict,
-            ssl=settings.CDIP_ADMIN_SSL_VERIFY,
         )
         response.raise_for_status()
-        text = await response.text()
-        logger.info(f"update device_states resp: {response.status}")
+        text = response.json()
+        logger.info(f"update device_states resp: {response.json()}")
         return text
 
-    async def _get(self, session: ClientSession, url: str, params=None):
-        headers = await self.get_auth_header(session)
-        response = await session.get(
+    async def _get(self, url: str, params=None):
+        headers = await self.get_auth_header()
+        response = await self._session.get(
             url=url,
             headers=headers,
             params=params,
-            ssl=settings.CDIP_ADMIN_SSL_VERIFY,
         )
         response.raise_for_status()
-        return await response.json()
+        return response.json()
 
-    async def get_bridge_integration(self, session: ClientSession, bridge_id: str):
+    async def get_bridge_integration(self, bridge_id: str):
         return await self._get(
-            session=session,
-            url=f"{settings.PORTAL_API_ENDPOINT}/integrations/bridges/{bridge_id}",
+            url=f"{self.portal_api_endpoint}/integrations/bridges/{bridge_id}",
         )
 
     async def get_inbound_integration(
-        self, session: ClientSession, integration_id: str
+        self, integration_id: str
     ):
         return await self._get(
-            session=session,
-            url=f"{settings.PORTAL_API_ENDPOINT}/integrations/inbound/configurations/{integration_id}",
+            url=f"{self.portal_api_endpoint}/integrations/inbound/configurations/{integration_id}",
         )
 
     async def get_outbound_integration(
-        self, session: ClientSession, integration_id: str
+        self, integration_id: str
     ):
         return await self._get(
-            session=session,
-            url=f"{settings.PORTAL_API_ENDPOINT}/integrations/outbound/configurations/{integration_id}",
+            url=f"{self.portal_api_endpoint}/integrations/outbound/configurations/{integration_id}",
         )
 
     async def get_outbound_integration_list(
-        self, session: ClientSession, **query_params
+        self, **query_params
     ):
         return await self._get(
-            session=session,
-            url=f"{settings.PORTAL_API_ENDPOINT}/integrations/outbound/configurations",
+            url=f"{self.portal_api_endpoint}/integrations/outbound/configurations",
             params=query_params,
         )
```

### Comparing `gundi_client-0.2.2/gundi_client/schemas.py` & `gundi_client-1.0.0/gundi_client/schemas.py`

 * *Files identical despite different names*

### Comparing `gundi_client-0.2.2/gundi_client/settings.py` & `gundi_client-1.0.0/gundi_client/settings.py`

 * *Files identical despite different names*

