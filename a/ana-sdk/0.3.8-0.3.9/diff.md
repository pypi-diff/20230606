# Comparing `tmp/ana_sdk-0.3.8.tar.gz` & `tmp/ana_sdk-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.3.8.tar", max compression
+gzip compressed data, was "ana_sdk-0.3.9.tar", max compression
```

## Comparing `ana_sdk-0.3.8.tar` & `ana_sdk-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.3.8/ana_sdk/__init__.py
--rw-r--r--   0        0        0    14393 2023-06-02 01:39:27.893197 ana_sdk-0.3.8/ana_sdk/ana.py
--rw-r--r--   0        0        0      138 2023-06-01 17:01:33.190199 ana_sdk-0.3.8/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4480 2023-06-01 17:05:04.633378 ana_sdk-0.3.8/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1725 2023-06-01 16:58:50.036423 ana_sdk-0.3.8/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4634 2023-06-01 17:00:04.904107 ana_sdk-0.3.8/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     2606 2023-06-06 02:13:06.960392 ana_sdk-0.3.8/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3218 2023-06-01 16:57:50.848033 ana_sdk-0.3.8/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.3.8/ana_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0      733 2023-06-06 01:08:29.138897 ana_sdk-0.3.8/ana_sdk/requests_auth.py
--rw-r--r--   0        0        0     4934 2023-05-25 23:15:52.044789 ana_sdk-0.3.8/ana_sdk/result_factory.py
--rw-r--r--   0        0        0      463 2023-06-06 02:13:12.643529 ana_sdk-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.3.8/README.md
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-06 03:25:49.925223 ana_sdk-0.3.9/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    14667 2023-06-06 03:48:25.043955 ana_sdk-0.3.9/ana_sdk/ana.py
+-rw-r--r--   0        0        0      140 2023-06-06 03:27:02.514357 ana_sdk-0.3.9/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4548 2023-06-06 03:30:34.311580 ana_sdk-0.3.9/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1797 2023-06-06 03:29:58.456822 ana_sdk-0.3.9/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4634 2023-06-01 17:00:04.904107 ana_sdk-0.3.9/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     2824 2023-06-06 03:33:15.589202 ana_sdk-0.3.9/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3351 2023-06-06 03:35:28.169552 ana_sdk-0.3.9/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.3.9/ana_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0      852 2023-06-06 03:40:27.284582 ana_sdk-0.3.9/ana_sdk/requests_auth.py
+-rw-r--r--   0        0        0     5251 2023-06-06 03:52:16.330061 ana_sdk-0.3.9/ana_sdk/result_factory.py
+-rw-r--r--   0        0        0      463 2023-06-06 03:52:35.249069 ana_sdk-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.3.9/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.3.9/PKG-INFO
```

### Comparing `ana_sdk-0.3.8/ana_sdk/ana.py` & `ana_sdk-0.3.9/ana_sdk/ana.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from requests import Session
 
 from .clients.dashboard_api_client import DashboardAPIClient
 from .clients.rpa_api_client import RPAAPIClient
 from .clients.ana_data_client import ANADataClient
 from .result_factory import ResultFactory
 from .requests_auth import RefreshAuth
+from ..ana_sdk import logger
 
 
 class ANA:
     """
     A classe ANA fornece uma interface para interagir com os serviços
     relacionados ao ambiente de automação de negócios, dados e clientes.
     Permite realizar login, executar comandos, definir tenant, cliente
@@ -159,14 +160,16 @@
             email or env_user_email,
             password or env_user_password,
             self.oauth_token_full_url
         )
         self.session = Session()
         self.session.auth = self._auth
 
+        logger.info(f"Usuário {self._auth.email} logado com sucesso!")
+
         self.api = DashboardAPIClient(self.session, self.dashboard_api_base_url)
         self.rpa = RPAAPIClient(self.session, self.rpa_api_base_url)
 
     def logout(self):
         """
         Faz o logout do usuário, limpando todas as informações.
 
@@ -181,14 +184,16 @@
         self.rpa = None
         self.data = None
 
         self.current_empresa = None
         self.current_cliente = None
         self.current_tenant = None
 
+        logger.info(f"Logout efetuado com sucesso.")
+
     def help(self, mope: str = None) -> dict[str, str]:
         """
         Exibe informações sobre os comandos disponíveis para automação.
         Se um MOPE for fornecido, exibe o JSON Schema do comando
         relacionado.
 
         Args:
@@ -254,14 +259,16 @@
         self.data = ANADataClient(
             self.ana_email,
             self._ana_password,
             self.current_tenant["configuracoes"]["ana_data_base_url"],
             self.oauth_token_full_url
         )
 
+        logger.debug("ANA-Data configurado com sucesso!")
+
     def set_cliente(self, id: int) -> None:
         """
         Define o cliente atual com base no ID fornecido. Obtém o
         tenant associado ao cliente e chama o método set_tenant()
         para configurar o ANA Data.
         
         Args:
@@ -370,8 +377,11 @@
         validate(instance=data, schema=schema)
         
         response = self.rpa.execute_command(mope, data)
         task_id = response.get("job_id")
 
         if wait_for_task:
             task_info = self._wait_for_task(task_id)
+
+            logger.debug("Comando executado!")
+
             return ResultFactory.create_result_handler(task_info)
```

### Comparing `ana_sdk-0.3.8/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.3.9/ana_sdk/clients/ana_data_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 
 from ..clients.base_client import BaseClient
 from ..requests_auth import RefreshAuth
+from ...ana_sdk import logger
 
 
 class ANADataClient(BaseClient):
     """
     Classe para interagir com a API do ANA Data.
 
     Attributes:
@@ -47,14 +48,15 @@
 
         Returns:
             list[dict] | dict: O conteúdo obtido da URL.
 
         Raises:
             requests.HTTPError: Se ocorrer um erro ao fazer a requisição.
         """
+        logger.debug(f"GET: {url}")
 
         response = self.session.get(url=url)
         response.raise_for_status()
 
         content = response.json()
         if "results" in content:
             next_page = content["next"]
```

### Comparing `ana_sdk-0.3.8/ana_sdk/clients/base_client.py` & `ana_sdk-0.3.9/ana_sdk/clients/base_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from urllib.parse import urlencode
 
 import requests
 from requests import Session
 
+from ...ana_sdk import logger
+
 
 class BaseClient:
 
     session: Session
 
     @staticmethod
     def _dict_to_query_string(query_parameters: dict) -> str:
@@ -37,14 +39,16 @@
         Returns:
             list[dict] | dict: Conteúdo da resposta da requisição.
 
         Raises:
             requests.HTTPError: Se ocorrer um erro ao fazer a requisição.
         """
         
+        logger.debug(f"GET: {url}")
+
         response = self.session.get(url=url)
         response.raise_for_status()
 
         content = response.json()
         if "data" in content:
             next_page = content["next_page"]
             data = content["data"]
```

### Comparing `ana_sdk-0.3.8/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.3.9/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.8/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.3.9/ana_sdk/clients/oauth_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import requests
 
+from ...ana_sdk import logger
+
 
 class OAuthClient:
     """
     Classe para interagir com o cliente OAuth.
 
     Atributos:
         email (str): Email do usuário.
@@ -62,26 +64,32 @@
             str: Token de acesso com todas as suas informações.
 
         Raises:
             requests.HTTPError: Se ocorrer um erro ao fazer a requisição.
         """
 
         if not self._token_is_valid():
+            logger.debug("Nenhum token válido encontrado.")
+
             data = {
                 "client_id": "pontoweb",
                 "username": self.email,
                 "password": self._password,
                 "grant_type": "password"
             }
 
+            logger.debug("Adquirindo novo token...")
+
             url = self.keycloak_url + "/token"
             response = requests.post(
                 url,
                 data=data,
                 headers={'Content-Type': 'application/x-www-form-urlencoded'}
             )
             response.raise_for_status()
             token = response.json()
 
             self.token = token
+
+            logger.debug("Novo token adquirido com sucesso!")
         
         return self.token
```

### Comparing `ana_sdk-0.3.8/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.3.9/ana_sdk/clients/rpa_api_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from requests import Session
 
 from ..clients.base_client import BaseClient
+from ...ana_sdk import logger
 
 
 class RPAAPIClient(BaseClient):
     """
     Classe para interagir com o cliente RPA API.
 
     Atributos:
@@ -102,14 +103,17 @@
 
         Returns:
             dict: Resultado da execução do comando.
 
         Raises:
             requests.HTTPError: Se ocorrer um erro ao fazer a requisição.
         """
+        
+        logger.info(f"Executando comando de MOPE [{mope}]...")
+        logger.debug(data)
 
         url = self._base_url + f"/jobs/{mope}"
         response = self.session.post(url=url, json=data)
         response.raise_for_status()
 
         content = response.json()
```

### Comparing `ana_sdk-0.3.8/ana_sdk/exceptions/__init__.py` & `ana_sdk-0.3.9/ana_sdk/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.8/ana_sdk/requests_auth.py` & `ana_sdk-0.3.9/ana_sdk/requests_auth.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,13 +12,15 @@
         
         self.oauth_client = OAuthClient(
             self.email,
             self._password,
             self.env_oauth_token_full_url
         )
 
-        self._token = self.oauth_client.get_token()
+        # Tenta pegar o token do usuário já na instanciação, levantando
+        # exceção caso login não consiga ser feito.
+        self.oauth_client.get_token()
 
     def __call__(self, r):
         access_token = self.oauth_client.get_token()["access_token"]
         r.headers['Authorization'] = "Bearer " + access_token        
         return r
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ana_sdk-0.3.8/ana_sdk/result_factory.py` & `ana_sdk-0.3.9/ana_sdk/result_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import requests
 
 from .exceptions import (
     ResultNotFoundError,
     NoResultHandlerImplementedError,
     TaskError,
 )
+from ..ana_sdk import logger
 
 
 class AbstractResultHandler(ABC):
     """
     Classe abstrata utilizada como interface para todos os manipuladores
     de resultado.
     """
@@ -60,14 +61,16 @@
         Obtém o resultado da execução de um relatório.
 
         Returns:
             Report: A instância atual da classe Report, possibilitando
             method chaining.
         """
         
+        logger.debug("Recuperando resultado da execução...")
+
         self.file = self._result["data"]["file"]
         self.error = self._result["error"]
         self.meta = self._result["meta"]
         self.status = self._result["status"]
 
         return self
     
@@ -91,29 +94,36 @@
                 url = self.file["link"]
                 filename = new_filename or self.file["name"]
                 filename_with_extension = filename + "." + self.file["extension"]
 
                 Path(path).mkdir(parents=True, exist_ok=True)
                 full_filename = path if path.endswith("/") else (path + "/") + filename_with_extension
 
+                logger.debug("Fazendo download do arquivo...")
+
                 response = requests.get(url)
                 response.raise_for_status()
 
+                logger.debug(f"Salvando arquivo em {full_filename}...")
+
                 with open(full_filename, "w") as file:
                     file.write(response.text)
 
         return self
     
     def get_link(self) -> str | None:
         """
         Recupera o link do relatório, caso exista um.
 
         Returns:
             str: Link do relatório, caso exista. Ou `None`.
         """
+        
+        logger.debug("Recuperando link de download do arquivo...")
+
         return self.file.get("link") 
 
 
 class Task(AbstractResultHandler):
     """
     Classe que lida com resultados de execuções de tasks que não geram
     relatórios.
```

### Comparing `ana_sdk-0.3.8/README.md` & `ana_sdk-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.8/PKG-INFO` & `ana_sdk-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.3.8
+Version: 0.3.9
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

