# Comparing `tmp/libeeepy-1.8.0-py3-none-any.whl.zip` & `tmp/libeeepy-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 12130 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      114 b- defN 21-Dec-30 03:41 libeeepy/__init__.py
--rw-rw-rw-  2.0 fat    53148 b- defN 22-Jan-05 09:13 libeeepy/calculateaccuracy.py
+Zip file size: 12175 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      114 b- defN 22-Jan-06 01:45 libeeepy/__init__.py
+-rw-rw-rw-  2.0 fat    53726 b- defN 22-Jan-06 01:43 libeeepy/calculateaccuracy.py
 -rw-rw-rw-  2.0 fat     6448 b- defN 21-Dec-30 03:41 libeeepy/dataprocessing.py
 -rw-rw-rw-  2.0 fat     5054 b- defN 21-Dec-30 03:41 libeeepy/operatemysql.py
--rw-rw-rw-  2.0 fat      465 b- defN 22-Jan-05 09:17 libeeepy-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 22-Jan-05 09:17 libeeepy-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Jan-05 09:17 libeeepy-1.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      627 b- defN 22-Jan-05 09:17 libeeepy-1.8.0.dist-info/RECORD
-8 files, 65962 bytes uncompressed, 11038 bytes compressed:  83.3%
+-rw-rw-rw-  2.0 fat      465 b- defN 22-Jan-06 01:46 libeeepy-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 22-Jan-06 01:46 libeeepy-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 22-Jan-06 01:46 libeeepy-1.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      627 b- defN 22-Jan-06 01:46 libeeepy-1.9.0.dist-info/RECORD
+8 files, 66540 bytes uncompressed, 11083 bytes compressed:  83.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: libeeepy/dataprocessing.py
 Comment: 
 
 Filename: libeeepy/operatemysql.py
 Comment: 
 
-Filename: libeeepy-1.8.0.dist-info/METADATA
+Filename: libeeepy-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: libeeepy-1.8.0.dist-info/WHEEL
+Filename: libeeepy-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: libeeepy-1.8.0.dist-info/top_level.txt
+Filename: libeeepy-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: libeeepy-1.8.0.dist-info/RECORD
+Filename: libeeepy-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libeeepy/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .operatemysql import *
 from .dataprocessing import *
 from .calculateaccuracy import *
-__version__ = "v1.6.0"
+__version__ = "v1.9.0"
```

## libeeepy/calculateaccuracy.py

```diff
@@ -61,18 +61,25 @@
 
         index_more = numpy.where(self.power_real > self.capacity * para)
         dt = self.date_time[index_more[0]]
         pr = self.power_real[index_more[0]]
         pf = self.power_forecast[index_more[0]]
         len_loop = len(dt)
         time_list = []
-        for loop in range(len_loop):
-            t = datetime.datetime.strptime(dt[loop], '%Y-%m-%d_%H:%M:%S')
-            y_m = t.strftime('%Y-%m')
-            time_list.append(y_m)
+
+        if self.date_time[0][10] == '_':
+            for loop in range(len_loop):
+                t = datetime.datetime.strptime(dt[loop], '%Y-%m-%d_%H:%M:%S')
+                y_m = t.strftime('%Y-%m')
+                time_list.append(y_m)
+        else:
+            for loop in range(len_loop):
+                t = datetime.datetime.strptime(dt[loop], '%Y-%m-%d %H:%M:%S')
+                y_m = t.strftime('%Y-%m')
+                time_list.append(y_m)
 
         bias_abs = abs(pr - pf)
 
         # 创建 DataFrame
         df = pandas.DataFrame({'date': time_list, 'bias': bias_abs})
         error_mean = df['bias'].groupby(df['date']).mean()
         MAE = error_mean/float(self.capacity) * 100.0
@@ -80,18 +87,25 @@
         return MAE
 
     def calculate_MSE(self):
 
         len_loop = len(self.date_time)
         ymd_list = []
 
-        for a_loop in range(len_loop):
-            t = datetime.datetime.strptime(self.date_time[a_loop], '%Y-%m-%d_%H:%M:%S')
-            y_m_d = t.strftime('%Y-%m-%d')
-            ymd_list.append(y_m_d)
+        if self.date_time[0][10] == '_':
+
+            for a_loop in range(len_loop):
+                t = datetime.datetime.strptime(self.date_time[a_loop], '%Y-%m-%d_%H:%M:%S')
+                y_m_d = t.strftime('%Y-%m-%d')
+                ymd_list.append(y_m_d)
+        else:
+            for a_loop in range(len_loop):
+                t = datetime.datetime.strptime(self.date_time[a_loop], '%Y-%m-%d %H:%M:%S')
+                y_m_d = t.strftime('%Y-%m-%d')
+                ymd_list.append(y_m_d)
 
         bias = self.power_real - self.power_forecast
         bias_square = numpy.square(bias)
 
         # 创建 DataFrame
         df_day = pandas.DataFrame({'date': ymd_list, 'bias_square': bias_square})
         error_day_mean = df_day['bias_square'].groupby(df_day['date']).mean()
```

## Comparing `libeeepy-1.8.0.dist-info/RECORD` & `libeeepy-1.9.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-libeeepy/__init__.py,sha256=30cf5bFDZcWJ2UHsOzFQZvVmdbBwohXLAh4LrXgEVuE,114
-libeeepy/calculateaccuracy.py,sha256=yC0-Ftm16zYpXaSo5ul-snJ_-LHxNchcOLwDMzeYizU,53148
+libeeepy/__init__.py,sha256=KIgec28wWmxyDiHQ0ZNfuKCe5F7IqaaGWvTKCUAhw8Q,114
+libeeepy/calculateaccuracy.py,sha256=SZIU-OQXISyfadE7x3uL6jORWFYJI33c9hfaeq6XcY0,53726
 libeeepy/dataprocessing.py,sha256=T2iQ07NvScIGYqiYDQZLX9C9k0fNd0BXhcqtKJLdw4U,6448
 libeeepy/operatemysql.py,sha256=xVAAtub3JHis9kxjXzgVKDS31AM1ad2aEJrg9rf6TDQ,5054
-libeeepy-1.8.0.dist-info/METADATA,sha256=FVCS5jNzTYsWsL9svENPysFq2giwjvUS1IupUMr3Z5c,465
-libeeepy-1.8.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-libeeepy-1.8.0.dist-info/top_level.txt,sha256=GwgaDIXkQNHqRQlrOZ32alGenGFq8Q3nqdvyZvmyi_g,9
-libeeepy-1.8.0.dist-info/RECORD,,
+libeeepy-1.9.0.dist-info/METADATA,sha256=yhltQcCPP5kyhHhY-KUjaEU8wiidor_S9L6ybO6saJ8,465
+libeeepy-1.9.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+libeeepy-1.9.0.dist-info/top_level.txt,sha256=GwgaDIXkQNHqRQlrOZ32alGenGFq8Q3nqdvyZvmyi_g,9
+libeeepy-1.9.0.dist-info/RECORD,,
```

