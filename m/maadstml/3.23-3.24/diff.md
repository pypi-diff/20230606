# Comparing `tmp/maadstml-3.23.tar.gz` & `tmp/maadstml-3.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\maadstml-3.23.tar", last modified: Tue Feb 28 18:12:36 2023, max compression
+gzip compressed data, was "maadstml-3.24.tar", last modified: Mon Jun  5 23:52:28 2023, max compression
```

## Comparing `maadstml-3.23.tar` & `maadstml-3.24.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 18:12:36.000000 maadstml-3.23/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.23/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.23/MANIFEST.in
--rw-rw-rw-   0        0        0   201274 2023-02-28 18:12:36.000000 maadstml-3.23/PKG-INFO
--rw-rw-rw-   0        0        0   165160 2023-02-28 18:02:17.000000 maadstml-3.23/README.md
-drwxrwxrwx   0        0        0        0 2023-02-28 18:12:36.000000 maadstml-3.23/maadstml/
--rw-rw-rw-   0        0        0     2084 2023-02-19 21:08:01.000000 maadstml-3.23/maadstml/__init__.py
--rw-rw-rw-   0        0        0    64739 2023-02-19 21:07:09.000000 maadstml-3.23/maadstml/sendfiles.py
-drwxrwxrwx   0        0        0        0 2023-02-28 18:12:36.000000 maadstml-3.23/maadstml.egg-info/
--rw-rw-rw-   0        0        0   201274 2023-02-28 18:12:36.000000 maadstml-3.23/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-02-28 18:12:36.000000 maadstml-3.23/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 18:12:36.000000 maadstml-3.23/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-02-28 18:12:36.000000 maadstml-3.23/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-28 18:12:36.000000 maadstml-3.23/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      122 2021-02-05 16:13:04.000000 maadstml-3.23/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-28 18:12:36.000000 maadstml-3.23/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-02-28 18:02:41.000000 maadstml-3.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 23:52:28.488510 maadstml-3.24/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.24/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.24/MANIFEST.in
+-rw-rw-rw-   0        0        0   171433 2023-06-05 23:52:28.488510 maadstml-3.24/PKG-INFO
+-rw-rw-rw-   0        0        0   170836 2023-06-05 23:48:59.000000 maadstml-3.24/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 23:52:28.472869 maadstml-3.24/maadstml/
+-rw-rw-rw-   0        0        0     2084 2023-02-19 21:08:01.000000 maadstml-3.24/maadstml/__init__.py
+-rw-rw-rw-   0        0        0    64739 2023-02-19 21:07:09.000000 maadstml-3.24/maadstml/sendfiles.py
+drwxrwxrwx   0        0        0        0 2023-06-05 23:52:28.488510 maadstml-3.24/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   171433 2023-06-05 23:52:28.000000 maadstml-3.24/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-05 23:52:28.000000 maadstml-3.24/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 23:52:28.000000 maadstml-3.24/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-06-05 23:52:28.000000 maadstml-3.24/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 23:52:28.000000 maadstml-3.24/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      122 2021-02-05 16:13:04.000000 maadstml-3.24/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 23:52:28.488510 maadstml-3.24/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-05 23:51:33.000000 maadstml-3.24/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `maadstml-3.23/LICENSE.txt` & `maadstml-3.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.23/README.md` & `maadstml-3.24/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,22 @@
   - Users can pre-process data streams using the following functions: MIN, MAX, AVG, COUNT, COUNTSTR, DIFF, DIFFMARGIN, SUM, MEDIAN, VARIANCE, OUTLIERS, OUTLIERSX-Y,VARIED, 
     ANOMPROB,ANOMPROBX-Y,ENTROPY, AUTOCORR, TREND, CONSISTENCY, IQR (InterQuartileRange), Midhinge, GM (Geometric mean), HM (Harmonic mean), Trimean, 
 	CV (coefficient of Variation),Mad (Mean absolute deviation), Skewness, Kurtosis, Spikedetect, Unique, Uniquestr, Timediff: time should be in this 
 	layout:2006-01-02T15:04:05, Timediff returns the difference in seconds between the first date/time and last datetime. Avgtimediff returns the 
     average time in seconds between consecutive dates.. Spikedetect uses a Zscore method to detect 
 	spikes in the data using lag of 5, StD of 3.5 from mean and influence of 0.5.  Geodiff (returns distance in Kilometers between two lat/long points)
 	
-    Unique Checks numeric data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
+    Dataage_[UTC offset]_[timetype], dataage can be used to check the last update time of the data in the data stream from
+	current local time.  You can specify the UTC offset to adjust the current time to match the timezone of the data stream.
+	You can specify timetype as millisecond, second, minute, hour, day.  For example, if Dataage_1_minute, then this processtype
+	will compare the last timestamp in the data stream, to the local UTC time offset +1 and compute the time difference
+	between the data stream timestamp and current local time and return the difference in minutes.  This is a very powerful processtype
+	for data quality and data assurance programs for any number of data streams.
+		
+	Unique Checks numeric data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
  
     Uniquestr Checks string data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
 
     Uniquecount Checks numeric data for duplication.  Returns count of unique numbers.
  
     Uniquestrcount Checks string data for duplication.  Returns count of unique strings.
 	
@@ -547,14 +554,21 @@
   AUTOCORR, TREND, CONSISTENCY, Unique, Uniquestr, Geodiff (returns distance in Kilometers between two lat/long points)
   IQR (InterQuartileRange), Midhinge, GM (Geometric mean), HM (Harmonic mean), Trimean, CV (coefficient of Variation), 
   Mad (Mean absolute deviation), Skewness, Kurtosis, Spikedetect, Timediff: time should be in this layout:2006-01-02T15:04:05,
   Timediff returns the difference in seconds between the first date/time and last datetime. Avgtimediff returns the 
   average time in seconds between consecutive dates.
   Spikedetect uses a Zscore method to detect spikes in the data using lag of 5, StD of 3.5 from mean and influence of 0.5.   
 
+  Dataage_[UTC offset]_[timetype], dataage can be used to check the last update time of the data in the data stream from
+  current local time.  You can specify the UTC offset to adjust the current time to match the timezone of the data stream.
+  You can specify timetype as millisecond, second, minute, hour, day.  For example, if Dataage_1_minute, then this processtype
+  will compare the last timestamp in the data stream, to the local UTC time offset +1 and compute the time difference
+  between the data stream timestamp and current local time and return the difference in minutes.  This is a very powerful processtype
+  for data quality and data assurance programs for any number of data streams.
+
   Unique Checks numeric data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
 
   Uniquestr Checks string data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
 
   Uniquecount Checks numeric data for duplication.  Returns count of unique numbers.
  
   Uniquestrcount Checks string data for duplication.  Returns count of unique strings.
@@ -670,14 +684,21 @@
   Mad (Mean absolute deviation), Skewness, Kurtosis, Spikedetect, Unique, Uniquestr, Timediff: time should be in this layout:2006-01-02T15:04:05,
   Timediff returns the difference in seconds between the first date/time and last datetime. Avgtimediff returns the 
   average time in seconds between consecutive dates. 
   Spikedetect uses a Zscore method to detect spikes in the data using lag of 5, StD of 3.5 from mean and influence of 0.5.   
   Geodiff (returns distance in Kilometers between two lat/long points)
   Unique Checks numeric data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
 
+  Dataage_[UTC offset]_[timetype], dataage can be used to check the last update time of the data in the data stream from
+  current local time.  You can specify the UTC offset to adjust the current time to match the timezone of the data stream.
+  You can specify timetype as millisecond, second, minute, hour, day.  For example, if Dataage_1_minute, then this processtype
+  will compare the last timestamp in the data stream, to the local UTC time offset +1 and compute the time difference
+  between the data stream timestamp and current local time and return the difference in minutes.  This is a very powerful processtype
+  for data quality and data assurance programs for any number of data streams.
+
   Uniquestr Checks string data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
 
   Uniquecount Checks numeric data for duplication.  Returns count of unique numbers.
  
   Uniquestrcount Checks string data for duplication.  Returns count of unique strings.
   
   CONSISTENCY checks if the data all have consistent data types. Returns 1 for consistent data types, 0 otherwise.
@@ -3161,14 +3182,21 @@
   Mad (Mean absolute deviation),Skewness, Kurtosis, Spikedetect, Unique, Uniquestr, Timediff: time should be in this layout:2006-01-02T15:04:05,
   Timediff returns the difference in seconds between the first date/time and last datetime. Avgtimediff returns the 
   average time in seconds between consecutive dates.
   Spikedetect uses a Zscore method to detect spikes in the data using lag of 5, StD of 3.5 from mean and influence of 0.5.
   Geodiff (returns distance in Kilometers between two lat/long points)
   Unique Checks numeric data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
 
+  Dataage_[UTC offset]_[timetype], dataage can be used to check the last update time of the data in the data stream from
+  current local time.  You can specify the UTC offset to adjust the current time to match the timezone of the data stream.
+  You can specify timetype as millisecond, second, minute, hour, day.  For example, if Dataage_1_minute, then this processtype
+  will compare the last timestamp in the data stream, to the local UTC time offset +1 and compute the time difference
+  between the data stream timestamp and current local time and return the difference in minutes.  This is a very powerful processtype
+  for data quality and data assurance programs for any number of data streams.
+
   Uniquestr Checks string data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
 
   Uniquecount Checks numeric data for duplication.  Returns count of unique numbers.
  
   Uniquestrcount Checks string data for duplication.  Returns count of unique strings.
   
   CONSISTENCY checks if the data all have consistent data types. Returns 1 for consistent data types, 0 otherwise.
@@ -3255,14 +3283,21 @@
   MAX, MIN, AVG, COUNT, COUNTSTR, SUM, DIFF, DIFFMARGIN, VARIANCE, MEDIAN, OUTLIERS, OUTLIERSX-Y, VARIED, ANOMPROB, ANOMPROBX-Y, ENTROPY, 
   AUTOCORR, TREND, CONSISTENCY, Unique, Uniquestr, Geodiff (returns distance in Kilometers between two lat/long points),
   IQR (InterQuartileRange), Midhinge, GM (Geometric mean), HM (Harmonic mean), Trimean, CV (coefficient of Variation), 
   Mad (Mean absolute deviation), Skewness, Kurtosis, Spikedetect, Timediff: time should be in this layout:2006-01-02T15:04:05,
   Timediff returns the difference in seconds between the first date/time and last datetime. Avgtimediff returns the 
   average time in seconds between consecutive dates.
   Uniquecount Checks numeric data for duplication.  Returns count of unique numbers.
+
+  Dataage_[UTC offset]_[timetype], dataage can be used to check the last update time of the data in the data stream from
+  current local time.  You can specify the UTC offset to adjust the current time to match the timezone of the data stream.
+  You can specify timetype as millisecond, second, minute, hour, day.  For example, if Dataage_1_minute, then this processtype
+  will compare the last timestamp in the data stream, to the local UTC time offset +1 and compute the time difference
+  between the data stream timestamp and current local time and return the difference in minutes.  This is a very powerful processtype
+  for data quality and data assurance programs for any number of data streams.
  
   Uniquestrcount Checks string data for duplication.  Returns count of unique strings.
   
   Meanci95 or Meanci99 - returns a 95% or 99% confidence interval: mean, low, high 
 
   RAW for no processing.
   
@@ -3528,14 +3563,21 @@
 
 - You can set conditions to aggregate functions: MIN, MAX, AVG, COUNT, COUNTSTR, DIFF, SUM, MEDIAN, VARIANCE, OUTLIERS, OUTLIERSX-Y, VARIED, ANOMPROB,ANOMPROBX-Y,
   ENTROPY, AUTOCORR, TREND, IQR (InterQuartileRange), Midhinge, GM (Geometric mean), HM (Harmonic mean), Trimean, CV (coefficient of Variation), 
   Mad (Mean absolute deviation),Skewness, Kurtosis, Spikedetect, Unique, Uniquestr, Timediff: time should be in this layout:2006-01-02T15:04:05,
   Timediff returns the difference in seconds between the first date/time and last datetime. Avgtimediff returns the 
   average time in seconds between consecutive dates.  Spikedetect uses a Zscore method to detect spikes in the data using lag of 5, 
   StD of 3.5 from mean and influence of 0.5.  Geodiff (returns distance in Kilometers between two lat/long points).
+
+  Dataage_[UTC offset]_[timetype], dataage can be used to check the last update time of the data in the data stream from
+  current local time.  You can specify the UTC offset to adjust the current time to match the timezone of the data stream.
+  You can specify timetype as millisecond, second, minute, hour, day.  For example, if Dataage_1_minute, then this processtype
+  will compare the last timestamp in the data stream, to the local UTC time offset +1 and compute the time difference
+  between the data stream timestamp and current local time and return the difference in minutes.  This is a very powerful processtype
+  for data quality and data assurance programs for any number of data streams.
   
   Unique Checks numeric data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
 
   Uniquestr Checks string data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
   Uniquecount Checks numeric data for duplication.  Returns count of unique numbers. 
   Uniquestrcount Checks string data for duplication.  Returns count of unique strings.
   
@@ -3623,14 +3665,21 @@
   Timediff returns the difference in seconds between the first date/time and last datetime. Avgtimediff returns the 
   average time in seconds between consecutive dates. 
   Geodiff (returns distance in Kilometers between two lat/long points).
   Spikedetect uses a Zscore method to detect spikes in the data using lag of 5, StD of 3.5 from mean and influence of 0.5.
   Uniquecount Checks numeric data for duplication.  Returns count of unique numbers.
   Uniquestrcount Checks string data for duplication.  Returns count of unique strings.
 
+  Dataage_[UTC offset]_[timetype], dataage can be used to check the last update time of the data in the data stream from
+  current local time.  You can specify the UTC offset to adjust the current time to match the timezone of the data stream.
+  You can specify timetype as millisecond, second, minute, hour, day.  For example, if Dataage_1_minute, then this processtype
+  will compare the last timestamp in the data stream, to the local UTC time offset +1 and compute the time difference
+  between the data stream timestamp and current local time and return the difference in minutes.  This is a very powerful processtype
+  for data quality and data assurance programs for any number of data streams.
+
   Meanci95 or Meanci99 - returns a 95% or 99% confidence interval: mean, low, high 
 
   The order of the operation must match the 
   order of the stream.  If you specified topicid, you can perform TML on the new preprocessed stream append appending: 
   _preprocessed_processlogic
   For example, if streamstojoin="stream1,stream2,streams3", and preprocesslogic="min,max,diff", the new streams will be:
   stream1_preprocessed_Min, stream2_preprocessed_Max, stream3_preprocessed_Diff.
@@ -3757,14 +3806,21 @@
   Mad (Mean absolute deviation),Skewness, Kurtosis, Spikedetect, Unique, Uniquestr, Timediff: time should be in this layout:2006-01-02T15:04:05,
   Timediff returns the difference in seconds between the first date/time and last datetime. Avgtimediff returns the 
   average time in seconds between consecutive dates.
   Spikedetect uses a Zscore method to detect spikes in the data using lag of 5, StD of 3.5 from mean and influence of 0.5.
   Geodiff (returns distance in Kilometers between two lat/long points)
   Unique Checks numeric data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
 
+  Dataage_[UTC offset]_[timetype], dataage can be used to check the last update time of the data in the data stream from
+  current local time.  You can specify the UTC offset to adjust the current time to match the timezone of the data stream.
+  You can specify timetype as millisecond, second, minute, hour, day.  For example, if Dataage_1_minute, then this processtype
+  will compare the last timestamp in the data stream, to the local UTC time offset +1 and compute the time difference
+  between the data stream timestamp and current local time and return the difference in minutes.  This is a very powerful processtype
+  for data quality and data assurance programs for any number of data streams.
+
   Uniquestr Checks string data for duplication.  Returns 1 if no data duplication (unique), 0 otherwise.
 
   Uniquecount Checks numeric data for duplication.  Returns count of unique numbers.
  
   Uniquestrcount Checks string data for duplication.  Returns count of unique strings.
   
   CONSISTENCY checks if the data all have consistent data types. Returns 1 for consistent data types, 0 otherwise.
```

### Comparing `maadstml-3.23/maadstml/__init__.py` & `maadstml-3.24/maadstml/__init__.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.23/maadstml/sendfiles.py` & `maadstml-3.24/maadstml/sendfiles.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.23/setup.py` & `maadstml-3.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.23',
+    version='3.24',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

