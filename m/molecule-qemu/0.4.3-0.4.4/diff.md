# Comparing `tmp/molecule-qemu-0.4.3.tar.gz` & `tmp/molecule-qemu-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.4.3.tar", last modified: Tue Jun  6 04:55:26 2023, max compression
+gzip compressed data, was "molecule-qemu-0.4.4.tar", last modified: Tue Jun  6 05:14:28 2023, max compression
```

## Comparing `molecule-qemu-0.4.3.tar` & `molecule-qemu-0.4.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.391897 molecule-qemu-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.github/workflows/pycodestyle.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.391897 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.775431 molecule-qemu-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-06 05:14:28.000000 molecule-qemu-0.4.4/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-06 05:14:28.000000 molecule-qemu-0.4.4/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:14:28.000000 molecule-qemu-0.4.4/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 05:14:28.000000 molecule-qemu-0.4.4/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 05:14:28.000000 molecule-qemu-0.4.4/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 05:14:28.000000 molecule-qemu-0.4.4/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 05:14:15.000000 molecule-qemu-0.4.4/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 05:14:28.779430 molecule-qemu-0.4.4/setup.cfg
```

### Comparing `molecule-qemu-0.4.3/.gitignore` & `molecule-qemu-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.3/.yamllint` & `molecule-qemu-0.4.4/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.3/LICENSE` & `molecule-qemu-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.3/Makefile` & `molecule-qemu-0.4.4/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.3/PKG-INFO` & `molecule-qemu-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.3
+Version: 0.4.4
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.4.3/README.md` & `molecule-qemu-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.3/molecule_qemu/driver.py` & `molecule-qemu-0.4.4/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.3/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.4.4/molecule_qemu/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.3/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.4.4/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.3/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.4.4/molecule_qemu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.3
+Version: 0.4.4
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.4.3/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.4.4/molecule_qemu.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+.ansible-lint
 .gitignore
 .yamllint
 LICENSE
 Makefile
 README.md
 pyproject.toml
 requirements.yml
 setup.cfg
-.github/workflows/ansible-lint.yml
-.github/workflows/pycodestyle.yml
-.github/workflows/python-publish.yml
+.github/workflows/lint.yml
+.github/workflows/publish.yml
 .github/workflows/release.yml
 .vscode/settings.json
 molecule_qemu/__init__.py
 molecule_qemu/driver.py
 molecule_qemu.egg-info/PKG-INFO
 molecule_qemu.egg-info/SOURCES.txt
 molecule_qemu.egg-info/dependency_links.txt
```

### Comparing `molecule-qemu-0.4.3/pyproject.toml` & `molecule-qemu-0.4.4/pyproject.toml`

 * *Files identical despite different names*

