# Comparing `tmp/django_cloudwatch_metrics-0.0.6.tar.gz` & `tmp/django_cloudwatch_metrics-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cloudwatch_metrics-0.0.6.tar", max compression
+gzip compressed data, was "django_cloudwatch_metrics-0.0.7.tar", max compression
```

## Comparing `django_cloudwatch_metrics-0.0.6.tar` & `django_cloudwatch_metrics-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0       27 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/README.md
--rw-r--r--   0        0        0      197 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/apps.py
--rw-r--r--   0        0        0        0 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      722 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/management/commands/increment.py
--rw-r--r--   0        0        0     2310 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/management/commands/publish_metrics.py
--rw-r--r--   0        0        0     1244 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/metrics.py
--rw-r--r--   0        0        0      926 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0      462 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/migrations/0002_alter_metricaggregation_id.py
--rw-r--r--   0        0        0        0 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/migrations/__init__.py
--rw-r--r--   0        0        0      502 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/models.py
--rw-r--r--   0        0        0    12871 2023-05-30 08:33:19.953344 django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/signals.py
--rw-r--r--   0        0        0      543 2023-05-30 08:33:19.957344 django_cloudwatch_metrics-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 django_cloudwatch_metrics-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/README.md
+-rw-r--r--   0        0        0      197 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/apps.py
+-rw-r--r--   0        0        0      635 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/hashing.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      722 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/management/commands/increment.py
+-rw-r--r--   0        0        0     2278 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/management/commands/publish_metrics.py
+-rw-r--r--   0        0        0     1282 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/metrics.py
+-rw-r--r--   0        0        0      926 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0      462 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/migrations/0002_alter_metricaggregation_id.py
+-rw-r--r--   0        0        0     1650 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/migrations/0003_auto_20230606_1148.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/migrations/__init__.py
+-rw-r--r--   0        0        0      377 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/models.py
+-rw-r--r--   0        0        0    12871 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/signals.py
+-rw-r--r--   0        0        0      543 2023-06-06 12:01:21.003825 django_cloudwatch_metrics-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 django_cloudwatch_metrics-0.0.7/PKG-INFO
```

### Comparing `django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/management/commands/increment.py` & `django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/management/commands/increment.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/management/commands/publish_metrics.py` & `django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/management/commands/publish_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,31 +17,32 @@
 def publish_metrics():
     logger.info("Publishing metrics to CloudWatch")
     cloudwatch = boto3.client("cloudwatch")
     metric_data = []
 
     metric_aggregations = MetricAggregation.objects.filter(datetime_period__lte=datetime.now(pytz.utc) - timedelta(minutes=1))
 
-    for datetime_period, metric_name, value, dimension_name, dimension_value in metric_aggregations.values_list(
-        "datetime_period", "metric_name", "value", "dimension_name", "dimension_value"
+    for datetime_period, metric_name, value, dimension_data in metric_aggregations.values_list(
+        "datetime_period", "metric_name", "value", "dimension_data"
     ):
         logger.info(
             f"Publishing metric: {metric_name} " +
-            (f"({dimension_name}:{dimension_value}) " if dimension_name and dimension_value else "") +
+            (f"({dimension_data} " if dimension_data else "") +
             f"with value: {value} at {datetime_period}"
         )
         metric_data.append(
             {
                 "MetricName": metric_name,
                 "Dimensions": [
                     {
                         "Name": dimension_name,
                         "Value": dimension_value
-                    },
-                ] if dimension_name and dimension_value else [],
+                    }
+                    for dimension_name, dimension_value in (dimension_data or {}).items()
+                ],
                 "Timestamp": datetime_period,
                 "Value": value
             }
         )
 
     if metric_data:
         # split in batches of max 1000
```

### Comparing `django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/migrations/0001_initial.py` & `django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.6/django_cloudwatch_metrics/signals.py` & `django_cloudwatch_metrics-0.0.7/django_cloudwatch_metrics/signals.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.6/pyproject.toml` & `django_cloudwatch_metrics-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cloudwatch-metrics"
-version = "0.0.6"
+version = "0.0.7"
 description = "Metric tracking in Django using caching and CloudWatch"
 authors = ["Bart Machielsen <bartmachielsen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "django_cloudwatch_metrics" }
```

### Comparing `django_cloudwatch_metrics-0.0.6/PKG-INFO` & `django_cloudwatch_metrics-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloudwatch-metrics
-Version: 0.0.6
+Version: 0.0.7
 Summary: Metric tracking in Django using caching and CloudWatch
 License: MIT
 Author: Bart Machielsen
 Author-email: bartmachielsen@gmail.com
 Requires-Python: >=3.6.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

