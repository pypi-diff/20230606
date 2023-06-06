# Comparing `tmp/LbProdRun-1.4.1.tar.gz` & `tmp/LbProdRun-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbProdRun-1.4.1.tar", last modified: Wed Apr 19 09:27:16 2023, max compression
+gzip compressed data, was "LbProdRun-1.5.0.tar", last modified: Tue Jun  6 06:44:27 2023, max compression
```

## Comparing `LbProdRun-1.4.1.tar` & `LbProdRun-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:16.840000 LbProdRun-1.4.1/
--rw-r--r--   0 root         (0) root         (0)     2055 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2482 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    16310 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2655 2023-04-19 09:27:16.840000 LbProdRun-1.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2233 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/README.md
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-19 09:27:16.844000 LbProdRun-1.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:16.836000 LbProdRun-1.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:16.840000 LbProdRun-1.4.1/src/LbProdRun/
--rw-r--r--   0 root         (0) root         (0)    12272 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/src/LbProdRun/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/src/LbProdRun/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/src/LbProdRun/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:16.840000 LbProdRun-1.4.1/src/LbProdRun.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2655 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      458 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:16.840000 LbProdRun-1.4.1/tests/
--rw-r--r--   0 root         (0) root         (0)     4749 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     3028 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/tests/test_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    16310 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:44:27.896000 LbProdRun-1.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/src/LbProdRun/
+-rw-r--r--   0 root         (0) root         (0)    12272 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/src/LbProdRun/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/src/LbProdRun/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4715 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/src/LbProdRun/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/src/LbProdRun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4704 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/tests/test_options.py
```

### Comparing `LbProdRun-1.4.1/.gitignore` & `LbProdRun-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.1/.gitlab-ci.yml` & `LbProdRun-1.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.1/.pre-commit-config.yaml` & `LbProdRun-1.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.1/.pylintrc` & `LbProdRun-1.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.1/LICENSE` & `LbProdRun-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.1/PKG-INFO` & `LbProdRun-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbProdRun
-Version: 1.4.1
+Version: 1.5.0
 Summary: CLI for running LHCb applications from LHCbDIRAC
 Home-page: https://gitlab.cern.ch/lhcb-core/lbprodrun
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `LbProdRun-1.4.1/README.md` & `LbProdRun-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.1/setup.cfg` & `LbProdRun-1.5.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 [options]
 python_requires = >=3.9
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	click ~=8.0
+	click >=8.0
 	lbenv
-	pydantic ~=1.9.1
-	typer[all] ~=0.4.1
+	pydantic >=1.10
+	typer[all] >=0.4.1
 	packaging
-	pyyaml ~=6.0
+	pyyaml >=6.0
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 testing = 
 	black
```

### Comparing `LbProdRun-1.4.1/src/LbProdRun/__init__.py` & `LbProdRun-1.5.0/src/LbProdRun/__init__.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.1/src/LbProdRun/__main__.py` & `LbProdRun-1.5.0/src/LbProdRun/__main__.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.1/src/LbProdRun/models.py` & `LbProdRun-1.5.0/src/LbProdRun/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,36 +64,36 @@
         entrypoint: str
         extra_options: dict[str, Any]
         extra_args: list[str] = []
 
     options: Union[LegacyOptions, LbExecOptions]
 
     class Input(BaseModel):
-        files: Optional[list[str]]
-        xml_summary_file: Optional[str]
-        xml_file_catalog: Optional[str]
-        run_number: Optional[int]
-        tck: Optional[str]
+        files: Optional[list[str]] = None
+        xml_summary_file: Optional[str] = None
+        xml_file_catalog: Optional[str] = None
+        run_number: Optional[int] = None
+        tck: Optional[str] = None
         n_of_events: int = -1
-        first_event_number: Optional[int]
+        first_event_number: Optional[int] = None
 
     input: Input = Input()
 
     class Output(BaseModel):
         prefix: str
         types: list[str]
         histogram_file: Optional[str]
         compression: Optional[str]
 
     output: Output
 
     class DBTags(BaseModel):
-        dddb_tag: Optional[str]
-        conddb_tag: Optional[str]
-        dq_tag: Optional[str]
+        dddb_tag: Optional[str] = None
+        conddb_tag: Optional[str] = None
+        dq_tag: Optional[str] = None
 
     db_tags: DBTags = DBTags()
 
 
 KNOWN_SPECS = {
     1: JobSpecV1,
 }
```

### Comparing `LbProdRun-1.4.1/src/LbProdRun.egg-info/PKG-INFO` & `LbProdRun-1.5.0/src/LbProdRun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbProdRun
-Version: 1.4.1
+Version: 1.5.0
 Summary: CLI for running LHCb applications from LHCbDIRAC
 Home-page: https://gitlab.cern.ch/lhcb-core/lbprodrun
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `LbProdRun-1.4.1/tests/test_cli.py` & `LbProdRun-1.5.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     assert result.exit_code != 0
     assert "is a directory" in result.stdout
 
     tmp_path = tmp_path / "prod_spec.json"
 
     result = runner.invoke(app, str(tmp_path))
     assert result.exit_code != 0
-    assert "does not exist" in result.stdout
 
     tmp_path.write_text("")
     result = runner.invoke(app, str(tmp_path))
     assert result.exit_code >= 64
     assert "Failed to parse" in result.stdout
 
     tmp_path.write_text("{}")
```

### Comparing `LbProdRun-1.4.1/tests/test_options.py` & `LbProdRun-1.5.0/tests/test_options.py`

 * *Files identical despite different names*

