# Comparing `tmp/poetry-exec-plugin-0.3.5.tar.gz` & `tmp/poetry-exec-plugin-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-exec-plugin-0.3.5.tar", max compression
+gzip compressed data, was "poetry-exec-plugin-0.3.6.tar", max compression
```

## Comparing `poetry-exec-plugin-0.3.5.tar` & `poetry-exec-plugin-0.3.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2022-08-26 22:52:22.255396 poetry-exec-plugin-0.3.5/LICENSE
--rw-r--r--   0        0        0     1914 2022-08-26 22:52:22.255396 poetry-exec-plugin-0.3.5/README.md
--rw-r--r--   0        0        0     3011 2022-08-26 22:52:22.255396 poetry-exec-plugin-0.3.5/poetry_exec_plugin/plugin.py
--rw-r--r--   0        0        0      905 2022-08-26 22:52:22.255396 poetry-exec-plugin-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 poetry-exec-plugin-0.3.5/setup.py
--rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 poetry-exec-plugin-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-05 23:06:41.193583 poetry-exec-plugin-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1914 2023-06-05 23:06:41.193583 poetry-exec-plugin-0.3.6/README.md
+-rw-r--r--   0        0        0     3039 2023-06-05 23:06:41.193583 poetry-exec-plugin-0.3.6/poetry_exec_plugin/plugin.py
+-rw-r--r--   0        0        0      923 2023-06-05 23:06:41.193583 poetry-exec-plugin-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 poetry-exec-plugin-0.3.6/setup.py
+-rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 poetry-exec-plugin-0.3.6/PKG-INFO
```

### Comparing `poetry-exec-plugin-0.3.5/LICENSE` & `poetry-exec-plugin-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-exec-plugin-0.3.5/README.md` & `poetry-exec-plugin-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `poetry-exec-plugin-0.3.5/poetry_exec_plugin/plugin.py` & `poetry-exec-plugin-0.3.6/poetry_exec_plugin/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 import os
 import shlex
 import sys
+from typing import Any, List
 
-from cleo.helpers import argument
 from cleo.application import Application
-
+from cleo.helpers import argument
 from poetry.console.commands.env_command import EnvCommand
 from poetry.plugins.application_plugin import ApplicationPlugin
 
-from typing import Any, List
-
 
 def shlex_join(cmd_list: List[str]) -> str:
     if sys.version_info < (3, 8):
         # shlex.join has been introduced in Python 3.8
         # https://github.com/python/cpython/blob/3.9/Lib/shlex.py#L318
         return " ".join(shlex.quote(x) for x in cmd_list)
     else:
         return shlex.join(cmd_list)
 
 
 class ExecCommand(EnvCommand):
-
     name = "exec"
     description = "Execute a predefined command from your pyproject.toml."
 
     arguments = [
-        argument("cmd", "The command to run from your pyproject.toml.", multiple=False),
+        argument(
+            "cmd", "The command to run from your pyproject.toml.", multiple=False
+        ),
         argument(
             "arguments",
             "Additional arguments to append to the command.",
             multiple=True,
             optional=True,
         ),
     ]
 
     def handle(self) -> Any:
-        pyproject_folder_path = self.poetry.pyproject._file.path.parent
+        pyproject_folder_path = self.poetry.pyproject.file.path.parent
         pyproject_data = self.poetry.pyproject.data
 
         cmd_name = self.argument("cmd")
         cmd = (
             pyproject_data.get("tool", {})
             .get("poetry-exec-plugin", {})
             .get("commands", {})
             .get(cmd_name)
         )
 
         if not cmd:
             self.line_error(
-                f"\nUnable to find the command '{cmd_name}'. To configure a command you must "
-                "add it to your pyproject.toml under the path "
+                f"\nUnable to find the command '{cmd_name}'. To configure a command "
+                "you must add it to your pyproject.toml under the path "
                 "[tool.poetry-exec-plugin.commands]. For example:"
                 "\n\n"
                 "[tool.poetry-exec-plugin.commands]\n"
                 f'{cmd_name} = "echo Hello World"\n',
                 style="error",
             )
             return 1
 
         full_cmd = f"{cmd} {shlex_join(self.argument('arguments'))}"
         shell = os.environ.get("SHELL", "/bin/sh")
 
-        # Change directory to the folder that contains the pyproject.toml so that the command runs
-        # from that folder (even if you call poetry exec from a subfolder). This mimics the
-        # behaviour of npm/yarn.
+        # Change directory to the folder that contains the pyproject.toml so that
+        # the command runs from that folder (even if you call poetry exec from a
+        # subfolder). This mimics the behaviour of npm/yarn.
         os.chdir(pyproject_folder_path)
 
         self.line(f"Exec: {full_cmd}\n", style="info")
         result = self.env.execute(*[shell, "-c", full_cmd])
 
-        # NOTE: If running on mac or linux nothing will be executed after the previous line. This
-        # is because poetry uses os.execvpe to run the command which means that the current process
-        # is replaced by the command. If on windows it uses subprocess.run which means the code
-        # after this comment will be executed.
+        # NOTE: If running on mac or linux nothing will be executed after the
+        # previous line. This is because poetry uses os.execvpe to run the command
+        # which means that the current process is replaced by the command. If on
+        # windows it uses subprocess.run which means the code after this comment
+        # will be executed.
 
         self.line("\n✨ Done!")
 
         if result:
             return result.returncode
```

### Comparing `poetry-exec-plugin-0.3.5/pyproject.toml` & `poetry-exec-plugin-0.3.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-exec-plugin"
-version = "0.3.5"
+version = "0.3.6"
 description = "A plugin for poetry that allows you to execute scripts defined in your pyproject.toml, just like you can in npm or pipenv."
 authors = ["keattang"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/keattang/poetry-exec-plugin"
 repository = "https://github.com/keattang/poetry-exec-plugin"
 
@@ -19,17 +19,18 @@
 mypy = "^0.910"
 pytest = "^6.2.4"
 types-toml = "^0.1.5"
 
 [tool.poetry-exec-plugin.commands]
 lint = "flake8 && black --check . && mypy ."
 test = "pytest"
+format = "black ."
 
 [tool.poetry.plugins."poetry.application.plugin"]
 exec = "poetry_exec_plugin.plugin:ExecPlugin"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-line-length = 100
+line-length = 85
```

### Comparing `poetry-exec-plugin-0.3.5/setup.py` & `poetry-exec-plugin-0.3.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['poetry>=1.2.0.a2,<2.0.0', 'toml>=0.10.2,<0.11.0']
 
 entry_points = \
 {'poetry.application.plugin': ['exec = poetry_exec_plugin.plugin:ExecPlugin']}
 
 setup_kwargs = {
     'name': 'poetry-exec-plugin',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'A plugin for poetry that allows you to execute scripts defined in your pyproject.toml, just like you can in npm or pipenv.',
     'long_description': '# poetry-exec-plugin\n\nA plugin for poetry that allows you to execute scripts defined in your pyproject.toml, just like you can in npm or pipenv\n\n## Installation\n\nInstallation requires poetry 1.2.0+. To install this plugin run:\n\n`poetry self add poetry-exec-plugin`\n\nFor other methods of installing plugins see the [poetry documentation](https://python-poetry.org/docs/master/plugins/#the-plugin-add-command).\n\n## Usage\n\nTo use this plugin, first define the scripts that you wish to be able to execute in your `pyproject.toml` file under a section called `tool.poetry-exec-plugin.commands`. For example:\n\n```toml\n[tool.poetry-exec-plugin.commands]\nhello-world = "TEXT=hello-world; echo $TEXT"\nlint = "flake8"\n```\n\nThis will define a script that you can then execute with the `poetry exec <script>` command. This will execute your script inside of the environment that poetry creates for you, allowing you to access the dependencies installed for your project. The script will also always run from the same directory as your `pyproject.toml` file. This mimics the behaviour of npm/yarn. For example:\n\n```bash\n$ poetry exec hello-world\nhello-world\n\n$ poetry exec lint\n./my_file.py:29:25: E222 multiple spaces after operator\n```\n\nAnything that you append to your exec command will be appended to the script. You can use this to pass extra flags and arguments to the commands in your scripts. For example:\n\n```bash\n$ poetry exec hello-world one two three\nhello-world one two three\n\n$ poetry exec lint --version\n3.9.2 (mccabe: 0.6.1, pycodestyle: 2.7.0, pyflakes: 2.3.1) CPython 3.9.0 on Darwin\n```\n\n## Publishing\n\nTo publish a new version,first bump the package version in `pyproject.toml` and commit your changes to the `main` branch (via pull request). Then in GitHub create a new release with the new version as the tag and name. You can use the handy auto release notes feature to populate the release description.\n',
     'author': 'keattang',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/keattang/poetry-exec-plugin',
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_rhkpi8fa_/tmpeik14eni_TarContainer/0/4.py", line 35, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_rhkpi8fa_/tmpeik14eni_TarContainer/0/4.py", line 35, column 0: CDATA terminal not found*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['poetry_exec_plugin'] package_data = \ {'': ['*']} install_requires = \
 ['poetry>=1.2.0.a2,<2.0.0', 'toml>=0.10.2,<0.11.0'] entry_points = \
 {'poetry.application.plugin': ['exec = poetry_exec_plugin.plugin:ExecPlugin']}
-setup_kwargs = { 'name': 'poetry-exec-plugin', 'version': '0.3.5',
+setup_kwargs = { 'name': 'poetry-exec-plugin', 'version': '0.3.6',
 'description': 'A plugin for poetry that allows you to execute scripts defined
 in your pyproject.toml, just like you can in npm or pipenv.',
 'long_description': '# poetry-exec-plugin\n\nA plugin for poetry that allows
 you to execute scripts defined in your pyproject.toml, just like you can in npm
 or pipenv\n\n## Installation\n\nInstallation requires poetry 1.2.0+. To install
 this plugin run:\n\n`poetry self add poetry-exec-plugin`\n\nFor other methods
 of installing plugins see the [poetry documentation](https://python-poetry.org/
```

### Comparing `poetry-exec-plugin-0.3.5/PKG-INFO` & `poetry-exec-plugin-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-exec-plugin
-Version: 0.3.5
+Version: 0.3.6
 Summary: A plugin for poetry that allows you to execute scripts defined in your pyproject.toml, just like you can in npm or pipenv.
 Home-page: https://github.com/keattang/poetry-exec-plugin
 License: MIT
 Author: keattang
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_rhkpi8fa_/tmpeik14eni_TarContainer/0/5", line 66, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_rhkpi8fa_/tmpeik14eni_TarContainer/0/5", line 66, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-exec-plugin Version: 0.3.5 Summary: A plugin
+Metadata-Version: 2.1 Name: poetry-exec-plugin Version: 0.3.6 Summary: A plugin
 for poetry that allows you to execute scripts defined in your pyproject.toml,
 just like you can in npm or pipenv. Home-page: https://github.com/keattang/
 poetry-exec-plugin License: MIT Author: keattang Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

