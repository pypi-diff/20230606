# Comparing `tmp/run_rx-0.0.5.tar.gz` & `tmp/run_rx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_rx-0.0.5.tar", max compression
+gzip compressed data, was "run_rx-0.0.6.tar", max compression
```

## Comparing `run_rx-0.0.5.tar` & `run_rx-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     1679 2023-05-19 14:53:21.015913 run_rx-0.0.5/README.md
--rw-r--r--   0        0        0      313 2023-06-01 23:35:09.526681 run_rx-0.0.5/install/.rxignore
--rw-r--r--   0        0        0      274 2023-06-04 16:34:29.656668 run_rx-0.0.5/install/README.md
--rw-r--r--   0        0        0       98 2023-05-16 20:24:41.277933 run_rx-0.0.5/install/python-cpu
--rw-r--r--   0        0        0       98 2023-05-16 20:24:41.278137 run_rx-0.0.5/install/python-gpu
--rw-r--r--   0        0        0      736 2023-06-05 01:42:19.164130 run_rx-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      300 2023-05-16 20:24:41.279362 run_rx-0.0.5/rx/__main__.py
--rw-r--r--   0        0        0     2799 2023-06-04 17:02:00.126921 run_rx-0.0.5/rx/client/commands/exec.py
--rw-r--r--   0        0        0     1284 2023-06-01 23:40:03.839582 run_rx-0.0.5/rx/client/commands/init.py
--rw-r--r--   0        0        0     2109 2023-06-04 16:41:38.419103 run_rx-0.0.5/rx/client/configuration/config_base.py
--rw-r--r--   0        0        0     7016 2023-06-05 01:42:40.149599 run_rx-0.0.5/rx/client/configuration/local.py
--rw-r--r--   0        0        0      501 2023-05-16 20:24:41.281326 run_rx-0.0.5/rx/client/configuration/remote.py
--rw-r--r--   0        0        0     3045 2023-06-04 16:47:27.983133 run_rx-0.0.5/rx/client/executor.py
--rw-r--r--   0        0        0      256 2023-05-16 20:24:41.281715 run_rx-0.0.5/rx/client/grpc_helper.py
--rw-r--r--   0        0        0     5353 2023-06-01 23:06:43.816386 run_rx-0.0.5/rx/client/init_client.py
--rw-r--r--   0        0        0     9694 2023-05-16 20:24:41.282187 run_rx-0.0.5/rx/client/login.py
--rw-r--r--   0        0        0     2029 2023-05-16 20:24:41.282556 run_rx-0.0.5/rx/client/menu.py
--rw-r--r--   0        0        0     1092 2023-05-16 20:24:41.282728 run_rx-0.0.5/rx/client/output_handler.py
--rw-r--r--   0        0        0     3307 2023-06-04 16:44:15.057168 run_rx-0.0.5/rx/client/rsync.py
--rw-r--r--   0        0        0     1603 2023-05-16 20:24:41.283538 run_rx-0.0.5/rx/client/user.py
--rw-r--r--   0        0        0     5866 2023-05-09 18:41:10.568989 run_rx-0.0.5/rx/proto/rx_pb2.py
--rw-r--r--   0        0        0     7595 2023-05-09 18:41:10.570471 run_rx-0.0.5/rx/proto/rx_pb2.pyi
--rw-r--r--   0        0        0    12663 2023-05-09 18:41:10.570796 run_rx-0.0.5/rx/proto/rx_pb2_grpc.py
--rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 run_rx-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1679 2023-05-19 14:53:21.015913 run_rx-0.0.6/README.md
+-rw-r--r--   0        0        0      313 2023-06-01 23:35:09.526681 run_rx-0.0.6/install/.rxignore
+-rw-r--r--   0        0        0      274 2023-06-04 16:34:29.656668 run_rx-0.0.6/install/README.md
+-rw-r--r--   0        0        0       98 2023-05-16 20:24:41.277933 run_rx-0.0.6/install/python-cpu
+-rw-r--r--   0        0        0       98 2023-06-06 18:01:13.521487 run_rx-0.0.6/install/python-gpu
+-rw-r--r--   0        0        0      736 2023-06-06 18:24:21.616376 run_rx-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-05-16 20:24:41.279362 run_rx-0.0.6/rx/__main__.py
+-rw-r--r--   0        0        0     2818 2023-06-06 18:25:15.327114 run_rx-0.0.6/rx/client/commands/exec.py
+-rw-r--r--   0        0        0     1284 2023-06-06 18:01:13.522952 run_rx-0.0.6/rx/client/commands/init.py
+-rw-r--r--   0        0        0     2109 2023-06-04 16:41:38.419103 run_rx-0.0.6/rx/client/configuration/config_base.py
+-rw-r--r--   0        0        0     7016 2023-06-06 18:24:36.468419 run_rx-0.0.6/rx/client/configuration/local.py
+-rw-r--r--   0        0        0      641 2023-06-06 18:04:41.546820 run_rx-0.0.6/rx/client/configuration/remote.py
+-rw-r--r--   0        0        0     3017 2023-06-06 18:07:01.812095 run_rx-0.0.6/rx/client/executor.py
+-rw-r--r--   0        0        0      256 2023-05-16 20:24:41.281715 run_rx-0.0.6/rx/client/grpc_helper.py
+-rw-r--r--   0        0        0     5307 2023-06-06 18:09:45.366400 run_rx-0.0.6/rx/client/init_client.py
+-rw-r--r--   0        0        0     9694 2023-05-16 20:24:41.282187 run_rx-0.0.6/rx/client/login.py
+-rw-r--r--   0        0        0     2029 2023-05-16 20:24:41.282556 run_rx-0.0.6/rx/client/menu.py
+-rw-r--r--   0        0        0     1092 2023-05-16 20:24:41.282728 run_rx-0.0.6/rx/client/output_handler.py
+-rw-r--r--   0        0        0     3306 2023-06-06 18:01:13.524830 run_rx-0.0.6/rx/client/rsync.py
+-rw-r--r--   0        0        0     1603 2023-05-16 20:24:41.283538 run_rx-0.0.6/rx/client/user.py
+-rw-r--r--   0        0        0     5866 2023-05-09 18:41:10.568989 run_rx-0.0.6/rx/proto/rx_pb2.py
+-rw-r--r--   0        0        0     7595 2023-05-09 18:41:10.570471 run_rx-0.0.6/rx/proto/rx_pb2.pyi
+-rw-r--r--   0        0        0    12663 2023-05-09 18:41:10.570796 run_rx-0.0.6/rx/proto/rx_pb2_grpc.py
+-rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 run_rx-0.0.6/PKG-INFO
```

### Comparing `run_rx-0.0.5/LICENSE.txt` & `run_rx-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/README.md` & `run_rx-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/pyproject.toml` & `run_rx-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "run-rx"
-version = "0.0.5"
+version = "0.0.6"
 description = "A tool to simplify remote execution"
 authors = ["Kris Chodorow <k.chodorow@gmail.com>"]
 license = "LICENSE.txt"
 readme = "README.md"
 homepage = "https://www.run-rx.com"
 repository = "https://github.com/run-rx/rx"
 packages = [
```

### Comparing `run_rx-0.0.5/rx/client/commands/exec.py` & `run_rx-0.0.6/rx/client/commands/exec.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     self._config = local.find_local_config(cwd)
 
   def run(self) -> int:
     if self._config is None:
       print ('Run `rx init` first!')
       return -1
     remote_cfg = remote.Remote(self._config.cwd)
-    with grpc_helper.get_channel(remote_cfg['grpc_addr']) as ch:
+    with grpc_helper.get_channel(remote_cfg.worker_addr) as ch:
       client = executor.Client(ch, self._config, remote_cfg)
       return self._try_exec(client)
 
   def _try_exec(self, client: executor.Client) -> int:
     """Sends the command to the server."""
     if len(self._argv) < 1:
       print('No command given.')
@@ -67,16 +67,17 @@
         'instance.')
       return e.code
 
 
 class VersionCommand:
   """Prints the version."""
 
-  def run(self):
+  def run(self) -> int:
     print(local.VERSION)
+    return 0
 
 
 def main(argv):
   logging.get_absl_handler().python_handler.use_absl_log_file(
     program_name='rx', log_dir=tempfile.gettempdir())
   if len(argv) == 1:
     print('No command given.\n')
```

### Comparing `run_rx-0.0.5/rx/client/commands/init.py` & `run_rx-0.0.6/rx/client/commands/init.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/rx/client/configuration/config_base.py` & `run_rx-0.0.6/rx/client/configuration/config_base.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/rx/client/configuration/local.py` & `run_rx-0.0.6/rx/client/configuration/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from absl import flags
 from absl import logging
 import sty
 
 from rx.client.configuration import config_base
 from rx.proto import rx_pb2
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 IGNORE = pathlib.Path('.rxignore')
 
 _REMOTE = flags.DEFINE_string(
   'remote', None,
   'The path to the remote configuration file to use (see .rx/README.md).')
 _RSYNC_PATH = flags.DEFINE_string('rsync_path', None, 'Path to rsync binary')
```

### Comparing `run_rx-0.0.5/rx/client/executor.py` & `run_rx-0.0.6/rx/client/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   """Handle contacting the remote server."""
 
   def __init__(
       self,
       channel: grpc.Channel,
       local_cfg: local.LocalConfig,
       remote_cfg: remote.Remote):
-    self._uri = remote_cfg['grpc_addr']
+    self._uri = remote_cfg.worker_addr
     self._rsync = rsync.RsyncClient(local_cfg, remote_cfg)
     self._stub = rx_pb2_grpc.ExecutionServiceStub(channel)
     self._metadata = local.get_grpc_metadata()
     self._local_cfg = local_cfg
     self._remote_cfg = remote_cfg
     self._login = login.LoginManager(local_cfg.cwd)
     self._current_execution_id = None
@@ -41,19 +41,19 @@
     logging.info(f'Running `{cmd_str}` on {self._uri}')
 
     self._login.login()
     self._metadata += self._login.grpc_metadata
 
     result = self._rsync.to_remote()
     if result != 0:
-      raise UnreachableError(self._local_cfg["worker_addr"], result)
+      raise UnreachableError(self._uri, result)
     result = None
 
     request = rx_pb2.ExecRequest(
-      workspace_id=self._remote_cfg['workspace_id'],
+      workspace_id=self._remote_cfg.workspace_id,
       argv=argv,
       rsync_source=self._local_cfg.rsync_source)
 
     out_handler = output_handler.OutputHandler(self._local_cfg.cwd)
     response = None
     try:
       for response in self._stub.Exec(request, metadata=self._metadata):
@@ -87,15 +87,15 @@
   def maybe_kill(self):
     """Kill the process, if it exists."""
     if self._current_execution_id is None:
       logging.error('No ID to kill.')
       return
 
     req = rx_pb2.KillRequest(
-      workspace_id=self._remote_cfg['workspace_id'],
+      workspace_id=self._remote_cfg.workspace_id,
       execution_id=self._current_execution_id,
     )
     self._stub.Kill(req, metadata=self._metadata)
 
 
 class UnreachableError(RuntimeError):
   def __init__(self, worker_addr: str, code: int, *args: object) -> None:
```

### Comparing `run_rx-0.0.5/rx/client/init_client.py` & `run_rx-0.0.6/rx/client/init_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,19 +76,18 @@
 
     # TODO: create a threaded UserStatus class with __enter__/__exit__.
     sys.stdout.write('Copying source code... ')
     sys.stdout.flush()
     with remote.WritableRemote(self._local_cfg.cwd) as r:
       r['workspace_id'] = resp.workspace_id
       r['worker_addr'] = resp.worker_addr
-      r['grpc_addr'] = f'{resp.worker_addr}'
       r['daemon_module'] = resp.rsync_dest.daemon_module
     self._run_initial_rsync()
     sys.stdout.write('Done.\n')
-    self._install_deps(f'{resp.worker_addr}', resp.workspace_id)
+    self._install_deps(resp.worker_addr, resp.workspace_id)
     print('\nDone setting up rx! To use, run:\n\n\t$ rx <your command>\n')
     return 0
 
   def _create_username(self) -> str:
     username = user.username_prompt(self._login.id_token['email'])
     req = rx_pb2.SetUsernameRequest(username=username)
     try:
@@ -122,16 +121,16 @@
   def _run_initial_rsync(self):
     r = rsync.RsyncClient(
       self._local_cfg, remote.Remote(self._local_cfg.cwd))
     return_code = r.to_remote()
     if return_code == 0:
       logging.info('Copied files to %s', r.host)
 
-  def _install_deps(self, grpc_addr: str, workspace_id: str) -> int:
-    channel = grpc_helper.get_channel(grpc_addr)
+  def _install_deps(self, worker_addr: str, workspace_id: str) -> int:
+    channel = grpc_helper.get_channel(worker_addr)
     stub = rx_pb2_grpc.ExecutionServiceStub(channel)
     req = rx_pb2.InstallDepsRequest(workspace_id=workspace_id)
     resp = None
     try:
       for resp in stub.InstallDeps(
         req, metadata=self._metadata, timeout=(10 * 60)):
         if resp.stdout:
```

### Comparing `run_rx-0.0.5/rx/client/login.py` & `run_rx-0.0.6/rx/client/login.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/rx/client/menu.py` & `run_rx-0.0.6/rx/client/menu.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/rx/client/output_handler.py` & `run_rx-0.0.6/rx/client/output_handler.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/rx/client/rsync.py` & `run_rx-0.0.6/rx/client/rsync.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
       tab_count -= 1
     tabs = '  ' * tab_count
     slash = '/' if is_dir else ''
     pretty_name = f'{pathlib.Path(filename).name}{slash}'
     # TODO: handle file deletion.
     print(f'{tabs}{pretty_name}')
 
-
 class RsyncClient:
   """Rsync tools."""
 
   def __init__(
       self, local_cfg: local.LocalConfig, remote_cfg: abc.Mapping):
     self._sync_dir = local_cfg.cwd
     self._cfg = remote_cfg
```

### Comparing `run_rx-0.0.5/rx/client/user.py` & `run_rx-0.0.6/rx/client/user.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/rx/proto/rx_pb2.py` & `run_rx-0.0.6/rx/proto/rx_pb2.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/rx/proto/rx_pb2.pyi` & `run_rx-0.0.6/rx/proto/rx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/rx/proto/rx_pb2_grpc.py` & `run_rx-0.0.6/rx/proto/rx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.5/PKG-INFO` & `run_rx-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-rx
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool to simplify remote execution
 Home-page: https://www.run-rx.com
 License: LICENSE.txt
 Author: Kris Chodorow
 Author-email: k.chodorow@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

