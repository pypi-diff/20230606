# Comparing `tmp/nmaquifertool-0.0.4.tar.gz` & `tmp/nmaquifertool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmaquifertool-0.0.4.tar", last modified: Tue Jun  6 13:52:55 2023, max compression
+gzip compressed data, was "nmaquifertool-0.0.5.tar", last modified: Tue Jun  6 19:31:06 2023, max compression
```

## Comparing `nmaquifertool-0.0.4.tar` & `nmaquifertool-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:52:55.709425 nmaquifertool-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:52:55.701425 nmaquifertool-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:52:55.705425 nmaquifertool-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/.github/workflows/format_code.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-06 13:52:55.709425 nmaquifertool-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:52:55.705425 nmaquifertool-0.0.4/nmaquifertool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-06 13:52:55.000000 nmaquifertool-0.0.4/nmaquifertool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-06 13:52:55.000000 nmaquifertool-0.0.4/nmaquifertool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:52:55.000000 nmaquifertool-0.0.4/nmaquifertool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 13:52:55.000000 nmaquifertool-0.0.4/nmaquifertool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 13:52:55.000000 nmaquifertool-0.0.4/nmaquifertool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 13:52:55.000000 nmaquifertool-0.0.4/nmaquifertool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:52:55.705425 nmaquifertool-0.0.4/nmat/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/bc_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:52:55.705425 nmaquifertool-0.0.4/nmat/config/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/geo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:52:55.705425 nmaquifertool-0.0.4/nmat/indata/
--rw-r--r--   0 runner    (1001) docker     (123)   592485 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/indata/sp2023berncowls.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/onyx_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:52:55.709425 nmaquifertool-0.0.4/nmat/output/
--rw-r--r--   0 runner    (1001) docker     (123)   592141 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/output/onyx_export.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/nmat/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:52:55.709425 nmaquifertool-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-06 13:52:46.000000 nmaquifertool-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.653514 nmaquifertool-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.645514 nmaquifertool-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.645514 nmaquifertool-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/.github/workflows/format_code.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 19:31:06.653514 nmaquifertool-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.649514 nmaquifertool-0.0.5/nmaquifertool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 19:31:06.000000 nmaquifertool-0.0.5/nmaquifertool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.649514 nmaquifertool-0.0.5/nmat/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/bc_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.649514 nmaquifertool-0.0.5/nmat/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/geo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.649514 nmaquifertool-0.0.5/nmat/indata/
+-rw-r--r--   0 runner    (1001) docker     (123)   536602 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/indata/sp2023berncowls.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/onyx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/ose_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:31:06.653514 nmaquifertool-0.0.5/nmat/output/
+-rw-r--r--   0 runner    (1001) docker     (123)   592141 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/output/onyx_export.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/nmat/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:31:06.653514 nmaquifertool-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-06 19:30:55.000000 nmaquifertool-0.0.5/setup.py
```

### Comparing `nmaquifertool-0.0.4/.github/workflows/format_code.yaml` & `nmaquifertool-0.0.5/.github/workflows/format_code.yaml`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.4/.github/workflows/publish_to_pypi.yaml` & `nmaquifertool-0.0.5/.github/workflows/publish_to_pypi.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -24,18 +24,18 @@
           pip install
           build
           --user
       - name: Build a binary wheel and a source tarball
         run: >-
           python -m
           build
-#      - name: Publish distribution 📦 to Test PyPI
-#        uses: pypa/gh-action-pypi-publish@release/v1
-#        with:
-##          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-#          repository_url: https://test.pypi.org/legacy/
-#          skip_existing: true
+      - name: Publish distribution 📦 to Test PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+#          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+          repository_url: https://test.pypi.org/legacy/
+          skip_existing: true
       - name: Publish distribution 📦 to PyPI
-#        if: startsWith(github.ref, 'refs/tags')
+        if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
 #        with:
 #          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `nmaquifertool-0.0.4/.gitignore` & `nmaquifertool-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.4/nmaquifertool.egg-info/SOURCES.txt` & `nmaquifertool-0.0.5/nmaquifertool.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 nmaquifertool.egg-info/top_level.txt
 nmat/__init__.py
 nmat/bc_uploader.py
 nmat/cli.py
 nmat/db.py
 nmat/geo_utils.py
 nmat/onyx_export.py
+nmat/ose_downloader.py
 nmat/query.py
 nmat/runner.py
 nmat/util.py
 nmat/version.py
 nmat/config/config.yaml
 nmat/indata/sp2023berncowls.xlsx
 nmat/output/onyx_export.csv
```

### Comparing `nmaquifertool-0.0.4/nmat/__init__.py` & `nmaquifertool-0.0.5/nmat/__init__.py`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.4/nmat/bc_uploader.py` & `nmaquifertool-0.0.5/nmat/bc_uploader.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,112 +10,156 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
 import pandas as pd
-import requests as requests
+# import requests as requests
 
 from nmat.db import get_db_client
+from nmat.geo_utils import latlon_to_utm
 from nmat.query import execute_fetch, execute_insert, make_insert, make_select
+from nmat.util import message, warning, info
 
 CKAN_URL = "https://catalog.newmexicowaterdata.org/"
 
 
-def add_records_to_db(client, group):
+def add_records_to_db(client, pointid, group, dry=True, verbose=True):
     for i, row in group.iterrows():
-        sql = make_insert("WaterLevels", row.keys(), row.values)
-        execute_insert(sql, client=client)
+        info(f"Adding {i}, {row['Well_Name']} to database")
 
-
-def add_point_to_db(client, row):
-    last_pointid = get_last_point_id_like(client, "BC-")
+        keys = ['PointID',
+                'DateMeasured',
+                'DepthToWater',
+                'DepthToWaterBGS',
+                'MPHeight']
+
+        values = [pointid,
+                  row['MSRMNT_Dat'].date(),
+                  row['Depth_To_W'],
+                  row['Depth_To_W'],
+                  row['Stick_up'],
+                  ]
+
+        sql = make_insert("WaterLevels", keys, values)
+        execute_insert(sql, client=client, dry=dry, verbose=verbose)
+
+
+def add_point_to_db(client, row, dry=True, verbose=True):
+    result = get_last_point_id_like(client, "BC-", verbose=verbose)
+    last_pointid = result['PointID']
 
     n = int(last_pointid.split("-")[1])
     pointid = f"BC-{n + 1:04n}"
 
-    sql = make_insert("Location", row.keys(), row.values)
-    execute_insert(sql, client=client)
+    keys = ['PointID', 'Easting', 'Northing', 'Altitude']
+    easting, northing = latlon_to_utm(row['Long_DD'], row['Lat_DD'])
+
+    values = [pointid, easting, northing, row['Elev_ft']]
+
+    sql = make_insert("Location", keys, values)
+    execute_insert(sql, client=client, dry=dry, verbose=verbose)
 
     return pointid
 
 
-def get_last_point_id_like(client, point_id):
+def get_last_point_id_like(client, point_id, verbose=True):
     """
     This function is used to get the last PointID from the database that is like point_id.
     :param point_id:
     :return:
     """
     sql = make_select(where=f"PointID LIKE '{point_id}%'", order=f"PointID DESC")
-    return execute_fetch(sql, client=client, fetch="fetchfirst")
+    return execute_fetch(sql, client=client, fetch="fetchone", verbose=verbose)
 
 
-def get_point_id(client, point_id):
+def get_point_id(client, point_id, verbose=True):
     """
     This function is used to get the point_id from the database.
     :param point_id:
     :return:
     """
 
     sql = make_select(attributes="PointID", where=f"PointID = '{point_id}'")
-    return execute_fetch(sql, client=client, fetch="fetchone")
+    return execute_fetch(sql, client=client, fetch="fetchone", verbose=verbose)
 
 
-def get_latest_record(client, pointid):
+def get_latest_record(client, pointid, verbose=True):
     sql = make_select(
         table="WaterLevels", where=f"PointID = '{pointid}'", order="DateMeasured DESC"
     )
-    return execute_fetch(sql, client=client, fetch="fetchone")
+    return execute_fetch(sql, client=client, fetch="fetchone", verbose=verbose)
 
 
 def get_latest_data():
     resource_id = ""
 
     url = f"{CKAN_URL}/datastore/dump/{resource_id}"
-    resp = requests.get(url)
-    return resp.text
+    # resp = requests.get(url)
+    # return resp.text
 
 
-def main():
-    client = get_db_client()
-
-    get_latest_data()
+def upload_waterlevels_from_file(p, sheetname, client=None, dry=True, verbose=False):
+    message(f'Uploading waterlevels from {p}, sheet={sheetname}, dry={dry}')
 
-    p = "./indata/sp2023berncowls.xlsx"
-    sheetname = "Sp2023BernCoWLs"
+    if client is None:
+        client = get_db_client()
 
     df = pd.read_excel(p, sheet_name=sheetname)
 
     # filter out any rows with Well_Name that starts with Z -
     filtered = df[~df["Well_Name"].str.startswith("Z -")]
 
     # group df by Well_Name column
     grouped = filtered.groupby("Well_Name")
     for name, group in grouped:
         # check if in database
-
         repr_row = group.iloc[0]
-        pointid = get_point_id(client, repr_row["PointID"])
+
+        pointid = repr_row["PointID"]
+        if pointid and pointid != "nan":
+            info(f'Checking if {name}, ({pointid}) in database')
+            result = get_point_id(client, pointid, verbose=verbose)
+            pointid = result['PointID'] if result else None
+        else:
+            info(f'no PointID provided. Assuming {name} not in database')
+            break
+
         if pointid:
-            print(f"{name} already in database")
+            warning(f"{name} already in database")
+
         else:
-            pointid = add_point_to_db(client, repr_row)
+            pointid = add_point_to_db(client, repr_row, dry=dry, verbose=verbose)
 
         # iterate over each row in the group
         # sort group by date
-        group = group.sort_values(by="Date")
+        group = group.sort_values(by="MSRMNT_Dat")
 
         # get the latest record from the database
-        dbrecord = get_latest_record(client, pointid)
+        dbrecord = get_latest_record(client, pointid, verbose=verbose)
+
         if dbrecord:
+            print('asdf', dbrecord['DateMeasured'])
             # filter out all records that are older than the latest record in the database
-            group = group[group["Date"] > dbrecord["Date"]]
+            group = group[group["MSRMNT_Dat"].dt.date > dbrecord["DateMeasured"]]
+            # print(group)
+            # print(group['MSRMNT_Dat'].dt.date)
 
         # add records to database
-        add_records_to_db(client, group)
+        add_records_to_db(client, pointid, group, dry=dry, verbose=verbose)
+
+
+def main():
+    client = get_db_client()
+
+    get_latest_data()
+
+    p = "./indata/sp2023berncowls.xlsx"
+    sheetname = "Sp2023BernCoWLs"
+    upload_waterlevels_from_file(p, sheetname, client=client)
 
 
 if __name__ == "__main__":
     main()
 
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.4/nmat/cli.py` & `nmaquifertool-0.0.5/nmat/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,41 +12,57 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
 import os
 from pathlib import Path
 
-import click as click
+import click
+
+from nmat.util import info, message
 
 
 @click.command()
 @click.option(
     "--config", prompt="Config path", help="Path to configuration file. e.g config.yaml"
 )
 def cli_c(config):
-    click.echo("Doing NMAT config run")
-    click.echo(f"Using config file: {config}")
+    # click.secho("Doing NMAT config run", fg="green")
+    # click.secho(f"Using config file: {config}", fg="green")
+    info("Doing NMAT config run")
+    message(f"Using config file: {config}")
     from nmat.runner import run
 
-    # print(os.path.curdir, os.getcwd())
-    # config = os.path.join(os.getcwd(), './nmat/config/config.yaml')
     config = Path("./nmat/config/config.yaml")
     run(config)
 
 
 @click.group()
 def cli():
     pass
 
 
 @cli.command()
 @click.option("--output", prompt="Specify output path", help="Output path")
 def onyx_export(output):
-    click.echo(f"Exporting to {output}")
+    info(f"Exporting to {output}")
+    from nmat.runner import onyx_export as export
+
+    export(output)
+
+
+@cli.group()
+def upload():
+    pass
+
 
-    # """Simple program that greets NAME for a total of COUNT times."""
-    # for x in range(count):
-    #     click.echo(f"Hello {name}!")
+@upload.command()
+@click.option("--file", prompt="Specify input file path", help="Input file path")
+@click.option("--sheetname", default='Sheet1', help="The sheet name")
+@click.option("--dry_run", default=True, help="Dry run")
+@click.option("--verbose", default=False, help="Verbose logging")
+def waterlevels(file, sheetname, dry_run, verbose):
+    from nmat.runner import waterlevels
 
+    waterlevels(file, sheetname, dry=dry_run, verbose=verbose)
 
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.4/nmat/db.py` & `nmaquifertool-0.0.5/nmat/db.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
 import os
 
 import yaml
 
+from nmat.util import warning, message, error
+
 # ===============================================================================
 # Database credentials
-# cp = './config/credentials.yaml'
-# ycfg = {}
-# if os.path.isfile(cp):
-#     with open(cp, 'r') as f:
-#         ycfg = yaml.load(f, Loader=yaml.FullLoader)
-#
+cp = os.path.join(os.path.expanduser('~'), '.nmat', 'credentials.yaml')
+
+ycfg = {}
+if os.path.isfile(cp):
+    with open(cp, 'r') as f:
+        ycfg = yaml.load(f, Loader=yaml.FullLoader)
 
 
 def get_credential(key):
-    return os.environ.get(key, "default")
-    # return os.environ.get(key, ycfg.get(key, 'default'))
+    # return os.environ.get(key, "default")
+    return os.environ.get(key, ycfg.get(key, 'default'))
 
 
 HOST = get_credential("NM_AQUIFER_HOST")
 USER = get_credential("NM_AQUIFER_USER")
 PWD = get_credential("NM_AQUIFER_PWD")
 DB = get_credential("NM_AQUIFER_DB")
 
@@ -46,24 +48,24 @@
     """
 
     import pymssql
 
     try:
         client = pymssql.connect(HOST, USER, PWD, DB, login_timeout=1)
     except pymssql.OperationalError as e:
-        print("Error connecting to database. Check your credentials.")
-        print("Using credentials =============")
-        print("HOST: ", HOST)
-        print("USER: ", USER)
-        print("DB: ", DB)
-        print("===============================")
+        error(e)
+        warning("Error connecting to database. Check your credentials.")
+        message("======== Using credentials ==========")
+        message(f"HOST: {HOST}")
+        message(f"USER: {USER}")
+        message(f"DB: {DB}")
+        message("=====================================")
         if HOST == "default" and USER == "default" and DB == "default":
-            print(
-                "Please set db credentials in your config file or as environment variables "
+            message(
+                "Please set db credentials in your config file or as environment variables ",
+                fg="blue",
             )
-        print(e)
         exit()
 
     return client
 
-
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.4/nmat/geo_utils.py` & `nmaquifertool-0.0.5/nmat/geo_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,18 @@
         pr = pyproj.Proj(proj="utm", zone=int(zone), ellps="WGS84")
         PROJECTIONS[name] = pr
 
     pr = PROJECTIONS[name]
     return pr(e, n, inverse=True)
 
 
-def latlon_to_utm(lon, lat):
+def latlon_to_utm(lon, lat, zone=13):
     name = "latlon"
     if name not in PROJECTIONS:
-        pr = pyproj.Proj(proj="utm", ellps="WGS84")
+        pr = pyproj.Proj(proj="utm", ellps="WGS84", zone=int(zone))
         PROJECTIONS[name] = pr
 
     pr = PROJECTIONS[name]
     return pr(lon, lat)
 
 
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.4/nmat/onyx_export.py` & `nmaquifertool-0.0.5/nmat/onyx_export.py`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.4/nmat/output/onyx_export.csv` & `nmaquifertool-0.0.5/nmat/output/onyx_export.csv`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.4/nmat/query.py` & `nmaquifertool-0.0.5/nmat/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,33 +10,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
 import csv
+from datetime import datetime, date
 
 from nmat.db import get_db_client
 
 
 def make_insert(table, attributes, values):
     attributes = ", ".join(attributes)
-    values = ", ".join(values)
+    values = ", ".join([f"'{v}'" if isinstance(v, (str, datetime, date)) else str(v) for v in values])
 
     sql = f"""
     INSERT INTO dbo.{table} ({attributes})
-    VALUES ({values})
-    """
+    VALUES ({values})"""
     return sql
 
 
 def make_select(attributes="*", table="Location", where=None, order=None):
     sql = f"""
-    SELECT {attributes} FROM dbo.{table}
-    """
+    SELECT {attributes} FROM dbo.{table}"""
 
     if where:
         sql = f"{sql} WHERE {where}"
     if order:
         sql = f"{sql} ORDER BY {order}"
 
     return sql
@@ -62,19 +61,20 @@
 
     cursor = client.cursor(as_dict=True)
     cursor.execute(sql)
     func = getattr(cursor, fetch)
     return func()
 
 
-def execute_insert(sql, client=None, verbose=True):
+def execute_insert(sql, client=None, verbose=True, dry=True):
     if verbose:
         print("executing insert================")
         print("sql: ", sql)
         print("===============================")
 
     cursor = client.cursor()
     cursor.execute(sql)
-    cursor.commit()
+    if not dry:
+        cursor.commit()
 
 
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.4/nmat/runner.py` & `nmaquifertool-0.0.5/nmat/runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,14 +33,19 @@
     for step in config["steps"]:
         func = step["function"]
         func = globals()[func]
         func(**step["args"])
 
 
 def onyx_export(output):
-    print(f"Exporting to {output}")
     from nmat.onyx_export import export
 
     export(output)
 
 
+def waterlevels(file, sheetname, **kw):
+    file = './nmat/indata/sp2023berncowls.xlsx'
+    sheetname = "Sp2023BernCoWLs"
+
+    from nmat.bc_uploader import upload_waterlevels_from_file
+    upload_waterlevels_from_file(file, sheetname, **kw)
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.4/nmat/version.py` & `nmaquifertool-0.0.5/nmat/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 # ============= EOF =============================================
```

### Comparing `nmaquifertool-0.0.4/pyproject.toml` & `nmaquifertool-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nmaquifertool-0.0.4/setup.py` & `nmaquifertool-0.0.5/setup.py`

 * *Files identical despite different names*

