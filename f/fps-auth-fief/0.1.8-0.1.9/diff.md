# Comparing `tmp/fps_auth_fief-0.1.8.tar.gz` & `tmp/fps_auth_fief-0.1.9.tar.gz`

## Comparing `fps_auth_fief-0.1.8.tar` & `fps_auth_fief-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/fps_auth_fief/config.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/fps_auth_fief/main.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/COPYING.md
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/COPYING.md
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/PKG-INFO
```

### Comparing `fps_auth_fief-0.1.8/fps_auth_fief/backend.py` & `fps_auth_fief-0.1.9/fps_auth_fief/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,110 @@
+from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Tuple
 
 from fastapi import Depends, HTTPException, Request, Response, WebSocket, status
 from fastapi.security import APIKeyCookie
 from fief_client import FiefAccessTokenInfo, FiefAsync, FiefUserInfo
 from fief_client.integrations.fastapi import FiefAuth
 from jupyverse_api.auth import User
 
 from .config import _AuthFiefConfig
 
 
-class Backend:
-    def __init__(self, auth_fief_config: _AuthFiefConfig):
-        class CustomFiefAuth(FiefAuth):
-            client: FiefAsync
-
-            async def get_unauthorized_response(self, request: Request, response: Response):
-                redirect_uri = str(request.url_for("auth_callback"))
-                auth_url = await self.client.auth_url(redirect_uri, scope=["openid"])
-                raise HTTPException(
-                    status_code=status.HTTP_307_TEMPORARY_REDIRECT,
-                    headers={"Location": auth_url},
-                )
-
-        self.fief = FiefAsync(
-            auth_fief_config.base_url,
-            auth_fief_config.client_id,
-            auth_fief_config.client_secret,
+class CustomFiefAuth(FiefAuth):
+    client: FiefAsync
+
+    async def get_unauthorized_response(self, request: Request, response: Response):
+        redirect_uri = str(request.url_for("auth_callback"))
+        auth_url = await self.client.auth_url(redirect_uri, scope=["openid"])
+        raise HTTPException(
+            status_code=status.HTTP_307_TEMPORARY_REDIRECT,
+            headers={"Location": auth_url},
         )
 
-        self.SESSION_COOKIE_NAME = "fps_auth_fief_user_session"
-        scheme = APIKeyCookie(name=self.SESSION_COOKIE_NAME, auto_error=False)
-        self.auth = CustomFiefAuth(self.fief, scheme)
-
-        async def update_user(
-            user: FiefUserInfo = Depends(self.auth.current_user()),
-            access_token_info: FiefAccessTokenInfo = Depends(self.auth.authenticated()),
-        ):
-            async def _(data: Dict[str, Any]) -> FiefUserInfo:
-                user = await self.fief.update_profile(
-                    access_token_info["access_token"], {"fields": data}
-                )
-                return user
-
-            return _
-
-        def websocket_auth(permissions: Optional[Dict[str, List[str]]] = None):
-            async def _(
-                websocket: WebSocket,
-            ) -> Optional[Tuple[WebSocket, Optional[Dict[str, List[str]]]]]:
-                accept_websocket = False
-                checked_permissions: Optional[Dict[str, List[str]]] = None
-                if self.SESSION_COOKIE_NAME in websocket._cookies:
-                    access_token = websocket._cookies[self.SESSION_COOKIE_NAME]
-                    if permissions is None:
-                        accept_websocket = True
-                    else:
-                        checked_permissions = {}
-                        for resource, actions in permissions.items():
-                            allowed = checked_permissions[resource] = []
-                            for action in actions:
-                                try:
-                                    await self.fief.validate_access_token(
-                                        access_token, required_permissions=[f"{resource}:{action}"]
-                                    )
-                                except BaseException:
-                                    pass
-                                else:
-                                    allowed.append(action)
-                                    accept_websocket = True
-                if accept_websocket:
-                    return websocket, checked_permissions
+
+@dataclass
+class Res:
+    fief: FiefAsync
+    session_cookie_name: str
+    auth: CustomFiefAuth
+    current_user: Any
+    update_user: Any
+    websocket_auth: Any
+
+
+def get_backend(auth_fief_config: _AuthFiefConfig) -> Res:
+    fief = FiefAsync(
+        auth_fief_config.base_url,
+        auth_fief_config.client_id,
+        auth_fief_config.client_secret,
+    )
+
+    session_cookie_name = "fps_auth_fief_user_session"
+    scheme = APIKeyCookie(name=session_cookie_name, auto_error=False)
+    auth = CustomFiefAuth(fief, scheme)
+
+    async def update_user(
+        user: FiefUserInfo = Depends(auth.current_user()),
+        access_token_info: FiefAccessTokenInfo = Depends(auth.authenticated()),
+    ):
+        async def _(data: Dict[str, Any]) -> FiefUserInfo:
+            user = await fief.update_profile(access_token_info["access_token"], {"fields": data})
+            return user
+
+        return _
+
+    def websocket_auth(permissions: Optional[Dict[str, List[str]]] = None):
+        async def _(
+            websocket: WebSocket,
+        ) -> Optional[Tuple[WebSocket, Optional[Dict[str, List[str]]]]]:
+            accept_websocket = False
+            checked_permissions: Optional[Dict[str, List[str]]] = None
+            if session_cookie_name in websocket._cookies:
+                access_token = websocket._cookies[session_cookie_name]
+                if permissions is None:
+                    accept_websocket = True
                 else:
-                    await websocket.close(code=status.WS_1008_POLICY_VIOLATION)
-                    return None
+                    checked_permissions = {}
+                    for resource, actions in permissions.items():
+                        allowed = checked_permissions[resource] = []
+                        for action in actions:
+                            try:
+                                await fief.validate_access_token(
+                                    access_token, required_permissions=[f"{resource}:{action}"]
+                                )
+                            except BaseException:
+                                pass
+                            else:
+                                allowed.append(action)
+                                accept_websocket = True
+            if accept_websocket:
+                return websocket, checked_permissions
+            else:
+                await websocket.close(code=status.WS_1008_POLICY_VIOLATION)
+                return None
+
+        return _
+
+    def current_user(permissions=None):
+        if permissions is not None:
+            permissions = [
+                f"{resource}:{action}"
+                for resource, actions in permissions.items()
+                for action in actions
+            ]
+
+        async def _(
+            user: FiefUserInfo = Depends(auth.current_user(permissions=permissions)),
+        ):
+            return User(**user["fields"])
 
-            return _
+        return _
 
-        def current_user(permissions=None):
-            if permissions is not None:
-                permissions = [
-                    f"{resource}:{action}"
-                    for resource, actions in permissions.items()
-                    for action in actions
-                ]
-
-            async def _(
-                user: FiefUserInfo = Depends(self.auth.current_user(permissions=permissions)),
-            ):
-                return User(**user["fields"])
-
-            return _
-
-        self.current_user = current_user
-        self.update_user = update_user
-        self.websocket_auth = websocket_auth
+    return Res(
+        fief=fief,
+        session_cookie_name=session_cookie_name,
+        auth=auth,
+        current_user=current_user,
+        update_user=update_user,
+        websocket_auth=websocket_auth,
+    )
```

### Comparing `fps_auth_fief-0.1.8/fps_auth_fief/main.py` & `fps_auth_fief-0.1.9/fps_auth_fief/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from asphalt.core import Component, Context
 from jupyverse_api.auth import Auth, AuthConfig
 from jupyverse_api.app import App
 
 from .config import _AuthFiefConfig
-from .routes import _AuthFief
+from .routes import auth_factory
 
 
 class AuthFiefComponent(Component):
     def __init__(self, **kwargs):
         self.auth_fief_config = _AuthFiefConfig(**kwargs)
 
     async def start(
         self,
         ctx: Context,
     ) -> None:
         ctx.add_resource(self.auth_fief_config, types=AuthConfig)
 
         app = await ctx.request_resource(App)
 
-        auth_fief = _AuthFief(app, self.auth_fief_config)
+        auth_fief = auth_factory(app, self.auth_fief_config)
         ctx.add_resource(auth_fief, types=Auth)
```

### Comparing `fps_auth_fief-0.1.8/fps_auth_fief/routes.py` & `fps_auth_fief-0.1.9/fps_auth_fief/routes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,88 @@
 import json
-from typing import Dict, List
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from fastapi import APIRouter, Depends, Query, Request, Response
 from fastapi.responses import RedirectResponse
 from fief_client import FiefAccessTokenInfo
 from jupyverse_api import Router
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 
-from .backend import Backend
+from .backend import get_backend
 from .config import _AuthFiefConfig
 
 
-class _AuthFief(Backend, Auth, Router):
-    def __init__(
-        self,
-        app: App,
-        auth_fief_config: _AuthFiefConfig,
-    ) -> None:
-        Router.__init__(self, app)
-        Backend.__init__(self, auth_fief_config)
-
-        router = APIRouter()
-
-        @router.get("/auth-callback", name="auth_callback")
-        async def auth_callback(request: Request, response: Response, code: str = Query(...)):
-            redirect_uri = str(request.url_for("auth_callback"))
-            tokens, _ = await self.fief.auth_callback(code, redirect_uri)
-
-            response = RedirectResponse(request.url_for("root"))
-            response.set_cookie(
-                self.SESSION_COOKIE_NAME,
-                tokens["access_token"],
-                max_age=tokens["expires_in"],
-                httponly=True,
-                secure=False,
-            )
-
-            return response
-
-        @router.get("/api/me")
-        async def get_api_me(
-            request: Request,
-            user: User = Depends(self.current_user()),
-            access_token_info: FiefAccessTokenInfo = Depends(self.auth.authenticated()),
-        ):
-            checked_permissions: Dict[str, List[str]] = {}
-            permissions = json.loads(
-                dict(request.query_params).get("permissions", "{}").replace("'", '"')
-            )
-            if permissions:
-                user_permissions: Dict[str, List[str]] = {}
-                for permission in access_token_info["permissions"]:
-                    resource, action = permission.split(":")
-                    if resource not in user_permissions:
-                        user_permissions[resource] = []
-                    user_permissions[resource].append(action)
-                for resource, actions in permissions.items():
-                    user_resource_permissions = user_permissions.get(resource, [])
-                    allowed = checked_permissions[resource] = []
-                    for action in actions:
-                        if action in user_resource_permissions:
-                            allowed.append(action)
-
-            keys = ["username", "name", "display_name", "initials", "avatar_url", "color"]
-            identity = {k: getattr(user, k) for k in keys}
-            return {
-                "identity": identity,
-                "permissions": checked_permissions,
-            }
+def auth_factory(
+    app: App,
+    auth_fief_config: _AuthFiefConfig,
+):
+    backend = get_backend(auth_fief_config)
+
+    class _AuthFief(Auth, Router):
+        def __init__(self) -> None:
+            super().__init__(app)
+
+            router = APIRouter()
+
+            @router.get("/auth-callback", name="auth_callback")
+            async def auth_callback(request: Request, response: Response, code: str = Query(...)):
+                redirect_uri = str(request.url_for("auth_callback"))
+                tokens, _ = await backend.fief.auth_callback(code, redirect_uri)
+
+                response = RedirectResponse(request.url_for("root"))
+                response.set_cookie(
+                    backend.session_cookie_name,
+                    tokens["access_token"],
+                    max_age=tokens["expires_in"],
+                    httponly=True,
+                    secure=False,
+                )
+
+                return response
+
+            @router.get("/api/me")
+            async def get_api_me(
+                request: Request,
+                user: User = Depends(self.current_user()),
+                access_token_info: FiefAccessTokenInfo = Depends(backend.auth.authenticated()),
+            ):
+                checked_permissions: Dict[str, List[str]] = {}
+                permissions = json.loads(
+                    dict(request.query_params).get("permissions", "{}").replace("'", '"')
+                )
+                if permissions:
+                    user_permissions: Dict[str, List[str]] = {}
+                    for permission in access_token_info["permissions"]:
+                        resource, action = permission.split(":")
+                        if resource not in user_permissions:
+                            user_permissions[resource] = []
+                        user_permissions[resource].append(action)
+                    for resource, actions in permissions.items():
+                        user_resource_permissions = user_permissions.get(resource, [])
+                        allowed = checked_permissions[resource] = []
+                        for action in actions:
+                            if action in user_resource_permissions:
+                                allowed.append(action)
+
+                keys = ["username", "name", "display_name", "initials", "avatar_url", "color"]
+                identity = {k: getattr(user, k) for k in keys}
+                return {
+                    "identity": identity,
+                    "permissions": checked_permissions,
+                }
+
+            self.include_router(router)
+
+        def current_user(self, permissions: Optional[Dict[str, List[str]]] = None) -> Callable:
+            return backend.current_user(permissions)
+
+        async def update_user(self, update_user=Depends(backend.update_user)) -> Callable:
+            return update_user
+
+        def websocket_auth(
+            self,
+            permissions: Optional[Dict[str, List[str]]] = None,
+        ) -> Callable[[], Tuple[Any, Dict[str, List[str]]]]:
+            return backend.websocket_auth(permissions)
 
-        self.include_router(router)
+    return _AuthFief()
```

### Comparing `fps_auth_fief-0.1.8/.gitignore` & `fps_auth_fief-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.8/COPYING.md` & `fps_auth_fief-0.1.9/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.8/pyproject.toml` & `fps_auth_fief-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.8/PKG-INFO` & `fps_auth_fief-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_auth_fief
-Version: 0.1.8
+Version: 0.1.9
 Summary: An FPS plugin for the authentication API, using Fief
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

