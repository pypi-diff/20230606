# Comparing `tmp/molecule-qemu-0.4.2.tar.gz` & `tmp/molecule-qemu-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.4.2.tar", last modified: Mon Jun  5 04:49:33 2023, max compression
+gzip compressed data, was "molecule-qemu-0.4.3.tar", last modified: Tue Jun  6 04:55:26 2023, max compression
```

## Comparing `molecule-qemu-0.4.2.tar` & `molecule-qemu-0.4.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.336269 molecule-qemu-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.324269 molecule-qemu-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.328269 molecule-qemu-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/.github/workflows/pycodestyle.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.328269 molecule-qemu-0.4.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-05 04:49:33.336269 molecule-qemu-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.328269 molecule-qemu-0.4.2/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.332270 molecule-qemu-0.4.2/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.324269 molecule-qemu-0.4.2/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.332270 molecule-qemu-0.4.2/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.332270 molecule-qemu-0.4.2/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.336269 molecule-qemu-0.4.2/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:49:33.332270 molecule-qemu-0.4.2/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-05 04:49:33.000000 molecule-qemu-0.4.2/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-05 04:49:33.000000 molecule-qemu-0.4.2/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 04:49:33.000000 molecule-qemu-0.4.2/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 04:49:33.000000 molecule-qemu-0.4.2/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 04:49:33.000000 molecule-qemu-0.4.2/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 04:49:33.000000 molecule-qemu-0.4.2/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-05 04:49:21.000000 molecule-qemu-0.4.2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 04:49:33.336269 molecule-qemu-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.391897 molecule-qemu-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.github/workflows/pycodestyle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.391897 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 04:55:26.000000 molecule-qemu-0.4.3/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 04:55:17.000000 molecule-qemu-0.4.3/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 04:55:26.395897 molecule-qemu-0.4.3/setup.cfg
```

### Comparing `molecule-qemu-0.4.2/.github/workflows/python-publish.yml` & `molecule-qemu-0.4.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/.github/workflows/release.yml` & `molecule-qemu-0.4.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/.gitignore` & `molecule-qemu-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/.yamllint` & `molecule-qemu-0.4.3/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/LICENSE` & `molecule-qemu-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/Makefile` & `molecule-qemu-0.4.3/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/PKG-INFO` & `molecule-qemu-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.2
+Version: 0.4.3
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.4.2/README.md` & `molecule-qemu-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/molecule_qemu/driver.py` & `molecule-qemu-0.4.3/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.4.3/molecule_qemu/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.4.3/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.4.3/molecule_qemu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.2
+Version: 0.4.3
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.4.2/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.4.3/molecule_qemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.2/pyproject.toml` & `molecule-qemu-0.4.3/pyproject.toml`

 * *Files identical despite different names*

