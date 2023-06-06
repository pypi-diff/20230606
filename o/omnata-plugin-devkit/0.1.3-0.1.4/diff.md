# Comparing `tmp/omnata_plugin_devkit-0.1.3.tar.gz` & `tmp/omnata_plugin_devkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_plugin_devkit-0.1.3.tar", max compression
+gzip compressed data, was "omnata_plugin_devkit-0.1.4.tar", max compression
```

## Comparing `omnata_plugin_devkit-0.1.3.tar` & `omnata_plugin_devkit-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    26526 2023-06-05 23:03:11.913088 omnata_plugin_devkit-0.1.3/LICENSE
--rw-r--r--   0        0        0       99 2023-06-05 23:03:11.913088 omnata_plugin_devkit-0.1.3/README.md
--rw-r--r--   0        0        0      640 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/__init__.py
--rw-r--r--   0        0        0    11266 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/airbyte_wrapper.py
--rw-r--r--   0        0        0     7280 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/cli/__init__.py
--rw-r--r--   0        0        0    26217 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/development_session.py
--rw-r--r--   0        0        0      492 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/initialiser.py
--rw-r--r--   0        0        0     1184 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja
--rw-r--r--   0        0        0     1222 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/APPLY.sql.jinja
--rw-r--r--   0        0        0     2630 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja
--rw-r--r--   0        0        0     2418 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja
--rw-r--r--   0        0        0     1221 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja
--rw-r--r--   0        0        0     1840 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja
--rw-r--r--   0        0        0     2257 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja
--rw-r--r--   0        0        0      818 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CREATE_SECRET_OBJECT.sql.jinja
--rw-r--r--   0        0        0      852 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja
--rw-r--r--   0        0        0     2999 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja
--rw-r--r--   0        0        0      372 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/manifest.yml.jinja
--rw-r--r--   0        0        0     4340 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/native_app_packaging.py
--rw-r--r--   0        0        0     2520 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/plugin_registration.py
--rw-r--r--   0        0        0      596 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/plugin_template/icon.svg
--rw-r--r--   0        0        0     3563 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/plugin_template/plugin.py
--rw-r--r--   0        0        0       30 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/plugin_template/requirements.txt
--rw-r--r--   0        0        0    18395 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/plugin_uploader.py
--rw-r--r--   0        0        0     7064 2023-06-05 23:03:11.917089 omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/test_step_definitions.py
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 omnata_plugin_devkit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/LICENSE
+-rw-r--r--   0        0        0       99 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/README.md
+-rw-r--r--   0        0        0      640 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/__init__.py
+-rw-r--r--   0        0        0    11266 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/airbyte_wrapper.py
+-rw-r--r--   0        0        0     7280 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/cli/__init__.py
+-rw-r--r--   0        0        0    26217 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/development_session.py
+-rw-r--r--   0        0        0      492 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/initialiser.py
+-rw-r--r--   0        0        0     1184 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja
+-rw-r--r--   0        0        0     1222 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/APPLY.sql.jinja
+-rw-r--r--   0        0        0     2630 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja
+-rw-r--r--   0        0        0     2418 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja
+-rw-r--r--   0        0        0     1221 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja
+-rw-r--r--   0        0        0     1840 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja
+-rw-r--r--   0        0        0     2257 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja
+-rw-r--r--   0        0        0      818 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CREATE_SECRET_OBJECT.sql.jinja
+-rw-r--r--   0        0        0      852 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja
+-rw-r--r--   0        0        0     2999 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja
+-rw-r--r--   0        0        0      372 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/manifest.yml.jinja
+-rw-r--r--   0        0        0     4340 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/native_app_packaging.py
+-rw-r--r--   0        0        0     2520 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/plugin_registration.py
+-rw-r--r--   0        0        0      596 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/plugin_template/icon.svg
+-rw-r--r--   0        0        0     3563 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/plugin_template/plugin.py
+-rw-r--r--   0        0        0       30 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/plugin_template/requirements.txt
+-rw-r--r--   0        0        0    18395 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/plugin_uploader.py
+-rw-r--r--   0        0        0     7064 2023-06-06 10:57:49.712754 omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/test_step_definitions.py
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 omnata_plugin_devkit-0.1.4/PKG-INFO
```

### Comparing `omnata_plugin_devkit-0.1.3/LICENSE` & `omnata_plugin_devkit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/pyproject.toml` & `omnata_plugin_devkit-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "omnata-plugin-devkit"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{include = "omnata_plugin_devkit", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 omnata_cli = "^0.1.4"
-omnata-plugin-runtime = "^0.1.11"
+omnata-plugin-runtime = "^0.1.21"
 #snowflake-connector-python = "^3"
 pandas = "*"
 jinja2 = "^3"
 pydantic = "^1"
 python-slugify = "^8"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/airbyte_wrapper.py` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/airbyte_wrapper.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/cli/__init__.py` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/development_session.py` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/development_session.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/APPLY.sql.jinja` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/APPLY.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/CREATE_SECRET_OBJECT.sql.jinja` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/CREATE_SECRET_OBJECT.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/native_app_packaging.py` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/native_app_packaging.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/plugin_registration.py` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/plugin_registration.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/plugin_template/icon.svg` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/plugin_template/icon.svg`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/plugin_template/plugin.py` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/plugin_template/plugin.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/plugin_uploader.py` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/plugin_uploader.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/src/omnata_plugin_devkit/test_step_definitions.py` & `omnata_plugin_devkit-0.1.4/src/omnata_plugin_devkit/test_step_definitions.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.3/PKG-INFO` & `omnata_plugin_devkit-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: omnata-plugin-devkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3,<4)
-Requires-Dist: omnata-plugin-runtime (>=0.1.11,<0.2.0)
+Requires-Dist: omnata-plugin-runtime (>=0.1.21,<0.2.0)
 Requires-Dist: omnata_cli (>=0.1.4,<0.2.0)
 Requires-Dist: pandas
 Requires-Dist: pydantic (>=1,<2)
 Requires-Dist: python-slugify (>=8,<9)
 Description-Content-Type: text/markdown
 
 # omnata-plugin-devkit
```

