# Comparing `tmp/mysqlx-1.1.6.tar.gz` & `tmp/mysqlx-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.1.6.tar", last modified: Tue Jun  6 08:34:12 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.1.8.tar", last modified: Tue Jun  6 12:34:29 2023, max compression
```

## Comparing `mysqlx-1.1.6.tar` & `mysqlx-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 08:34:12.000000 mysqlx-1.1.6/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.1.6/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-06 08:34:12.000000 mysqlx-1.1.6/mysqlx/
--rw-rw-rw-   0        0        0     4695 2023-06-06 01:46:24.000000 mysqlx-1.1.6/mysqlx/coder.py
--rw-rw-rw-   0        0        0    10181 2023-06-06 08:33:31.000000 mysqlx-1.1.6/mysqlx/db.py
--rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.1.6/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     5285 2023-06-06 08:02:21.000000 mysqlx-1.1.6/mysqlx/helper.py
--rw-rw-rw-   0        0        0     8173 2023-06-05 13:04:14.000000 mysqlx-1.1.6/mysqlx/orm.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.1.6/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:34:12.000000 mysqlx-1.1.6/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-06 08:34:12.000000 mysqlx-1.1.6/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.1.6/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      411 2023-06-06 08:34:12.000000 mysqlx-1.1.6/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-06 08:34:12.000000 mysqlx-1.1.6/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      287 2023-06-06 08:34:12.000000 mysqlx-1.1.6/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 08:34:12.000000 mysqlx-1.1.6/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      411 2023-06-06 08:34:12.000000 mysqlx-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-06 08:34:12.000000 mysqlx-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      814 2023-06-06 08:33:55.000000 mysqlx-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:34:29.000000 mysqlx-1.1.8/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.1.8/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx/
+-rw-rw-rw-   0        0        0     4695 2023-06-06 01:46:24.000000 mysqlx-1.1.8/mysqlx/coder.py
+-rw-rw-rw-   0        0        0    10185 2023-06-06 12:23:19.000000 mysqlx-1.1.8/mysqlx/db.py
+-rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.1.8/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     5285 2023-06-06 08:02:21.000000 mysqlx-1.1.8/mysqlx/helper.py
+-rw-rw-rw-   0        0        0     9143 2023-06-06 12:33:16.000000 mysqlx-1.1.8/mysqlx/orm.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.1.8/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.1.8/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      404 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      297 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      404 2023-06-06 12:34:29.000000 mysqlx-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2598 2023-06-06 12:09:45.000000 mysqlx-1.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 12:34:29.000000 mysqlx-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-06-06 12:33:16.000000 mysqlx-1.1.8/setup.py
```

### Comparing `mysqlx-1.1.6/LICENSE` & `mysqlx-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.6/mysqlx/coder.py` & `mysqlx-1.1.8/mysqlx/coder.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.6/mysqlx/db.py` & `mysqlx-1.1.8/mysqlx/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     global _DB_CTX
     sql, args = dynamic_sql(sql, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def select_one(sql: str, *args, **kwargs):
     """
-    Execute select SQL and expected one result.
+    Execute select SQL and expected one row result.
     If no result found, return None.
     If multiple results found, the first one returned.
     >>> u1 = dict(id=100, name='Alice', email='alice@test.org', passwd='ABC-12345', last_modified=time.time())
     >>> u2 = dict(id=101, name='Sarah', email='sarah@test.org', passwd='ABC-12345', last_modified=time.time())
     >>> insert('user', **u1)
     1
     >>> insert('user', **u2)
```

### Comparing `mysqlx-1.1.6/mysqlx/dbx.py` & `mysqlx-1.1.8/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.6/mysqlx/helper.py` & `mysqlx-1.1.8/mysqlx/helper.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.6/mysqlx/orm.py` & `mysqlx-1.1.8/mysqlx/orm.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,105 +80,138 @@
                 sql = 'UPDATE `%s` SET `del_flag`=1, `update_by`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (self.__table__, UPDATE_TIME, pk)
                 return db.do_execute(sql, update_by, _id)
         else:
             raise KeyError("Not primary key.")
 
     @classmethod
     def insert(cls, **kwargs):
-        table = Model._get_table(cls)
+        table = cls._get_table(cls)
         return db.insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
-        table = Model._get_table(cls)
+        table = cls._get_table(cls)
         return db.save(table, **kwargs)
 
     @classmethod
     def find_by_id(cls, id: int, *selection):
-        pk, table = Model._get_pk_and_table(cls)
+        """
+        Return one object or None if no result.
+        """
+        pk, table = cls._get_pk_and_table(cls)
+        result = cls.select_by_id(id, *selection)
+        return cls.dict2obj(result, cls, pk, table) if result else None
+
+    @classmethod
+    def find_by_ids(cls, ids: Iterable[int], *selection):
+        """
+        Return list(object) or empty list if no result.
+        """
+        pk, table = cls._get_pk_and_table(cls)
+        return [cls.dict2obj(d, cls, pk, table) for d in cls.select_by_ids(ids, *selection)]
+
+    @classmethod
+    def select_by_id(cls, id: int, *selection):
+        """
+        Return one row(dict) or None if no result.
+        """
+        pk, table = cls._get_pk_and_table(cls)
         if len(selection) == 0:
             sql = 'SELECT * FROM `%s` WHERE `%s`=? limit 1' % (table, pk)
         else:
             sql = 'SELECT %s FROM `%s` WHERE `%s`=? limit 1' % (','.join(['`%s`' % col for col in selection]), table, pk)
-        result = db.do_select_one(sql, id)
-        return Model.dict2obj(result, cls, pk, table) if result else None
+        return db.do_select_one(sql, id)
 
     @classmethod
-    def find_by_ids(cls, ids: Iterable[int], *selection):
+    def select_by_ids(cls, ids: Iterable[int], *selection):
+        """
+        Return list(dict) or empty list if no result.
+        """
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
-        pk, table = Model._get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table(cls)
         ids_str = ','.join(list(map(str, ids)))
         if len(selection) == 0:
             sql = 'SELECT * FROM `%s` WHERE `%s` in (%s) limit %d' % (table, pk, ids_str, ids_size)
         else:
             sql = 'SELECT %s FROM `%s` WHERE `%s` in (%s) limit %d' % (','.join(['`%s`' % col for col in selection]), table, pk, ids_str, ids_size)
-        return [Model.dict2obj(d, cls, pk, table) for d in db.do_select(sql)]
+        return db.do_select(sql)
 
     @classmethod
     def update_by_id(cls, id: int, **kwargs):
-        pk, table = Model._get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table(cls)
         cols, args = zip(*kwargs.items())
         args = [*args, id]
         if UPDATE_TIME in kwargs:
             sql = 'UPDATE `%s` SET %s WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), UPDATE_TIME, pk)
         else:
             sql = 'UPDATE `%s` SET %s, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), UPDATE_TIME, pk)
         db.do_execute(sql, *args)
 
     @classmethod
     def delete_by_id(cls, id: int):
-        pk, table = Model._get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table(cls)
         sql = 'DELETE FROM `%s` WHERE `%s`=? limit 1' % (table, pk)
         return db.do_execute(sql, id)
 
     @classmethod
     def delete_by_ids(cls, ids: Iterable[int]):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
-        pk, table = Model._get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table(cls)
         sql = 'DELETE FROM `%s` WHERE `%s` in (%s) limit %d' % (table, pk, ','.join(list(map(str, ids))), ids_size)
         return db.do_execute(sql)
 
     @classmethod
     def logic_delete_by_id(cls, id: int, update_by: int = None):
-        pk, table = Model._get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table(cls)
         if update_by is None:
             sql = 'UPDATE `%s` SET `del_flag`=1, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, UPDATE_TIME, pk)
             return db.do_execute(sql, id)
         else:
             sql = 'UPDATE `%s` SET `del_flag`=1, `update_by`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, UPDATE_TIME, pk)
             return db.do_execute(sql, update_by, id)
 
     @classmethod
     def logic_delete_by_ids(cls, ids: Iterable[int], update_by: int = None):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
-        pk, table = Model._get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table(cls)
         ids_str = ','.join(list(map(str, ids)))
         if update_by is None:
             sql = 'UPDATE `%s` SET `del_flag`=1, `%s`=CURRENT_TIMESTAMP WHERE `%s` in (%s) limit %d' % (table, UPDATE_TIME, pk, ids_str, ids_size)
             return db.execute(sql)
         else:
             sql = 'UPDATE `%s` SET `del_flag`=1, `update_by`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s` in (%s) limit %d' % (table, UPDATE_TIME, pk, ids_str, ids_size)
             return db.do_execute(sql, update_by)
 
     @classmethod
     def find_all(cls, *selection, limit=100):
-        pk, table = Model._get_pk_and_table(cls)
+        """
+        Return list(object) or empty list if no result.
+        """
+        pk, table = cls._get_pk_and_table(cls)
+        return [cls.dict2obj(d, cls, pk, table) for d in cls.select_all(*selection, limit=limit)]
+
+    @classmethod
+    def select_all(cls, *selection, limit=100):
+        """
+        Return list(dict) or empty list if no result.
+        """
+        pk, table = cls._get_pk_and_table(cls)
         if len(selection) == 0:
             sql = 'SELECT * FROM `%s` limit %d' % (table, limit)
         else:
             sql = 'SELECT %s FROM `%s` limit %d' % (','.join(['`%s`' % col for col in selection]), table, limit)
-        return [Model.dict2obj(d, cls, pk, table) for d in db.do_select(sql)]
+        return db.do_select(sql)
 
     @staticmethod
     def _get_pk_and_table(cls):
-        pk = Model._get_pk(cls)
-        table = Model._get_table(cls)
+        pk = cls._get_pk(cls)
+        table = cls._get_table(cls)
         return pk, table
 
     @staticmethod
     def _get_pk(cls):
         pk = cls.__dict__.get(PK)
         return pk if pk else 'id'
```

### Comparing `mysqlx-1.1.6/setup.py` & `mysqlx-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     packages=find_packages(),
     description="mysqlx is a simple python sql executor for MySQL like iBatis.",
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.1.6',
-    url='https://gitee.com/summry/mysqlx/mysqlx',
+    version='1.1.8',
+    url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.txt'],
     },
```

