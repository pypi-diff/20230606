# Comparing `tmp/pofinance-0.0.2.tar.gz` & `tmp/pofinance-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pofinance-0.0.2.tar", last modified: Tue Jun  6 12:46:22 2023, max compression
+gzip compressed data, was "pofinance-0.0.3.tar", last modified: Tue Jun  6 17:31:50 2023, max compression
```

## Comparing `pofinance-0.0.2.tar` & `pofinance-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.289601 pofinance-0.0.2/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pofinance-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4115 2023-06-06 12:46:22.289601 pofinance-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3570 2023-06-04 03:26:57.000000 pofinance-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.262300 pofinance-0.0.2/pofinance/
--rw-rw-rw-   0        0        0       36 2023-06-02 15:40:09.000000 pofinance-0.0.2/pofinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.276075 pofinance-0.0.2/pofinance/api/
--rw-rw-rw-   0        0        0        0 2023-06-02 15:40:09.000000 pofinance-0.0.2/pofinance/api/__init__.py
--rw-rw-rw-   0        0        0     4598 2023-06-05 15:28:12.000000 pofinance-0.0.2/pofinance/api/shares.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.281084 pofinance-0.0.2/pofinance/core/
--rw-rw-rw-   0        0        0     8970 2023-06-02 15:33:35.000000 pofinance-0.0.2/pofinance/core/PDFType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.2/pofinance/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.283085 pofinance-0.0.2/pofinance/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.2/pofinance/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.286687 pofinance-0.0.2/pofinance/lib/pdf/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 pofinance-0.0.2/pofinance/lib/pdf/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-03-24 15:13:04.000000 pofinance-0.0.2/pofinance/lib/pdf/add_watermark_service.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.271565 pofinance-0.0.2/pofinance.egg-info/
--rw-rw-rw-   0        0        0     4115 2023-06-06 12:46:22.000000 pofinance-0.0.2/pofinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-06 12:46:22.000000 pofinance-0.0.2/pofinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 12:46:22.000000 pofinance-0.0.2/pofinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 15:37:07.000000 pofinance-0.0.2/pofinance.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-06 12:46:22.000000 pofinance-0.0.2/pofinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      708 2023-06-06 12:46:22.291606 pofinance-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pofinance-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.479105 pofinance-0.0.3/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pofinance-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4117 2023-06-06 17:31:50.479105 pofinance-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3572 2023-06-06 12:47:55.000000 pofinance-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.454366 pofinance-0.0.3/pofinance/
+-rw-rw-rw-   0        0        0       36 2023-06-02 15:40:09.000000 pofinance-0.0.3/pofinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.466881 pofinance-0.0.3/pofinance/api/
+-rw-rw-rw-   0        0        0        0 2023-06-02 15:40:09.000000 pofinance-0.0.3/pofinance/api/__init__.py
+-rw-rw-rw-   0        0        0     4986 2023-06-06 17:31:05.000000 pofinance-0.0.3/pofinance/api/shares.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.473090 pofinance-0.0.3/pofinance/core/
+-rw-rw-rw-   0        0        0     8970 2023-06-02 15:33:35.000000 pofinance-0.0.3/pofinance/core/PDFType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.3/pofinance/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.474106 pofinance-0.0.3/pofinance/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.3/pofinance/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.477105 pofinance-0.0.3/pofinance/lib/pdf/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 pofinance-0.0.3/pofinance/lib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-03-24 15:13:04.000000 pofinance-0.0.3/pofinance/lib/pdf/add_watermark_service.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:31:50.461870 pofinance-0.0.3/pofinance.egg-info/
+-rw-rw-rw-   0        0        0     4117 2023-06-06 17:31:50.000000 pofinance-0.0.3/pofinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-06 17:31:50.000000 pofinance-0.0.3/pofinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:31:50.000000 pofinance-0.0.3/pofinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 15:37:07.000000 pofinance-0.0.3/pofinance.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-06 17:31:50.000000 pofinance-0.0.3/pofinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      708 2023-06-06 17:31:50.480104 pofinance-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pofinance-0.0.3/setup.py
```

### Comparing `pofinance-0.0.2/LICENSE` & `pofinance-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pofinance-0.0.2/PKG-INFO` & `pofinance-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pofinance
-Version: 0.0.2
+Version: 0.0.3
 Summary: pip install pofinance
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pofinance/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/pofinance/blob/master/README.md
@@ -89,15 +89,15 @@
 6. 等待维护者合并
 
 
 ### 🐞提供bug反馈或建议
 
 提交问题反馈时，请务必填写和python-office代码本身有关的问题，不进行有关python学习，甚至是个人练习的知识答疑和讨论。
 
-- [Github issue](https://github.com/CoderWanFeng/wftools/issues)
+- [Github issue](https://github.com/CoderWanFeng/pofinance/issues)
 
 -------------------------------------------------------------------------------
 
 
 ## 📌联系作者
```

### Comparing `pofinance-0.0.2/README.md` & `pofinance-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 6. 等待维护者合并
 
 
 ### 🐞提供bug反馈或建议
 
 提交问题反馈时，请务必填写和python-office代码本身有关的问题，不进行有关python学习，甚至是个人练习的知识答疑和讨论。
 
-- [Github issue](https://github.com/CoderWanFeng/wftools/issues)
+- [Github issue](https://github.com/CoderWanFeng/pofinance/issues)
 
 -------------------------------------------------------------------------------
 
 
 ## 📌联系作者
```

### Comparing `pofinance-0.0.2/pofinance/api/shares.py` & `pofinance-0.0.3/pofinance/api/shares.py`

 * *Files 25% similar despite different names*

```diff
@@ -99,37 +99,37 @@
         Args:
             sale_price_num: 批量卖出的数据，格式： [(500, 27.33), (300, 24.67), (数量, 价格)]
 
         Returns:
             批量卖出的全部数量，一次全部买入的最低盈利价格
         """
         base_price = 0
-        while True:
+        sum_num = 0  # 总股数
+        compare_goog_list = []
+        while base_price < max([item[1] for item in sale_price_num]):
             sum_num = 0  # 股票总数
             sale_good_list = []  # 每次交易的收益
             for item in sale_price_num:
                 sale_num = item[0]
                 sum_num += sale_num
                 sale_price = item[1]
                 sale_good_list.append(self.single_t(base_price, sale_price, sale_num))
-            if sum(sale_good_list) > 0:
-                if sum(sale_good_list) - self.cal_buy_cost(base_price, sum_num)[1] <= 0:
-                    base_price = base_price - 0.01
-                    break
-                # elif
-                else:
-                    base_price = base_price + 0.01
-
-        return (sum_num, base_price)
+            if sum(sale_good_list) > 0 and sum(sale_good_list) - self.cal_buy_cost(base_price, sum_num)[1] > 0:
+                compare_goog_list.append((base_price, sum(sale_good_list) - self.cal_buy_cost(base_price, sum_num)[1]))
+            base_price = base_price + 0.01
+        return f"一次性卖出的总股数：{sum_num}，最高价格为：{min(compare_goog_list, key=lambda t: t[1])[0]}，最小收益为： {min(compare_goog_list, key=lambda t: t[1])[1]}"
 
 
 if __name__ == '__main__':
     s_p = [(500, 27.33), (300, 26.9)]
 
     # print(t1(s_p))
 
     # print(t0(27.11, 26.9, 300))
     # print(t0(27.11, 27.33, 500))
 
-    t = MakeT()
-    print(t.single_t(27.11, 26.9, 300))
-    print(t.batch_t(s_p))
+    # t = MakeT()
+    # print(t.single_t(27.11, 26.9, 300))
+    # print(t.batch_t(s_p))
+    a = [('a', 2), ('ee', 3), ('mm', 4), ('x', 1)]
+    a = [(0, 22042), (0.01, 22022), (0.02, 3), ]
+    print(min(a, key=lambda t: t[1]))
```

### Comparing `pofinance-0.0.2/pofinance/core/PDFType.py` & `pofinance-0.0.3/pofinance/core/PDFType.py`

 * *Files identical despite different names*

### Comparing `pofinance-0.0.2/pofinance/lib/pdf/add_watermark_service.py` & `pofinance-0.0.3/pofinance/lib/pdf/add_watermark_service.py`

 * *Files identical despite different names*

### Comparing `pofinance-0.0.2/pofinance.egg-info/PKG-INFO` & `pofinance-0.0.3/pofinance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pofinance
-Version: 0.0.2
+Version: 0.0.3
 Summary: pip install pofinance
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pofinance/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/pofinance/blob/master/README.md
@@ -89,15 +89,15 @@
 6. 等待维护者合并
 
 
 ### 🐞提供bug反馈或建议
 
 提交问题反馈时，请务必填写和python-office代码本身有关的问题，不进行有关python学习，甚至是个人练习的知识答疑和讨论。
 
-- [Github issue](https://github.com/CoderWanFeng/wftools/issues)
+- [Github issue](https://github.com/CoderWanFeng/pofinance/issues)
 
 -------------------------------------------------------------------------------
 
 
 ## 📌联系作者
```

### Comparing `pofinance-0.0.2/setup.cfg` & `pofinance-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f66 696e 616e 6365 0d0a 7665   = pofinance..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 320d 0a64  rsion = 0.0.2..d
+00000020: 7273 696f 6e20 3d20 302e 302e 330d 0a64  rsion = 0.0.3..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2070 6970  escription = pip
 00000040: 2069 6e73 7461 6c6c 2070 6f66 696e 616e   install pofinan
 00000050: 6365 0d0a 6c6f 6e67 5f64 6573 6372 6970  ce..long_descrip
 00000060: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000070: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000080: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
 00000090: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
```

