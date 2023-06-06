# Comparing `tmp/mysqlx-1.1.4.tar.gz` & `tmp/mysqlx-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.1.4.tar", last modified: Wed Dec 29 04:18:27 2021, max compression
+gzip compressed data, was "dist\mysqlx-1.1.5.tar", last modified: Tue Jun  6 08:06:39 2023, max compression
```

## Comparing `mysqlx-1.1.4.tar` & `mysqlx-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2021-12-29 04:18:27.000000 mysqlx-1.1.4/
-drwxrwxrwx   0        0        0        0 2021-12-29 04:18:27.000000 mysqlx-1.1.4/mysqlx/
--rw-rw-rw-   0        0        0     8404 2021-12-29 04:18:09.000000 mysqlx-1.1.4/mysqlx/db.py
--rw-rw-rw-   0        0        0     2846 2021-12-27 16:48:30.000000 mysqlx-1.1.4/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     4609 2021-12-27 17:26:53.000000 mysqlx-1.1.4/mysqlx/model.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.1.4/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-29 04:18:27.000000 mysqlx-1.1.4/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2021-12-29 04:18:27.000000 mysqlx-1.1.4/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-29 04:18:27.000000 mysqlx-1.1.4/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      397 2021-12-29 04:18:27.000000 mysqlx-1.1.4/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2021-12-29 04:18:27.000000 mysqlx-1.1.4/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      248 2021-12-29 04:18:27.000000 mysqlx-1.1.4/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2021-12-29 04:18:27.000000 mysqlx-1.1.4/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      397 2021-12-29 04:18:27.000000 mysqlx-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2021-12-29 04:18:27.000000 mysqlx-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      814 2021-12-29 04:18:09.000000 mysqlx-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:06:39.000000 mysqlx-1.1.5/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.1.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-06 08:06:39.000000 mysqlx-1.1.5/mysqlx/
+-rw-rw-rw-   0        0        0     4695 2023-06-06 01:46:24.000000 mysqlx-1.1.5/mysqlx/coder.py
+-rw-rw-rw-   0        0        0    10109 2023-06-06 02:59:25.000000 mysqlx-1.1.5/mysqlx/db.py
+-rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.1.5/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     5285 2023-06-06 08:02:21.000000 mysqlx-1.1.5/mysqlx/helper.py
+-rw-rw-rw-   0        0        0     8173 2023-06-05 13:04:14.000000 mysqlx-1.1.5/mysqlx/orm.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.1.5/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:06:39.000000 mysqlx-1.1.5/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-06 08:06:39.000000 mysqlx-1.1.5/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.1.5/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      411 2023-06-06 08:06:39.000000 mysqlx-1.1.5/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-06-06 08:06:39.000000 mysqlx-1.1.5/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      287 2023-06-06 08:06:39.000000 mysqlx-1.1.5/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 08:06:39.000000 mysqlx-1.1.5/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      411 2023-06-06 08:06:39.000000 mysqlx-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-06 08:06:39.000000 mysqlx-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      814 2023-06-06 08:05:56.000000 mysqlx-1.1.5/setup.py
```

### Comparing `mysqlx-1.1.4/mysqlx/db.py` & `mysqlx-1.1.5/mysqlx/db.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-import re, time, functools, logging
-from mysqlx.model import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx
+import time
+import logging
+import functools
+from typing import Iterable, Any
+from .helper import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql
 
-# thread-local context:
 _DB_CTX = None
-_REGEX = r':[\w|\d]*'
+_SHOW_SQL = False
+_PK_SQL = 'SELECT LAST_INSERT_ID()'
 
 
-def init_db(user, password, database, host='127.0.0.1', port=3306, use_unicode=True, pool_size=5, **kwargs):
+def init_db(user: str, password: str, database: str, host='127.0.0.1', port=3306, pool_size=8, use_unicode=True, show_sql=False, **kwargs):
     from mysql.connector import connect
     global _DB_CTX
-    if pool_size is not None and 'pool_name' not in kwargs:
-        kwargs['pool_name'] = database + "_pool"
+    global _SHOW_SQL
+    _SHOW_SQL = show_sql
+    if pool_size:
+        kwargs['pool_size'] = pool_size
+        if 'pool_name' not in kwargs:
+            kwargs['pool_name'] = "%s_pool" % database
 
     kwargs['user'] = user
     kwargs['password'] = password
     kwargs['database'] = database
     kwargs['host'] = host
     kwargs['port'] = port
     kwargs['use_unicode'] = use_unicode
@@ -35,15 +42,14 @@
 def with_connection(func):
     """
     Decorator for reuse connection.
     @with_connection
     def foo(*args, **kw):
         f1()
         f2()
-        f3()
     """
 
     global _DB_CTX
 
     @functools.wraps(func)
     def _wrapper(*args, **kw):
         with ConnectionCtx(_DB_CTX):
@@ -107,64 +113,25 @@
         with TransactionCtx(_DB_CTX):
             return func(*args, **kw)
         _profiling(_start)
 
     return _wrapper
 
 
-def _select(sql, first, *args):
-    """execute select SQL and return unique result or list results."""
-    global _DB_CTX
-    cursor = None
-    logging.info('SQL: %s, ARGS: %s' % (sql, args))
-    sql = sql.replace('?', '%s')
-    try:
-        cursor = _DB_CTX.cursor()
-        cursor.execute(sql, args)
-        if cursor.description:
-            names = [x[0] for x in cursor.description]
-        if first:
-            values = cursor.fetchone()
-            if not values:
-                return None
-            return Dict(names, values)
-        return [Dict(names, x) for x in cursor.fetchall()]
-    finally:
-        if cursor:
-            cursor.close()
-
-
-@with_connection
-def get(sql, *args, **kwargs):
+def get(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result.
     MultiColumnsError: Expect only one column.
     """
     global _DB_CTX
-    cursor = None
-    if kwargs:
-        sql, args = _get_named_sql_args(sql, **kwargs)
-
-    logging.info('SQL: %s, ARGS: %s' % (sql, args))
-    sql = sql.replace('?', '%s')
-    try:
-        cursor = _DB_CTX.cursor()
-        cursor.execute(sql, args)
-        values = cursor.fetchone()
-        if len(values) == 1:
-            return values[0]
-        else:
-            raise MultiColumnsError('Expect only one column.')
-    finally:
-        if cursor:
-            cursor.close()
+    sql, args = dynamic_sql(sql, *args, **kwargs)
+    return do_get(sql, *args)
 
 
-@with_connection
-def select_one(sql, *args, **kwargs):
+def select_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one result.
     If no result found, return None.
     If multiple results found, the first one returned.
     >>> u1 = dict(id=100, name='Alice', email='alice@test.org', passwd='ABC-12345', last_modified=time.time())
     >>> u2 = dict(id=101, name='Sarah', email='sarah@test.org', passwd='ABC-12345', last_modified=time.time())
     >>> insert('user', **u1)
@@ -175,21 +142,19 @@
     >>> u.name
     u'Alice'
     >>> select_one('select * from user where email=?', 'abc@email.com')
     >>> u2 = select_one('select * from user where passwd=? order by email', 'ABC-12345')
     >>> u2.name
     u'Alice'
     """
-    if kwargs:
-        sql, args = _get_named_sql_args(sql, **kwargs)
-    return _select(sql, True, *args)
+    sql, args = dynamic_sql(sql, *args, **kwargs)
+    return do_select_one(sql, *args)
 
 
-@with_connection
-def select(sql, *args, **kwargs):
+def select(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     >>> u1 = dict(id=200, name='Wall.E', email='wall.e@test.org', passwd='back-to-earth', last_modified=time.time())
     >>> u2 = dict(id=201, name='Eva', email='eva@test.org', passwd='back-to-earth', last_modified=time.time())
     >>> insert('user', **u1)
     1
     >>> insert('user', **u2)
@@ -202,82 +167,174 @@
     u'wall.e@test.org'
     >>> L = select('select * from user where passwd=? order by id desc', 'back-to-earth')
     >>> L[0].name
     u'Eva'
     >>> L[1].name
     u'Wall.E'
     """
-    if kwargs:
-        sql, args = _get_named_sql_args(sql, **kwargs)
-    return _select(sql, False, *args)
+    sql, args = dynamic_sql(sql, *args, **kwargs)
+    return do_select(sql, *args)
+
+
+def insert(table: str, **kwargs):
+    """
+    Execute insert SQL, return effect rowcount.
+    IntegrityError: 1062 (23000): Duplicate entry '2000' for key 'PRIMARY'
+    """
+    sql, args = _insert_sql(table, ** kwargs)
+    return do_execute(sql, *args)
+
+
+def execute(sql: str, *args, **kwargs):
+    """
+    Execute SQL.
+    """
+    sql, args = dynamic_sql(sql, *args, **kwargs)
+    return do_execute(sql, *args)
 
 
 @with_connection
-def _execute(sql, *args):
+def save(table: str, **kwargs):
+    """
+    Execute insert SQL, return primary key.
+    IntegrityError: 1062 (23000): Duplicate entry '2000' for key 'PRIMARY'
+    """
     global _DB_CTX
     cursor = None
-    logging.info('SQL: %s, ARGS: %s' % (sql, args))
-    sql = sql.replace('?', '%s')
+    sql, args = _insert_sql(table, ** kwargs)
+    sql = _before_execute('db.save', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
-        r = cursor.rowcount
-        if _DB_CTX.transactions == 0:
-            _DB_CTX.connection.commit()
-        return r
+        cursor.execute(_PK_SQL)
+        result = cursor.fetchone()
+        try_commit(_DB_CTX)
+        return result[0]
     finally:
         if cursor:
             cursor.close()
 
 
-def insert(table, **kwargs):
-    """
-    Execute insert SQL.
-    IntegrityError: 1062 (23000): Duplicate entry '2000' for key 'PRIMARY'
-    """
-    cols, args = zip(*kwargs.items())
-    sql = 'insert into `%s` (%s) values (%s)' % (table, ','.join(['`%s`' % col for col in cols]), ','.join(['?' for i in range(len(cols))]))
-    return _execute(sql, *args)
+@with_connection
+def batch_execute(sql: str, args: Iterable[Iterable[Any]]):
+    global _DB_CTX
+    cursor = None
+    sql = _before_execute('db.batch_execute', sql, *args)
+    try:
+        cursor = _DB_CTX.cursor()
+        cursor.executemany(sql, args)
+        effect_rowcount = cursor.rowcount
+        try_commit(_DB_CTX)
+        return effect_rowcount
+    finally:
+        if cursor:
+            cursor.close()
 
 
-def execute(sql, *args, **kwargs):
+@with_connection
+def do_get(sql: str, *args):
     """
-    Execute SQL.
+    Execute select SQL and expected one int and only one int result.
+    MultiColumnsError: Expect only one column.
     """
-    if kwargs:
-        sql, args = _get_named_sql_args(sql, **kwargs)
-    return _execute(sql, *args)
+    global _DB_CTX
+    cursor = None
+    if 'limit' not in sql:
+        sql = '%s limit 1' % sql
+
+    sql = _before_execute('db.do_get', sql, *args)
+    try:
+        cursor = _DB_CTX.cursor()
+        cursor.execute(sql, args)
+        result = cursor.fetchone()
+        if result:
+            if len(result) == 1:
+                return result[0]
+            raise MultiColumnsError('Expect only one column but %d.' % len(result))
+        return None
+    finally:
+        if cursor:
+            cursor.close()
 
 
 @with_connection
-def batch_execute(sql, args: list):
+def do_select_one(sql: str, *args):
+    """execute select SQL and return unique result or list results."""
     global _DB_CTX
     cursor = None
-    logging.info('SQL: %s, ARGS: %s' % (sql, args))
-    sql = sql.replace('?', '%s')
+    if 'limit' not in sql:
+        sql = '%s limit 1' % sql
+
+    sql = _before_execute('db.do_select_one', sql, *args)
     try:
         cursor = _DB_CTX.cursor()
-        cursor.executemany(sql, args)
-        r = cursor.rowcount
-        if _DB_CTX.transactions == 0:
-            _DB_CTX.connection.commit()
-        return r
+        cursor.execute(sql, args)
+        if cursor.description:
+            names = [x[0] for x in cursor.description]
+            result = cursor.fetchone()
+            return Dict(names, result) if result else None
+        else:
+            return cursor.fetchone()
+    finally:
+        if cursor:
+            cursor.close()
+
+
+@with_connection
+def do_select(sql: str, *args):
+    """execute select SQL and return unique result or list results."""
+    global _DB_CTX
+    cursor = None
+    sql = _before_execute('db.do_select', sql, *args)
+    try:
+        cursor = _DB_CTX.cursor()
+        cursor.execute(sql, args)
+        if cursor.description:
+            names = [x[0] for x in cursor.description]
+            return [Dict(names, x) for x in cursor.fetchall()]
+        else:
+            return cursor.fetchall()
+    finally:
+        if cursor:
+            cursor.close()
+
+
+@with_connection
+def do_execute(sql: str, *args):
+    global _DB_CTX
+    cursor = None
+    sql = _before_execute('db.do_execute', sql, *args)
+    try:
+        cursor = _DB_CTX.connection.cursor()
+        cursor.execute(sql, args)
+        effect_rowcount = cursor.rowcount
+        try_commit(_DB_CTX)
+        return effect_rowcount
     finally:
         if cursor:
             cursor.close()
 
 
 def get_connection():
     global _DB_CTX
-    if not _DB_CTX.is_init():
+    if _DB_CTX.is_not_init():
         _DB_CTX.init()
     return _DB_CTX.connection
 
 
 def prepare(prepared=True):
     global _DB_CTX
     _DB_CTX.prepared = prepared
 
 
-def _get_named_sql_args(sql, **kwargs):
-    args = [kwargs[r[1:]] for r in re.findall(_REGEX, sql)]
-    return re.sub(_REGEX, '?', sql), args
+def _before_execute(function: str, sql: str, *args):
+    global _SHOW_SQL
+    if _SHOW_SQL:
+        logging.info("Exec func '%s' \n\t\t  SQL: %s \n\t\t  ARGS: %s" % (function, sql, args))
+    return sql.replace('?', '%s')
+
+
+def _insert_sql(table: str, **kwargs):
+    cols, args = zip(*kwargs.items())
+    sql = 'insert into `%s` (%s) values (%s)' % (table, ','.join(['`%s`' % col for col in cols]), ','.join(['?' for i in range(len(cols))]))
+    return sql, args
+
```

### Comparing `mysqlx-1.1.4/mysqlx/dbx.py` & `mysqlx-1.1.5/mysqlx/dbx.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,103 +1,114 @@
 import os
 import re
-from mysqlx import db
+from . import db
+from .helper import SqlModel
 from jinja2 import Template
-from mysqlx.model import SqlModel
+from typing import Iterable, Any
+from .helper import DYNAMIC_REGEX, simple_sql
 try:
     import xml.etree.cElementTree as ET
 except ImportError:
     import xml.etree.ElementTree as ET
 
-_REGEX = '{%|{{|}}|%}'
 _SQL_CONTAINER = dict()
 
 
-def init_db(user, password, database, host='127.0.0.1', port=3306, use_unicode=True, pool_size=5, mapper_path='mapper', **kw):
+def init_db(user: str, password: str, database: str, host='127.0.0.1', port=3306, pool_size=8, use_unicode=True, show_sql=False, mapper_path='mapper',
+            **kwargs):
     _load_sql(mapper_path)
-    db.init_db(user, password, database, host, port, use_unicode, pool_size, **kw)
+    db.init_db(user, password, database, host, port, pool_size, use_unicode, show_sql, **kwargs)
 
 
-def insert(table, **kw):
-    return db.insert(table, **kw)
+def get(sql_id: str, *args, **kwargs):
+    sql = get_sql(sql_id, **kwargs)
+    sql, args = simple_sql(sql, *args, **kwargs)
+    return db.do_get(sql, *args)
 
 
-def execute(sql_id, *args, **kwargs):
+def select_one(sql_id: str, *args, **kwargs):
     sql = get_sql(sql_id, **kwargs)
-    return db.execute(sql, *args, **kwargs)
+    sql, args = simple_sql(sql, *args, **kwargs)
+    return db.do_select_one(sql, *args)
 
 
-def batch_execute(sql_id, args: list):
-    sql = get_sql(sql_id)
-    return db.batch_execute(sql, args)
+def select(sql_id: str, *args, **kwargs):
+    sql = get_sql(sql_id, **kwargs)
+    sql, args = simple_sql(sql, *args, **kwargs)
+    return db.do_select(sql, *args)
 
 
-def get(sql_id, *args, **kwargs):
-    sql = get_sql(sql_id, **kwargs)
-    return db.get(sql, *args, **kwargs)
+def insert(table: str, **kwargs):
+    return db.insert(table, **kwargs)
 
 
-def select_one(sql_id, *args, **kwargs):
-    sql = get_sql(sql_id, **kwargs)
-    return db.select_one(sql, *args, **kwargs)
+def save(table: str, **kwargs):
+    return db.save(table, **kwargs)
 
 
-def select(sql_id, *args, **kwargs):
+def execute(sql_id: str, *args, **kwargs):
     sql = get_sql(sql_id, **kwargs)
-    return db.select(sql, *args, **kwargs)
+    sql, args = simple_sql(sql, *args, **kwargs)
+    return db.do_execute(sql, *args)
+
+
+def batch_execute(sql_id: str, args: Iterable[Iterable[Any]]):
+    sql = get_sql(sql_id)
+    return db.batch_execute(sql, args)
 
 
 def get_connection():
     return db.get_connection()
 
 
-def _get_path(path):
+def _get_path(path: str):
     if path.startswith("../"):
         rpath = ''.join(re.findall("../", path))
         os.chdir(rpath)
         path = path[len(rpath):]
     elif path.startswith("./"):
         path = path[2:]
     return os.path.join(os.getcwd(), path)
 
 
-def _load_sql(path):
+def _load_sql(path: str):
     if not os.path.isabs(path):
         path = _get_path(path)
 
     for f in os.listdir(path):
         file = os.path.join(path, f)
         if os.path.isfile(file) and f.endswith(".xml"):
             _read_mapper(file)
         elif os.path.isdir(file):
             _load_sql(file)
 
 
-def _read_mapper(file):
+def _read_mapper(file: str):
     global _SQL_CONTAINER
     tree = ET.parse(file)
     root = tree.getroot()
     namespace = root.attrib.get('namespace', '')
     for child in root:
         sql_id = namespace + "." + child.attrib.get('id')
-        include = child.attrib.get('include')
+        assert sql_id not in _SQL_CONTAINER, "Sql id '%s' repeat." % sql_id
+        includes = child.attrib.get('include')
         sql = child.text
-        if include or re.search(_REGEX, sql):
-            _SQL_CONTAINER[sql_id] = SqlModel(sql=Template(sql), dynamic=True, include=include)
+        if includes or re.search(DYNAMIC_REGEX, sql):
+            _SQL_CONTAINER[sql_id] = SqlModel(sql=Template(sql), dynamic=True, include=includes)
         else:
             _SQL_CONTAINER[sql_id] = SqlModel(sql=sql)
 
 
-def get_sql(sql_id, **kwargs):
+def get_sql(sql_id: str, **kwargs):
     sql_model = _get_sql_model(sql_id)
     includes = sql_model.include
     if includes:
         for include in includes.split(","):
             include_sql_id = sql_id[:sql_id.index(".")+1] + include
             kwargs[include] = get_sql(include_sql_id, **kwargs)
     return sql_model.sql.render(**kwargs) if sql_model.dynamic else sql_model.sql
 
 
-def _get_sql_model(sql_id):
+def _get_sql_model(sql_id: str):
     global _SQL_CONTAINER
     return _SQL_CONTAINER[sql_id]
```

### Comparing `mysqlx-1.1.4/mysqlx/model.py` & `mysqlx-1.1.5/mysqlx/helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,102 @@
+import re
 import logging
 import threading
+from jinja2 import Template
+
+_REGEX = r':[\w|\d]*'
+DYNAMIC_REGEX = '{%|{{|}}|%}'
+
+
+def try_commit(db_ctx):
+    if db_ctx.transactions == 0:
+        logging.debug('Commit transaction...')
+        try:
+            db_ctx.connection.commit()
+            logging.debug('Commit ok.')
+        except Exception:
+            logging.warning('Commit failed, try rollback...')
+            db_ctx.connection.rollback()
+            logging.warning('Rollback ok.')
+            raise
+
+
+def simple_sql(sql, *args, **kwargs):
+    return _get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
+
+
+def dynamic_sql(sql, *args, **kwargs):
+    if kwargs:
+        if re.search(DYNAMIC_REGEX, sql):
+            sql = Template(sql).render(**kwargs)
+        return _get_named_sql_args(sql, **kwargs)
+
+    return sql, args
+
+
+def _get_named_sql_args(sql: str, **kwargs):
+    args = [kwargs[r[1:]] for r in re.findall(_REGEX, sql)]
+    return re.sub(_REGEX, '?', sql), args
 
 
 class DBCtx(threading.local):
     """
     Thread local object that holds connection info.
     """
 
     def __init__(self, connect):
         self.connect = connect
         self.connection = None
         self.transactions = 0
         self.prepared = True
 
-    def is_init(self):
-        return self.connection is not None
+    def is_not_init(self):
+        return self.connection is None
 
     def init(self):
         self.transactions = 0
         self.connection = self.connect()
-        logging.debug('use connection <%s>...' % hex(id(self.connection)))
+        logging.debug('Use connection <%s>...' % hex(id(self.connection)))
 
     def release(self):
         if self.connection:
-            logging.debug('release connection <%s>...' % hex(id(self.connection)))
+            logging.debug('Release connection <%s>...' % hex(id(self.connection)))
             self.connection.close()
             self.connection = None
 
     def cursor(self):
         """
         Return cursor
         """
-        logging.debug('cursor prepared: %s' % self.prepared)
+        logging.debug('Cursor prepared: %s' % self.prepared)
         return self.connection.cursor(prepared=self.prepared)
 
     def statement(self, sql):
         """
         Return statement
         """
         return self.connection.statement(sql)
 
 
 class ConnectionCtx(object):
     """
-    ConnectionCtx object that can open and close connection context. _ConnectionCtx object can be nested and only the most
+    ConnectionCtx object that can open and close connection context. ConnectionCtx object can be nested and only the most
     outer connection has effect.
     with connection():
         pass
         with connection():
             pass
     """
 
     def __init__(self, db_ctx):
         self.db_ctx = db_ctx
 
     def __enter__(self):
         self.should_cleanup = False
-        if not self.db_ctx.is_init():
+        if self.db_ctx.is_not_init():
             self.db_ctx.init()
             self.should_cleanup = True
         return self
 
     def __exit__(self, exctype, excvalue, traceback):
         if self.should_cleanup:
             self.db_ctx.release()
@@ -74,20 +110,20 @@
     """
 
     def __init__(self, db_ctx):
         self.db_ctx = db_ctx
 
     def __enter__(self):
         self.should_close_conn = False
-        if not self.db_ctx.is_init():
+        if self.db_ctx.is_not_init():
             # needs open a connection first:
             self.db_ctx.init()
             self.should_close_conn = True
-        self.db_ctx.transactions = self.db_ctx.transactions + 1
-        logging.info('begin transaction...' if self.db_ctx.transactions == 1 else 'join current transaction...')
+        self.db_ctx.transactions += 1
+        logging.debug('Begin transaction...' if self.db_ctx.transactions == 1 else 'Join current transaction...')
         return self
 
     def __exit__(self, exctype, excvalue, traceback):
         self.db_ctx.transactions -= 1
         try:
             if self.db_ctx.transactions == 0:
                 if exctype is None:
@@ -95,28 +131,20 @@
                 else:
                     self.rollback()
         finally:
             if self.should_close_conn:
                 self.db_ctx.release()
 
     def commit(self):
-        logging.info('commit transaction...')
-        try:
-            self.db_ctx.connection.commit()
-            logging.info('commit ok.')
-        except Exception:
-            logging.warning('commit failed. try rollback...')
-            self.db_ctx.connection.rollback()
-            logging.warning('rollback ok.')
-            raise
+        try_commit(self.db_ctx)
 
     def rollback(self):
-        logging.warning('rollback transaction...')
+        logging.warning('Rollback transaction...')
         self.db_ctx.connection.rollback()
-        logging.info('rollback ok.')
+        logging.debug('Rollback ok.')
 
 
 class DBError(Exception):
     pass
 
 
 class MultiColumnsError(DBError):
@@ -165,13 +193,12 @@
             raise AttributeError(r"'Dict' object has no attribute '%s'" % key)
 
     def __setattr__(self, key, value):
         self[key] = value
 
 
 class SqlModel:
-
-    def __init__(self, sql, dynamic=False, include=None):
+    def __init__(self, sql: str, dynamic: bool = False, include: str = None):
         self.sql = sql
         self.dynamic = dynamic
         self.include = include
```

### Comparing `mysqlx-1.1.4/setup.py` & `mysqlx-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 setup(
     name='mysqlx',
     packages=find_packages(),
     description="mysqlx is a simple python sql executor for MySQL like iBatis.",
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
-        'mysql-connector-python>=8.0.27',
+        'mysql-connector-python>=8.0.20',
     ],
-    version='1.1.4',
+    version='1.1.5',
     url='https://gitee.com/summry/mysqlx/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.txt'],
```

