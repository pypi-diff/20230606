# Comparing `tmp/threadbare-3.0.0.tar.gz` & `tmp/threadbare-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadbare-3.0.0.tar", last modified: Wed Aug  3 04:27:09 2022, max compression
+gzip compressed data, was "threadbare-3.1.0.tar", last modified: Tue Jun  6 04:32:32 2023, max compression
```

## Comparing `threadbare-3.0.0.tar` & `threadbare-3.1.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-08-03 04:27:09.507053 threadbare-3.0.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    35147 2022-08-03 04:26:43.000000 threadbare-3.0.0/LICENCE.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      604 2022-08-03 04:27:09.507053 threadbare-3.0.0/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     5287 2022-08-03 04:26:43.000000 threadbare-3.0.0/README.md
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2022-08-03 04:27:09.507053 threadbare-3.0.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      764 2022-08-03 04:26:43.000000 threadbare-3.0.0/setup.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-08-03 04:27:09.507053 threadbare-3.0.0/threadbare/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2022-08-03 04:26:43.000000 threadbare-3.0.0/threadbare/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     3274 2022-08-03 04:26:43.000000 threadbare-3.0.0/threadbare/common.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    10351 2022-08-03 04:26:43.000000 threadbare-3.0.0/threadbare/execute.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    38313 2022-08-03 04:26:43.000000 threadbare-3.0.0/threadbare/operations.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     3953 2022-08-03 04:26:43.000000 threadbare-3.0.0/threadbare/state.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-08-03 04:27:09.507053 threadbare-3.0.0/threadbare.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      604 2022-08-03 04:27:09.000000 threadbare-3.0.0/threadbare.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      310 2022-08-03 04:27:09.000000 threadbare-3.0.0/threadbare.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2022-08-03 04:27:09.000000 threadbare-3.0.0/threadbare.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2022-08-03 04:27:09.000000 threadbare-3.0.0/threadbare.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       11 2022-08-03 04:27:09.000000 threadbare-3.0.0/threadbare.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-06 04:32:32.886560 threadbare-3.1.0/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    35147 2023-06-06 04:32:01.000000 threadbare-3.1.0/LICENCE.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      604 2023-06-06 04:32:32.886560 threadbare-3.1.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     5296 2023-06-06 04:32:01.000000 threadbare-3.1.0/README.md
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-06-06 04:32:32.886560 threadbare-3.1.0/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      764 2023-06-06 04:32:01.000000 threadbare-3.1.0/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-06 04:32:32.882560 threadbare-3.1.0/tests/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     2030 2023-06-06 04:32:01.000000 threadbare-3.1.0/tests/test_common.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    12453 2023-06-06 04:32:01.000000 threadbare-3.1.0/tests/test_execute.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    23949 2023-06-06 04:32:01.000000 threadbare-3.1.0/tests/test_operations.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     6438 2023-06-06 04:32:01.000000 threadbare-3.1.0/tests/test_state.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-06 04:32:32.882560 threadbare-3.1.0/threadbare/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2023-06-06 04:32:01.000000 threadbare-3.1.0/threadbare/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     3274 2023-06-06 04:32:01.000000 threadbare-3.1.0/threadbare/common.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    10351 2023-06-06 04:32:01.000000 threadbare-3.1.0/threadbare/execute.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    38946 2023-06-06 04:32:01.000000 threadbare-3.1.0/threadbare/operations.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     3953 2023-06-06 04:32:01.000000 threadbare-3.1.0/threadbare/state.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-06 04:32:32.886560 threadbare-3.1.0/threadbare.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      604 2023-06-06 04:32:32.000000 threadbare-3.1.0/threadbare.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      398 2023-06-06 04:32:32.000000 threadbare-3.1.0/threadbare.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-06-06 04:32:32.000000 threadbare-3.1.0/threadbare.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2023-06-06 04:32:32.000000 threadbare-3.1.0/threadbare.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       11 2023-06-06 04:32:32.000000 threadbare-3.1.0/threadbare.egg-info/top_level.txt
```

### Comparing `threadbare-3.0.0/LICENCE.txt` & `threadbare-3.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `threadbare-3.0.0/PKG-INFO` & `threadbare-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadbare
-Version: 3.0.0
+Version: 3.1.0
 Summary: A Fabric and Paramiko replacement library
 Home-page: https://github.com/elifesciences/threadbare
 Maintainer: Luke
 Maintainer-email: lsh-0@users.noreply.github.com
 License: GPLv3
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threadbare-3.0.0/README.md` & `threadbare-3.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     remote("echo 'hello world!'")
 ```
 
 ## local tests
 
 Run the [test suite](./test.sh) with `./test.sh`
 
-Individual tests can be run with `./test.sh -k test_fn_name`
+Individual tests can be run with `./test.sh example.py::test_fn_name`
 
 ## remote tests
 
 A set of tests that also serve as working examples of threadbare's functionality can be executed by starting a dummy SSH 
 server:
 
     ./tests-remote/sshd-server.sh
```

### Comparing `threadbare-3.0.0/setup.py` & `threadbare-3.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='threadbare',
-    version='3.0.0',
+    version='3.1.0',
     description='A Fabric and Paramiko replacement library',
     long_description="A partial replacement of the Fabric and Paramiko libraries using ParallelSSH.",
     long_description_content_type="text/markdown",
     url="https://github.com/elifesciences/threadbare",
     maintainer="Luke",
     maintainer_email="lsh-0@users.noreply.github.com",
     install_requires=["parallel-ssh>=1.9.1"],
```

### Comparing `threadbare-3.0.0/threadbare/__init__.py` & `threadbare-3.1.0/threadbare/__init__.py`

 * *Files identical despite different names*

### Comparing `threadbare-3.0.0/threadbare/common.py` & `threadbare-3.1.0/threadbare/common.py`

 * *Files identical despite different names*

### Comparing `threadbare-3.0.0/threadbare/execute.py` & `threadbare-3.1.0/threadbare/execute.py`

 * *Files identical despite different names*

### Comparing `threadbare-3.0.0/threadbare/operations.py` & `threadbare-3.1.0/threadbare/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from functools import wraps
+from functools import wraps, partial
 from datetime import datetime
 import tempfile
 import contextlib
 import subprocess
 from threading import Timer
 import getpass
-from pssh import exceptions as pssh_exceptions
+import pssh.exceptions
 import os, sys
 from pssh.clients.native import SSHClient as PSSHClient
 import gevent
 import io
 import logging
 from . import state
 from .common import (
@@ -53,21 +53,25 @@
         # we have the opportunity here to tweak the error messages to make them
         # similar to their equivalents in Fabric.
         # original error messages are still available via `str(excinst.wrapped)`
         space = " "
         custom_error_prefixes = {
             # builder: https://github.com/elifesciences/builder/blob/master/src/buildercore/core.py#L345-L347
             # pssh: https://github.com/ParallelSSH/parallel-ssh/blob/8b7bb4bcb94d913c3b7da77db592f84486c53b90/pssh/clients/native/parallel.py#L272-L274
-            pssh_exceptions.Timeout: "Timed out trying to connect.",
+            pssh.exceptions.Timeout: "Timed out trying to connect.",
             # builder: https://github.com/elifesciences/builder/blob/master/src/buildercore/core.py#L348-L350
             # fabric: https://github.com/mathiasertl/fabric/blob/master/fabric/network.py#L601-L605
             # pssh: https://github.com/ParallelSSH/parallel-ssh/blob/2e9668cf4b58b38316b1d515810d7e6c595c76f3/pssh/exceptions.py
-            pssh_exceptions.SSHException: "Low level socket error connecting to host.",
-            pssh_exceptions.SessionError: "Low level socket error connecting to host.",
-            pssh_exceptions.ConnectionErrorException: "Low level socket error connecting to host.",
+            pssh.exceptions.SSHException: "Low level socket error connecting to host.",
+            pssh.exceptions.SessionError: "Low level socket error connecting to host.",
+            # lsh@2023-05-08: changed in pssh 2.9.0 and deprecated, pssh uses the builtin now.
+            pssh.exceptions.ConnectionErrorException: "Low level socket error connecting to host.",
+            ConnectionError: "Low level socket error connecting to host.",
+            # lsh@2023-05-08: introduced in pssh 2.9.0, we have to capture this and retry it ourselves.
+            ConnectionRefusedError: "Low level socket error connecting to host.",
         }
         new_error = custom_error_prefixes.get(type(self.wrapped)) or ""
         original_error = str(self.wrapped)
         return new_error + space + original_error
 
 
 def pem_key():
@@ -205,21 +209,26 @@
     shell = False  # handled ourselves
     sudo = False  # handled ourselves
     user = None  # user to sudo to
     encoding = "utf-8"  # used everywhere
 
     try:
         # https://parallel-ssh.readthedocs.io/en/latest/native_single.html#pssh.clients.native.single.SSHClient.run_command
-        channel, host_string, stdout, stderr, stdin = client.run_command(
+        # https://github.com/ParallelSSH/parallel-ssh/blob/master/pssh/output.py
+        host_output = client.run_command(
             command, sudo, user, use_pty, shell, encoding, timeout
         )
 
+        host_string = host_output.host
+        stdout = host_output.stdout
+        stderr = host_output.stderr
+
         def get_exit_code():
-            client.wait_finished(channel)
-            return channel.get_exit_status()
+            client.wait_finished(host_output)
+            return host_output.exit_code
 
         return {
             # defer executing as it consumes output entirely before returning. this
             # removes our chance to display/transform output as it is streamed to us
             "return_code": get_exit_code,
             "command": command,
             "stdout": stdout,
@@ -266,34 +275,33 @@
         }
 
         # render template and write to given pipe
         template = final_kwargs["line_template"]
 
         if not final_kwargs["display_prefix"]:
             try:
-                template = template[template.index("{line}") :]
+                template = template[template.index("{line}"):]
             except ValueError:  # "substring not found"
                 msg = "'display_prefix' option ignored: '{line}' not found in 'line_template' setting"
                 LOG.warning(msg)
-                pass
 
         output_pipe.write(template.format(**template_kwargs))
 
     if not final_kwargs["discard_output"]:
         return line  # free of any formatting
 
 
-def _process_output(output_pipe, result_list, **kwargs):
+def _process_output(output_pipe, result_buffer, **kwargs):
     "calls `_print_line` on each result in `result_list`."
 
     # always process the results as soon as we have them
     # use `quiet=True` to hide the printing of output to stdout/stderr
     # use `discard_output=True` to discard the results as soon as they are read.
     # `stderr` results may be empty if `combine_stderr` in call to `remote` was `True`
-    new_results = [_print_line(output_pipe, line, **kwargs) for line in result_list]
+    new_results = [_print_line(output_pipe, line, **kwargs) for line in result_buffer]
     output_pipe.flush()
     if "discard_output" in kwargs and not kwargs["discard_output"]:
         return new_results
 
 
 def _print_running(command, output_pipe, **kwargs):
     """Prints the command to be run on a line of output prior to executing a command.
@@ -685,15 +693,15 @@
         local("mkdir -p %r" % (abs_local_dir,))
     return execute_rsync_command(_rsync_download(remote_path, local_path, **kwargs))
 
 
 def _transfer_fn(client, direction, **kwargs):
     """returns the `client` object's appropriate transfer *method* given a `direction`.
     `direction` is either 'upload' or 'download'.
-    Also accepts the `transfer_protocol` keyword parameter that is either 'scp' (default) or 'sftp'."""
+    Also accepts the `transfer_protocol` keyword parameter that is either 'rsync' (default), 'scp' or 'sftp'."""
     base_kwargs = {
         "overwrite": True,
         # sftp is *exceptionally* slow.
         # Paramiko's implementation is faster than native SFTP but slower than SCP:
         # - https://github.com/ParallelSSH/parallel-ssh/issues/177
         # however, SCP is buggy and may randomly hang or complete without uploading anything.
         # take slow and reliable over fast and buggy.
@@ -710,15 +718,17 @@
                     % (remote_file,)
                 )
 
             if final_kwargs["transfer_protocol"] == "rsync":
                 fn(local_file, remote_file)
             else:
                 # https://github.com/ParallelSSH/parallel-ssh/blob/8b7bb4bcb94d913c3b7da77db592f84486c53b90/pssh/clients/native/parallel.py#L524
-                gevent.joinall(fn(local_file, remote_file), raise_error=True)
+                g = fn(local_file, remote_file)
+                if g:
+                    gevent.joinall(g, raise_error=True)
 
             # lsh@2020-04, local testing didn't reveal anything but small files uploaded via SCP SCP during CI
             # were either missing or had empty bodies. SFTP seemed to be fine.
             # This sanity check seems to fix the issue (lending more credence to my theory it's an unflushed buffer somewhere),
             # when waiting 3 seconds between upload of file and check of file was still failing.
             ensure(
                 remote_file_exists(remote_file, **kwargs),
@@ -736,22 +746,24 @@
                 raise NetworkError(
                     "Local file exists and 'overwrite' is set to 'False'. Refusing to write: %s"
                     % (local_file,)
                 )
             if final_kwargs["transfer_protocol"] == "rsync":
                 fn(remote_file, local_file)
             else:
-                # https://github.com/ParallelSSH/parallel-ssh/blob/8b7bb4bcb94d913c3b7da77db592f84486c53b90/pssh/clients/native/parallel.py#L560
-                gevent.joinall(fn(remote_file, local_file), raise_error=True)
+                # https://github.com/ParallelSSH/parallel-ssh/blob/d812ff32d828009ddb94f458fe43920c22df4c0e/pssh/clients/native/single.py#L558
+                g = fn(remote_file, local_file)
+                if g:
+                    gevent.joinall(g, raise_error=True)
 
         return wrapper
 
     upload_backends = {
-        "sftp": client.copy_file,
-        "scp": client.scp_send,
+        "sftp": partial(client.copy_file, recurse=True),
+        "scp": partial(client.scp_send, recurse=True),
         "rsync": rsync_upload,
     }
 
     download_backends = {
         "sftp": client.copy_remote_file,
         "scp": client.scp_recv,
         "rsync": rsync_download,
@@ -809,15 +821,15 @@
 
     transfer_fn = _transfer_fn(client, "download", **kwargs)
 
     try:
         transfer_fn(remote_tempfile, local_path)
         return local_path
 
-    except (pssh_exceptions.SFTPError, pssh_exceptions.SCPError) as exc:
+    except (pssh.exceptions.SFTPError, pssh.exceptions.SCPError) as exc:
         # permissions or network issues may cause these
         raise NetworkError(exc)
 
     finally:
         remote_sudo('rm -f "%s"' % remote_tempfile, **kwargs)
 
 
@@ -864,15 +876,15 @@
                     "remote file does not exist: %s" % (remote_path,)
                 )
             client = _ssh_client(**kwargs)
             transfer_fn = _transfer_fn(client, "download", **kwargs)
 
             try:
                 transfer_fn(remote_path, local_path)
-            except (pssh_exceptions.SFTPError, pssh_exceptions.SCPError) as exc:
+            except (pssh.exceptions.SFTPError, pssh.exceptions.SCPError) as exc:
                 # permissions or network issues may cause these
                 raise NetworkError(exc)
 
         if temp_file:
             flags = "r" if isinstance(data_buffer, io.StringIO) else "rb"
             data = open(local_path, flags).read()
             data_buffer.write(data)
@@ -910,15 +922,15 @@
         transfer_fn(local_path, remote_temp_path)
         move_file_into_place = 'mv "%s" "%s"' % (remote_temp_path, remote_path)
         remote_sudo(move_file_into_place, **kwargs)
         ensure(
             remote_file_exists(remote_path, use_sudo=True, **kwargs),
             "remote path does not exist: %s" % (remote_path),
         )
-    except (pssh_exceptions.SFTPError, pssh_exceptions.SCPError) as exc:
+    except (pssh.exceptions.SFTPError, pssh.exceptions.SCPError) as exc:
         # permissions or network issues may cause these
         raise NetworkError(exc)
 
 
 def _write_bytes_to_temporary_file(local_path):
     """if `local_path` is a file-like object, write the contents to an *actual* file and
     return a pair of new local filename and a function that removes the temporary file when called."""
@@ -959,10 +971,10 @@
             raise EnvironmentError("local file does not exist: %s" % (local_path,))
 
         client = _ssh_client(**kwargs)
 
         try:
             transfer_fn = _transfer_fn(client, "upload", **kwargs)
             transfer_fn(local_path, remote_path)
-        except (pssh_exceptions.SFTPError, pssh_exceptions.SCPError) as exc:
+        except (pssh.exceptions.SFTPError, pssh.exceptions.SCPError) as exc:
             # permissions or network issues may cause these
             raise NetworkError(exc)
```

### Comparing `threadbare-3.0.0/threadbare/state.py` & `threadbare-3.1.0/threadbare/state.py`

 * *Files identical despite different names*

### Comparing `threadbare-3.0.0/threadbare.egg-info/PKG-INFO` & `threadbare-3.1.0/threadbare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadbare
-Version: 3.0.0
+Version: 3.1.0
 Summary: A Fabric and Paramiko replacement library
 Home-page: https://github.com/elifesciences/threadbare
 Maintainer: Luke
 Maintainer-email: lsh-0@users.noreply.github.com
 License: GPLv3
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
```

