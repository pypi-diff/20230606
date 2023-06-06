# Comparing `tmp/data-science-common-core-1.7.5.tar.gz` & `tmp/data-science-common-core-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-science-common-core-1.7.5.tar", max compression
+gzip compressed data, was "data-science-common-core-1.7.6.tar", max compression
```

## Comparing `data-science-common-core-1.7.5.tar` & `data-science-common-core-1.7.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       31 2022-08-16 12:51:34.846327 data-science-common-core-1.7.5/common/__init__.py
--rw-r--r--   0        0        0     1772 2023-01-04 09:26:13.978265 data-science-common-core-1.7.5/common/catrf.py
--rw-r--r--   0        0        0     2239 2023-06-02 13:30:43.079798 data-science-common-core-1.7.5/common/constants.py
--rw-r--r--   0        0        0    28618 2022-09-16 13:05:55.366098 data-science-common-core-1.7.5/common/custom_hgb.py
--rw-r--r--   0        0        0    14915 2022-10-06 09:48:34.061975 data-science-common-core-1.7.5/common/custom_multi.py
--rw-r--r--   0        0        0    17492 2023-06-02 13:33:52.153362 data-science-common-core-1.7.5/common/ft.py
--rw-r--r--   0        0        0    12414 2023-06-02 13:30:43.079972 data-science-common-core-1.7.5/common/io.py
--rw-r--r--   0        0        0    23926 2022-11-18 13:02:14.591758 data-science-common-core-1.7.5/common/logic.py
--rw-r--r--   0        0        0    15836 2023-01-04 09:26:13.980885 data-science-common-core-1.7.5/common/model.py
--rw-r--r--   0        0        0     1013 2023-06-02 13:30:43.080198 data-science-common-core-1.7.5/common/pipeline.py
--rw-r--r--   0        0        0    11465 2023-06-02 13:30:43.082632 data-science-common-core-1.7.5/common/plot.py
--rw-r--r--   0        0        0     2100 2022-09-08 15:24:02.191811 data-science-common-core-1.7.5/common/query.py
--rw-r--r--   0        0        0     6947 2023-01-04 09:26:13.981645 data-science-common-core-1.7.5/common/setup.py
--rw-r--r--   0        0        0     2639 2023-06-02 13:30:43.082938 data-science-common-core-1.7.5/common/transformer.py
--rw-r--r--   0        0        0     8736 2022-11-25 15:53:01.257516 data-science-common-core-1.7.5/common/utils.py
--rw-r--r--   0        0        0     1089 2023-06-02 13:53:26.121282 data-science-common-core-1.7.5/pyproject.toml
--rw-r--r--   0        0        0     1343 2023-06-02 14:00:02.818002 data-science-common-core-1.7.5/setup.py
--rw-r--r--   0        0        0     1479 2023-06-02 14:00:02.818182 data-science-common-core-1.7.5/PKG-INFO
+-rw-r--r--   0        0        0       31 2022-08-16 12:51:34.846327 data-science-common-core-1.7.6/common/__init__.py
+-rw-r--r--   0        0        0     1772 2023-01-04 09:26:13.978265 data-science-common-core-1.7.6/common/catrf.py
+-rw-r--r--   0        0        0     2343 2023-06-06 12:45:28.311456 data-science-common-core-1.7.6/common/constants.py
+-rw-r--r--   0        0        0    28618 2022-09-16 13:05:55.366098 data-science-common-core-1.7.6/common/custom_hgb.py
+-rw-r--r--   0        0        0    14915 2022-10-06 09:48:34.061975 data-science-common-core-1.7.6/common/custom_multi.py
+-rw-r--r--   0        0        0    17492 2023-06-06 11:26:49.982009 data-science-common-core-1.7.6/common/ft.py
+-rw-r--r--   0        0        0    12414 2023-06-02 13:30:43.079972 data-science-common-core-1.7.6/common/io.py
+-rw-r--r--   0        0        0    27223 2023-06-06 12:45:28.311861 data-science-common-core-1.7.6/common/logic.py
+-rw-r--r--   0        0        0    15836 2023-01-04 09:26:13.980885 data-science-common-core-1.7.6/common/model.py
+-rw-r--r--   0        0        0     1013 2023-06-02 13:30:43.080198 data-science-common-core-1.7.6/common/pipeline.py
+-rw-r--r--   0        0        0    11465 2023-06-02 13:30:43.082632 data-science-common-core-1.7.6/common/plot.py
+-rw-r--r--   0        0        0     2100 2022-09-08 15:24:02.191811 data-science-common-core-1.7.6/common/query.py
+-rw-r--r--   0        0        0     6947 2023-01-04 09:26:13.981645 data-science-common-core-1.7.6/common/setup.py
+-rw-r--r--   0        0        0     2639 2023-06-02 13:30:43.082938 data-science-common-core-1.7.6/common/transformer.py
+-rw-r--r--   0        0        0     8736 2022-11-25 15:53:01.257516 data-science-common-core-1.7.6/common/utils.py
+-rw-r--r--   0        0        0     1089 2023-06-06 12:45:28.312147 data-science-common-core-1.7.6/pyproject.toml
+-rw-r--r--   0        0        0     1343 2023-06-06 12:45:35.809176 data-science-common-core-1.7.6/setup.py
+-rw-r--r--   0        0        0     1479 2023-06-06 12:45:35.809364 data-science-common-core-1.7.6/PKG-INFO
```

### Comparing `data-science-common-core-1.7.5/common/catrf.py` & `data-science-common-core-1.7.6/common/catrf.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/constants.py` & `data-science-common-core-1.7.6/common/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "train_data_file": "train_val_data.pkl.gz",
     "test_data_file": "test_data.pkl.gz",
     "abs_corr_collinearity": 0.9,
     "na_replace_val": -0.42069,
     "random_state": 42,
     "train_test_split": 0.75,
     "id_field": "shipment_id",
+    "agg_datetime": False,  # whether to aggregate labels based on id. Merge on id and datetime if True
     "is_date_date_ratio": 0.1,
     "is_numeric_nan_count_mean": 0.1,
     "nan_value_percentage": 0.9,
     "if_n_estimators": 650,
     "if_sr_isolation": 0.05,
     "if_contamination": 0.135,
     "extract_feature_per_shipment_single": True,
```

### Comparing `data-science-common-core-1.7.5/common/custom_hgb.py` & `data-science-common-core-1.7.6/common/custom_hgb.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/custom_multi.py` & `data-science-common-core-1.7.6/common/custom_multi.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/ft.py` & `data-science-common-core-1.7.6/common/ft.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/io.py` & `data-science-common-core-1.7.6/common/io.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/logic.py` & `data-science-common-core-1.7.6/common/logic.py`

 * *Files 8% similar despite different names*

```diff
@@ -453,47 +453,111 @@
 
         if "validation_test_split" in params and params["validation_test_split"]:
             segments = ["train", "val", "test"]
         else:
             segments = ["train", "val"]
         for segment in segments:
             # Do label gathering first since you need it for LDA
-            data[f"label_{segment}"] = (
-                data[f"id_{segment}"]
-                .merge(labels, on=params["id_field"], how="left")
-                .set_index(params["id_field"])
-                .fillna(0)
-            )
+            if "label_use_datetime" in params and params["label_use_datetime"]:
+                data[f"label_{segment}"] = (
+                    data[f"df_{segment}"][
+                        [params["id_field"], params["datetime_field"]]
+                    ]
+                    .merge(
+                        labels,
+                        on=[params["id_field"], params["datetime_field"]],
+                        how="left",
+                    )
+                    .set_index(params["id_field"])
+                    .drop(params["datetime_field"], axis=1)
+                    .fillna(0)
+                )
+            else:
+                data[f"label_{segment}"] = (
+                    data[f"id_{segment}"]
+                    .merge(labels, on=params["id_field"], how="left")
+                    .set_index(params["id_field"])
+                    .fillna(0)
+                )
 
             if (
                 "data_normalization_field" in params
                 and params["data_normalization_field"]
             ):
-                data[f"norm_{segment}"] = data[f"df_{segment}"][
-                    [params["id_field"], params["data_normalization_field"]]
-                ].set_index(params["id_field"])
-                data[f"norm_{segment}"] = data[f"norm_{segment}"][
-                    ~data[f"norm_{segment}"].index.duplicated(keep="first")
-                ]
+                # Do label gathering first since you need it for LDA
+                if "label_use_datetime" in params and params["label_use_datetime"]:
+                    data[f"norm_{segment}"](
+                        data[f"df_{segment}"][
+                            [
+                                params["id_field"],
+                                params["data_normalization_field"],
+                                params["datetime_field"],
+                            ]
+                        ]
+                        .merge(
+                            labels,
+                            on=[params["id_field"], params["datetime_field"]],
+                            how="left",
+                        )
+                        .set_index(params["id_field"])
+                        .drop(params["datetime_field"], axis=1)
+                        .fillna(0)
+                    )
+                else:
+                    data[f"norm_{segment}"] = data[f"df_{segment}"][
+                        [params["id_field"], params["data_normalization_field"]]
+                    ].set_index(params["id_field"])
+                    data[f"norm_{segment}"] = data[f"norm_{segment}"][
+                        ~data[f"norm_{segment}"].index.duplicated(keep="first")
+                    ]
 
             if segment == "train":
                 logger.info("Feature extraction... Fitting")
                 ft.fit(
                     params, data["df_train"], data["label_train"], params["type_dict"]
                 )
 
             data[f"df_{segment}"] = ft.transform(params, data[f"df_{segment}"])
 
             # Do it again since Feature Transformer groups shipments
-            data[f"label_{segment}"] = (
-                pd.DataFrame(data[f"df_{segment}"][params["id_field"]])
-                .merge(labels, on=params["id_field"], how="left")
-                .set_index(params["id_field"])
-                .fillna(0)
-            )
+            # if 'label_use_datetime' in params and params['label_use_datetime']:
+            #     data[f"label_{segment}"] = (
+            #         data[f"df_{segment}"][[params['id_field'], params['datetime_field']]]
+            #         .merge(labels, on=[params["id_field"], params['datetime_field']], how="left")
+            #         .set_index(params["id_field"]).drop(params['datetime_field'], axis=1)
+            #         .fillna(0)
+            #     )
+            # else:
+            #     data[f"label_{segment}"] = (
+            #         data[f"id_{segment}"]
+            #         .merge(labels, on=params["id_field"], how="left")
+            #         .set_index(params["id_field"])
+            #         .fillna(0)
+            #     )
+            #
+            # if (
+            #         "data_normalization_field" in params
+            #         and params["data_normalization_field"]
+            # ):
+            #     # Do label gathering first since you need it for LDA
+            #     if 'label_use_datetime' in params and params['label_use_datetime']:
+            #         data[f"norm_{segment}"](
+            #             data[f"df_{segment}"][
+            #                 [params['id_field'], params["data_normalization_field"], params['datetime_field']]]
+            #             .merge(labels, on=[params["id_field"], params['datetime_field']], how="left")
+            #             .set_index(params["id_field"]).drop(params['datetime_field'], axis=1)
+            #             .fillna(0)
+            #         )
+            #     else:
+            #         data[f"norm_{segment}"] = data[f"df_{segment}"][
+            #             [params["id_field"], params["data_normalization_field"]]
+            #         ].set_index(params["id_field"])
+            #         data[f"norm_{segment}"] = data[f"norm_{segment}"][
+            #             ~data[f"norm_{segment}"].index.duplicated(keep="first")
+            #         ]
 
             data[f"id_{segment}"] = pd.DataFrame(
                 data[f"df_{segment}"][params["id_field"]]
             )
 
             data[f"df_{segment}"] = (
                 data[f"df_{segment}"]
```

### Comparing `data-science-common-core-1.7.5/common/model.py` & `data-science-common-core-1.7.6/common/model.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/pipeline.py` & `data-science-common-core-1.7.6/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/plot.py` & `data-science-common-core-1.7.6/common/plot.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/query.py` & `data-science-common-core-1.7.6/common/query.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/setup.py` & `data-science-common-core-1.7.6/common/setup.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/transformer.py` & `data-science-common-core-1.7.6/common/transformer.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/common/utils.py` & `data-science-common-core-1.7.6/common/utils.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.5/pyproject.toml` & `data-science-common-core-1.7.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-science-common-core"
-version = "1.7.5"
+version = "1.7.6"
 description = "Data Science Common Core"
 authors = ["Unsal Gokdag <unsal.gokdag@forto.com>", "PietroAnsidei <pietro.ansidei@forto.com>", "Naomi Nguyen <naomi.nguyen@forto.com>", "Kumar Rajendrababu <kumar.rajendrababu@forto.com>"]
 packages = [
     { include = "common/*.py"},
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `data-science-common-core-1.7.5/setup.py` & `data-science-common-core-1.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
  'toml>=0.10.2,<0.11.0',
  'tomli>=2.0.1,<3.0.0',
  'tqdm>=4.64.0,<5.0.0',
  'webencodings>=0.5.1,<0.6.0']
 
 setup_kwargs = {
     'name': 'data-science-common-core',
-    'version': '1.7.5',
+    'version': '1.7.6',
     'description': 'Data Science Common Core',
     'long_description': None,
     'author': 'Unsal Gokdag',
     'author_email': 'unsal.gokdag@forto.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `data-science-common-core-1.7.5/PKG-INFO` & `data-science-common-core-1.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-science-common-core
-Version: 1.7.5
+Version: 1.7.6
 Summary: Data Science Common Core
 Author: Unsal Gokdag
 Author-email: unsal.gokdag@forto.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

