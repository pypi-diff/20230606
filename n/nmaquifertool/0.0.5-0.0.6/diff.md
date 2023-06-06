# Comparing `tmp/nmaquifertool-0.0.5.tar.gz` & `tmp/nmaquifertool-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmaquifertool-0.0.5.tar", last modified: Tue Jun  6 19:31:06 2023, max compression
+gzip compressed data, was "nmaquifertool-0.0.6.tar", last modified: Tue Jun  6 19:41:15 2023, max compression
```

## Comparing `nmaquifertool-0.0.5.tar` & `nmaquifertool-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.653514 nmaquifertool-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.645514 nmaquifertool-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.645514 nmaquifertool-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/.github/workflows/format_code.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 19:31:06.653514 nmaquifertool-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.649514 nmaquifertool-0.0.5/nmaquifertool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.649514 nmaquifertool-0.0.5/nmat/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/bc_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.649514 nmaquifertool-0.0.5/nmat/config/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/geo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.649514 nmaquifertool-0.0.5/nmat/indata/
--rw-r--r--   0 runner    (1001) docker     (123)   536602 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/indata/sp2023berncowls.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/onyx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/ose_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.653514 nmaquifertool-0.0.5/nmat/output/
--rw-r--r--   0 runner    (1001) docker     (123)   592141 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/output/onyx_export.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:31:06.653514 nmaquifertool-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:41:15.205119 nmaquifertool-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:41:15.197119 nmaquifertool-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:41:15.201119 nmaquifertool-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/.github/workflows/format_code.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-06 19:41:15.205119 nmaquifertool-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:41:15.201119 nmaquifertool-0.0.6/nmaquifertool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-06 19:41:15.000000 nmaquifertool-0.0.6/nmaquifertool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-06 19:41:15.000000 nmaquifertool-0.0.6/nmaquifertool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:41:15.000000 nmaquifertool-0.0.6/nmaquifertool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 19:41:15.000000 nmaquifertool-0.0.6/nmaquifertool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 19:41:15.000000 nmaquifertool-0.0.6/nmaquifertool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 19:41:15.000000 nmaquifertool-0.0.6/nmaquifertool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:41:15.201119 nmaquifertool-0.0.6/nmat/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/bc_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:41:15.201119 nmaquifertool-0.0.6/nmat/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/geo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:41:15.201119 nmaquifertool-0.0.6/nmat/indata/
+-rw-r--r--   0 runner    (1001) docker     (123)   536602 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/indata/sp2023berncowls.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/onyx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/ose_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:41:15.205119 nmaquifertool-0.0.6/nmat/output/
+-rw-r--r--   0 runner    (1001) docker     (123)   592141 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/output/onyx_export.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/nmat/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:41:15.205119 nmaquifertool-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-06 19:41:04.000000 nmaquifertool-0.0.6/setup.py
```

### Comparing `nmaquifertool-0.0.5/.github/workflows/format_code.yaml` & `nmaquifertool-0.0.6/.github/workflows/format_code.yaml`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/.github/workflows/publish_to_pypi.yaml` & `nmaquifertool-0.0.6/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/.gitignore` & `nmaquifertool-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/nmaquifertool.egg-info/SOURCES.txt` & `nmaquifertool-0.0.6/nmaquifertool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/nmat/__init__.py` & `nmaquifertool-0.0.6/nmat/__init__.py`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/nmat/bc_uploader.py` & `nmaquifertool-0.0.6/nmat/bc_uploader.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,56 +10,60 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
 import pandas as pd
+
 # import requests as requests
 
 from nmat.db import get_db_client
 from nmat.geo_utils import latlon_to_utm
 from nmat.query import execute_fetch, execute_insert, make_insert, make_select
 from nmat.util import message, warning, info
 
 CKAN_URL = "https://catalog.newmexicowaterdata.org/"
 
 
 def add_records_to_db(client, pointid, group, dry=True, verbose=True):
     for i, row in group.iterrows():
         info(f"Adding {i}, {row['Well_Name']} to database")
 
-        keys = ['PointID',
-                'DateMeasured',
-                'DepthToWater',
-                'DepthToWaterBGS',
-                'MPHeight']
-
-        values = [pointid,
-                  row['MSRMNT_Dat'].date(),
-                  row['Depth_To_W'],
-                  row['Depth_To_W'],
-                  row['Stick_up'],
-                  ]
+        keys = [
+            "PointID",
+            "DateMeasured",
+            "DepthToWater",
+            "DepthToWaterBGS",
+            "MPHeight",
+        ]
+
+        values = [
+            pointid,
+            row["MSRMNT_Dat"].date(),
+            row["Depth_To_W"],
+            row["Depth_To_W"],
+            row["Stick_up"],
+        ]
 
         sql = make_insert("WaterLevels", keys, values)
         execute_insert(sql, client=client, dry=dry, verbose=verbose)
 
 
 def add_point_to_db(client, row, dry=True, verbose=True):
     result = get_last_point_id_like(client, "BC-", verbose=verbose)
-    last_pointid = result['PointID']
+    last_pointid = result["PointID"]
 
     n = int(last_pointid.split("-")[1])
     pointid = f"BC-{n + 1:04n}"
 
-    keys = ['PointID', 'Easting', 'Northing', 'Altitude']
-    easting, northing = latlon_to_utm(row['Long_DD'], row['Lat_DD'])
+    keys = ["PointID", "Easting", "Northing", "Altitude"]
+    easting, northing = latlon_to_utm(row["Long_DD"], row["Lat_DD"])
 
-    values = [pointid, easting, northing, row['Elev_ft']]
+    values = [pointid, easting, northing, row["Elev_ft"]]
 
     sql = make_insert("Location", keys, values)
     execute_insert(sql, client=client, dry=dry, verbose=verbose)
 
     return pointid
 
 
@@ -96,15 +100,15 @@
 
     url = f"{CKAN_URL}/datastore/dump/{resource_id}"
     # resp = requests.get(url)
     # return resp.text
 
 
 def upload_waterlevels_from_file(p, sheetname, client=None, dry=True, verbose=False):
-    message(f'Uploading waterlevels from {p}, sheet={sheetname}, dry={dry}')
+    message(f"Uploading waterlevels from {p}, sheet={sheetname}, dry={dry}")
 
     if client is None:
         client = get_db_client()
 
     df = pd.read_excel(p, sheet_name=sheetname)
 
     # filter out any rows with Well_Name that starts with Z -
@@ -114,19 +118,19 @@
     grouped = filtered.groupby("Well_Name")
     for name, group in grouped:
         # check if in database
         repr_row = group.iloc[0]
 
         pointid = repr_row["PointID"]
         if pointid and pointid != "nan":
-            info(f'Checking if {name}, ({pointid}) in database')
+            info(f"Checking if {name}, ({pointid}) in database")
             result = get_point_id(client, pointid, verbose=verbose)
-            pointid = result['PointID'] if result else None
+            pointid = result["PointID"] if result else None
         else:
-            info(f'no PointID provided. Assuming {name} not in database')
+            info(f"no PointID provided. Assuming {name} not in database")
             break
 
         if pointid:
             warning(f"{name} already in database")
 
         else:
             pointid = add_point_to_db(client, repr_row, dry=dry, verbose=verbose)
@@ -135,15 +139,15 @@
         # sort group by date
         group = group.sort_values(by="MSRMNT_Dat")
 
         # get the latest record from the database
         dbrecord = get_latest_record(client, pointid, verbose=verbose)
 
         if dbrecord:
-            print('asdf', dbrecord['DateMeasured'])
+            print("asdf", dbrecord["DateMeasured"])
             # filter out all records that are older than the latest record in the database
             group = group[group["MSRMNT_Dat"].dt.date > dbrecord["DateMeasured"]]
             # print(group)
             # print(group['MSRMNT_Dat'].dt.date)
 
         # add records to database
         add_records_to_db(client, pointid, group, dry=dry, verbose=verbose)
```

### Comparing `nmaquifertool-0.0.5/nmat/cli.py` & `nmaquifertool-0.0.6/nmat/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,16 +53,17 @@
 @cli.group()
 def upload():
     pass
 
 
 @upload.command()
 @click.option("--file", prompt="Specify input file path", help="Input file path")
-@click.option("--sheetname", default='Sheet1', help="The sheet name")
-@click.option("--dry_run", default=True, help="Dry run")
-@click.option("--verbose", default=False, help="Verbose logging")
-def waterlevels(file, sheetname, dry_run, verbose):
+@click.option("--sheetname", default="Sheet1", help="The sheet name")
+@click.option("--commit", is_flag=True, default=False, help="Commit data to database")
+@click.option("--verbose", is_flag=True, default=False, help="Verbose logging")
+def waterlevels(file, sheetname, commit, verbose):
     from nmat.runner import waterlevels
 
-    waterlevels(file, sheetname, dry=dry_run, verbose=verbose)
+    waterlevels(file, sheetname, dry=not commit, verbose=verbose)
+
 
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.5/nmat/db.py` & `nmaquifertool-0.0.6/nmat/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 import yaml
 
 from nmat.util import warning, message, error
 
 # ===============================================================================
 # Database credentials
-cp = os.path.join(os.path.expanduser('~'), '.nmat', 'credentials.yaml')
+cp = os.path.join(os.path.expanduser("~"), ".nmat", "credentials.yaml")
 
 ycfg = {}
 if os.path.isfile(cp):
-    with open(cp, 'r') as f:
+    with open(cp, "r") as f:
         ycfg = yaml.load(f, Loader=yaml.FullLoader)
 
 
 def get_credential(key):
     # return os.environ.get(key, "default")
-    return os.environ.get(key, ycfg.get(key, 'default'))
+    return os.environ.get(key, ycfg.get(key, "default"))
 
 
 HOST = get_credential("NM_AQUIFER_HOST")
 USER = get_credential("NM_AQUIFER_USER")
 PWD = get_credential("NM_AQUIFER_PWD")
 DB = get_credential("NM_AQUIFER_DB")
 
@@ -64,8 +64,9 @@
                 "Please set db credentials in your config file or as environment variables ",
                 fg="blue",
             )
         exit()
 
     return client
 
+
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.5/nmat/geo_utils.py` & `nmaquifertool-0.0.6/nmat/geo_utils.py`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/nmat/indata/sp2023berncowls.xlsx` & `nmaquifertool-0.0.6/nmat/indata/sp2023berncowls.xlsx`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/nmat/onyx_export.py` & `nmaquifertool-0.0.6/nmat/onyx_export.py`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/nmat/ose_downloader.py` & `nmaquifertool-0.0.6/nmat/ose_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
 
+
 def get_well_log():
     pass
 
 
-# ============= EOF =============================================
+# ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.5/nmat/output/onyx_export.csv` & `nmaquifertool-0.0.6/nmat/output/onyx_export.csv`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/nmat/query.py` & `nmaquifertool-0.0.6/nmat/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from datetime import datetime, date
 
 from nmat.db import get_db_client
 
 
 def make_insert(table, attributes, values):
     attributes = ", ".join(attributes)
-    values = ", ".join([f"'{v}'" if isinstance(v, (str, datetime, date)) else str(v) for v in values])
+    values = ", ".join(
+        [f"'{v}'" if isinstance(v, (str, datetime, date)) else str(v) for v in values]
+    )
 
     sql = f"""
     INSERT INTO dbo.{table} ({attributes})
     VALUES ({values})"""
     return sql
```

### Comparing `nmaquifertool-0.0.5/nmat/runner.py` & `nmaquifertool-0.0.6/nmat/runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,13 +39,16 @@
 def onyx_export(output):
     from nmat.onyx_export import export
 
     export(output)
 
 
 def waterlevels(file, sheetname, **kw):
-    file = './nmat/indata/sp2023berncowls.xlsx'
+    file = "./nmat/indata/sp2023berncowls.xlsx"
     sheetname = "Sp2023BernCoWLs"
 
     from nmat.bc_uploader import upload_waterlevels_from_file
+
     upload_waterlevels_from_file(file, sheetname, **kw)
+
+
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.5/nmat/util.py` & `nmaquifertool-0.0.6/nmat/util.py`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/nmat/version.py` & `nmaquifertool-0.0.6/nmat/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.5/pyproject.toml` & `nmaquifertool-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.5/setup.py` & `nmaquifertool-0.0.6/setup.py`

 * *Files identical despite different names*

