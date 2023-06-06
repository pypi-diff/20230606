# Comparing `tmp/xpypact-0.4.1.tar.gz` & `tmp/xpypact-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpypact-0.4.1.tar", max compression
+gzip compressed data, was "xpypact-0.4.2.tar", max compression
```

## Comparing `xpypact-0.4.1.tar` & `xpypact-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2023-05-20 11:43:57.656528 xpypact-0.4.1/LICENSE
--rw-r--r--   0        0        0     3296 2023-05-20 11:43:57.656528 xpypact-0.4.1/README.rst
--rw-r--r--   0        0        0    17470 2023-05-20 11:44:11.505156 xpypact-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1199 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/__init__.py
--rw-r--r--   0        0        0      174 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/dao/__init__.py
--rw-r--r--   0        0        0     2241 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/dao/api.py
--rw-r--r--   0        0        0      168 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/dao/duckdb/__init__.py
--rw-r--r--   0        0        0     2870 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/dao/duckdb/create_schema.sql
--rw-r--r--   0        0        0     7978 2023-05-20 11:44:11.505156 xpypact-0.4.1/src/xpypact/dao/duckdb/implementation.py
--rw-r--r--   0        0        0    14156 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/data_arrays.py
--rw-r--r--   0        0        0     5307 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/data_frames.py
--rw-r--r--   0        0        0    12337 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/fluxes.py
--rw-r--r--   0        0        0     5862 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/inventory.py
--rw-r--r--   0        0        0     1965 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/nuclide.py
--rw-r--r--   0        0        0        0 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/py.typed
--rw-r--r--   0        0        0      515 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/run_data.py
--rw-r--r--   0        0        0     4924 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/time_step.py
--rw-r--r--   0        0        0       29 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/utils/__init__.py
--rw-r--r--   0        0        0      809 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/utils/io.py
--rw-r--r--   0        0        0        0 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/utils/py.typed
--rw-r--r--   0        0        0      768 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/utils/resource.py
--rw-r--r--   0        0        0      270 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/utils/types.py
--rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 xpypact-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-06 15:30:37.781278 xpypact-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3296 2023-06-06 15:30:37.781278 xpypact-0.4.2/README.rst
+-rw-r--r--   0        0        0    17279 2023-06-06 15:30:56.133574 xpypact-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1199 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/dao/__init__.py
+-rw-r--r--   0        0        0     2241 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/dao/api.py
+-rw-r--r--   0        0        0      234 2023-06-06 15:30:56.133574 xpypact-0.4.2/src/xpypact/dao/duckdb/__init__.py
+-rw-r--r--   0        0        0     2870 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/dao/duckdb/create_schema.sql
+-rw-r--r--   0        0        0     9057 2023-06-06 15:30:56.133574 xpypact-0.4.2/src/xpypact/dao/duckdb/implementation.py
+-rw-r--r--   0        0        0    14156 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/data_arrays.py
+-rw-r--r--   0        0        0     5307 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/data_frames.py
+-rw-r--r--   0        0        0    12337 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/fluxes.py
+-rw-r--r--   0        0        0     5862 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/inventory.py
+-rw-r--r--   0        0        0     1965 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/nuclide.py
+-rw-r--r--   0        0        0        0 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/py.typed
+-rw-r--r--   0        0        0      515 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/run_data.py
+-rw-r--r--   0        0        0     4924 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/time_step.py
+-rw-r--r--   0        0        0       29 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/utils/__init__.py
+-rw-r--r--   0        0        0      809 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/utils/io.py
+-rw-r--r--   0        0        0        0 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/utils/py.typed
+-rw-r--r--   0        0        0      768 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/utils/resource.py
+-rw-r--r--   0        0        0      270 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/utils/types.py
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 xpypact-0.4.2/PKG-INFO
```

### Comparing `xpypact-0.4.1/LICENSE` & `xpypact-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/README.rst` & `xpypact-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/pyproject.toml` & `xpypact-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xpypact"
-version = "0.4.1"
+version = "0.4.2"
 description = "\"Python tools to work with elements and isotopes\""
 authors = ["dvp <dmitri_portnov@yahoo.com>"]
 license = "MIT"
 homepage = "https://github.com/MC-kit/xpypact"
 repository = "https://github.com/MC-kit/xpypact"
 documentation = "https://xpypact.readthedocs.io"
 keywords = [
@@ -346,55 +346,33 @@
 # see https://github.com/gotcha/ipdb
 context=5
 
 [tool.tryceratops]
 include = ["src"]
 experimental = true
 
-[tool.pycln]
-path = "src"
-exclude = '''
-(
-    \.egg-info
-  | \.eggs
-  | \.git
-  | \.mypy_cache
-  | \.pytest_cache
-  | \.nox
-  | \.venv
-  | \.idea
-  | _build
-  | 3rd-party
-  | build
-  | build_configs
-  | data
-  | dist
-  | notebooks
-  | htmlcov
-  | wrk
-  | [Pp]arser
-  | tab\.py
-)
-'''
-#silence = true
-
 
 [tool.pydocstringformatter]
 write = true
 style = "pep257"
 exclude = ["tools/**","src/**/*_parser.py","src/**/*_tab.py"]
 strip-whitespaces = true
 max-line-length = 100
 summary-quotes-same-line = true
 
 
 [tool.pylint]
 good-names-rgxs=["."]  # a single character variable is okay
 logging-format-style="new"   # use {} in logging messages
 deprecated-modules=["six"]
+extension-pkg-allow-list=["duckdb"]
+disable=[
+    "wrong-import-order"  # this is `isort` responsibility
+]
+
 
 [tool.ruff]
 target-version = "py38"
 #see full list: https://beta.ruff.rs/docs/rules/#pyflakes-f
 #or run 'ruff linter' to see a brief list
 select= [
     "A", # flake8-builtins
@@ -563,15 +541,15 @@
 exclude = [
   "docs/source/conf.py",
   "__pycache__",
   "adhoc",
   "wrk",
   "*.egg-info",
   ".cache",
-  "notebooks/dvp/*.py"
+  "notebooks/dvp/*.py",
 ]
 # Assume Python 3.10.
 # target-version = "py310"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402"]
 "src/xpypact/fluxes.py" = ["F811"]
```

### Comparing `xpypact-0.4.1/src/xpypact/__init__.py` & `xpypact-0.4.2/src/xpypact/__init__.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/dao/api.py` & `xpypact-0.4.2/src/xpypact/dao/api.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/dao/duckdb/create_schema.sql` & `xpypact-0.4.2/src/xpypact/dao/duckdb/create_schema.sql`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/dao/duckdb/implementation.py` & `xpypact-0.4.2/src/xpypact/dao/duckdb/implementation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """Code to implement DuckDB DAO."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast
 
 from dataclasses import dataclass
+from multiprocessing import cpu_count
 from pathlib import Path
 
 import duckdb as db
 
 from xpypact import get_gamma, get_nuclides, get_run_data, get_time_steps, get_timestep_nuclides
 from xpypact.dao import DataAccessInterface
 from xpypact.utils.resource import path_resolver
 
 if TYPE_CHECKING:
     import pandas as pd
     import xarray as xr
 
 
+# On using DuckDB with multiple threads, see
+# https://duckdb.org/docs/guides/python/multiple_threads.html
+
+
 # noinspection SqlNoDataSourceInspection
 @dataclass
 class DuckDBDAO(DataAccessInterface):
     """Implementation of DataAccessInterface for DuckDB."""
 
     con: db.DuckDBPyConnection
 
@@ -79,110 +84,151 @@
         """
         self._save_run_data(ds, material_id, case_id)
         self._save_nuclides(ds)
         self._save_time_steps(ds)
         self._save_time_step_nuclides(ds)
         self._save_gamma(ds)
 
-    def load_rundata(self) -> pd.DataFrame:
+    def load_rundata(self) -> db.DuckDBPyRelation:
         """Load FISPACT run data as table.
 
         Returns:
-            FISPACT run data
+            FISPACT run data ad RelObj
         """
-        return self.con.execute("select * from rundata").df()
+        return self.con.table("rundata")
 
-    def load_nuclides(self) -> pd.DataFrame:
+    def load_nuclides(self) -> db.DuckDBPyRelation:
         """Load nuclide table.
 
         Returns:
             time nuclide
         """
-        return self.con.execute("select * from nuclide").df()
+        return self.con.table("nuclide")
 
-    def load_time_steps(self) -> pd.DataFrame:
+    def load_time_steps(self) -> db.DuckDBPyRelation:
         """Load time step table.
 
         Returns:
             time step table
         """
-        return self.con.execute("select * from timestep").df()
+        return self.con.table("timestep")
 
-    def load_time_step_nuclides(self) -> pd.DataFrame:
+    def load_time_step_nuclides(self) -> db.DuckDBPyRelation:
         """Load time step x nuclides table.
 
         Returns:
             time step x nuclides table
         """
-        return self.con.execute("select * from timestep_nuclide").df()
+        return self.con.table("timestep_nuclide")
 
-    def load_gamma(self, time_step_number: int | None = None) -> pd.DataFrame:
+    def load_gamma(self, time_step_number: int | None = None) -> db.DuckDBPyRelation:
         """Load time step x gamma table.
 
         Args:
             time_step_number: filter for time_step_number
 
         Returns:
             time step x gamma table
         """
         sql = "select * from timestep_gamma"
         if time_step_number is not None:
             sql += f" where time_step_number == {time_step_number}"
-        return self.con.execute(sql).df()
+        return self.con.sql(sql)
 
-    def _save_run_data(self, ds: xr.Dataset, material_id=1, case_id=1):
+    def _save_run_data(self, ds: xr.Dataset, material_id=1, case_id=1) -> None:
         _table = get_run_data(ds)
         _table = _add_material_and_case_columns(_table, material_id, case_id)
-        self.con.execute("insert into rundata from _table")
-        self.con.commit()
+        sql = """
+            begin transaction;
+            insert into rundata from _table;
+            commit;
+            """
+        self.con.sql(sql)
 
     def _save_nuclides(self, ds: xr.Dataset):
         _table = get_nuclides(ds)  # noqa: F841 - used below
-        sql = "insert or ignore into nuclide select * from _table"
-        self.con.execute(sql)
-        self.con.commit()
+        sql = """
+            begin transaction;
+            insert or ignore into nuclide select * from _table;
+            commit;
+        """
+        self.con.sql(sql)
 
     def _save_time_steps(self, ds: xr.Dataset, material_id=1, case_id=1):
         _table = get_time_steps(ds)
         _table = _add_material_and_case_columns(_table, material_id, case_id)
-        self.con.execute("insert into timestep from _table")
+        sql = """
+            begin transaction;
+            insert into timestep from _table;
+            commit;
+            """
+        self.con.execute(sql)
         self.con.commit()
 
     def _save_time_step_nuclides(self, ds: xr.Dataset, material_id=1, case_id=1):
         _table = get_timestep_nuclides(ds)
         _table = _add_material_and_case_columns(_table, material_id, case_id)
-        self.con.execute("insert into timestep_nuclide from _table")
-        self.con.commit()
+        sql = """
+            begin transaction;
+            insert into timestep_nuclide from _table;
+            commit;
+            """
+        self.con.sql(sql)
 
     def _save_gamma(self, ds: xr.Dataset, material_id=1, case_id=1):
         _table = get_gamma(ds)
         _table = _add_material_and_case_columns(_table, material_id, case_id)
-        self.con.execute("insert into timestep_gamma from _table")
-        self.con.commit()
+        self.con.sql(
+            """
+            begin transaction;
+            insert into timestep_gamma from _table;
+            commit;
+            """,
+        )
+
+
+def compute_optimal_row_group_size(frame_size: int, _cpu_count: int = 0) -> int:
+    """Compute DuckDB row group size for writing to parquet files.
+
+    This should optimize speed of reading from parquet files.
+
+    Args:
+        frame_size: length of rows to be writed
+        _cpu_count: number to split the rows
+
+    Returns:
+        the row group size
+    """
+    if not _cpu_count:
+        _cpu_count = max(4, cpu_count())
+    size = frame_size // _cpu_count
+    return min(max(size, 2048), 1_000_000)
 
 
 def write_parquet(target_dir: Path, ds: xr.Dataset, material_id: int, case_id: int) -> None:
     """Store xpypact dataset to parquet directories.
 
-    Create in 4 subdirectories in `target_dir` for run_data, time_steps,
+    Create in 4 subdirectories in `target_dir` for data subjects run_data, time_steps,
     time_step_nuclides, and gamma dataframes.
-    Save the dataframes as parquet files. The arguments material_id and case_id
-    allow to organize two level Hive partitioning. Other inventories can be
-    saved in the same `target_dir` as long as the material_id and case_id are
-    unique for an inventory.
+    Save the dataframes as parquet files.
+    Hive partiotioning is not used in this version, because resulting partions are too small.
+    The data for  can be  saved in the same `target_dir` as long as the material_id and case_id are
+    unique for an data subject.
 
     This structure can be easily and efficiently accessed from DuckDB as external data.
     For instance to collect all the inventories:
     ```
         select * from read_parquet('<target_dir>/inventory/*/*/*.parquet', hive_partitioning=true)
     ```
 
     We use in memory DuckDB instance to transfer data to parquet to ensure compatibility
     for later reading back to DuckDB.
 
+    See about row_group_size: https://duckdb.org/docs/data/parquet/tips
+
     Args:
         target_dir: root directory to store a dataset in subdirectories
         ds: dataset to store
         material_id: the level 1 key to distinguish with other datasets in the folder,
                      may correspond to material in R2S
         case_id: the level 2 key, may correspond neutron group or case in R2S of fispact run.
                  The case may be registered in the database to provide additional information.
@@ -190,33 +236,34 @@
     to_proces: dict[str, pd.DataFrame] = {
         "run_data": get_run_data(ds),
         "nuclides": get_nuclides(ds),
         "time_steps": get_time_steps(ds),
         "timestep_nuclides": get_timestep_nuclides(ds),
         "gamma": get_gamma(ds),
     }
-    con = db.connect(":memory:")
+    con = db.connect()
     try:
         for k, v in to_proces.items():
             path: Path = target_dir / k
             path.mkdir(parents=True, exist_ok=True)
-            frame = _add_material_and_case_columns(  # noqa: F841 - used in query
+            frame = _add_material_and_case_columns(
                 v,
                 material_id,
                 case_id,
             )
-            time_step_partition = "time_step_number, " if "time_step_number" in v.columns else ""
             sql = f"""
                 copy
                 (select * from frame)
                 to '{path}'
                 (
                     format parquet,
-                    partition_by ({time_step_partition}material_id, case_id),
-                    overwrite_or_ignore true
+                    per_thread_output true,
+                    overwrite_or_ignore true,
+                    filename_pattern "data_material_id={material_id}_case_id={case_id}_{{i}}",
+                    row_group_size {compute_optimal_row_group_size(frame.shape[0])}
                 )
                 """  # noqa: S608 - sql injection
             con.execute(sql)
     finally:
         con.close()
```

### Comparing `xpypact-0.4.1/src/xpypact/data_arrays.py` & `xpypact-0.4.2/src/xpypact/data_arrays.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/data_frames.py` & `xpypact-0.4.2/src/xpypact/data_frames.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/fluxes.py` & `xpypact-0.4.2/src/xpypact/fluxes.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/inventory.py` & `xpypact-0.4.2/src/xpypact/inventory.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/nuclide.py` & `xpypact-0.4.2/src/xpypact/nuclide.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/run_data.py` & `xpypact-0.4.2/src/xpypact/run_data.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/time_step.py` & `xpypact-0.4.2/src/xpypact/time_step.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/utils/io.py` & `xpypact-0.4.2/src/xpypact/utils/io.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/src/xpypact/utils/resource.py` & `xpypact-0.4.2/src/xpypact/utils/resource.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.1/PKG-INFO` & `xpypact-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpypact
-Version: 0.4.1
+Version: 0.4.2
 Summary: "Python tools to work with elements and isotopes"
 Home-page: https://github.com/MC-kit/xpypact
 License: MIT
 Keywords: element,nuclide,isotope,abundance,FISPACT,activation,duckdb,parquet
 Author: dvp
 Author-email: dmitri_portnov@yahoo.com
 Requires-Python: >=3.8.1,<4.0
```

