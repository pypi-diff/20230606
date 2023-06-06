# Comparing `tmp/m_mock-1.3.1.tar.gz` & `tmp/m_mock-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m_mock-1.3.1.tar", last modified: Tue Mar  7 01:24:10 2023, max compression
+gzip compressed data, was "m_mock-1.3.2.tar", last modified: Tue Jun  6 01:49:05 2023, max compression
```

## Comparing `m_mock-1.3.1.tar` & `m_mock-1.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 01:24:10.949267 m_mock-1.3.1/
--rw-rw-rw-   0        0        0    35823 2023-01-10 07:52:57.000000 m_mock-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     4084 2023-03-07 01:24:10.948476 m_mock-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3669 2023-02-20 05:50:41.000000 m_mock-1.3.1/README.md
--rw-rw-rw-   0        0        0      590 2023-02-02 02:44:01.000000 m_mock-1.3.1/license.txt
-drwxrwxrwx   0        0        0        0 2023-03-07 01:24:10.937438 m_mock-1.3.1/m_mock.egg-info/
--rw-rw-rw-   0        0        0     4084 2023-03-07 01:24:10.000000 m_mock-1.3.1/m_mock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-03-07 01:24:10.000000 m_mock-1.3.1/m_mock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 01:24:10.000000 m_mock-1.3.1/m_mock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-03-07 01:24:10.000000 m_mock-1.3.1/m_mock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-07 01:24:10.000000 m_mock-1.3.1/m_mock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      423 2023-03-07 01:23:07.000000 m_mock-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-07 01:24:10.949267 m_mock-1.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-07 01:24:10.941441 m_mock-1.3.1/x_mock/
--rw-rw-rw-   0        0        0     2771 2023-03-06 07:38:46.000000 m_mock-1.3.1/x_mock/m_mock.py
--rw-rw-rw-   0        0        0    29432 2023-03-06 14:14:15.000000 m_mock-1.3.1/x_mock/m_random.py
--rw-rw-rw-   0        0        0     2394 2023-03-06 08:01:50.000000 m_mock-1.3.1/x_mock/m_random_source.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:24:10.947450 m_mock-1.3.1/x_mock/test_case/
--rw-rw-rw-   0        0        0      212 2023-03-06 07:38:46.000000 m_mock-1.3.1/x_mock/test_case/common_utils.py
--rw-rw-rw-   0        0        0     1852 2023-03-06 07:38:46.000000 m_mock-1.3.1/x_mock/test_case/test_basic.py
--rw-rw-rw-   0        0        0     1463 2023-03-06 07:38:46.000000 m_mock-1.3.1/x_mock/test_case/test_date.py
--rw-rw-rw-   0        0        0      219 2023-03-06 07:38:46.000000 m_mock-1.3.1/x_mock/test_case/test_helper.py
--rw-rw-rw-   0        0        0      768 2023-03-06 08:03:03.000000 m_mock-1.3.1/x_mock/test_case/test_name.py
+drwxrwxrwx   0        0        0        0 2023-06-06 01:49:05.169645 m_mock-1.3.2/
+-rw-rw-rw-   0        0        0    35823 2023-01-10 07:52:57.000000 m_mock-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     4221 2023-06-06 01:49:05.168673 m_mock-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3806 2023-06-06 01:34:11.000000 m_mock-1.3.2/README.md
+-rw-rw-rw-   0        0        0      590 2023-02-02 02:44:01.000000 m_mock-1.3.2/license.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 01:49:05.150058 m_mock-1.3.2/m_mock/
+-rw-rw-rw-   0        0        0    29432 2023-06-05 15:24:20.000000 m_mock-1.3.2/m_mock/m_random.py
+-rw-rw-rw-   0        0        0     2394 2023-03-06 08:01:50.000000 m_mock-1.3.2/m_mock/m_random_source.py
+-rw-rw-rw-   0        0        0     2815 2023-06-05 15:24:20.000000 m_mock-1.3.2/m_mock/mock.py
+drwxrwxrwx   0        0        0        0 2023-06-06 01:49:05.166648 m_mock-1.3.2/m_mock/test_case/
+-rw-rw-rw-   0        0        0      210 2023-06-06 01:30:27.000000 m_mock-1.3.2/m_mock/test_case/common_utils.py
+-rw-rw-rw-   0        0        0     1929 2023-06-06 01:31:58.000000 m_mock-1.3.2/m_mock/test_case/test_basic.py
+-rw-rw-rw-   0        0        0     1463 2023-06-05 15:24:20.000000 m_mock-1.3.2/m_mock/test_case/test_date.py
+-rw-rw-rw-   0        0        0      219 2023-06-05 15:24:20.000000 m_mock-1.3.2/m_mock/test_case/test_helper.py
+-rw-rw-rw-   0        0        0      768 2023-06-05 15:24:20.000000 m_mock-1.3.2/m_mock/test_case/test_name.py
+drwxrwxrwx   0        0        0        0 2023-06-06 01:49:05.156678 m_mock-1.3.2/m_mock.egg-info/
+-rw-rw-rw-   0        0        0     4221 2023-06-06 01:49:05.000000 m_mock-1.3.2/m_mock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-06-06 01:49:05.000000 m_mock-1.3.2/m_mock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 01:49:05.000000 m_mock-1.3.2/m_mock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-06 01:49:05.000000 m_mock-1.3.2/m_mock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 01:49:05.000000 m_mock-1.3.2/m_mock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      433 2023-06-06 01:35:12.000000 m_mock-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 01:49:05.169645 m_mock-1.3.2/setup.cfg
```

### Comparing `m_mock-1.3.1/LICENSE` & `m_mock-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m_mock-1.3.1/PKG-INFO` & `m_mock-1.3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: m_mock
-Version: 1.3.1
+Version: 1.3.2
 Summary: This is a tool for producing random data.
-Author-email: Franciz <912953887@qq.com>
+Author-email: Franciz <franciz467@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: license.txt
 
+# v1.3.2更改了方法名称
+更新后需要更改原方法的import
+
+# install
+pip install m-mock
+
 # mock
 
 仿照mock.js生成随机数据
 
 ## Basic
 
 ### character 字符
@@ -51,29 +57,30 @@
 m_mock.mock("@float(3)"):229342892631770.44
 m_mock.mock("@float()"):872256.00439
 ```
 
 ### string 字符串
 
 ```python
-m_mock.mock("@string(2)"):$@
-m_mock.mock("@string("lower", 3)"):nyx
-m_mock.mock("@string("upper", 3)"):HWS
-m_mock.mock("@string("number", 3)"):987
-m_mock.mock("@string("symbol", 3)"):^)<
-m_mock.mock("@string("aeiou", 3)"):iee
-m_mock.mock("@string("lower", 1, 3)"):gn
-m_mock.mock("@string("upper", 1, 3)"):DSZ
-m_mock.mock("@string("number", 1, 3)"):773
-m_mock.mock("@string("symbol", 1, 3)"):#(<
-m_mock.mock("@string("aeiou", 1, 3)"):eaa
-m_mock.mock("@string("chinese", 1, 3)"):太主截
-m_mock.mock("@string("cn_symbol", 1, 3)"):『“
-m_mock.mock("@string("cn_string", 3, 9)"):〕壁辨钻眠素举沾。
-m_mock.mock("@string("cn_string", 1)"):柔
+m_mock.mock('@string(2)'):W3
+m_mock.mock('@string('lower', 3)'):icz
+m_mock.mock('@string('upper', 3)'):NBE
+m_mock.mock('@string('number', 3)'):108
+m_mock.mock('@string('symbol', 3)'):!%=
+m_mock.mock('@string('aeiou', 3)'):eia
+m_mock.mock('@string('lower', 1, 3)'):fih
+m_mock.mock('@string('upper', 1, 3)'):F
+m_mock.mock('@string('number', 1, 3)'):102
+m_mock.mock('@string('symbol', 1, 3)'):`
+m_mock.mock('@string('aeiou', 1, 3)'):aao
+m_mock.mock('@string('chinese', 1, 3)'):捎创
+m_mock.mock('@string('cn_symbol', 1, 3)'):～
+m_mock.mock('@string('cn_string', 3, 9)'):〉·，（鉴或【落【
+m_mock.mock('@string('cn_string', 1)'):侄
+m_mock.mock('@string('abcd', 2)'):bd
 ```
 
 ## name 中英文姓名
 
 ```python
 m_mock.mock("@clast()"):折
 m_mock.mock("@cfirst()"):丰
```

### Comparing `m_mock-1.3.1/README.md` & `m_mock-1.3.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# v1.3.2更改了方法名称
+更新后需要更改原方法的import
+
+# install
+pip install m-mock
+
 # mock
 
 仿照mock.js生成随机数据
 
 ## Basic
 
 ### character 字符
@@ -38,29 +44,30 @@
 m_mock.mock("@float(3)"):229342892631770.44
 m_mock.mock("@float()"):872256.00439
 ```
 
 ### string 字符串
 
 ```python
-m_mock.mock("@string(2)"):$@
-m_mock.mock("@string("lower", 3)"):nyx
-m_mock.mock("@string("upper", 3)"):HWS
-m_mock.mock("@string("number", 3)"):987
-m_mock.mock("@string("symbol", 3)"):^)<
-m_mock.mock("@string("aeiou", 3)"):iee
-m_mock.mock("@string("lower", 1, 3)"):gn
-m_mock.mock("@string("upper", 1, 3)"):DSZ
-m_mock.mock("@string("number", 1, 3)"):773
-m_mock.mock("@string("symbol", 1, 3)"):#(<
-m_mock.mock("@string("aeiou", 1, 3)"):eaa
-m_mock.mock("@string("chinese", 1, 3)"):太主截
-m_mock.mock("@string("cn_symbol", 1, 3)"):『“
-m_mock.mock("@string("cn_string", 3, 9)"):〕壁辨钻眠素举沾。
-m_mock.mock("@string("cn_string", 1)"):柔
+m_mock.mock('@string(2)'):W3
+m_mock.mock('@string('lower', 3)'):icz
+m_mock.mock('@string('upper', 3)'):NBE
+m_mock.mock('@string('number', 3)'):108
+m_mock.mock('@string('symbol', 3)'):!%=
+m_mock.mock('@string('aeiou', 3)'):eia
+m_mock.mock('@string('lower', 1, 3)'):fih
+m_mock.mock('@string('upper', 1, 3)'):F
+m_mock.mock('@string('number', 1, 3)'):102
+m_mock.mock('@string('symbol', 1, 3)'):`
+m_mock.mock('@string('aeiou', 1, 3)'):aao
+m_mock.mock('@string('chinese', 1, 3)'):捎创
+m_mock.mock('@string('cn_symbol', 1, 3)'):～
+m_mock.mock('@string('cn_string', 3, 9)'):〉·，（鉴或【落【
+m_mock.mock('@string('cn_string', 1)'):侄
+m_mock.mock('@string('abcd', 2)'):bd
 ```
 
 ## name 中英文姓名
 
 ```python
 m_mock.mock("@clast()"):折
 m_mock.mock("@cfirst()"):丰
@@ -112,8 +119,8 @@
 m_mock.mock("@now('day')"):2023-02-20 00:00:00
 m_mock.mock("@now('hour')"):2023-02-20 13:00:00
 m_mock.mock("@now('minute')"):2023-02-20 13:42:00
 m_mock.mock("@now('second')"):2023-02-20 13:42:44
 m_mock.mock("@now()"):2023-02-20 13:42:44
 m_mock.mock("@now('year','%Y年-%m月-%d日 %H:%M:%S')"):2023年-01月-01日 00:00:00
 m_mock.mock("@now('week','%Y年 %m月 %d日 %H:%M:%S')"):2023年 02月 26日 00:00:00
-```
+```
```

### Comparing `m_mock-1.3.1/license.txt` & `m_mock-1.3.2/license.txt`

 * *Files identical despite different names*

### Comparing `m_mock-1.3.1/m_mock.egg-info/PKG-INFO` & `m_mock-1.3.2/m_mock.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: m-mock
-Version: 1.3.1
+Version: 1.3.2
 Summary: This is a tool for producing random data.
-Author-email: Franciz <912953887@qq.com>
+Author-email: Franciz <franciz467@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: license.txt
 
+# v1.3.2更改了方法名称
+更新后需要更改原方法的import
+
+# install
+pip install m-mock
+
 # mock
 
 仿照mock.js生成随机数据
 
 ## Basic
 
 ### character 字符
@@ -51,29 +57,30 @@
 m_mock.mock("@float(3)"):229342892631770.44
 m_mock.mock("@float()"):872256.00439
 ```
 
 ### string 字符串
 
 ```python
-m_mock.mock("@string(2)"):$@
-m_mock.mock("@string("lower", 3)"):nyx
-m_mock.mock("@string("upper", 3)"):HWS
-m_mock.mock("@string("number", 3)"):987
-m_mock.mock("@string("symbol", 3)"):^)<
-m_mock.mock("@string("aeiou", 3)"):iee
-m_mock.mock("@string("lower", 1, 3)"):gn
-m_mock.mock("@string("upper", 1, 3)"):DSZ
-m_mock.mock("@string("number", 1, 3)"):773
-m_mock.mock("@string("symbol", 1, 3)"):#(<
-m_mock.mock("@string("aeiou", 1, 3)"):eaa
-m_mock.mock("@string("chinese", 1, 3)"):太主截
-m_mock.mock("@string("cn_symbol", 1, 3)"):『“
-m_mock.mock("@string("cn_string", 3, 9)"):〕壁辨钻眠素举沾。
-m_mock.mock("@string("cn_string", 1)"):柔
+m_mock.mock('@string(2)'):W3
+m_mock.mock('@string('lower', 3)'):icz
+m_mock.mock('@string('upper', 3)'):NBE
+m_mock.mock('@string('number', 3)'):108
+m_mock.mock('@string('symbol', 3)'):!%=
+m_mock.mock('@string('aeiou', 3)'):eia
+m_mock.mock('@string('lower', 1, 3)'):fih
+m_mock.mock('@string('upper', 1, 3)'):F
+m_mock.mock('@string('number', 1, 3)'):102
+m_mock.mock('@string('symbol', 1, 3)'):`
+m_mock.mock('@string('aeiou', 1, 3)'):aao
+m_mock.mock('@string('chinese', 1, 3)'):捎创
+m_mock.mock('@string('cn_symbol', 1, 3)'):～
+m_mock.mock('@string('cn_string', 3, 9)'):〉·，（鉴或【落【
+m_mock.mock('@string('cn_string', 1)'):侄
+m_mock.mock('@string('abcd', 2)'):bd
 ```
 
 ## name 中英文姓名
 
 ```python
 m_mock.mock("@clast()"):折
 m_mock.mock("@cfirst()"):丰
```

### Comparing `m_mock-1.3.1/x_mock/m_mock.py` & `m_mock-1.3.2/m_mock/mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from x_mock import m_random
+from m_mock import m_random
 
 
 class MockM:
 
     def mock(self, mock_str):
         keyword = self.get_mocker_key(mock_str)
         args = self.get_mocker_params_to_tuple(mock_str)
@@ -38,14 +38,16 @@
             return m_random.m_name.cname(*args)
         elif keyword == 'first':
             return m_random.m_name.first(*args)
         elif keyword == 'last':
             return m_random.m_name.last(*args)
         elif keyword == 'name':
             return m_random.m_name.name(*args)
+        else:
+            return mock_str
 
     @classmethod
     def get_mocker_key(cls, mock_str):
         if not mock_str.startswith('@'):
             raise m_random.MockPyExpressionException()
         if not mock_str.endswith(')'):
             # 非)结尾说明是@date,则直接返回属性名
```

### Comparing `m_mock-1.3.1/x_mock/m_random.py` & `m_mock-1.3.2/m_mock/m_random.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 import re
 import string
 from datetime import datetime, timedelta
 
 from dateutil.relativedelta import relativedelta
 
-from x_mock.m_random_source import single_family_name, en_family_name, en_name
+from m_mock.m_random_source import single_family_name, en_family_name, en_name
 
 
 def inNone(obj):
     if isinstance(obj, (tuple, list)):
         # 都为空的就返回True
         boo = []
         for i in obj:
```

### Comparing `m_mock-1.3.1/x_mock/m_random_source.py` & `m_mock-1.3.2/m_mock/m_random_source.py`

 * *Files identical despite different names*

### Comparing `m_mock-1.3.1/x_mock/test_case/test_date.py` & `m_mock-1.3.2/m_mock/test_case/test_date.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from x_mock import m_random
-from x_mock.test_case.common_utils import execute
+from m_mock import m_random
+from m_mock.test_case.common_utils import execute
 
 
 class TestDate:
     def test_date(self):
         execute("@date('%Y-%m-%d %H:%M:%S', '+1d')")
         execute("@date('%Y-%m-%d %H:%M:%S', '+24h')")
         # 格式化
```

### Comparing `m_mock-1.3.1/x_mock/test_case/test_name.py` & `m_mock-1.3.2/m_mock/test_case/test_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from x_mock.m_random import m_name
-from x_mock.test_case.common_utils import execute
+from m_mock.m_random import m_name
+from m_mock.test_case.common_utils import execute
 
 
 class TestName:
     def test_name(self):
         execute("""@clast()""")
         execute("""@cfirst()""")
         execute("""@cname()""")
```

