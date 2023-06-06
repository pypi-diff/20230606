# Comparing `tmp/mofish-1.0.4.tar.gz` & `tmp/mofish-2023.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mofish-1.0.4.tar", last modified: Fri Mar 11 06:20:21 2022, max compression
+gzip compressed data, was "mofish-2023.6.6.tar", last modified: Tue Jun  6 09:40:48 2023, max compression
```

## Comparing `mofish-1.0.4.tar` & `mofish-2023.6.6.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-03-11 06:20:21.461459 mofish-1.0.4/
--rw-rw-rw-   0        0        0      114 2022-02-10 09:50:46.000000 mofish-1.0.4/.gitignore
--rw-rw-rw-   0        0        0    11558 2022-02-10 07:21:54.000000 mofish-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1506 2022-03-11 06:20:21.461459 mofish-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      404 2022-02-10 07:16:55.000000 mofish-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2022-03-11 06:20:21.458588 mofish-1.0.4/mofish.egg-info/
--rw-rw-rw-   0        0        0     1506 2022-03-11 06:20:20.000000 mofish-1.0.4/mofish.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2022-03-11 06:20:21.000000 mofish-1.0.4/mofish.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-11 06:20:20.000000 mofish-1.0.4/mofish.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2022-03-11 06:20:20.000000 mofish-1.0.4/mofish.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2022-03-11 06:20:20.000000 mofish-1.0.4/mofish.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-03-11 06:20:20.000000 mofish-1.0.4/mofish.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       15 2022-02-10 07:09:41.000000 mofish-1.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-03-11 06:20:21.462461 mofish-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1802 2022-03-11 06:20:15.000000 mofish-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-11 06:20:21.460583 mofish-1.0.4/src/
--rw-rw-rw-   0        0        0        0 2022-02-10 09:36:47.000000 mofish-1.0.4/src/__init__.py
--rw-rw-rw-   0        0        0     5178 2022-03-11 06:16:57.000000 mofish-1.0.4/src/main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:40:48.636819 mofish-2023.6.6/
+-rw-rw-rw-   0        0        0    11558 2023-06-06 09:37:30.000000 mofish-2023.6.6/LICENSE
+-rw-rw-rw-   0        0        0     1509 2023-06-06 09:40:48.636819 mofish-2023.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-06-06 09:37:30.000000 mofish-2023.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 09:40:48.634930 mofish-2023.6.6/mofish.egg-info/
+-rw-rw-rw-   0        0        0     1509 2023-06-06 09:40:48.000000 mofish-2023.6.6/mofish.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-06-06 09:40:48.000000 mofish-2023.6.6/mofish.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 09:40:48.000000 mofish-2023.6.6/mofish.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-06 09:40:48.000000 mofish-2023.6.6/mofish.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2023-06-06 09:40:48.000000 mofish-2023.6.6/mofish.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-06 09:40:48.000000 mofish-2023.6.6/mofish.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 09:40:48.638117 mofish-2023.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1807 2023-06-06 09:40:36.000000 mofish-2023.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:40:48.636819 mofish-2023.6.6/src/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:37:30.000000 mofish-2023.6.6/src/__init__.py
+-rw-rw-rw-   0        0        0     5178 2023-06-06 09:38:58.000000 mofish-2023.6.6/src/main.py
+-rw-rw-rw-   0        0        0      478 2023-06-06 09:37:30.000000 mofish-2023.6.6/src/utils.py
```

### Comparing `mofish-1.0.4/LICENSE` & `mofish-2023.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mofish-1.0.4/PKG-INFO` & `mofish-2023.6.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mofish
-Version: 1.0.4
+Version: 2023.6.6
 Summary: 你好，摸鱼人，工作再累，一定不要忘记摸鱼哦! 有事没事起身去茶水间去廊道去天台走走，别老在工位上坐着。多喝点水，钱是老板的，但命是自己的!
 Home-page: https://github.com/PY-GZKY/Moyu_
 Author: PY-GZKY
 Author-email: 341796767@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mofish-1.0.4/mofish.egg-info/PKG-INFO` & `mofish-2023.6.6/mofish.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mofish
-Version: 1.0.4
+Version: 2023.6.6
 Summary: 你好，摸鱼人，工作再累，一定不要忘记摸鱼哦! 有事没事起身去茶水间去廊道去天台走走，别老在工位上坐着。多喝点水，钱是老板的，但命是自己的!
 Home-page: https://github.com/PY-GZKY/Moyu_
 Author: PY-GZKY
 Author-email: 341796767@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mofish-1.0.4/setup.py` & `mofish-2023.6.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 description = '你好，摸鱼人，工作再累，一定不要忘记摸鱼哦! 有事没事起身去茶水间去廊道去天台走走，别老在工位上坐着。多喝点水，钱是老板的，但命是自己的!'
 
 setup(
     name='mofish',
-    version='1.0.4',
+    version='2023.06.06',
     description=description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Framework :: AsyncIO',
         'Intended Audience :: Developers',
```

### Comparing `mofish-1.0.4/src/main.py` & `mofish-2023.6.6/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         5: '星期六',
         6: '星期天',
     }
     day = date.weekday()
     return week_day_dict[day]
 
 
-def get_closing_time(closing_time: str = "18:00:00"):
+def get_closing_time(closing_time: str = "17:45:00"):
     now_ = datetime.datetime.now()
     target_ = datetime.datetime.strptime(f"{now_.year}-{now_.month}-{now_.day} {closing_time}", '%Y-%m-%d %H:%M:%S')
     if now_ < target_:
         time_delta_ = target_ - now_
         secs = time_delta_.seconds
         hours = secs // 3600
         mins = (secs % 3600) // 60
```

