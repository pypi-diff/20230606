# Comparing `tmp/batcave-42.0.0.tar.gz` & `tmp/batcave-42.0.0rc19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batcave-42.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "batcave-42.0.0rc19.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `batcave-42.0.0.tar` & `batcave-42.0.0rc19.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     4792 2023-06-06 19:51:17.123964 batcave-42.0.0/.gitignore
--rw-r--r--   0        0        0     3569 2023-06-06 19:51:17.123964 batcave-42.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0       23 2023-06-06 19:51:17.123964 batcave-42.0.0/.p4cfg
--rw-r--r--   0        0        0     5043 2023-06-06 19:51:17.123964 batcave-42.0.0/.p4ignore
--rw-r--r--   0        0        0      158 2023-06-06 19:51:17.123964 batcave-42.0.0/.pypirc
--rw-r--r--   0        0        0       39 2023-06-06 19:51:17.123964 batcave-42.0.0/.readthedocs.yml
--rw-r--r--   0        0        0     4034 2023-06-06 19:51:17.123964 batcave-42.0.0/.vscode/.ropeproject/config.py
--rw-r--r--   0        0        0      592 2023-06-06 19:51:17.124964 batcave-42.0.0/.vscode/.ropeproject/objectdb
--rw-r--r--   0        0        0     5757 2023-06-06 19:51:17.124964 batcave-42.0.0/.vscode/launch.json
--rw-r--r--   0        0        0      468 2023-06-06 19:51:17.124964 batcave-42.0.0/.vscode/tasks.json
--rw-r--r--   0        0        0    38215 2023-06-06 19:51:17.124964 batcave-42.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       86 2023-06-06 19:51:17.124964 batcave-42.0.0/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2023-06-06 19:51:17.124964 batcave-42.0.0/LICENSE
--rw-r--r--   0        0        0       93 2023-06-06 19:51:17.124964 batcave-42.0.0/MANIFEST.in
--rw-r--r--   0        0        0     1017 2023-06-06 19:51:17.124964 batcave-42.0.0/README.md
--rw-r--r--   0        0        0     1832 2023-06-06 19:51:43.154917 batcave-42.0.0/batcave/__init__.py
--rw-r--r--   0        0        0     5483 2023-06-06 19:51:17.124964 batcave-42.0.0/batcave/automation.py
--rw-r--r--   0        0        0    14410 2023-06-06 19:51:17.124964 batcave-42.0.0/batcave/cloudmgr.py
--rw-r--r--   0        0        0    74524 2023-06-06 19:51:17.124964 batcave-42.0.0/batcave/cms.py
--rw-r--r--   0        0        0     8590 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/commander.py
--rw-r--r--   0        0        0     9565 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/configmgr.py
--rw-r--r--   0        0        0    27694 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/data.py
--rw-r--r--   0        0        0    31760 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/expander.py
--rw-r--r--   0        0        0     8908 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/fileutil.py
--rw-r--r--   0        0        0    10747 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/gui.py
--rw-r--r--   0        0        0    28879 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/iispy.py
--rw-r--r--   0        0        0    17890 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/k8s.py
--rw-r--r--   0        0        0    10608 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/lang.py
--rw-r--r--   0        0        0     3140 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/menu.py
--rw-r--r--   0        0        0     2378 2023-06-06 19:51:17.125964 batcave-42.0.0/batcave/netutil.py
--rw-r--r--   0        0        0     3842 2023-06-06 19:51:17.126964 batcave-42.0.0/batcave/platarch.py
--rw-r--r--   0        0        0        0 2023-06-06 19:51:17.149964 batcave-42.0.0/batcave/py.typed
--rw-r--r--   0        0        0    13093 2023-06-06 19:51:17.126964 batcave-42.0.0/batcave/qbpy.py
--rw-r--r--   0        0        0    28247 2023-06-06 19:51:17.126964 batcave-42.0.0/batcave/reporter.py
--rw-r--r--   0        0        0    52830 2023-06-06 19:51:17.126964 batcave-42.0.0/batcave/servermgr.py
--rw-r--r--   0        0        0    11200 2023-06-06 19:51:17.126964 batcave-42.0.0/batcave/serverpath.py
--rw-r--r--   0        0        0     7801 2023-06-06 19:51:17.126964 batcave-42.0.0/batcave/statemachine.py
--rw-r--r--   0        0        0    23468 2023-06-06 19:51:17.126964 batcave-42.0.0/batcave/sysutil.py
--rw-r--r--   0        0        0     5429 2023-06-06 19:51:17.126964 batcave-42.0.0/batcave/tcpy.py
--rw-r--r--   0        0        0     3340 2023-06-06 19:51:17.126964 batcave-42.0.0/batcave/version.py
--rw-r--r--   0        0        0      634 2023-06-06 19:51:17.126964 batcave-42.0.0/docs/Makefile
--rw-r--r--   0        0        0     3747 2023-06-06 19:51:17.126964 batcave-42.0.0/docs/batcave.rst
--rw-r--r--   0        0        0     9167 2023-06-06 19:51:17.127964 batcave-42.0.0/docs/coding_standards.py
--rw-r--r--   0        0        0     2109 2023-06-06 19:51:17.127964 batcave-42.0.0/docs/conf.py
--rw-r--r--   0        0        0      469 2023-06-06 19:51:17.127964 batcave-42.0.0/docs/index.rst
--rw-r--r--   0        0        0      795 2023-06-06 19:51:17.127964 batcave-42.0.0/docs/make.bat
--rw-r--r--   0        0        0       65 2023-06-06 19:51:17.127964 batcave-42.0.0/docs/modules.rst
--rw-r--r--   0        0        0      229 2023-06-06 19:51:17.127964 batcave-42.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     2748 2023-06-06 19:51:43.155917 batcave-42.0.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-06 19:51:17.127964 batcave-42.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1253 2023-06-06 19:51:17.127964 batcave-42.0.0/tests/test_lang.py
--rw-r--r--   0        0        0     2744 2023-06-06 19:51:17.127964 batcave-42.0.0/tests/test_statemachine.py
--rw-r--r--   0        0        0     3062 2023-06-06 19:51:17.127964 batcave-42.0.0/tests/test_sysutil.py
--rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 batcave-42.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4792 2023-06-02 20:09:51.007814 batcave-42.0.0rc19/.gitignore
+-rw-r--r--   0        0        0     3569 2023-06-02 20:09:51.007814 batcave-42.0.0rc19/.gitlab-ci.yml
+-rw-r--r--   0        0        0       23 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/.p4cfg
+-rw-r--r--   0        0        0     5043 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/.p4ignore
+-rw-r--r--   0        0        0      158 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/.pypirc
+-rw-r--r--   0        0        0       39 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/.readthedocs.yml
+-rw-r--r--   0        0        0     4034 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/.vscode/.ropeproject/config.py
+-rw-r--r--   0        0        0      592 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/.vscode/.ropeproject/objectdb
+-rw-r--r--   0        0        0     5757 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/.vscode/launch.json
+-rw-r--r--   0        0        0      468 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/.vscode/tasks.json
+-rw-r--r--   0        0        0    38215 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/CHANGELOG.md
+-rw-r--r--   0        0        0       86 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/LICENSE
+-rw-r--r--   0        0        0       93 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/MANIFEST.in
+-rw-r--r--   0        0        0     1017 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/README.md
+-rw-r--r--   0        0        0     1836 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/batcave/__init__.py
+-rw-r--r--   0        0        0     5483 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/batcave/automation.py
+-rw-r--r--   0        0        0    14410 2023-06-02 20:09:51.008813 batcave-42.0.0rc19/batcave/cloudmgr.py
+-rw-r--r--   0        0        0    74524 2023-06-02 20:09:51.009814 batcave-42.0.0rc19/batcave/cms.py
+-rw-r--r--   0        0        0     8590 2023-06-02 20:09:51.009814 batcave-42.0.0rc19/batcave/commander.py
+-rw-r--r--   0        0        0     9565 2023-06-02 20:09:51.009814 batcave-42.0.0rc19/batcave/configmgr.py
+-rw-r--r--   0        0        0    27694 2023-06-02 20:09:51.009814 batcave-42.0.0rc19/batcave/data.py
+-rw-r--r--   0        0        0    31760 2023-06-02 20:09:51.009814 batcave-42.0.0rc19/batcave/expander.py
+-rw-r--r--   0        0        0     8908 2023-06-02 20:09:51.009814 batcave-42.0.0rc19/batcave/fileutil.py
+-rw-r--r--   0        0        0    10747 2023-06-02 20:09:51.009814 batcave-42.0.0rc19/batcave/gui.py
+-rw-r--r--   0        0        0    28879 2023-06-02 20:09:51.010814 batcave-42.0.0rc19/batcave/iispy.py
+-rw-r--r--   0        0        0    17890 2023-06-02 20:09:51.010814 batcave-42.0.0rc19/batcave/k8s.py
+-rw-r--r--   0        0        0    10608 2023-06-02 20:09:51.010814 batcave-42.0.0rc19/batcave/lang.py
+-rw-r--r--   0        0        0     3140 2023-06-02 20:09:51.010814 batcave-42.0.0rc19/batcave/menu.py
+-rw-r--r--   0        0        0     2378 2023-06-02 20:09:51.010814 batcave-42.0.0rc19/batcave/netutil.py
+-rw-r--r--   0        0        0     3842 2023-06-02 20:09:51.010814 batcave-42.0.0rc19/batcave/platarch.py
+-rw-r--r--   0        0        0        0 2023-06-02 20:09:51.033813 batcave-42.0.0rc19/batcave/py.typed
+-rw-r--r--   0        0        0    13093 2023-06-02 20:09:51.010814 batcave-42.0.0rc19/batcave/qbpy.py
+-rw-r--r--   0        0        0    28247 2023-06-02 20:09:51.010814 batcave-42.0.0rc19/batcave/reporter.py
+-rw-r--r--   0        0        0    52830 2023-06-02 20:09:51.010814 batcave-42.0.0rc19/batcave/servermgr.py
+-rw-r--r--   0        0        0    11200 2023-06-02 20:09:51.010814 batcave-42.0.0rc19/batcave/serverpath.py
+-rw-r--r--   0        0        0     7801 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/batcave/statemachine.py
+-rw-r--r--   0        0        0    23468 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/batcave/sysutil.py
+-rw-r--r--   0        0        0     5429 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/batcave/tcpy.py
+-rw-r--r--   0        0        0     3340 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/batcave/version.py
+-rw-r--r--   0        0        0      634 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/docs/Makefile
+-rw-r--r--   0        0        0     3747 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/docs/batcave.rst
+-rw-r--r--   0        0        0     9167 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/docs/coding_standards.py
+-rw-r--r--   0        0        0     2109 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/docs/conf.py
+-rw-r--r--   0        0        0      469 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/docs/make.bat
+-rw-r--r--   0        0        0       65 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/docs/modules.rst
+-rw-r--r--   0        0        0      229 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/docs/requirements.txt
+-rw-r--r--   0        0        0     2752 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/tests/__init__.py
+-rw-r--r--   0        0        0     1253 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/tests/test_lang.py
+-rw-r--r--   0        0        0     2744 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/tests/test_statemachine.py
+-rw-r--r--   0        0        0     3062 2023-06-02 20:09:51.011813 batcave-42.0.0rc19/tests/test_sysutil.py
+-rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 batcave-42.0.0rc19/PKG-INFO
```

### Comparing `batcave-42.0.0/.gitignore` & `batcave-42.0.0rc19/.gitignore`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/.gitlab-ci.yml` & `batcave-42.0.0rc19/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/.p4ignore` & `batcave-42.0.0rc19/.p4ignore`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/.vscode/.ropeproject/config.py` & `batcave-42.0.0rc19/.vscode/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/.vscode/.ropeproject/objectdb` & `batcave-42.0.0rc19/.vscode/.ropeproject/objectdb`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/.vscode/launch.json` & `batcave-42.0.0rc19/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/CHANGELOG.md` & `batcave-42.0.0rc19/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/LICENSE` & `batcave-42.0.0rc19/LICENSE`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/README.md` & `batcave-42.0.0rc19/README.md`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/__init__.py` & `batcave-42.0.0rc19/batcave/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
            '__author__', '__email__',
            '__license__', '__copyright__')
 
 __title__ = 'BatCave'
 __summary__ = 'Python Programming Toolkit'
 __uri__ = 'https://gitlab.com/arisilon/batcave/'
 
-__version__ = '42.0.0'
+__version__ = '42.0.0rc19'
 __build_name__ = '{var:build_name}'
 __build_date__ = '{var:build_date}'
 
 __author__ = 'Jeffery G. Smith'
 __email__ = 'web@pobox.com'
 
 __license__ = 'MIT'
```

### Comparing `batcave-42.0.0/batcave/automation.py` & `batcave-42.0.0rc19/batcave/automation.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/cloudmgr.py` & `batcave-42.0.0rc19/batcave/cloudmgr.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/cms.py` & `batcave-42.0.0rc19/batcave/cms.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/commander.py` & `batcave-42.0.0rc19/batcave/commander.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/configmgr.py` & `batcave-42.0.0rc19/batcave/configmgr.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/data.py` & `batcave-42.0.0rc19/batcave/data.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/expander.py` & `batcave-42.0.0rc19/batcave/expander.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/fileutil.py` & `batcave-42.0.0rc19/batcave/fileutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/gui.py` & `batcave-42.0.0rc19/batcave/gui.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/iispy.py` & `batcave-42.0.0rc19/batcave/iispy.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/k8s.py` & `batcave-42.0.0rc19/batcave/k8s.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/lang.py` & `batcave-42.0.0rc19/batcave/lang.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/menu.py` & `batcave-42.0.0rc19/batcave/menu.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/netutil.py` & `batcave-42.0.0rc19/batcave/netutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/platarch.py` & `batcave-42.0.0rc19/batcave/platarch.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/qbpy.py` & `batcave-42.0.0rc19/batcave/qbpy.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/reporter.py` & `batcave-42.0.0rc19/batcave/reporter.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/servermgr.py` & `batcave-42.0.0rc19/batcave/servermgr.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/serverpath.py` & `batcave-42.0.0rc19/batcave/serverpath.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/statemachine.py` & `batcave-42.0.0rc19/batcave/statemachine.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/sysutil.py` & `batcave-42.0.0rc19/batcave/sysutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/tcpy.py` & `batcave-42.0.0rc19/batcave/tcpy.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/batcave/version.py` & `batcave-42.0.0rc19/batcave/version.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/docs/Makefile` & `batcave-42.0.0rc19/docs/Makefile`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/docs/batcave.rst` & `batcave-42.0.0rc19/docs/batcave.rst`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/docs/coding_standards.py` & `batcave-42.0.0rc19/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/docs/conf.py` & `batcave-42.0.0rc19/docs/conf.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/docs/make.bat` & `batcave-42.0.0rc19/docs/make.bat`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/pyproject.toml` & `batcave-42.0.0rc19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "wmi.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "42.0.0"
+current_version = "42.0.0rc19"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip-ci]"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `batcave-42.0.0/tests/test_lang.py` & `batcave-42.0.0rc19/tests/test_lang.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/tests/test_statemachine.py` & `batcave-42.0.0rc19/tests/test_statemachine.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/tests/test_sysutil.py` & `batcave-42.0.0rc19/tests/test_sysutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.0/PKG-INFO` & `batcave-42.0.0rc19/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batcave
-Version: 42.0.0
+Version: 42.0.0rc19
 Summary: BatCave Utilities module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

