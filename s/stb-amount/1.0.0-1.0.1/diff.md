# Comparing `tmp/stb_amount-1.0.0.tar.gz` & `tmp/stb_amount-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stb_amount-1.0.0.tar", last modified: Mon Jun  5 15:54:55 2023, max compression
+gzip compressed data, was "stb_amount-1.0.1.tar", last modified: Tue Jun  6 08:26:27 2023, max compression
```

## Comparing `stb_amount-1.0.0.tar` & `stb_amount-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-05 15:54:55.430004 stb_amount-1.0.0/
--rw-r--r--   0 mac        (501) staff       (20)      245 2023-06-05 15:54:55.429558 stb_amount-1.0.0/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-05 15:54:55.430159 stb_amount-1.0.0/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      498 2023-06-05 15:51:12.000000 stb_amount-1.0.0/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-05 15:54:55.426369 stb_amount-1.0.0/stb_amount/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-05 15:52:01.000000 stb_amount-1.0.0/stb_amount/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1228 2023-06-05 15:48:31.000000 stb_amount-1.0.0/stb_amount/stb.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-05 15:54:55.428993 stb_amount-1.0.0/stb_amount.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      245 2023-06-05 15:54:55.000000 stb_amount-1.0.0/stb_amount.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      185 2023-06-05 15:54:55.000000 stb_amount-1.0.0/stb_amount.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-05 15:54:55.000000 stb_amount-1.0.0/stb_amount.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2023-06-05 15:54:55.000000 stb_amount-1.0.0/stb_amount.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 08:26:27.265435 stb_amount-1.0.1/
+-rw-rw-rw-   0        0        0     1066 2023-06-06 07:28:10.000000 stb_amount-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      278 2023-06-06 08:26:27.265435 stb_amount-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-06 07:33:12.000000 stb_amount-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 08:26:27.265435 stb_amount-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-06-06 07:33:19.000000 stb_amount-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:26:27.250275 stb_amount-1.0.1/stb_amount/
+-rw-rw-rw-   0        0        0        0 2023-06-06 07:28:10.000000 stb_amount-1.0.1/stb_amount/__init__.py
+-rw-rw-rw-   0        0        0      943 2023-06-06 07:32:37.000000 stb_amount-1.0.1/stb_amount/stb.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:26:27.263436 stb_amount-1.0.1/stb_amount.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-06-06 08:26:27.000000 stb_amount-1.0.1/stb_amount.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-06-06 08:26:27.000000 stb_amount-1.0.1/stb_amount.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 08:26:27.000000 stb_amount-1.0.1/stb_amount.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 08:26:27.000000 stb_amount-1.0.1/stb_amount.egg-info/top_level.txt
```

### Comparing `stb_amount-1.0.0/stb_amount/stb.py` & `stb_amount-1.0.1/stb_amount/stb.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,33 +14,20 @@
         self._available = available
 
 
 class STBAmount(ISTBAmount):
 
     def insert(self, amount):
         self.available = self.available + amount
-        return self
+        return self.available
 
     def update_insert(self, last_amount, new_amount):
         self.available = self.available - last_amount + new_amount
-        return self
+        return self.available
 
     def update_remove(self, last_amount, new_amount):
         self.available = self.available + last_amount - new_amount
-        return self
+        return self.available
 
     def remove(self, amount):
         self.available = self.available - amount
-        return self
-
-    def get(self):
         return self.available
-
-# sf = SFCalculator(10)
-# sf.insert(1)
-# print("insert: {}".format(sf.get()))
-# sf.update_insert(1, 2)
-# print("update insert: {}".format(sf.get()))
-# sf.update_remove(1, 2)
-# print("update remove: {}".format(sf.get()))
-# sf.remove(1)
-# print("remove: {}".format(sf.get()))
```

