# Comparing `tmp/pofinance-0.0.3.tar.gz` & `tmp/pofinance-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pofinance-0.0.3.tar", last modified: Tue Jun  6 17:31:50 2023, max compression
+gzip compressed data, was "pofinance-0.0.4.tar", last modified: Tue Jun  6 17:35:29 2023, max compression
```

## Comparing `pofinance-0.0.3.tar` & `pofinance-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.479105 pofinance-0.0.3/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pofinance-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4117 2023-06-06 17:31:50.479105 pofinance-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3572 2023-06-06 12:47:55.000000 pofinance-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.454366 pofinance-0.0.3/pofinance/
--rw-rw-rw-   0        0        0       36 2023-06-02 15:40:09.000000 pofinance-0.0.3/pofinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.466881 pofinance-0.0.3/pofinance/api/
--rw-rw-rw-   0        0        0        0 2023-06-02 15:40:09.000000 pofinance-0.0.3/pofinance/api/__init__.py
--rw-rw-rw-   0        0        0     4986 2023-06-06 17:31:05.000000 pofinance-0.0.3/pofinance/api/shares.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.473090 pofinance-0.0.3/pofinance/core/
--rw-rw-rw-   0        0        0     8970 2023-06-02 15:33:35.000000 pofinance-0.0.3/pofinance/core/PDFType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.3/pofinance/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.474106 pofinance-0.0.3/pofinance/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.3/pofinance/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.477105 pofinance-0.0.3/pofinance/lib/pdf/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 pofinance-0.0.3/pofinance/lib/pdf/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-03-24 15:13:04.000000 pofinance-0.0.3/pofinance/lib/pdf/add_watermark_service.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.461870 pofinance-0.0.3/pofinance.egg-info/
--rw-rw-rw-   0        0        0     4117 2023-06-06 17:31:50.000000 pofinance-0.0.3/pofinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-06 17:31:50.000000 pofinance-0.0.3/pofinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 17:31:50.000000 pofinance-0.0.3/pofinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 15:37:07.000000 pofinance-0.0.3/pofinance.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-06 17:31:50.000000 pofinance-0.0.3/pofinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      708 2023-06-06 17:31:50.480104 pofinance-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pofinance-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:35:29.714750 pofinance-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pofinance-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4117 2023-06-06 17:35:29.714750 pofinance-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3572 2023-06-06 12:47:55.000000 pofinance-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 17:35:29.691881 pofinance-0.0.4/pofinance/
+-rw-rw-rw-   0        0        0       36 2023-06-02 15:40:09.000000 pofinance-0.0.4/pofinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:35:29.702210 pofinance-0.0.4/pofinance/api/
+-rw-rw-rw-   0        0        0        0 2023-06-02 15:40:09.000000 pofinance-0.0.4/pofinance/api/__init__.py
+-rw-rw-rw-   0        0        0     4986 2023-06-06 17:35:03.000000 pofinance-0.0.4/pofinance/api/shares.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:35:29.707230 pofinance-0.0.4/pofinance/core/
+-rw-rw-rw-   0        0        0     8970 2023-06-02 15:33:35.000000 pofinance-0.0.4/pofinance/core/PDFType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.4/pofinance/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:35:29.709230 pofinance-0.0.4/pofinance/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.4/pofinance/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:35:29.713747 pofinance-0.0.4/pofinance/lib/pdf/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 pofinance-0.0.4/pofinance/lib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-03-24 15:13:04.000000 pofinance-0.0.4/pofinance/lib/pdf/add_watermark_service.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:35:29.697851 pofinance-0.0.4/pofinance.egg-info/
+-rw-rw-rw-   0        0        0     4117 2023-06-06 17:35:29.000000 pofinance-0.0.4/pofinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-06 17:35:29.000000 pofinance-0.0.4/pofinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:35:29.000000 pofinance-0.0.4/pofinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 15:37:07.000000 pofinance-0.0.4/pofinance.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-06 17:35:29.000000 pofinance-0.0.4/pofinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      708 2023-06-06 17:35:29.715749 pofinance-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pofinance-0.0.4/setup.py
```

### Comparing `pofinance-0.0.3/LICENSE` & `pofinance-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pofinance-0.0.3/PKG-INFO` & `pofinance-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pofinance
-Version: 0.0.3
+Version: 0.0.4
 Summary: pip install pofinance
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pofinance/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/pofinance/blob/master/README.md
```

### Comparing `pofinance-0.0.3/README.md` & `pofinance-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pofinance-0.0.3/pofinance/api/shares.py` & `pofinance-0.0.4/pofinance/api/shares.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 sale_num = item[0]
                 sum_num += sale_num
                 sale_price = item[1]
                 sale_good_list.append(self.single_t(base_price, sale_price, sale_num))
             if sum(sale_good_list) > 0 and sum(sale_good_list) - self.cal_buy_cost(base_price, sum_num)[1] > 0:
                 compare_goog_list.append((base_price, sum(sale_good_list) - self.cal_buy_cost(base_price, sum_num)[1]))
             base_price = base_price + 0.01
-        return f"一次性卖出的总股数：{sum_num}，最高价格为：{min(compare_goog_list, key=lambda t: t[1])[0]}，最小收益为： {min(compare_goog_list, key=lambda t: t[1])[1]}"
+        return f"一次性买出的总股数：{sum_num}，最高价格为：{min(compare_goog_list, key=lambda t: t[1])[0]}，最小收益为： {min(compare_goog_list, key=lambda t: t[1])[1]}"
 
 
 if __name__ == '__main__':
     s_p = [(500, 27.33), (300, 26.9)]
 
     # print(t1(s_p))
```

### Comparing `pofinance-0.0.3/pofinance/core/PDFType.py` & `pofinance-0.0.4/pofinance/core/PDFType.py`

 * *Files identical despite different names*

### Comparing `pofinance-0.0.3/pofinance/lib/pdf/add_watermark_service.py` & `pofinance-0.0.4/pofinance/lib/pdf/add_watermark_service.py`

 * *Files identical despite different names*

### Comparing `pofinance-0.0.3/pofinance.egg-info/PKG-INFO` & `pofinance-0.0.4/pofinance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pofinance
-Version: 0.0.3
+Version: 0.0.4
 Summary: pip install pofinance
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pofinance/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/pofinance/blob/master/README.md
```

### Comparing `pofinance-0.0.3/setup.cfg` & `pofinance-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f66 696e 616e 6365 0d0a 7665   = pofinance..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 330d 0a64  rsion = 0.0.3..d
+00000020: 7273 696f 6e20 3d20 302e 302e 340d 0a64  rsion = 0.0.4..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2070 6970  escription = pip
 00000040: 2069 6e73 7461 6c6c 2070 6f66 696e 616e   install pofinan
 00000050: 6365 0d0a 6c6f 6e67 5f64 6573 6372 6970  ce..long_descrip
 00000060: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000070: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000080: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
 00000090: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
```

