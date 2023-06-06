# Comparing `tmp/huhangkai-1.2.0.tar.gz` & `tmp/huhangkai-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.2.0.tar", last modified: Fri Jun  2 10:32:55 2023, max compression
+gzip compressed data, was "huhangkai-1.2.2.tar", last modified: Tue Jun  6 08:37:54 2023, max compression
```

## Comparing `huhangkai-1.2.0.tar` & `huhangkai-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 10:32:55.447068 huhangkai-1.2.0/
--rw-rw-rw-   0        0        0      228 2023-06-02 10:32:55.446068 huhangkai-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 10:32:55.435098 huhangkai-1.2.0/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.2.0/commen/__init__.py
--rw-rw-rw-   0        0        0    31571 2023-06-02 07:34:45.000000 huhangkai-1.2.0/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.2.0/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.2.0/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    20438 2023-06-02 10:32:12.000000 huhangkai-1.2.0/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.2.0/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-06-02 10:02:56.000000 huhangkai-1.2.0/commen/unit_request.py
--rw-rw-rw-   0        0        0     2461 2023-05-25 08:37:49.000000 huhangkai-1.2.0/commen/unit_tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:32:55.445071 huhangkai-1.2.0/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-06-02 10:32:55.000000 huhangkai-1.2.0/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-06-02 10:32:55.000000 huhangkai-1.2.0/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 10:32:55.000000 huhangkai-1.2.0/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-02 10:32:55.000000 huhangkai-1.2.0/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 10:32:55.000000 huhangkai-1.2.0/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 10:32:55.447068 huhangkai-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-06-02 10:32:46.000000 huhangkai-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:37:54.897881 huhangkai-1.2.2/
+-rw-rw-rw-   0        0        0      228 2023-06-06 08:37:54.896884 huhangkai-1.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 08:37:54.884765 huhangkai-1.2.2/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.2.2/commen/__init__.py
+-rw-rw-rw-   0        0        0    31571 2023-06-02 07:34:45.000000 huhangkai-1.2.2/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.2.2/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.2.2/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    22834 2023-06-06 08:37:33.000000 huhangkai-1.2.2/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.2.2/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-06-02 10:02:56.000000 huhangkai-1.2.2/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2461 2023-05-25 08:37:49.000000 huhangkai-1.2.2/commen/unit_tasks.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:37:54.895887 huhangkai-1.2.2/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-06-06 08:37:54.000000 huhangkai-1.2.2/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-06-06 08:37:54.000000 huhangkai-1.2.2/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 08:37:54.000000 huhangkai-1.2.2/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-06-06 08:37:54.000000 huhangkai-1.2.2/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 08:37:54.000000 huhangkai-1.2.2/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 08:37:54.897881 huhangkai-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      600 2023-06-06 08:37:40.000000 huhangkai-1.2.2/setup.py
```

### Comparing `huhangkai-1.2.0/commen/__init__.py` & `huhangkai-1.2.2/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.0/commen/init_project.py` & `huhangkai-1.2.2/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.0/commen/unit_dict.py` & `huhangkai-1.2.2/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.0/commen/unit_encryption.py` & `huhangkai-1.2.2/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.0/commen/unit_fun.py` & `huhangkai-1.2.2/commen/unit_fun.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,22 +22,21 @@
         self._route = ""
         self._token = ""
         self._host = ""
 
     # mock 方法，默认中国，详情搜python Faker模块
     def faker(self, locale='zh_CN'):
         return Faker(locale=locale)
-    
+
     def seelp(self, v=1, *args, **kwargs):
         if isinstance(v, int):
             self.log_info("seelp: %s" % v)
             time.sleep(v)
         else:
             time.sleep(1)
-            
 
     def _faker_name(self):
         return self._faker.name() + str(self._faker.numerify())
 
     @staticmethod
     def random_vin():
         # 内容的权值
@@ -70,15 +69,16 @@
         char3 = '1234567890'
         while True:
             code = random.choice(char0)
             code += random.choice(char1)
             code += "".join(random.choices(char2, k=4))
             code += random.choice(char3)
             return code
-            test = re.match('^.\w.[A-Z]\d{4}$|^.\w.\d[A-Z]\d{3}$|^.\w.\d{2}[A-Z]\d{2}$|^.\w.\d{3}[A-Z]\d$|^.\w.\d{5}$', code)
+            test = re.match('^.\w.[A-Z]\d{4}$|^.\w.\d[A-Z]\d{3}$|^.\w.\d{2}[A-Z]\d{2}$|^.\w.\d{3}[A-Z]\d$|^.\w.\d{5}$',
+                            code)
             if test:
                 return code
 
     # # mock方法，国家locale_list随机，也可根据数字获取第几个国家，超出时随机
     # def faker_random_country(self, locale=None):
     #     country = None
     #     if locale:
@@ -118,14 +118,15 @@
 
     def time_ms(self, string=None, fmt="%Y-%m-%d"):
         time_array = self.time(string=string, fmt=fmt)
         return time_array * 1000
 
     def data_str(self):
         return datetime.datetime.now().strftime("%Y-%m-%d")
+
     # # 根据sql语句执行sql
     # def run_mysql(self, sql_str="", host="", user="", password="", database=""):
     #     sql_str = sql_str or self.sql_str
     #     if self._db.get(host+database):
     #         cursor = self._db.get(host+database)
     #     else:
     #         try:
@@ -163,15 +164,15 @@
                 tmp_list.append("%s is null " % (i[6:],))
             elif "in__" in i:
                 if len(kwargs.get(i)) > 1:
                     tmp_list.append("%s in %s " % (i[4:], str(tuple(kwargs.get(i)))))
                 elif len(kwargs.get(i)) == 1:
                     tmp_list.append("%s = \"%s\" " % (i[4:], str(kwargs.get(i)[0])))
                 else:
-                    tmp_list.append("%s = \"&$#@\" " % (i[4:], ))
+                    tmp_list.append("%s = \"&$#@\" " % (i[4:],))
             else:
                 tmp_list.append("%s = \"%s\" " % (i, kwargs.get(i)))
         tmp_list.extend(kwargs.get("where_list") or [])
         if tmp_list:
             where_str += " where " + " and ".join(tmp_list)
         if kwargs.get("group_by"):
             where_str += " group by " + kwargs.get('group_by') + " "
@@ -206,21 +207,21 @@
                     if key in res2.keys():
                         key2 = key
                     else:
                         key2 = re.sub(r'[A-Z]', lambda n: "_" + str(n.group()).lower(), key)
                 else:
                     key1 = key[0]
                     key2 = key[1]
-                if not(not res1[key1] and not res2[key2]):
+                if not (not res1[key1] and not res2[key2]):
                     if type(res1[key1]) == int:
                         res2[key2] = int(res2[key2])
                     elif type(res1[key1]) == float:
                         res2[key2] = float(res2[key2])
-                    if not(res1[key1] == res2[key2] or str(res1[key1]).strip() == str(res2[key2]).strip() or
-                           (not res1[key1] and not res2[key2])):
+                    if not (res1[key1] == res2[key2] or str(res1[key1]).strip() == str(res2[key2]).strip() or
+                            (not res1[key1] and not res2[key2])):
                         if not ("time" in key1.lower() and len(str(res1[key1])) == 19 and len(str(res2[key2])) == 19
                                 and str(res1[key1])[0:10] == str(res2[key2])[0:10]
                                 and str(res1[key1])[11:] == str(res2[key2])[11:]):
                             self.log_info("比较字段：" + str(key) + "  不一致")
                             return False
             except Exception as e:
                 self.log_info("比较字段：" + str(key) + "  不一致")
@@ -365,15 +366,15 @@
         elif type == 3:
             self._time2 = self._time1
             self._time1 += random.randint(0, 30)
         elif type == 4:
             self._time2 = self._time1
             self._time1 += random.randint(0, 365)
         elif type == 5:
-            tmp = random.randint(self._time2, self._time1)\
+            tmp = random.randint(self._time2, self._time1) \
                 if self._time1 > self._time2 else random.randint(self._time1, self._time2)
 
             self._time2 = self._time1
             self._time1 = tmp
 
         data = str(self._faker.date_between(self._time1, self._time1))
         return (data if self._faker.boolean() else None) if null else data
@@ -412,15 +413,15 @@
             return kwargs.pop(name)
         except:
             return None
 
     def get_kwargs(self, kwargs):
         kwargs.update(kwargs.get('kwargs', {}))
         _kwargs = {k: v for k, v in kwargs.items() if (k not in ('self', 'kwargs') and k[0] != '_')
-                 or k in ('_route', '_token', '_host')}
+                   or k in ('_route', '_token', '_host')}
         if not kwargs.get('_route') and self._route:
             _kwargs['_route'] = self._route
         if not kwargs.get('_token') and self._token:
             _kwargs['_token'] = self._token
         if not kwargs.get('_host') and self._host:
             _kwargs['_host'] = self._host
         return _kwargs
@@ -447,33 +448,75 @@
                         return [i.get(name) for i in value]
                     elif isinstance(value, dict):
                         for key2, value2 in value.items():
                             if isinstance(value2, list):
                                 return [i.get(name) for i in value2 if i.get(name)]
             return []
 
-    def excelWriter(self, filename, data, sheet_name="sheet", set_column=[]):
+    def excelWriter(self, filename, data, sheet_name="sheet", set_column=[], header_format=None):
         from pandas import DataFrame, ExcelWriter
         filename = filename[:4] + filename[4:].replace(":", "").replace(' ', '_')
-        with ExcelWriter(filename) as writer:
-            # 写入到第一个sheet
-            if data and isinstance(data[0], list):
-                h = data[0]
-                data1 = []
-                for i in data[1:]:
-                    data1.append({x[0]: str(x[1]) for x in zip(h, i)})
-                data = data1
-            elif data and isinstance(data[0], dict):
-                data = [{k: str(v) for k, v in i.items()} for i in data]
-            DataFrame(data).to_excel(writer,
-                              sheet_name=sheet_name,
-                              index=False,
-                              engine="openpyxl"
-                              )
-
+        try:
+            with ExcelWriter(filename) as writer:
+                # 写入到第一个sheet
+                if data and isinstance(data[0], list):
+                    h = data[0]
+                    data1 = []
+                    for i in data[1:]:
+                        data1.append({x[0]: str(x[1]) for x in zip(h, i)})
+                    data = data1
+                elif data and isinstance(data[0], dict):
+                    data = [{k: str(v) for k, v in i.items()} for i in data]
+                result = DataFrame(data)
+                result.to_excel(writer, sheet_name=sheet_name, index=False, engine="openpyxl")
+
+                try:
+                    worksheet = writer.sheets.get(sheet_name) or writer.sheets.get("sheet1")
+                    for idx, v in enumerate(set_column):
+                        try:
+                            if idx < len(result.columns.values):
+                                worksheet.set_column(idx, idx, float(v.strip()))
+                        except Exception as e:
+                            logger.info(str(e))
+                except Exception as e:
+                    logger.info(str(e))
+
+                try:
+                    if header_format:
+                        if isinstance(header_format, str):
+                            header_format = eval(header_format)
+                        elif isinstance(header_format, dict):
+                            header_format = [header_format]
+
+                        if isinstance(header_format, list):
+                            header_format = header_format
+                            workbook = writer.book
+                            worksheet = writer.sheets.get(sheet_name) or writer.sheets.get("sheet1")
+                            for format in header_format:
+                                if "left_column" in format.keys():
+                                    left_colume = format['left_column']
+                                    del format['left_column']
+                                else:
+                                    left_colume = 0
+                                if "right_column" in format.keys():
+                                    right_column = format['right_column']
+                                    del format['right_column']
+                                else:
+                                    right_column = 999
+                                format = workbook.add_format(format)
+                                for col_num, value in enumerate(result.columns.values):
+                                    if col_num >= left_colume and col_num <= right_column:
+                                        try:
+                                            worksheet.write(0, col_num, value, format)
+                                        except Exception as e:
+                                            logger.info(str(e))
+                except Exception as e:
+                    logger.info(str(e))
+        except Exception as e:
+            logger.info(str(e))
 
 if __name__ == '__main__':
     print(FunBase().random_carnum())
     # f = FunBase().faker()
 
     # print(f.name())  # 随机姓名
     # print(f.ipv4())  # 随机IP4地址
```

### Comparing `huhangkai-1.2.0/commen/unit_logger.py` & `huhangkai-1.2.2/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.0/commen/unit_request.py` & `huhangkai-1.2.2/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.0/commen/unit_tasks.py` & `huhangkai-1.2.2/commen/unit_tasks.py`

 * *Files identical despite different names*

