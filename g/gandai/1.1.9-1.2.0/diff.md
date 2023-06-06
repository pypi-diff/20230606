# Comparing `tmp/gandai-1.1.9.tar.gz` & `tmp/gandai-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.1.9.tar", last modified: Tue May 16 10:29:15 2023, max compression
+gzip compressed data, was "gandai-1.2.0.tar", last modified: Tue Jun  6 18:45:50 2023, max compression
```

## Comparing `gandai-1.1.9.tar` & `gandai-1.2.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.128274 gandai-1.1.9/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.9/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-16 10:29:15.128153 gandai-1.1.9/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.122682 gandai-1.1.9/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       45 2023-05-13 19:24:50.000000 gandai-1.1.9/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.126221 gandai-1.1.9/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-05-13 19:25:52.000000 gandai-1.1.9/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.9/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-15 00:21:53.000000 gandai-1.1.9/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4064 2023-05-15 02:35:18.000000 gandai-1.1.9/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2075 2023-05-13 19:36:23.000000 gandai-1.1.9/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.9/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5474 2023-05-15 00:13:44.000000 gandai-1.1.9/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6137 2023-05-14 03:30:02.000000 gandai-1.1.9/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17744 2023-05-15 00:13:44.000000 gandai-1.1.9/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.9/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8074 2023-05-15 00:13:44.000000 gandai-1.1.9/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1703 2023-05-16 10:28:54.000000 gandai-1.1.9/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1583 2023-05-15 00:33:21.000000 gandai-1.1.9/gandai/datastore.py
--rw-r--r--   0 parker     (501) staff       (20)     2451 2023-05-13 19:35:44.000000 gandai-1.1.9/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     3526 2023-05-16 10:26:58.000000 gandai-1.1.9/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.127116 gandai-1.1.9/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.9/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.127631 gandai-1.1.9/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.1.9/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-14 19:49:36.000000 gandai-1.1.9/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      409 2023-05-13 19:26:13.000000 gandai-1.1.9/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1655 2023-05-15 12:42:15.000000 gandai-1.1.9/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3257 2023-05-14 17:36:57.000000 gandai-1.1.9/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.127900 gandai-1.1.9/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)     2913 2023-05-15 21:05:11.000000 gandai-1.1.9/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2642 2023-05-14 03:28:36.000000 gandai-1.1.9/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)     9337 2023-05-15 00:00:59.000000 gandai-1.1.9/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     5554 2023-05-16 10:27:56.000000 gandai-1.1.9/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.123356 gandai-1.1.9/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-16 10:29:15.000000 gandai-1.1.9/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1015 2023-05-16 10:29:15.000000 gandai-1.1.9/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-16 10:29:15.000000 gandai-1.1.9/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-16 10:29:15.000000 gandai-1.1.9/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2023-05-16 10:29:01.000000 gandai-1.1.9/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-16 10:29:15.128305 gandai-1.1.9/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.9/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-06-06 18:45:50.071389 gandai-1.2.0/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.2.0/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-06-06 18:45:50.071264 gandai-1.2.0/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-06-06 18:45:50.065190 gandai-1.2.0/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       45 2023-05-23 11:45:31.000000 gandai-1.2.0/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-06-06 18:45:50.069198 gandai-1.2.0/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-05-23 11:53:24.000000 gandai-1.2.0/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.2.0/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4157 2023-06-06 18:31:07.000000 gandai-1.2.0/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.2.0/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2016 2023-06-06 18:08:14.000000 gandai-1.2.0/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.2.0/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4131 2023-05-23 12:17:36.000000 gandai-1.2.0/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6153 2023-05-23 11:53:24.000000 gandai-1.2.0/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    22092 2023-05-23 12:27:15.000000 gandai-1.2.0/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1997 2023-06-06 18:17:51.000000 gandai-1.2.0/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.2.0/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8063 2023-06-06 18:28:45.000000 gandai-1.2.0/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1794 2023-06-06 18:31:06.000000 gandai-1.2.0/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1500 2023-06-06 18:24:12.000000 gandai-1.2.0/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     1205 2023-06-06 18:08:11.000000 gandai-1.2.0/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     2860 2023-05-23 12:17:34.000000 gandai-1.2.0/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-06-06 18:45:50.069899 gandai-1.2.0/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.2.0/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-06-06 18:45:50.070315 gandai-1.2.0/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.2.0/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.2.0/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      409 2023-05-23 11:45:31.000000 gandai-1.2.0/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1655 2023-06-06 18:34:56.000000 gandai-1.2.0/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3257 2023-05-23 11:45:31.000000 gandai-1.2.0/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-06-06 18:45:50.070991 gandai-1.2.0/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-05-23 16:11:22.000000 gandai-1.2.0/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2924 2023-05-23 15:19:19.000000 gandai-1.2.0/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2652 2023-05-23 11:45:31.000000 gandai-1.2.0/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    12867 2023-05-23 12:27:14.000000 gandai-1.2.0/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)      965 2023-06-06 18:14:26.000000 gandai-1.2.0/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     5534 2023-06-06 18:13:42.000000 gandai-1.2.0/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-06-06 18:45:50.065780 gandai-1.2.0/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-06-06 18:45:50.000000 gandai-1.2.0/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1116 2023-06-06 18:45:50.000000 gandai-1.2.0/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-06-06 18:45:50.000000 gandai-1.2.0/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-06-06 18:45:50.000000 gandai-1.2.0/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2023-06-06 18:43:29.000000 gandai-1.2.0/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-06-06 18:45:50.071420 gandai-1.2.0/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.2.0/setup.py
```

### Comparing `gandai-1.1.9/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.2.0/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.9/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.2.0/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,27 +1,25 @@
 magic:    0xa70d0d0a
-moddate:  0x207b6164 (Mon May 15 00:21:52 2023 UTC)
-files sz: 1703
+moddate:  0x6a7b7f64 (Tue Jun  6 18:31:06 2023 UTC)
+files sz: 1794
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a01640064016c025a02640064026c036d045a046d
       055a056d065a060100640064036c076d085a080100640064046c096d095a
       090100640064016c0a5a0a640064056c0b6d0c5a0c0100640064066c0d6d
-      0e5a0e01000200650ea6000000ab0000000000000000005a0f0200650c02
-      00650a6a1000000000000000006407a6010000ab01000000000000000002
-      00650a6a1000000000000000006408a6010000ab010000000000000000a6
-      020000ab0200000000000000005a1165050200470064098400640aa60200
-      00ab020000000000000000a6000000ab0000000000000000005a12640b65
-      12640c64016604640d84045a13640e6514640c64016604640f84045a1564
-      106514640c65126604641184045a1664126514640c65176604641384045a
-      1864015300
+      0e5a0e010069005a0f0200650c0200650e6407a6010000ab010000000000
+      0000000200650e6408a6010000ab010000000000000000a6020000ab0200
+      000000000000005a1065050200470064098400640aa6020000ab02000000
+      0000000000a6000000ab0000000000000000005a11640b6511640c640166
+      04640d84045a12640e6513640c64016604640f84045a1464106513640c65
+      116604641184045a1564126513640c65166604641384045a1764015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (pandas)
                  8 STORE_NAME               1 (pd)
    
@@ -63,172 +61,169 @@
      7          70 LOAD_CONST               0 (0)
                 72 LOAD_CONST               5 (('Client',))
                 74 IMPORT_NAME             11 (twilio.rest)
                 76 IMPORT_FROM             12 (Client)
                 78 STORE_NAME              12 (Client)
                 80 POP_TOP
    
-    11          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               6 (('Cloudstore',))
-                86 IMPORT_NAME             13 (gandai.datastore)
-                88 IMPORT_FROM             14 (Cloudstore)
-                90 STORE_NAME              14 (Cloudstore)
+    12          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               6 (('access_secret_version',))
+                86 IMPORT_NAME             13 (gandai.secrets)
+                88 IMPORT_FROM             14 (access_secret_version)
+                90 STORE_NAME              14 (access_secret_version)
                 92 POP_TOP
    
-    14          94 PUSH_NULL
-                96 LOAD_NAME               14 (Cloudstore)
-                98 PRECALL                  0
-               102 CALL                     0
-               112 STORE_NAME              15 (ds)
-   
-    15         114 PUSH_NULL
-               116 LOAD_NAME               12 (Client)
-               118 PUSH_NULL
-               120 LOAD_NAME               10 (os)
-               122 LOAD_ATTR               16 (getenv)
-               132 LOAD_CONST               7 ('TWILIO_APP')
-               134 PRECALL                  1
-               138 CALL                     1
-               148 PUSH_NULL
-               150 LOAD_NAME               10 (os)
-               152 LOAD_ATTR               16 (getenv)
-               162 LOAD_CONST               8 ('TWILIO_TOKEN')
-               164 PRECALL                  1
-               168 CALL                     1
-               178 PRECALL                  2
-               182 CALL                     2
-               192 STORE_NAME              17 (twilio_client)
-   
-    18         194 LOAD_NAME                5 (dataclass)
-   
-    19         196 PUSH_NULL
-               198 LOAD_BUILD_CLASS
-               200 LOAD_CONST               9 (<code object Auth, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 18>)
-               202 MAKE_FUNCTION            0
-               204 LOAD_CONST              10 ('Auth')
-               206 PRECALL                  2
-               210 CALL                     2
-   
-    18         220 PRECALL                  0
-               224 CALL                     0
-   
-    19         234 STORE_NAME              18 (Auth)
-   
-    35         236 LOAD_CONST              11 ('auth')
-               238 LOAD_NAME               18 (Auth)
-               240 LOAD_CONST              12 ('return')
-               242 LOAD_CONST               1 (None)
-               244 BUILD_TUPLE              4
-               246 LOAD_CONST              13 (<code object _send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 35>)
-               248 MAKE_FUNCTION            4 (annotations)
-               250 STORE_NAME              19 (_send_code)
-   
-    44         252 LOAD_CONST              14 ('phone')
-               254 LOAD_NAME               20 (str)
-               256 LOAD_CONST              12 ('return')
-               258 LOAD_CONST               1 (None)
-               260 BUILD_TUPLE              4
-               262 LOAD_CONST              15 (<code object send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 44>)
-               264 MAKE_FUNCTION            4 (annotations)
-               266 STORE_NAME              21 (send_code)
-   
-    52         268 LOAD_CONST              16 ('code')
-               270 LOAD_NAME               20 (str)
-               272 LOAD_CONST              12 ('return')
-               274 LOAD_NAME               18 (Auth)
-               276 BUILD_TUPLE              4
-               278 LOAD_CONST              17 (<code object authenticate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 52>)
-               280 MAKE_FUNCTION            4 (annotations)
-               282 STORE_NAME              22 (authenticate)
-   
-    64         284 LOAD_CONST              18 ('token')
-               286 LOAD_NAME               20 (str)
-               288 LOAD_CONST              12 ('return')
-               290 LOAD_NAME               23 (bool)
-               292 BUILD_TUPLE              4
-               294 LOAD_CONST              19 (<code object validate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 64>)
-               296 MAKE_FUNCTION            4 (annotations)
-               298 STORE_NAME              24 (validate)
-               300 LOAD_CONST               1 (None)
-               302 RETURN_VALUE
+    16          94 BUILD_MAP                0
+                96 STORE_NAME              15 (ds)
+   
+    17          98 PUSH_NULL
+               100 LOAD_NAME               12 (Client)
+   
+    18         102 PUSH_NULL
+               104 LOAD_NAME               14 (access_secret_version)
+               106 LOAD_CONST               7 ('TWILIO_APP')
+               108 PRECALL                  1
+               112 CALL                     1
+               122 PUSH_NULL
+               124 LOAD_NAME               14 (access_secret_version)
+               126 LOAD_CONST               8 ('TWILIO_TOKEN')
+               128 PRECALL                  1
+               132 CALL                     1
+   
+    17         142 PRECALL                  2
+               146 CALL                     2
+               156 STORE_NAME              16 (twilio_client)
+   
+    22         158 LOAD_NAME                5 (dataclass)
+   
+    23         160 PUSH_NULL
+               162 LOAD_BUILD_CLASS
+               164 LOAD_CONST               9 (<code object Auth, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 22>)
+               166 MAKE_FUNCTION            0
+               168 LOAD_CONST              10 ('Auth')
+               170 PRECALL                  2
+               174 CALL                     2
+   
+    22         184 PRECALL                  0
+               188 CALL                     0
+   
+    23         198 STORE_NAME              17 (Auth)
+   
+    39         200 LOAD_CONST              11 ('auth')
+               202 LOAD_NAME               17 (Auth)
+               204 LOAD_CONST              12 ('return')
+               206 LOAD_CONST               1 (None)
+               208 BUILD_TUPLE              4
+               210 LOAD_CONST              13 (<code object _send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 39>)
+               212 MAKE_FUNCTION            4 (annotations)
+               214 STORE_NAME              18 (_send_code)
+   
+    48         216 LOAD_CONST              14 ('phone')
+               218 LOAD_NAME               19 (str)
+               220 LOAD_CONST              12 ('return')
+               222 LOAD_CONST               1 (None)
+               224 BUILD_TUPLE              4
+               226 LOAD_CONST              15 (<code object send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 48>)
+               228 MAKE_FUNCTION            4 (annotations)
+               230 STORE_NAME              20 (send_code)
+   
+    56         232 LOAD_CONST              16 ('code')
+               234 LOAD_NAME               19 (str)
+               236 LOAD_CONST              12 ('return')
+               238 LOAD_NAME               17 (Auth)
+               240 BUILD_TUPLE              4
+               242 LOAD_CONST              17 (<code object authenticate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 56>)
+               244 MAKE_FUNCTION            4 (annotations)
+               246 STORE_NAME              21 (authenticate)
+   
+    68         248 LOAD_CONST              18 ('token')
+               250 LOAD_NAME               19 (str)
+               252 LOAD_CONST              12 ('return')
+               254 LOAD_NAME               22 (bool)
+               256 BUILD_TUPLE              4
+               258 LOAD_CONST              19 (<code object validate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 68>)
+               260 MAKE_FUNCTION            4 (annotations)
+               262 STORE_NAME              23 (validate)
+               264 LOAD_CONST               1 (None)
+               266 RETURN_VALUE
    consts
       0
       None
       ('asdict', 'dataclass', 'field')
       ('md5',)
       ('time',)
       ('Client',)
-      ('Cloudstore',)
+      ('access_secret_version',)
       'TWILIO_APP'
       'TWILIO_TOKEN'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a025500020065036401ac02a6010000ab01000000
             00000000005a046505650664033c0000006505650664043c000000650565
             0664053c000000020065036401ac02a6010000ab0100000000000000005a
             076508650664063c000000020065036401ac02a6010000ab010000000000
             0000005a096505650664073c000000640884005a0a64095300
-          18           0 RESUME                   0
+          22           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Auth')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          20          12 PUSH_NULL
+          24          12 PUSH_NULL
                       14 LOAD_NAME                3 (field)
                       16 LOAD_CONST               1 (False)
                       18 KW_NAMES                 2
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_NAME               4 (key)
                       36 LOAD_NAME                5 (str)
                       38 LOAD_NAME                6 (__annotations__)
                       40 LOAD_CONST               3 ('key')
                       42 STORE_SUBSCR
          
-          21          46 LOAD_NAME                5 (str)
+          25          46 LOAD_NAME                5 (str)
                       48 LOAD_NAME                6 (__annotations__)
                       50 LOAD_CONST               4 ('phone')
                       52 STORE_SUBSCR
          
-          22          56 LOAD_NAME                5 (str)
+          26          56 LOAD_NAME                5 (str)
                       58 LOAD_NAME                6 (__annotations__)
                       60 LOAD_CONST               5 ('code')
                       62 STORE_SUBSCR
          
-          23          66 PUSH_NULL
+          27          66 PUSH_NULL
                       68 LOAD_NAME                3 (field)
                       70 LOAD_CONST               1 (False)
                       72 KW_NAMES                 2
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_NAME               7 (expires)
                       90 LOAD_NAME                8 (int)
                       92 LOAD_NAME                6 (__annotations__)
                       94 LOAD_CONST               6 ('expires')
                       96 STORE_SUBSCR
          
-          24         100 PUSH_NULL
+          28         100 PUSH_NULL
                      102 LOAD_NAME                3 (field)
                      104 LOAD_CONST               1 (False)
                      106 KW_NAMES                 2
                      108 PRECALL                  1
                      112 CALL                     1
                      122 STORE_NAME               9 (token)
                      124 LOAD_NAME                5 (str)
                      126 LOAD_NAME                6 (__annotations__)
                      128 LOAD_CONST               7 ('token')
                      130 STORE_SUBSCR
          
-          26         134 LOAD_CONST               8 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 26>)
+          30         134 LOAD_CONST               8 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 30>)
                      136 MAKE_FUNCTION            0
                      138 STORE_NAME              10 (__post_init__)
                      140 LOAD_CONST               9 (None)
                      142 RETURN_VALUE
          consts
             'Auth'
             False
@@ -254,71 +249,71 @@
                   00000000007c017a0000007c005f06000000000000000064047c006a0300
                   000000000000009b0064057c006a0600000000000000009b009d047c005f
                   0700000000000000007411000000000000000000007c006a070000000000
                   000000a0090000000000000000000000000000000000000000a6000000ab
                   000000000000000000a6010000ab010000000000000000a00a0000000000
                   000000000000000000000000000000a6000000ab0000000000000000007c
                   005f0b000000000000000064005300
-                26           0 RESUME                   0
+                30           0 RESUME                   0
                
-                27           2 LOAD_GLOBAL              1 (NULL + len)
+                31           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_GLOBAL              3 (NULL + str)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (code)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 PRECALL                  1
                             56 CALL                     1
                             66 LOAD_CONST               1 (6)
                             68 COMPARE_OP               2 (==)
                             74 POP_JUMP_FORWARD_IF_TRUE     2 (to 80)
                             76 LOAD_ASSERTION_ERROR
                             78 RAISE_VARARGS            1
                
-                28     >>   80 LOAD_GLOBAL              1 (NULL + len)
+                32     >>   80 LOAD_GLOBAL              1 (NULL + len)
                             92 LOAD_GLOBAL              3 (NULL + str)
                            104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                3 (phone)
                            116 PRECALL                  1
                            120 CALL                     1
                            130 PRECALL                  1
                            134 CALL                     1
                            144 LOAD_CONST               2 (10)
                            146 COMPARE_OP               2 (==)
                            152 POP_JUMP_FORWARD_IF_TRUE     2 (to 158)
                            154 LOAD_ASSERTION_ERROR
                            156 RAISE_VARARGS            1
                
-                29     >>  158 LOAD_CONST               3 (604800)
+                33     >>  158 LOAD_CONST               3 (604800)
                            160 STORE_FAST               1 (SEVEN_DAYS)
                
-                30         162 LOAD_GLOBAL              9 (NULL + int)
+                34         162 LOAD_GLOBAL              9 (NULL + int)
                            174 LOAD_GLOBAL             11 (NULL + time)
                            186 PRECALL                  0
                            190 CALL                     0
                            200 PRECALL                  1
                            204 CALL                     1
                            214 LOAD_FAST                1 (SEVEN_DAYS)
                            216 BINARY_OP                0 (+)
                            220 LOAD_FAST                0 (self)
                            222 STORE_ATTR               6 (expires)
                
-                31         232 LOAD_CONST               4 ('auth/')
+                35         232 LOAD_CONST               4 ('auth/')
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                3 (phone)
                            246 FORMAT_VALUE             0
                            248 LOAD_CONST               5 ('/')
                            250 LOAD_FAST                0 (self)
                            252 LOAD_ATTR                6 (expires)
                            262 FORMAT_VALUE             0
                            264 BUILD_STRING             4
                            266 LOAD_FAST                0 (self)
                            268 STORE_ATTR               7 (key)
                
-                32         278 LOAD_GLOBAL             17 (NULL + md5)
+                36         278 LOAD_GLOBAL             17 (NULL + md5)
                            290 LOAD_FAST                0 (self)
                            292 LOAD_ATTR                7 (key)
                            302 LOAD_METHOD              9 (encode)
                            324 PRECALL                  0
                            328 CALL                     0
                            338 PRECALL                  1
                            342 CALL                     1
@@ -338,24 +333,24 @@
                   '/'
                names      ('len', 'str', 'code', 'phone', 'int', 'time', 'expires', 'key', 'md5', 'encode', 'hexdigest', 'token')
                varnames   ('self', 'SEVEN_DAYS')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
                name       '__post_init__'
-               firstlineno 26
+               firstlineno 30
                lnotab 0x02014e014e01040146012e01
             None
          names      ('__name__', '__module__', '__qualname__', 'field', 'key', 'str', '__annotations__', 'expires', 'int', 'token', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'Auth'
-         firstlineno 18
+         firstlineno 22
          lnotab 0x0c0222010a010a0122012202
       'Auth'
       'auth'
       'return'
       code
          argcount  : 1
          nlocals   : 2
@@ -365,41 +360,41 @@
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007c006a03000000000000000074
             09000000000000000000006a0500000000000000006401a6010000ab0100
             000000000000007c006a0600000000000000009b0064029d02ac03a60300
             00ab0300000000000000007d01740f0000000000000000000064047c006a
             0300000000000000009b009d02a6010000ab010000000000000000010064
             005300
-          35           0 RESUME                   0
+          39           0 RESUME                   0
          
-          36           2 LOAD_GLOBAL              0 (twilio_client)
+          40           2 LOAD_GLOBAL              0 (twilio_client)
                       14 LOAD_ATTR                1 (messages)
                       24 LOAD_METHOD              2 (create)
          
-          37          46 LOAD_FAST                0 (auth)
+          41          46 LOAD_FAST                0 (auth)
                       48 LOAD_ATTR                3 (phone)
          
-          38          58 LOAD_GLOBAL              9 (NULL + os)
+          42          58 LOAD_GLOBAL              9 (NULL + os)
                       70 LOAD_ATTR                5 (getenv)
                       80 LOAD_CONST               1 ('TWILIO_NUMBER')
                       82 PRECALL                  1
                       86 CALL                     1
          
-          39          96 LOAD_FAST                0 (auth)
+          43          96 LOAD_FAST                0 (auth)
                       98 LOAD_ATTR                6 (code)
                      108 FORMAT_VALUE             0
                      110 LOAD_CONST               2 (' is your GA Research authentication code.')
                      112 BUILD_STRING             2
          
-          36         114 KW_NAMES                 3
+          40         114 KW_NAMES                 3
                      116 PRECALL                  3
                      120 CALL                     3
                      130 STORE_FAST               1 (message)
          
-          41         132 LOAD_GLOBAL             15 (NULL + print)
+          45         132 LOAD_GLOBAL             15 (NULL + print)
                      144 LOAD_CONST               4 ('Login Sent to ')
                      146 LOAD_FAST                0 (auth)
                      148 LOAD_ATTR                3 (phone)
                      158 FORMAT_VALUE             0
                      160 BUILD_STRING             2
                      162 PRECALL                  1
                      166 CALL                     1
@@ -414,15 +409,15 @@
             'Login Sent to '
          names      ('twilio_client', 'messages', 'create', 'phone', 'os', 'getenv', 'code', 'print')
          varnames   ('auth', 'message')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       '_send_code'
-         firstlineno 35
+         firstlineno 39
          lnotab 0x02012c010c01260112fd1205
       'phone'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -430,45 +425,45 @@
             0x97007401000000000000000000007403000000000000000000006a0200
             0000000000000064016402a6020000ab020000000000000000a6010000ab
             0100000000000000007d017407000000000000000000007c007c01ac03a6
             020000ab0200000000000000007d027409000000000000000000007c02a6
             010000ab010000000000000000740a000000000000000000007c026a0600
             000000000000003c000000740f000000000000000000007c02a6010000ab
             010000000000000000010064005300
-          44           0 RESUME                   0
+          48           0 RESUME                   0
          
-          46           2 LOAD_GLOBAL              1 (NULL + str)
+          50           2 LOAD_GLOBAL              1 (NULL + str)
                       14 LOAD_GLOBAL              3 (NULL + random)
                       26 LOAD_ATTR                2 (randint)
                       36 LOAD_CONST               1 (100000)
                       38 LOAD_CONST               2 (999999)
                       40 PRECALL                  2
                       44 CALL                     2
                       54 PRECALL                  1
                       58 CALL                     1
                       68 STORE_FAST               1 (auth_code)
          
-          47          70 LOAD_GLOBAL              7 (NULL + Auth)
+          51          70 LOAD_GLOBAL              7 (NULL + Auth)
                       82 LOAD_FAST                0 (phone)
                       84 LOAD_FAST                1 (auth_code)
                       86 KW_NAMES                 3
                       88 PRECALL                  2
                       92 CALL                     2
                      102 STORE_FAST               2 (auth)
          
-          48         104 LOAD_GLOBAL              9 (NULL + asdict)
+          52         104 LOAD_GLOBAL              9 (NULL + asdict)
                      116 LOAD_FAST                2 (auth)
                      118 PRECALL                  1
                      122 CALL                     1
                      132 LOAD_GLOBAL             10 (ds)
                      144 LOAD_FAST                2 (auth)
                      146 LOAD_ATTR                6 (key)
                      156 STORE_SUBSCR
          
-          49         160 LOAD_GLOBAL             15 (NULL + _send_code)
+          53         160 LOAD_GLOBAL             15 (NULL + _send_code)
                      172 LOAD_FAST                2 (auth)
                      174 PRECALL                  1
                      178 CALL                     1
                      188 POP_TOP
                      190 LOAD_CONST               0 (None)
                      192 RETURN_VALUE
          consts
@@ -478,15 +473,15 @@
             ('phone', 'code')
          names      ('str', 'random', 'randint', 'Auth', 'asdict', 'ds', 'key', '_send_code')
          varnames   ('phone', 'auth_code', 'auth')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'send_code'
-         firstlineno 44
+         firstlineno 48
          lnotab 0x0202440122013801
       'code'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -500,80 +495,80 @@
             00000000000000740d00000000000000000000a6000000ab000000000000
             000000a6010000ab0100000000000000006b040000000019000000000000
             0000007d027c027c026404190000000000000000007c006b020000000019
             0000000000000000007d02740f000000000000000000007c02a6010000ab
             01000000000000000064056b0400000000721c7c02a00800000000000000
             000000000000000000000000006406ac07a6010000ab0100000000000000
             00640519000000000000000000530064005300
-          52           0 RESUME                   0
+          56           0 RESUME                   0
          
-          53           2 LOAD_GLOBAL              0 (ds)
+          57           2 LOAD_GLOBAL              0 (ds)
                       14 LOAD_METHOD              1 (keys)
                       36 LOAD_CONST               1 ('auth/')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 LOAD_CONST               2 (1)
                       54 LOAD_CONST               0 (None)
                       56 BUILD_SLICE              2
                       58 BINARY_SUBSCR
                       68 STORE_FAST               1 (keys)
          
-          54          70 LOAD_GLOBAL              5 (NULL + pd)
+          58          70 LOAD_GLOBAL              5 (NULL + pd)
                       82 LOAD_ATTR                3 (DataFrame)
                       92 LOAD_GLOBAL              0 (ds)
                      104 LOAD_METHOD              4 (load_async)
                      126 LOAD_FAST                1 (keys)
                      128 PRECALL                  1
                      132 CALL                     1
                      142 PRECALL                  1
                      146 CALL                     1
                      156 STORE_FAST               2 (df)
          
-          55         158 LOAD_FAST                2 (df)
+          59         158 LOAD_FAST                2 (df)
                      160 LOAD_FAST                2 (df)
                      162 LOAD_CONST               3 ('expires')
                      164 BINARY_SUBSCR
                      174 LOAD_GLOBAL             11 (NULL + int)
                      186 LOAD_GLOBAL             13 (NULL + time)
                      198 PRECALL                  0
                      202 CALL                     0
                      212 PRECALL                  1
                      216 CALL                     1
                      226 COMPARE_OP               4 (>)
                      232 BINARY_SUBSCR
                      242 STORE_FAST               2 (df)
          
-          56         244 LOAD_FAST                2 (df)
+          60         244 LOAD_FAST                2 (df)
                      246 LOAD_FAST                2 (df)
                      248 LOAD_CONST               4 ('code')
                      250 BINARY_SUBSCR
                      260 LOAD_FAST                0 (code)
                      262 COMPARE_OP               2 (==)
                      268 BINARY_SUBSCR
                      278 STORE_FAST               2 (df)
          
-          57         280 LOAD_GLOBAL             15 (NULL + len)
+          61         280 LOAD_GLOBAL             15 (NULL + len)
                      292 LOAD_FAST                2 (df)
                      294 PRECALL                  1
                      298 CALL                     1
                      308 LOAD_CONST               5 (0)
                      310 COMPARE_OP               4 (>)
                      316 POP_JUMP_FORWARD_IF_FALSE    28 (to 374)
          
-          59         318 LOAD_FAST                2 (df)
+          63         318 LOAD_FAST                2 (df)
                      320 LOAD_METHOD              8 (to_dict)
                      342 LOAD_CONST               6 ('records')
                      344 KW_NAMES                 7
                      346 PRECALL                  1
                      350 CALL                     1
                      360 LOAD_CONST               5 (0)
                      362 BINARY_SUBSCR
                      372 RETURN_VALUE
          
-          61     >>  374 LOAD_CONST               0 (None)
+          65     >>  374 LOAD_CONST               0 (None)
                      376 RETURN_VALUE
          consts
             None
             'auth/'
             1
             'expires'
             'code'
@@ -582,40 +577,40 @@
             ('orient',)
          names      ('ds', 'keys', 'pd', 'DataFrame', 'load_async', 'int', 'time', 'len', 'to_dict')
          varnames   ('code', 'keys', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'authenticate'
-         firstlineno 52
+         firstlineno 56
          lnotab 0x0201440158015601240126023802
       'token'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 1
          flags     : 3
          code 0x970064005300
-          64           0 RESUME                   0
+          68           0 RESUME                   0
          
-          65           2 LOAD_CONST               0 (None)
+          69           2 LOAD_CONST               0 (None)
                        4 RETURN_VALUE
          consts
             None
          names      ()
          varnames   ('token',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'validate'
-         firstlineno 64
+         firstlineno 68
          lnotab 0x0201
-   names      ('pandas', 'pd', 'random', 'dataclasses', 'asdict', 'dataclass', 'field', 'hashlib', 'md5', 'time', 'os', 'twilio.rest', 'Client', 'gandai.datastore', 'Cloudstore', 'ds', 'getenv', 'twilio_client', 'Auth', '_send_code', 'str', 'send_code', 'authenticate', 'bool', 'validate')
+   names      ('pandas', 'pd', 'random', 'dataclasses', 'asdict', 'dataclass', 'field', 'hashlib', 'md5', 'time', 'os', 'twilio.rest', 'Client', 'gandai.secrets', 'access_secret_version', 'ds', 'twilio_client', 'Auth', '_send_code', 'str', 'send_code', 'authenticate', 'bool', 'validate')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080114010c010c0108010c040c0314015003020118ff0e
-      01021010091008100c
+      0x00ff02010801080114010c010c0108010c050c040401040128ff100502
+      0118ff0e01021010091008100c
```

### Comparing `gandai-1.1.9/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.2.0/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files 23% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0xd17d6164 (Mon May 15 00:33:21 2023 UTC)
-files sz: 1583
+moddate:  0xcc797f64 (Tue Jun  6 18:24:12 2023 UTC)
+files sz: 1500
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       026c036d045a040100640064036c056d065a066d075a076d085a08010064
-      0064046c096d0a5a0a0100640064016c025a0202004700640584006406a6
-      020000ab0200000000000000005a0b64015300
+      0064046c096d0a5a0a0100640064016c025a02640064056c0b6d0c5a0c01
+      000200650ca6000000ab0000000000000000000100020047006406840064
+      07a6020000ab0200000000000000005a0d64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (datetime)
                  8 STORE_NAME               0 (datetime)
    
@@ -54,30 +55,44 @@
                 68 POP_TOP
    
      8          70 LOAD_CONST               0 (0)
                 72 LOAD_CONST               1 (None)
                 74 IMPORT_NAME              2 (os)
                 76 STORE_NAME               2 (os)
    
-    12          78 PUSH_NULL
-                80 LOAD_BUILD_CLASS
-                82 LOAD_CONST               5 (<code object Cloudstore, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 12>)
-                84 MAKE_FUNCTION            0
-                86 LOAD_CONST               6 ('Cloudstore')
-                88 PRECALL                  2
-                92 CALL                     2
-               102 STORE_NAME              11 (Cloudstore)
-               104 LOAD_CONST               1 (None)
-               106 RETURN_VALUE
+     9          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               5 (('load_dotenv',))
+                82 IMPORT_NAME             11 (dotenv)
+                84 IMPORT_FROM             12 (load_dotenv)
+                86 STORE_NAME              12 (load_dotenv)
+                88 POP_TOP
+   
+    10          90 PUSH_NULL
+                92 LOAD_NAME               12 (load_dotenv)
+                94 PRECALL                  0
+                98 CALL                     0
+               108 POP_TOP
+   
+    12         110 PUSH_NULL
+               112 LOAD_BUILD_CLASS
+               114 LOAD_CONST               6 (<code object Cloudstore, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 12>)
+               116 MAKE_FUNCTION            0
+               118 LOAD_CONST               7 ('Cloudstore')
+               120 PRECALL                  2
+               124 CALL                     2
+               134 STORE_NAME              13 (Cloudstore)
+               136 LOAD_CONST               1 (None)
+               138 RETURN_VALUE
    consts
       0
       None
       ('ThreadPoolExecutor',)
       ('Any', 'Dict', 'List')
       ('storage',)
+      ('load_dotenv',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640d6403650465051900000000
@@ -90,279 +105,261 @@
                        6 LOAD_CONST               0 ('Cloudstore')
                        8 STORE_NAME               2 (__qualname__)
          
           13          10 LOAD_CONST               1 (<code object __init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 13>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-          20          16 LOAD_CONST              13 (('',))
+          19          16 LOAD_CONST              13 (('',))
                       18 LOAD_CONST               3 ('return')
                       20 LOAD_NAME                4 (List)
                       22 LOAD_NAME                5 (str)
                       24 BINARY_SUBSCR
                       34 BUILD_TUPLE              2
-                      36 LOAD_CONST               4 (<code object keys, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 20>)
+                      36 LOAD_CONST               4 (<code object keys, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 19>)
                       38 MAKE_FUNCTION            5 (defaults, annotations)
                       40 STORE_NAME               6 (keys)
          
-          27          42 LOAD_CONST               5 ('key')
+          26          42 LOAD_CONST               5 ('key')
                       44 LOAD_NAME                5 (str)
                       46 LOAD_CONST               3 ('return')
                       48 LOAD_CONST               6 (None)
                       50 BUILD_TUPLE              4
-                      52 LOAD_CONST               7 (<code object delete, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 27>)
+                      52 LOAD_CONST               7 (<code object delete, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 26>)
                       54 MAKE_FUNCTION            4 (annotations)
                       56 STORE_NAME               7 (delete)
          
-          31          58 LOAD_CONST               5 ('key')
+          30          58 LOAD_CONST               5 ('key')
                       60 LOAD_NAME                5 (str)
                       62 LOAD_CONST               3 ('return')
                       64 LOAD_NAME                8 (json)
                       66 BUILD_TUPLE              4
-                      68 LOAD_CONST               8 (<code object __getitem__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 31>)
+                      68 LOAD_CONST               8 (<code object __getitem__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 30>)
                       70 MAKE_FUNCTION            4 (annotations)
                       72 STORE_NAME               9 (__getitem__)
          
-          35          74 LOAD_CONST               5 ('key')
+          34          74 LOAD_CONST               5 ('key')
                       76 LOAD_NAME                5 (str)
                       78 LOAD_CONST               3 ('return')
                       80 LOAD_CONST               6 (None)
                       82 BUILD_TUPLE              4
-                      84 LOAD_CONST               9 (<code object __setitem__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 35>)
+                      84 LOAD_CONST               9 (<code object __setitem__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 34>)
                       86 MAKE_FUNCTION            4 (annotations)
                       88 STORE_NAME              10 (__setitem__)
          
-          39          90 LOAD_CONST              10 (<code object load_async, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 39>)
+          38          90 LOAD_CONST              10 (<code object load_async, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 38>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              11 (load_async)
          
-          44          96 LOAD_CONST              14 ((72,))
+          43          96 LOAD_CONST              14 ((72,))
                       98 LOAD_CONST               5 ('key')
                      100 LOAD_NAME                5 (str)
                      102 LOAD_CONST               3 ('return')
                      104 LOAD_NAME                5 (str)
                      106 BUILD_TUPLE              4
-                     108 LOAD_CONST              12 (<code object get_signed_url, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 44>)
+                     108 LOAD_CONST              12 (<code object get_signed_url, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 43>)
                      110 MAKE_FUNCTION            5 (defaults, annotations)
                      112 STORE_NAME              12 (get_signed_url)
                      114 LOAD_CONST               6 (None)
                      116 RETURN_VALUE
          consts
             'Cloudstore'
             code
                argcount  : 1
-               nlocals   : 3
-               stacksize : 4
+               nlocals   : 2
+               stacksize : 3
                flags     : 3
                code
-                  0x97007401000000000000000000006a01000000000000000064016402a6
-                  020000ab0200000000000000007d017401000000000000000000006a0100
-                  0000000000000064036404a6020000ab0200000000000000007d027c019b
-                  0064057c029b009d037c005f020000000000000000740700000000000000
-                  0000006a0400000000000000007c01ac06a6010000ab0100000000000000
-                  007c005f0500000000000000007c006a050000000000000000a006000000
-                  00000000000000000000000000000000007c006a020000000000000000a6
-                  010000ab0100000000000000007c005f07000000000000000064005300
+                  0x97007401000000000000000000006a0100000000000000006401a60100
+                  00ab0100000000000000007d017c019b007c005f02000000000000000074
+                  07000000000000000000006a0400000000000000007c01ac02a6010000ab
+                  0100000000000000007c005f0500000000000000007c006a050000000000
+                  000000a00600000000000000000000000000000000000000007c006a0200
+                  00000000000000a6010000ab0100000000000000007c005f070000000000
+                  00000064005300
                 13           0 RESUME                   0
                
                 14           2 LOAD_GLOBAL              1 (NULL + os)
                             14 LOAD_ATTR                1 (getenv)
-                            24 LOAD_CONST               1 ('GCP_PROJECT')
-                            26 LOAD_CONST               2 ('gandai-prod')
-                            28 PRECALL                  2
-                            32 CALL                     2
-                            42 STORE_FAST               1 (GCP_PROJECT)
-               
-                15          44 LOAD_GLOBAL              1 (NULL + os)
-                            56 LOAD_ATTR                1 (getenv)
-                            66 LOAD_CONST               3 ('GCP_STAGE')
-                            68 LOAD_CONST               4 ('prod')
-                            70 PRECALL                  2
-                            74 CALL                     2
-                            84 STORE_FAST               2 (GCP_STAGE)
-               
-                16          86 LOAD_FAST                1 (GCP_PROJECT)
-                            88 FORMAT_VALUE             0
-                            90 LOAD_CONST               5 ('-')
-                            92 LOAD_FAST                2 (GCP_STAGE)
-                            94 FORMAT_VALUE             0
-                            96 BUILD_STRING             3
+                            24 LOAD_CONST               1 ('PROJECT_ID')
+                            26 PRECALL                  1
+                            30 CALL                     1
+                            40 STORE_FAST               1 (GCP_PROJECT)
+               
+                15          42 LOAD_FAST                1 (GCP_PROJECT)
+                            44 FORMAT_VALUE             0
+                            46 LOAD_FAST                0 (self)
+                            48 STORE_ATTR               2 (BUCKET_NAME)
+               
+                16          58 LOAD_GLOBAL              7 (NULL + storage)
+                            70 LOAD_ATTR                4 (Client)
+                            80 LOAD_FAST                1 (GCP_PROJECT)
+                            82 KW_NAMES                 2
+                            84 PRECALL                  1
+                            88 CALL                     1
                             98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               2 (BUCKET_NAME)
+                           100 STORE_ATTR               5 (client)
                
-                17         110 LOAD_GLOBAL              7 (NULL + storage)
-                           122 LOAD_ATTR                4 (Client)
-                           132 LOAD_FAST                1 (GCP_PROJECT)
-                           134 KW_NAMES                 6
-                           136 PRECALL                  1
-                           140 CALL                     1
-                           150 LOAD_FAST                0 (self)
-                           152 STORE_ATTR               5 (client)
-               
-                18         162 LOAD_FAST                0 (self)
-                           164 LOAD_ATTR                5 (client)
-                           174 LOAD_METHOD              6 (get_bucket)
-                           196 LOAD_FAST                0 (self)
-                           198 LOAD_ATTR                2 (BUCKET_NAME)
-                           208 PRECALL                  1
-                           212 CALL                     1
-                           222 LOAD_FAST                0 (self)
-                           224 STORE_ATTR               7 (bucket)
-                           234 LOAD_CONST               0 (None)
-                           236 RETURN_VALUE
+                17         110 LOAD_FAST                0 (self)
+                           112 LOAD_ATTR                5 (client)
+                           122 LOAD_METHOD              6 (get_bucket)
+                           144 LOAD_FAST                0 (self)
+                           146 LOAD_ATTR                2 (BUCKET_NAME)
+                           156 PRECALL                  1
+                           160 CALL                     1
+                           170 LOAD_FAST                0 (self)
+                           172 STORE_ATTR               7 (bucket)
+                           182 LOAD_CONST               0 (None)
+                           184 RETURN_VALUE
                consts
                   None
-                  'GCP_PROJECT'
-                  'gandai-prod'
-                  'GCP_STAGE'
-                  'prod'
-                  '-'
+                  'PROJECT_ID'
                   ('project',)
                names      ('os', 'getenv', 'BUCKET_NAME', 'storage', 'Client', 'client', 'get_bucket', 'bucket')
-               varnames   ('self', 'GCP_PROJECT', 'GCP_STAGE')
+               varnames   ('self', 'GCP_PROJECT')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
                name       '__init__'
                firstlineno 13
-               lnotab 0x02012a012a0118013401
+               lnotab 0x0201280110013401
             ''
             'return'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
                   0x9700640184007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c006a0200000000000000007c01ac02a60200
                   00ab0200000000000000004400a6000000ab0000000000000000007d027c
                   025300
-                20           0 RESUME                   0
+                19           0 RESUME                   0
                
-                21           2 LOAD_CONST               1 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 21>)
+                20           2 LOAD_CONST               1 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 20>)
                              4 MAKE_FUNCTION            0
                
-                23           6 LOAD_FAST                0 (self)
+                22           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (client)
                             18 LOAD_METHOD              1 (list_blobs)
                             40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                2 (BUCKET_NAME)
                             52 LOAD_FAST                1 (prefix)
                             54 KW_NAMES                 2
                             56 PRECALL                  2
                             60 CALL                     2
                
-                21          70 GET_ITER
+                20          70 GET_ITER
                             72 PRECALL                  0
                             76 CALL                     0
                             86 STORE_FAST               2 (keys)
                
-                25          88 LOAD_FAST                2 (keys)
+                24          88 LOAD_FAST                2 (keys)
                             90 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                      21           0 RESUME                   0
+                      20           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                      
-                      23           8 STORE_FAST               1 (blob)
+                      22           8 STORE_FAST               1 (blob)
                      
-                      22          10 LOAD_FAST                1 (blob)
+                      21          10 LOAD_FAST                1 (blob)
                                   12 LOAD_ATTR                0 (name)
                      
-                      21          22 LIST_APPEND              2
+                      20          22 LIST_APPEND              2
                                   24 JUMP_BACKWARD           10 (to 6)
                              >>   26 RETURN_VALUE
                      consts
                      names      ('name',)
                      varnames   ('.0', 'blob')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
                      name       '<listcomp>'
-                     firstlineno 21
+                     firstlineno 20
                      lnotab 0x080202ff0cff
                   ('prefix',)
                names      ('client', 'list_blobs', 'BUCKET_NAME')
                varnames   ('self', 'prefix', 'keys')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
                name       'keys'
-               firstlineno 20
+               firstlineno 19
                lnotab 0x0201040240fe1204
             'key'
             None
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000007d027c02a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   000000010064005300
-                27           0 RESUME                   0
+                26           0 RESUME                   0
                
-                28           2 LOAD_FAST                0 (self)
+                27           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (bucket)
                             14 LOAD_METHOD              1 (blob)
                             36 LOAD_FAST                1 (key)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               2 (blob)
                
-                29          54 LOAD_FAST                2 (blob)
+                28          54 LOAD_FAST                2 (blob)
                             56 LOAD_METHOD              2 (delete)
                             78 PRECALL                  0
                             82 CALL                     0
                             92 POP_TOP
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                consts
                   None
                names      ('bucket', 'blob', 'delete')
                varnames   ('self', 'key', 'blob')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
                name       'delete'
-               firstlineno 27
+               firstlineno 26
                lnotab 0x02013401
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000007d027405000000
                   000000000000006a0300000000000000007c02a004000000000000000000
                   0000000000000000000000a6000000ab000000000000000000a6010000ab
                   0100000000000000005300
-                31           0 RESUME                   0
+                30           0 RESUME                   0
                
-                32           2 LOAD_FAST                0 (self)
+                31           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (bucket)
                             14 LOAD_METHOD              1 (blob)
                             36 LOAD_FAST                1 (key)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               2 (blob)
                
-                33          54 LOAD_GLOBAL              5 (NULL + json)
+                32          54 LOAD_GLOBAL              5 (NULL + json)
                             66 LOAD_ATTR                3 (loads)
                             76 LOAD_FAST                2 (blob)
                             78 LOAD_METHOD              4 (download_as_string)
                            100 PRECALL                  0
                            104 CALL                     0
                            114 PRECALL                  1
                            118 CALL                     1
@@ -371,38 +368,38 @@
                   None
                names      ('bucket', 'blob', 'json', 'loads', 'download_as_string')
                varnames   ('self', 'key', 'blob')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
                name       '__getitem__'
-               firstlineno 31
+               firstlineno 30
                lnotab 0x02013401
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000007d037c03a00200
                   000000000000000000000000000000000000007407000000000000000000
                   006a0400000000000000007c02a6010000ab010000000000000000a60100
                   00ab010000000000000000010064005300
-                35           0 RESUME                   0
+                34           0 RESUME                   0
                
-                36           2 LOAD_FAST                0 (self)
+                35           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (bucket)
                             14 LOAD_METHOD              1 (blob)
                             36 LOAD_FAST                1 (key)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (blob)
                
-                37          54 LOAD_FAST                3 (blob)
+                36          54 LOAD_FAST                3 (blob)
                             56 LOAD_METHOD              2 (upload_from_string)
                             78 LOAD_GLOBAL              7 (NULL + json)
                             90 LOAD_ATTR                4 (dumps)
                            100 LOAD_FAST                2 (data)
                            102 PRECALL                  1
                            106 CALL                     1
                            116 PRECALL                  1
@@ -414,48 +411,48 @@
                   None
                names      ('bucket', 'blob', 'upload_from_string', 'json', 'dumps')
                varnames   ('self', 'key', 'data', 'blob')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
                name       '__setitem__'
-               firstlineno 35
+               firstlineno 34
                lnotab 0x02013401
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000006401ac02a6010000ab010000000000
                   00000035007d027c02a00100000000000000000000000000000000000000
                   007c006a0200000000000000007c01a6020000ab0200000000000000007d
                   03640064006400a6020000ab02000000000000000001006e0b2300310073
                   04770278035900770101005900010001007407000000000000000000007c
                   03a6010000ab0100000000000000005300
-                39           0 RESUME                   0
+                38           0 RESUME                   0
                
-                40           2 LOAD_GLOBAL              1 (NULL + ThreadPoolExecutor)
+                39           2 LOAD_GLOBAL              1 (NULL + ThreadPoolExecutor)
                             14 LOAD_CONST               1 (20)
                             16 KW_NAMES                 2
                             18 PRECALL                  1
                             22 CALL                     1
                             32 BEFORE_WITH
                             34 STORE_FAST               2 (exec)
                
-                41          36 LOAD_FAST                2 (exec)
+                40          36 LOAD_FAST                2 (exec)
                             38 LOAD_METHOD              1 (map)
                             60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                2 (__getitem__)
                             72 LOAD_FAST                1 (keys)
                             74 PRECALL                  2
                             78 CALL                     2
                             88 STORE_FAST               3 (futures)
                
-                40          90 LOAD_CONST               0 (None)
+                39          90 LOAD_CONST               0 (None)
                             92 LOAD_CONST               0 (None)
                             94 LOAD_CONST               0 (None)
                             96 PRECALL                  2
                            100 CALL                     2
                            110 POP_TOP
                            112 JUMP_FORWARD            11 (to 136)
                        >>  114 PUSH_EXC_INFO
@@ -466,15 +463,15 @@
                            124 POP_EXCEPT
                            126 RERAISE                  1
                        >>  128 POP_TOP
                            130 POP_EXCEPT
                            132 POP_TOP
                            134 POP_TOP
                
-                42     >>  136 LOAD_GLOBAL              7 (NULL + list)
+                41     >>  136 LOAD_GLOBAL              7 (NULL + list)
                            148 LOAD_FAST                3 (futures)
                            150 PRECALL                  1
                            154 CALL                     1
                            164 RETURN_VALUE
                ExceptionTable:
                  34 to 88 -> 114 [1] lasti
                  114 to 120 -> 122 [3] lasti
@@ -485,86 +482,86 @@
                   ('max_workers',)
                names      ('ThreadPoolExecutor', 'map', '__getitem__', 'list')
                varnames   ('self', 'keys', 'exec', 'futures')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
                name       'load_async'
-               firstlineno 39
+               firstlineno 38
                lnotab 0x0201220136ff2e02
             72
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000007d037405000000
                   000000000000006a0300000000000000007c02ac01a6010000ab01000000
                   00000000007d047c03a00400000000000000000000000000000000000000
                   0064027c046403ac04a6030000ab0300000000000000007d057c055300
-                44           0 RESUME                   0
+                43           0 RESUME                   0
                
-                45           2 LOAD_FAST                0 (self)
+                44           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (bucket)
                             14 LOAD_METHOD              1 (blob)
                             36 LOAD_FAST                1 (key)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (blob)
                
-                46          54 LOAD_GLOBAL              5 (NULL + datetime)
+                45          54 LOAD_GLOBAL              5 (NULL + datetime)
                             66 LOAD_ATTR                3 (timedelta)
                             76 LOAD_FAST                2 (hours_valid)
                             78 KW_NAMES                 1
                             80 PRECALL                  1
                             84 CALL                     1
                             94 STORE_FAST               4 (expiration)
                
-                47          96 LOAD_FAST                3 (blob)
+                46          96 LOAD_FAST                3 (blob)
                             98 LOAD_METHOD              4 (generate_signed_url)
                
-                48         120 LOAD_CONST               2 ('v4')
+                47         120 LOAD_CONST               2 ('v4')
                            122 LOAD_FAST                4 (expiration)
                            124 LOAD_CONST               3 ('GET')
                
-                47         126 KW_NAMES                 4
+                46         126 KW_NAMES                 4
                            128 PRECALL                  3
                            132 CALL                     3
                            142 STORE_FAST               5 (url)
                
-                50         144 LOAD_FAST                5 (url)
+                49         144 LOAD_FAST                5 (url)
                            146 RETURN_VALUE
                consts
                   None
                   ('hours',)
                   'v4'
                   'GET'
                   ('version', 'expiration', 'method')
                names      ('bucket', 'blob', 'datetime', 'timedelta', 'generate_signed_url')
                varnames   ('self', 'key', 'hours_valid', 'blob', 'expiration', 'url')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
                name       'get_signed_url'
-               firstlineno 44
+               firstlineno 43
                lnotab 0x020134012a01180106ff1203
             ('',)
             (72,)
          names      ('__name__', '__module__', '__qualname__', '__init__', 'List', 'str', 'keys', 'delete', 'json', '__getitem__', '__setitem__', 'load_async', 'get_signed_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
          name       'Cloudstore'
          firstlineno 12
-         lnotab 0x0a0106071a071004100410040605
+         lnotab 0x0a0106061a071004100410040605
       'Cloudstore'
-   names      ('datetime', 'json', 'os', 'concurrent.futures', 'ThreadPoolExecutor', 'typing', 'Any', 'Dict', 'List', 'google.cloud', 'storage', 'Cloudstore')
+   names      ('datetime', 'json', 'os', 'concurrent.futures', 'ThreadPoolExecutor', 'typing', 'Any', 'Dict', 'List', 'google.cloud', 'storage', 'dotenv', 'load_dotenv', 'Cloudstore')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010801080108010c0214010c010804
+   lnotab 0x00ff02010801080108010c0214010c0108010c011402
```

### Comparing `gandai-1.1.9/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.2.0/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.9/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.2.0/gandai/__pycache__/models.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x64556064 (Sun May 14 03:28:36 2023 UTC)
-files sz: 2642
+moddate:  0x5ba76c64 (Tue May 23 11:45:31 2023 UTC)
+files sz: 2652
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
@@ -291,16 +291,16 @@
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c00000064025a05650665
             0319000000000000000000650464033c00000064025a0765066503190000
             00000000000000650464043c000000020065086509ac05a6010000ab0100
             000000000000005a0a6509650464063c000000020065086402ac07a60100
             00ab0100000000000000005a0b650c650464083c000000020065086402ac
-            07a6010000ab0100000000000000005a0d650c650464093c000000640253
-            00
+            07a6010000ab0100000000000000005a0d6506650c190000000000000000
+            00650464093c00000064025300
           15           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Company')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -354,20 +354,22 @@
           22         142 PUSH_NULL
                      144 LOAD_NAME                8 (field)
                      146 LOAD_CONST               2 (None)
                      148 KW_NAMES                 7
                      150 PRECALL                  1
                      154 CALL                     1
                      164 STORE_NAME              13 (uid)
-                     166 LOAD_NAME               12 (int)
-                     168 LOAD_NAME                4 (__annotations__)
-                     170 LOAD_CONST               9 ('uid')
-                     172 STORE_SUBSCR
-                     176 LOAD_CONST               2 (None)
-                     178 RETURN_VALUE
+                     166 LOAD_NAME                6 (Optional)
+                     168 LOAD_NAME               12 (int)
+                     170 BINARY_SUBSCR
+                     180 LOAD_NAME                4 (__annotations__)
+                     182 LOAD_CONST               9 ('uid')
+                     184 STORE_SUBSCR
+                     188 LOAD_CONST               2 (None)
+                     190 RETURN_VALUE
          consts
             'Company'
             'domain'
             None
             'name'
             'description'
             ('default_factory',)
```

### Comparing `gandai-1.1.9/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.2.0/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,267 +1,326 @@
 magic:    0xa70d0d0a
-moddate:  0x3b766164 (Mon May 15 00:00:59 2023 UTC)
-files sz: 9337
+moddate:  0x22b16c64 (Tue May 23 12:27:14 2023 UTC)
+files sz: 12867
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 5
+   stacksize : 8
    flags     : 0
    code
-      0x9700640064016c005a00640064016c015a02640064026c036d045a0401
-      00640064036c056d065a060100640064046c076d085a086d095a096d0a5a
-      0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064016c0e5a0e640064056c0f6d
-      105a100100640064066c116d125a12010002006512a6000000ab00000000
-      00000000000100640064076c136d145a14010002006514a6000000ab0000
-      000000000000005a15640865096602640984045a16640a6508640b650866
-      04640c84045a17640d650b640b650b6604640e84045a18640f650c640b65
-      0c6604641084045a196411650d640b650d6604641284045a1a641384005a
-      1b64236414651c6415651d6604641684055a1e6414651c640b65026a1f00
-      000000000000006604641784045a206414651c640b65026a1f0000000000
-      0000006604641884045a21640b65026a1f00000000000000006602641984
-      045a226414651c640b65026a1f00000000000000006604641a84045a2364
-      14651c640b65026a1f00000000000000006604641b84045a246414651c64
-      0b650c6604641c84045a25641d651d640b65096604641e84045a26641f65
-      1c640b65086604642084045a2764086509640b64016604642184045a2864
-      0f650c640b64016604642284045a2964015300
+      0x9700640064016c005a00640064016c015a02640064026c036d045a046d
+      055a050100640064036c066d075a070100640064046c086d095a09010064
+      0064056c0a6d0b5a0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a1001
+      00640064016c115a11640064066c126d135a130100640064076c146d155a
+      15010002006515a6000000ab0000000000000000000100640064086c166d
+      175a17010002006517a6000000ab0000000000000000005a186409650c66
+      02640a84045a19640b650b640c650b6604640d84045a1a640e650e640c65
+      0e6604640f84045a1b6410650f640c650f6604641184045a1c6412651064
+      0c65106604641384045a1d64146504651e19000000000000000000641565
+      1f6416651e640c64016608641784045a2064186504650519000000000000
+      0000006415651f6416651e640c64016608641984045a21641a84005a2264
+      296415651f641b651e6604641c84055a236415651f640c65026a24000000
+      00000000006604641d84045a256415651f640c65026a2400000000000000
+      006604641e84045a26640c65026a2400000000000000006602641f84045a
+      276415651f640c65026a2400000000000000006604642084045a28641565
+      1f640c65026a2400000000000000006604642184045a296415651f640c65
+      0f6604642284045a2a6423651e640c650c6604642484045a2b6425651f64
+      0c650b6604642684045a2c6409650c640c64016604642784045a2d641065
+      0f640c64016604642884045a2e64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (json)
                  8 STORE_NAME               0 (json)
    
      2          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
                 14 IMPORT_NAME              1 (pandas)
                 16 STORE_NAME               2 (pd)
    
      3          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               2 (('asdict',))
-                22 IMPORT_NAME              3 (dataclasses)
-                24 IMPORT_FROM              4 (asdict)
-                26 STORE_NAME               4 (asdict)
-                28 POP_TOP
-   
-     4          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('from_dict',))
-                34 IMPORT_NAME              5 (dacite)
-                36 IMPORT_FROM              6 (from_dict)
-                38 STORE_NAME               6 (from_dict)
-                40 POP_TOP
-   
-     5          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               4 (('Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint'))
-                46 IMPORT_NAME              7 (gandai.models)
-                48 IMPORT_FROM              8 (Event)
-                50 STORE_NAME               8 (Event)
-                52 IMPORT_FROM              9 (Company)
-                54 STORE_NAME               9 (Company)
-                56 IMPORT_FROM             10 (EventType)
-                58 STORE_NAME              10 (EventType)
-                60 IMPORT_FROM             11 (Actor)
-                62 STORE_NAME              11 (Actor)
-                64 IMPORT_FROM             12 (Search)
-                66 STORE_NAME              12 (Search)
-                68 IMPORT_FROM             13 (Checkpoint)
-                70 STORE_NAME              13 (Checkpoint)
-                72 POP_TOP
-   
-    15          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               1 (None)
-                78 IMPORT_NAME             14 (sqlalchemy)
-                80 STORE_NAME              14 (sqlalchemy)
-   
-    17          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               5 (('Connector',))
-                86 IMPORT_NAME             15 (google.cloud.sql.connector)
-                88 IMPORT_FROM             16 (Connector)
-                90 STORE_NAME              16 (Connector)
-                92 POP_TOP
-   
-    18          94 LOAD_CONST               0 (0)
-                96 LOAD_CONST               6 (('load_dotenv',))
-                98 IMPORT_NAME             17 (dotenv)
-               100 IMPORT_FROM             18 (load_dotenv)
-               102 STORE_NAME              18 (load_dotenv)
-               104 POP_TOP
-   
-    20         106 PUSH_NULL
-               108 LOAD_NAME               18 (load_dotenv)
-               110 PRECALL                  0
-               114 CALL                     0
-               124 POP_TOP
-   
-    22         126 LOAD_CONST               0 (0)
-               128 LOAD_CONST               7 (('connect_with_connector',))
-               130 IMPORT_NAME             19 (gandai.db)
-               132 IMPORT_FROM             20 (connect_with_connector)
-               134 STORE_NAME              20 (connect_with_connector)
-               136 POP_TOP
-   
-    24         138 PUSH_NULL
-               140 LOAD_NAME               20 (connect_with_connector)
-               142 PRECALL                  0
-               146 CALL                     0
-               156 STORE_NAME              21 (db)
-   
-    30         158 LOAD_CONST               8 ('company')
-               160 LOAD_NAME                9 (Company)
-               162 BUILD_TUPLE              2
-               164 LOAD_CONST               9 (<code object insert_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 30>)
-               166 MAKE_FUNCTION            4 (annotations)
-               168 STORE_NAME              22 (insert_company)
-   
-    44         170 LOAD_CONST              10 ('event')
-               172 LOAD_NAME                8 (Event)
-               174 LOAD_CONST              11 ('return')
-               176 LOAD_NAME                8 (Event)
-               178 BUILD_TUPLE              4
-               180 LOAD_CONST              12 (<code object insert_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 44>)
+                20 LOAD_CONST               2 (('List', 'Any'))
+                22 IMPORT_NAME              3 (typing)
+                24 IMPORT_FROM              4 (List)
+                26 STORE_NAME               4 (List)
+                28 IMPORT_FROM              5 (Any)
+                30 STORE_NAME               5 (Any)
+                32 POP_TOP
+   
+     4          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               3 (('asdict',))
+                38 IMPORT_NAME              6 (dataclasses)
+                40 IMPORT_FROM              7 (asdict)
+                42 STORE_NAME               7 (asdict)
+                44 POP_TOP
+   
+     5          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('from_dict',))
+                50 IMPORT_NAME              8 (dacite)
+                52 IMPORT_FROM              9 (from_dict)
+                54 STORE_NAME               9 (from_dict)
+                56 POP_TOP
+   
+     6          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               5 (('Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint'))
+                62 IMPORT_NAME             10 (gandai.models)
+                64 IMPORT_FROM             11 (Event)
+                66 STORE_NAME              11 (Event)
+                68 IMPORT_FROM             12 (Company)
+                70 STORE_NAME              12 (Company)
+                72 IMPORT_FROM             13 (EventType)
+                74 STORE_NAME              13 (EventType)
+                76 IMPORT_FROM             14 (Actor)
+                78 STORE_NAME              14 (Actor)
+                80 IMPORT_FROM             15 (Search)
+                82 STORE_NAME              15 (Search)
+                84 IMPORT_FROM             16 (Checkpoint)
+                86 STORE_NAME              16 (Checkpoint)
+                88 POP_TOP
+   
+    16          90 LOAD_CONST               0 (0)
+                92 LOAD_CONST               1 (None)
+                94 IMPORT_NAME             17 (sqlalchemy)
+                96 STORE_NAME              17 (sqlalchemy)
+   
+    18          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               6 (('Connector',))
+               102 IMPORT_NAME             18 (google.cloud.sql.connector)
+               104 IMPORT_FROM             19 (Connector)
+               106 STORE_NAME              19 (Connector)
+               108 POP_TOP
+   
+    19         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               7 (('load_dotenv',))
+               114 IMPORT_NAME             20 (dotenv)
+               116 IMPORT_FROM             21 (load_dotenv)
+               118 STORE_NAME              21 (load_dotenv)
+               120 POP_TOP
+   
+    21         122 PUSH_NULL
+               124 LOAD_NAME               21 (load_dotenv)
+               126 PRECALL                  0
+               130 CALL                     0
+               140 POP_TOP
+   
+    23         142 LOAD_CONST               0 (0)
+               144 LOAD_CONST               8 (('connect_with_connector',))
+               146 IMPORT_NAME             22 (gandai.db)
+               148 IMPORT_FROM             23 (connect_with_connector)
+               150 STORE_NAME              23 (connect_with_connector)
+               152 POP_TOP
+   
+    25         154 PUSH_NULL
+               156 LOAD_NAME               23 (connect_with_connector)
+               158 PRECALL                  0
+               162 CALL                     0
+               172 STORE_NAME              24 (db)
+   
+    31         174 LOAD_CONST               9 ('company')
+               176 LOAD_NAME               12 (Company)
+               178 BUILD_TUPLE              2
+               180 LOAD_CONST              10 (<code object insert_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 31>)
                182 MAKE_FUNCTION            4 (annotations)
-               184 STORE_NAME              23 (insert_event)
+               184 STORE_NAME              25 (insert_company)
    
-    65         186 LOAD_CONST              13 ('actor')
-               188 LOAD_NAME               11 (Actor)
-               190 LOAD_CONST              11 ('return')
-               192 LOAD_NAME               11 (Actor)
+    45         186 LOAD_CONST              11 ('event')
+               188 LOAD_NAME               11 (Event)
+               190 LOAD_CONST              12 ('return')
+               192 LOAD_NAME               11 (Event)
                194 BUILD_TUPLE              4
-               196 LOAD_CONST              14 (<code object insert_actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 65>)
+               196 LOAD_CONST              13 (<code object insert_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 45>)
                198 MAKE_FUNCTION            4 (annotations)
-               200 STORE_NAME              24 (insert_actor)
+               200 STORE_NAME              26 (insert_event)
    
-    80         202 LOAD_CONST              15 ('search')
-               204 LOAD_NAME               12 (Search)
-               206 LOAD_CONST              11 ('return')
-               208 LOAD_NAME               12 (Search)
+    66         202 LOAD_CONST              14 ('actor')
+               204 LOAD_NAME               14 (Actor)
+               206 LOAD_CONST              12 ('return')
+               208 LOAD_NAME               14 (Actor)
                210 BUILD_TUPLE              4
-               212 LOAD_CONST              16 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 80>)
+               212 LOAD_CONST              15 (<code object insert_actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 66>)
                214 MAKE_FUNCTION            4 (annotations)
-               216 STORE_NAME              25 (insert_search)
+               216 STORE_NAME              27 (insert_actor)
    
-    99         218 LOAD_CONST              17 ('checkpoint')
-               220 LOAD_NAME               13 (Checkpoint)
-               222 LOAD_CONST              11 ('return')
-               224 LOAD_NAME               13 (Checkpoint)
+    81         218 LOAD_CONST              16 ('search')
+               220 LOAD_NAME               15 (Search)
+               222 LOAD_CONST              12 ('return')
+               224 LOAD_NAME               15 (Search)
                226 BUILD_TUPLE              4
-               228 LOAD_CONST              18 (<code object insert_checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 99>)
+               228 LOAD_CONST              17 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 81>)
                230 MAKE_FUNCTION            4 (annotations)
-               232 STORE_NAME              26 (insert_checkpoint)
+               232 STORE_NAME              28 (insert_search)
    
-   115         234 LOAD_CONST              19 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 115>)
-               236 MAKE_FUNCTION            0
-               238 STORE_NAME              27 (search)
-   
-   124         240 LOAD_CONST              35 ((None,))
-               242 LOAD_CONST              20 ('search_uid')
-               244 LOAD_NAME               28 (int)
-               246 LOAD_CONST              21 ('last_event_type')
-               248 LOAD_NAME               29 (str)
-               250 BUILD_TUPLE              4
-               252 LOAD_CONST              22 (<code object target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 124>)
-               254 MAKE_FUNCTION            5 (defaults, annotations)
-               256 STORE_NAME              30 (target)
-   
-   155         258 LOAD_CONST              20 ('search_uid')
-               260 LOAD_NAME               28 (int)
-               262 LOAD_CONST              11 ('return')
-               264 LOAD_NAME                2 (pd)
-               266 LOAD_ATTR               31 (DataFrame)
-               276 BUILD_TUPLE              4
-               278 LOAD_CONST              23 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 155>)
-               280 MAKE_FUNCTION            4 (annotations)
-               282 STORE_NAME              32 (target_count)
-   
-   171         284 LOAD_CONST              20 ('search_uid')
-               286 LOAD_NAME               28 (int)
-               288 LOAD_CONST              11 ('return')
-               290 LOAD_NAME                2 (pd)
-               292 LOAD_ATTR               31 (DataFrame)
-               302 BUILD_TUPLE              4
-               304 LOAD_CONST              24 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 171>)
-               306 MAKE_FUNCTION            4 (annotations)
-               308 STORE_NAME              33 (event)
-   
-   183         310 LOAD_CONST              11 ('return')
-               312 LOAD_NAME                2 (pd)
-               314 LOAD_ATTR               31 (DataFrame)
-               324 BUILD_TUPLE              2
-               326 LOAD_CONST              25 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 183>)
-               328 MAKE_FUNCTION            4 (annotations)
-               330 STORE_NAME              34 (company)
-   
-   194         332 LOAD_CONST              20 ('search_uid')
-               334 LOAD_NAME               28 (int)
-               336 LOAD_CONST              11 ('return')
-               338 LOAD_NAME                2 (pd)
-               340 LOAD_ATTR               31 (DataFrame)
-               350 BUILD_TUPLE              4
-               352 LOAD_CONST              26 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 194>)
-               354 MAKE_FUNCTION            4 (annotations)
-               356 STORE_NAME              35 (checkpoint)
-   
-   207         358 LOAD_CONST              20 ('search_uid')
-               360 LOAD_NAME               28 (int)
-               362 LOAD_CONST              11 ('return')
-               364 LOAD_NAME                2 (pd)
-               366 LOAD_ATTR               31 (DataFrame)
-               376 BUILD_TUPLE              4
-               378 LOAD_CONST              27 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 207>)
-               380 MAKE_FUNCTION            4 (annotations)
-               382 STORE_NAME              36 (comment_by_domain)
-   
-   228         384 LOAD_CONST              20 ('search_uid')
-               386 LOAD_NAME               28 (int)
-               388 LOAD_CONST              11 ('return')
-               390 LOAD_NAME               12 (Search)
-               392 BUILD_TUPLE              4
-               394 LOAD_CONST              28 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 228>)
-               396 MAKE_FUNCTION            4 (annotations)
-               398 STORE_NAME              37 (find_search_by_uid)
-   
-   244         400 LOAD_CONST              29 ('domain')
-               402 LOAD_NAME               29 (str)
-               404 LOAD_CONST              11 ('return')
-               406 LOAD_NAME                9 (Company)
-               408 BUILD_TUPLE              4
-               410 LOAD_CONST              30 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 244>)
-               412 MAKE_FUNCTION            4 (annotations)
-               414 STORE_NAME              38 (find_company_by_domain)
-   
-   260         416 LOAD_CONST              31 ('event_id')
-               418 LOAD_NAME               28 (int)
-               420 LOAD_CONST              11 ('return')
-               422 LOAD_NAME                8 (Event)
-               424 BUILD_TUPLE              4
-               426 LOAD_CONST              32 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 260>)
-               428 MAKE_FUNCTION            4 (annotations)
-               430 STORE_NAME              39 (find_event_by_id)
-   
-   278         432 LOAD_CONST               8 ('company')
-               434 LOAD_NAME                9 (Company)
-               436 LOAD_CONST              11 ('return')
-               438 LOAD_CONST               1 (None)
-               440 BUILD_TUPLE              4
-               442 LOAD_CONST              33 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 278>)
-               444 MAKE_FUNCTION            4 (annotations)
-               446 STORE_NAME              40 (update_company)
-   
-   302         448 LOAD_CONST              15 ('search')
-               450 LOAD_NAME               12 (Search)
-               452 LOAD_CONST              11 ('return')
-               454 LOAD_CONST               1 (None)
-               456 BUILD_TUPLE              4
-               458 LOAD_CONST              34 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 302>)
-               460 MAKE_FUNCTION            4 (annotations)
-               462 STORE_NAME              41 (update_search)
-               464 LOAD_CONST               1 (None)
-               466 RETURN_VALUE
+   100         234 LOAD_CONST              18 ('checkpoint')
+               236 LOAD_NAME               16 (Checkpoint)
+               238 LOAD_CONST              12 ('return')
+               240 LOAD_NAME               16 (Checkpoint)
+               242 BUILD_TUPLE              4
+               244 LOAD_CONST              19 (<code object insert_checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 100>)
+               246 MAKE_FUNCTION            4 (annotations)
+               248 STORE_NAME              29 (insert_checkpoint)
+   
+   113         250 LOAD_CONST              20 ('domains')
+   
+   114         252 LOAD_NAME                4 (List)
+               254 LOAD_NAME               30 (str)
+               256 BINARY_SUBSCR
+   
+   113         266 LOAD_CONST              21 ('search_uid')
+   
+   114         268 LOAD_NAME               31 (int)
+   
+   113         270 LOAD_CONST              22 ('actor_key')
+   
+   114         272 LOAD_NAME               30 (str)
+   
+   113         274 LOAD_CONST              12 ('return')
+   
+   115         276 LOAD_CONST               1 (None)
+   
+   113         278 BUILD_TUPLE              8
+               280 LOAD_CONST              23 (<code object insert_and_advance_targets_from_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 113>)
+               282 MAKE_FUNCTION            4 (annotations)
+               284 STORE_NAME              32 (insert_and_advance_targets_from_domains)
+   
+   167         286 LOAD_CONST              24 ('companies')
+   
+   168         288 LOAD_NAME                4 (List)
+               290 LOAD_NAME                5 (Any)
+               292 BINARY_SUBSCR
+   
+   167         302 LOAD_CONST              21 ('search_uid')
+   
+   168         304 LOAD_NAME               31 (int)
+   
+   167         306 LOAD_CONST              22 ('actor_key')
+   
+   168         308 LOAD_NAME               30 (str)
+   
+   167         310 LOAD_CONST              12 ('return')
+   
+   169         312 LOAD_CONST               1 (None)
+   
+   167         314 BUILD_TUPLE              8
+               316 LOAD_CONST              25 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 167>)
+               318 MAKE_FUNCTION            4 (annotations)
+               320 STORE_NAME              33 (insert_companies_as_targets)
+   
+   221         322 LOAD_CONST              26 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 221>)
+               324 MAKE_FUNCTION            0
+               326 STORE_NAME              34 (search)
+   
+   230         328 LOAD_CONST              41 ((None,))
+               330 LOAD_CONST              21 ('search_uid')
+               332 LOAD_NAME               31 (int)
+               334 LOAD_CONST              27 ('last_event_type')
+               336 LOAD_NAME               30 (str)
+               338 BUILD_TUPLE              4
+               340 LOAD_CONST              28 (<code object target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 230>)
+               342 MAKE_FUNCTION            5 (defaults, annotations)
+               344 STORE_NAME              35 (target)
+   
+   261         346 LOAD_CONST              21 ('search_uid')
+               348 LOAD_NAME               31 (int)
+               350 LOAD_CONST              12 ('return')
+               352 LOAD_NAME                2 (pd)
+               354 LOAD_ATTR               36 (DataFrame)
+               364 BUILD_TUPLE              4
+               366 LOAD_CONST              29 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 261>)
+               368 MAKE_FUNCTION            4 (annotations)
+               370 STORE_NAME              37 (target_count)
+   
+   277         372 LOAD_CONST              21 ('search_uid')
+               374 LOAD_NAME               31 (int)
+               376 LOAD_CONST              12 ('return')
+               378 LOAD_NAME                2 (pd)
+               380 LOAD_ATTR               36 (DataFrame)
+               390 BUILD_TUPLE              4
+               392 LOAD_CONST              30 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 277>)
+               394 MAKE_FUNCTION            4 (annotations)
+               396 STORE_NAME              38 (event)
+   
+   289         398 LOAD_CONST              12 ('return')
+               400 LOAD_NAME                2 (pd)
+               402 LOAD_ATTR               36 (DataFrame)
+               412 BUILD_TUPLE              2
+               414 LOAD_CONST              31 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 289>)
+               416 MAKE_FUNCTION            4 (annotations)
+               418 STORE_NAME              39 (company)
+   
+   300         420 LOAD_CONST              21 ('search_uid')
+               422 LOAD_NAME               31 (int)
+               424 LOAD_CONST              12 ('return')
+               426 LOAD_NAME                2 (pd)
+               428 LOAD_ATTR               36 (DataFrame)
+               438 BUILD_TUPLE              4
+               440 LOAD_CONST              32 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 300>)
+               442 MAKE_FUNCTION            4 (annotations)
+               444 STORE_NAME              40 (checkpoint)
+   
+   313         446 LOAD_CONST              21 ('search_uid')
+               448 LOAD_NAME               31 (int)
+               450 LOAD_CONST              12 ('return')
+               452 LOAD_NAME                2 (pd)
+               454 LOAD_ATTR               36 (DataFrame)
+               464 BUILD_TUPLE              4
+               466 LOAD_CONST              33 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 313>)
+               468 MAKE_FUNCTION            4 (annotations)
+               470 STORE_NAME              41 (comment_by_domain)
+   
+   334         472 LOAD_CONST              21 ('search_uid')
+               474 LOAD_NAME               31 (int)
+               476 LOAD_CONST              12 ('return')
+               478 LOAD_NAME               15 (Search)
+               480 BUILD_TUPLE              4
+               482 LOAD_CONST              34 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 334>)
+               484 MAKE_FUNCTION            4 (annotations)
+               486 STORE_NAME              42 (find_search_by_uid)
+   
+   350         488 LOAD_CONST              35 ('domain')
+               490 LOAD_NAME               30 (str)
+               492 LOAD_CONST              12 ('return')
+               494 LOAD_NAME               12 (Company)
+               496 BUILD_TUPLE              4
+               498 LOAD_CONST              36 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 350>)
+               500 MAKE_FUNCTION            4 (annotations)
+               502 STORE_NAME              43 (find_company_by_domain)
+   
+   366         504 LOAD_CONST              37 ('event_id')
+               506 LOAD_NAME               31 (int)
+               508 LOAD_CONST              12 ('return')
+               510 LOAD_NAME               11 (Event)
+               512 BUILD_TUPLE              4
+               514 LOAD_CONST              38 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 366>)
+               516 MAKE_FUNCTION            4 (annotations)
+               518 STORE_NAME              44 (find_event_by_id)
+   
+   385         520 LOAD_CONST               9 ('company')
+               522 LOAD_NAME               12 (Company)
+               524 LOAD_CONST              12 ('return')
+               526 LOAD_CONST               1 (None)
+               528 BUILD_TUPLE              4
+               530 LOAD_CONST              39 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 385>)
+               532 MAKE_FUNCTION            4 (annotations)
+               534 STORE_NAME              45 (update_company)
+   
+   409         536 LOAD_CONST              16 ('search')
+               538 LOAD_NAME               15 (Search)
+               540 LOAD_CONST              12 ('return')
+               542 LOAD_CONST               1 (None)
+               544 BUILD_TUPLE              4
+               546 LOAD_CONST              40 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 409>)
+               548 MAKE_FUNCTION            4 (annotations)
+               550 STORE_NAME              46 (update_search)
+               552 LOAD_CONST               1 (None)
+               554 RETURN_VALUE
    consts
       0
       None
+      ('List', 'Any')
       ('asdict',)
       ('from_dict',)
       ('Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint')
       ('Connector',)
       ('load_dotenv',)
       ('connect_with_connector',)
       'company'
@@ -276,50 +335,50 @@
             000000000000006a0300000000000000006401a6010000ab010000000000
             0000007d027c01a00400000000000000000000000000000000000000007c
             02740b000000000000000000007c00a6010000ab010000000000000000a6
             020000ab02000000000000000001007c01a0060000000000000000000000
             000000000000000000a6000000ab00000000000000000001006400640064
             00a6020000ab02000000000000000001006e0b2300310073047702780359
             00770101005900010001007c005300
-          30           0 RESUME                   0
+          31           0 RESUME                   0
          
-          31           2 LOAD_GLOBAL              0 (db)
+          32           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          32          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+          33          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                       66 LOAD_ATTR                3 (text)
          
-          33          76 LOAD_CONST               1 ('\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            ')
+          34          76 LOAD_CONST               1 ('\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            ')
          
-          32          78 PRECALL                  1
+          33          78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (statement)
          
-          39          94 LOAD_FAST                1 (con)
+          40          94 LOAD_FAST                1 (con)
                       96 LOAD_METHOD              4 (execute)
                      118 LOAD_FAST                2 (statement)
                      120 LOAD_GLOBAL             11 (NULL + asdict)
                      132 LOAD_FAST                0 (company)
                      134 PRECALL                  1
                      138 CALL                     1
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
          
-          40         164 LOAD_FAST                1 (con)
+          41         164 LOAD_FAST                1 (con)
                      166 LOAD_METHOD              6 (commit)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 POP_TOP
          
-          31         204 LOAD_CONST               0 (None)
+          32         204 LOAD_CONST               0 (None)
                      206 LOAD_CONST               0 (None)
                      208 LOAD_CONST               0 (None)
                      210 PRECALL                  2
                      214 CALL                     2
                      224 POP_TOP
                      226 JUMP_FORWARD            11 (to 250)
                  >>  228 PUSH_EXC_INFO
@@ -330,30 +389,30 @@
                      238 POP_EXCEPT
                      240 RERAISE                  1
                  >>  242 POP_TOP
                      244 POP_EXCEPT
                      246 POP_TOP
                      248 POP_TOP
          
-          41     >>  250 LOAD_FAST                0 (company)
+          42     >>  250 LOAD_FAST                0 (company)
                      252 RETURN_VALUE
          ExceptionTable:
            52 to 202 -> 228 [1] lasti
            228 to 234 -> 236 [3] lasti
            242 to 242 -> 236 [3] lasti
          consts
             None
             '\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            '
          names      ('db', 'connect', 'sqlalchemy', 'text', 'execute', 'asdict', 'commit')
          varnames   ('company', 'con', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_company'
-         firstlineno 30
+         firstlineno 31
          lnotab 0x02013401160102ff1007460128f72e0a
       'event'
       'return'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 6
@@ -371,91 +430,91 @@
             087c056403190000000000000000006e0164007c005f0900000000000000
             007c01a00700000000000000000000000000000000000000007405000000
             000000000000006a0300000000000000006404a6010000ab010000000000
             000000a6010000ab01000000000000000001007c01a00a00000000000000
             00000000000000000000000000a6000000ab000000000000000000010064
             0064006400a6020000ab02000000000000000001006e0b23003100730477
             0278035900770101005900010001007c005300
-          44           0 RESUME                   0
+          45           0 RESUME                   0
          
-          45           2 LOAD_GLOBAL              0 (db)
+          46           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          46          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+          47          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                       66 LOAD_ATTR                3 (text)
          
-          47          76 LOAD_CONST               1 ('\n                INSERT INTO event (search_uid, domain, actor_key, type, data) \n                VALUES(:search_uid, :domain, :actor_key, :type, :data)\n                ON CONFLICT DO NOTHING\n                RETURNING id\n            ')
+          48          76 LOAD_CONST               1 ('\n                INSERT INTO event (search_uid, domain, actor_key, type, data) \n                VALUES(:search_uid, :domain, :actor_key, :type, :data)\n                ON CONFLICT DO NOTHING\n                RETURNING id\n            ')
          
-          46          78 PRECALL                  1
+          47          78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (statement)
          
-          54          94 LOAD_GLOBAL              9 (NULL + asdict)
+          55          94 LOAD_GLOBAL              9 (NULL + asdict)
                      106 LOAD_FAST                0 (event)
                      108 PRECALL                  1
                      112 CALL                     1
                      122 STORE_FAST               3 (obj)
          
-          55         124 LOAD_GLOBAL             11 (NULL + json)
+          56         124 LOAD_GLOBAL             11 (NULL + json)
                      136 LOAD_ATTR                6 (dumps)
                      146 LOAD_FAST                3 (obj)
                      148 LOAD_CONST               2 ('data')
                      150 BINARY_SUBSCR
                      160 PRECALL                  1
                      164 CALL                     1
                      174 LOAD_FAST                3 (obj)
                      176 LOAD_CONST               2 ('data')
                      178 STORE_SUBSCR
          
-          56         182 LOAD_FAST                1 (con)
+          57         182 LOAD_FAST                1 (con)
                      184 LOAD_METHOD              7 (execute)
                      206 LOAD_FAST                2 (statement)
                      208 LOAD_FAST                3 (obj)
                      210 PRECALL                  2
                      214 CALL                     2
                      224 STORE_FAST               4 (result)
          
-          58         226 LOAD_FAST                4 (result)
+          59         226 LOAD_FAST                4 (result)
                      228 LOAD_METHOD              8 (first)
                      250 PRECALL                  0
                      254 CALL                     0
                      264 STORE_FAST               5 (_id)
          
-          59         266 LOAD_FAST                5 (_id)
+          60         266 LOAD_FAST                5 (_id)
                      268 POP_JUMP_FORWARD_IF_FALSE     8 (to 286)
                      270 LOAD_FAST                5 (_id)
                      272 LOAD_CONST               3 (0)
                      274 BINARY_SUBSCR
                      284 JUMP_FORWARD             1 (to 288)
                  >>  286 LOAD_CONST               0 (None)
                  >>  288 LOAD_FAST                0 (event)
                      290 STORE_ATTR               9 (id)
          
-          60         300 LOAD_FAST                1 (con)
+          61         300 LOAD_FAST                1 (con)
                      302 LOAD_METHOD              7 (execute)
                      324 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                      336 LOAD_ATTR                3 (text)
                      346 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW target')
                      348 PRECALL                  1
                      352 CALL                     1
                      362 PRECALL                  1
                      366 CALL                     1
                      376 POP_TOP
          
-          61         378 LOAD_FAST                1 (con)
+          62         378 LOAD_FAST                1 (con)
                      380 LOAD_METHOD             10 (commit)
                      402 PRECALL                  0
                      406 CALL                     0
                      416 POP_TOP
          
-          45         418 LOAD_CONST               0 (None)
+          46         418 LOAD_CONST               0 (None)
                      420 LOAD_CONST               0 (None)
                      422 LOAD_CONST               0 (None)
                      424 PRECALL                  2
                      428 CALL                     2
                      438 POP_TOP
                      440 JUMP_FORWARD            11 (to 464)
                  >>  442 PUSH_EXC_INFO
@@ -466,15 +525,15 @@
                      452 POP_EXCEPT
                      454 RERAISE                  1
                  >>  456 POP_TOP
                      458 POP_EXCEPT
                      460 POP_TOP
                      462 POP_TOP
          
-          62     >>  464 LOAD_FAST                0 (event)
+          63     >>  464 LOAD_FAST                0 (event)
                      466 RETURN_VALUE
          ExceptionTable:
            52 to 416 -> 442 [1] lasti
            442 to 448 -> 450 [3] lasti
            456 to 456 -> 450 [3] lasti
          consts
             None
@@ -484,15 +543,15 @@
             'REFRESH MATERIALIZED VIEW target'
          names      ('db', 'connect', 'sqlalchemy', 'text', 'asdict', 'json', 'dumps', 'execute', 'first', 'id', 'commit')
          varnames   ('event', 'con', 'statement', 'obj', 'result', '_id')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_event'
-         firstlineno 44
+         firstlineno 45
          lnotab 0x02013401160102ff10081e013a012c02280122014e0128f02e11
       'actor'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
@@ -502,53 +561,53 @@
             000000000000006a0300000000000000006401a6010000ab010000000000
             0000007d027409000000000000000000007c00a6010000ab010000000000
             0000007d037c01a00500000000000000000000000000000000000000007c
             027c03a6020000ab02000000000000000001007c01a00600000000000000
             00000000000000000000000000a6000000ab000000000000000000010064
             0064006400a6020000ab02000000000000000001006e0b23003100730477
             0278035900770101005900010001007c005300
-          65           0 RESUME                   0
+          66           0 RESUME                   0
          
-          66           2 LOAD_GLOBAL              0 (db)
+          67           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          67          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+          68          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                       66 LOAD_ATTR                3 (text)
          
-          68          76 LOAD_CONST               1 ('\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            ')
+          69          76 LOAD_CONST               1 ('\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            ')
          
-          67          78 PRECALL                  1
+          68          78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (statement)
          
-          74          94 LOAD_GLOBAL              9 (NULL + asdict)
+          75          94 LOAD_GLOBAL              9 (NULL + asdict)
                      106 LOAD_FAST                0 (actor)
                      108 PRECALL                  1
                      112 CALL                     1
                      122 STORE_FAST               3 (obj)
          
-          75         124 LOAD_FAST                1 (con)
+          76         124 LOAD_FAST                1 (con)
                      126 LOAD_METHOD              5 (execute)
                      148 LOAD_FAST                2 (statement)
                      150 LOAD_FAST                3 (obj)
                      152 PRECALL                  2
                      156 CALL                     2
                      166 POP_TOP
          
-          76         168 LOAD_FAST                1 (con)
+          77         168 LOAD_FAST                1 (con)
                      170 LOAD_METHOD              6 (commit)
                      192 PRECALL                  0
                      196 CALL                     0
                      206 POP_TOP
          
-          66         208 LOAD_CONST               0 (None)
+          67         208 LOAD_CONST               0 (None)
                      210 LOAD_CONST               0 (None)
                      212 LOAD_CONST               0 (None)
                      214 PRECALL                  2
                      218 CALL                     2
                      228 POP_TOP
                      230 JUMP_FORWARD            11 (to 254)
                  >>  232 PUSH_EXC_INFO
@@ -559,30 +618,30 @@
                      242 POP_EXCEPT
                      244 RERAISE                  1
                  >>  246 POP_TOP
                      248 POP_EXCEPT
                      250 POP_TOP
                      252 POP_TOP
          
-          77     >>  254 LOAD_FAST                0 (actor)
+          78     >>  254 LOAD_FAST                0 (actor)
                      256 RETURN_VALUE
          ExceptionTable:
            52 to 206 -> 232 [1] lasti
            232 to 238 -> 240 [3] lasti
            246 to 246 -> 240 [3] lasti
          consts
             None
             '\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            '
          names      ('db', 'connect', 'sqlalchemy', 'text', 'asdict', 'execute', 'commit')
          varnames   ('actor', 'con', 'statement', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_actor'
-         firstlineno 65
+         firstlineno 66
          lnotab 0x02013401160102ff10071e012c0128f62e0b
       'search'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
@@ -600,97 +659,97 @@
             0b000000000000000000006a0600000000000000007c0364051900000000
             0000000000a6010000ab0100000000000000007c0364053c0000007c01a0
             0700000000000000000000000000000000000000007c027c03a6020000ab
             02000000000000000001007c01a008000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006e0b230031007304770278035900770101
             005900010001007c005300
-          80           0 RESUME                   0
+          81           0 RESUME                   0
          
-          81           2 LOAD_GLOBAL              0 (db)
+          82           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          82          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+          83          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                       66 LOAD_ATTR                3 (text)
          
-          83          76 LOAD_CONST               1 ('\n                INSERT INTO search (uid, client_domain, label, meta, inclusion, exclusion, sort) \n                VALUES(:uid, :client_domain, :label, :meta, :inclusion, :exclusion, :sort)\n                ON CONFLICT DO NOTHING\n            ')
+          84          76 LOAD_CONST               1 ('\n                INSERT INTO search (uid, client_domain, label, meta, inclusion, exclusion, sort) \n                VALUES(:uid, :client_domain, :label, :meta, :inclusion, :exclusion, :sort)\n                ON CONFLICT DO NOTHING\n            ')
          
-          82          78 PRECALL                  1
+          83          78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (statement)
          
-          89          94 LOAD_GLOBAL              9 (NULL + asdict)
+          90          94 LOAD_GLOBAL              9 (NULL + asdict)
                      106 LOAD_FAST                0 (search)
                      108 PRECALL                  1
                      112 CALL                     1
                      122 STORE_FAST               3 (obj)
          
-          90         124 LOAD_GLOBAL             11 (NULL + json)
+          91         124 LOAD_GLOBAL             11 (NULL + json)
                      136 LOAD_ATTR                6 (dumps)
                      146 LOAD_FAST                3 (obj)
                      148 LOAD_CONST               2 ('meta')
                      150 BINARY_SUBSCR
                      160 PRECALL                  1
                      164 CALL                     1
                      174 LOAD_FAST                3 (obj)
                      176 LOAD_CONST               2 ('meta')
                      178 STORE_SUBSCR
          
-          91         182 LOAD_GLOBAL             11 (NULL + json)
+          92         182 LOAD_GLOBAL             11 (NULL + json)
                      194 LOAD_ATTR                6 (dumps)
                      204 LOAD_FAST                3 (obj)
                      206 LOAD_CONST               3 ('inclusion')
                      208 BINARY_SUBSCR
                      218 PRECALL                  1
                      222 CALL                     1
                      232 LOAD_FAST                3 (obj)
                      234 LOAD_CONST               3 ('inclusion')
                      236 STORE_SUBSCR
          
-          92         240 LOAD_GLOBAL             11 (NULL + json)
+          93         240 LOAD_GLOBAL             11 (NULL + json)
                      252 LOAD_ATTR                6 (dumps)
                      262 LOAD_FAST                3 (obj)
                      264 LOAD_CONST               4 ('exclusion')
                      266 BINARY_SUBSCR
                      276 PRECALL                  1
                      280 CALL                     1
                      290 LOAD_FAST                3 (obj)
                      292 LOAD_CONST               4 ('exclusion')
                      294 STORE_SUBSCR
          
-          93         298 LOAD_GLOBAL             11 (NULL + json)
+          94         298 LOAD_GLOBAL             11 (NULL + json)
                      310 LOAD_ATTR                6 (dumps)
                      320 LOAD_FAST                3 (obj)
                      322 LOAD_CONST               5 ('sort')
                      324 BINARY_SUBSCR
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_FAST                3 (obj)
                      350 LOAD_CONST               5 ('sort')
                      352 STORE_SUBSCR
          
-          94         356 LOAD_FAST                1 (con)
+          95         356 LOAD_FAST                1 (con)
                      358 LOAD_METHOD              7 (execute)
                      380 LOAD_FAST                2 (statement)
                      382 LOAD_FAST                3 (obj)
                      384 PRECALL                  2
                      388 CALL                     2
                      398 POP_TOP
          
-          95         400 LOAD_FAST                1 (con)
+          96         400 LOAD_FAST                1 (con)
                      402 LOAD_METHOD              8 (commit)
                      424 PRECALL                  0
                      428 CALL                     0
                      438 POP_TOP
          
-          81         440 LOAD_CONST               0 (None)
+          82         440 LOAD_CONST               0 (None)
                      442 LOAD_CONST               0 (None)
                      444 LOAD_CONST               0 (None)
                      446 PRECALL                  2
                      450 CALL                     2
                      460 POP_TOP
                      462 JUMP_FORWARD            11 (to 486)
                  >>  464 PUSH_EXC_INFO
@@ -701,15 +760,15 @@
                      474 POP_EXCEPT
                      476 RERAISE                  1
                  >>  478 POP_TOP
                      480 POP_EXCEPT
                      482 POP_TOP
                      484 POP_TOP
          
-          96     >>  486 LOAD_FAST                0 (search)
+          97     >>  486 LOAD_FAST                0 (search)
                      488 RETURN_VALUE
          ExceptionTable:
            52 to 438 -> 464 [1] lasti
            464 to 470 -> 472 [3] lasti
            478 to 478 -> 472 [3] lasti
          consts
             None
@@ -720,15 +779,15 @@
             'sort'
          names      ('db', 'connect', 'sqlalchemy', 'text', 'asdict', 'json', 'dumps', 'execute', 'commit')
          varnames   ('search', 'con', 'statement', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_search'
-         firstlineno 80
+         firstlineno 81
          lnotab 0x02013401160102ff10071e013a013a013a013a012c0128f22e0f
       'checkpoint'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
          flags     : 3
@@ -738,50 +797,50 @@
             000000000000006a0300000000000000006401a6010000ab010000000000
             0000007d027c01a00400000000000000000000000000000000000000007c
             02740b000000000000000000007c00a6010000ab010000000000000000a6
             020000ab02000000000000000001007c01a0060000000000000000000000
             000000000000000000a6000000ab00000000000000000001006400640064
             00a6020000ab02000000000000000001006e0b2300310073047702780359
             00770101005900010001007c005300
-          99           0 RESUME                   0
+         100           0 RESUME                   0
          
-         100           2 LOAD_GLOBAL              0 (db)
+         101           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-         101          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+         102          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                       66 LOAD_ATTR                3 (text)
          
-         102          76 LOAD_CONST               1 ('\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            ')
+         103          76 LOAD_CONST               1 ('\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            ')
          
-         101          78 PRECALL                  1
+         102          78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (statement)
          
-         107          94 LOAD_FAST                1 (con)
+         108          94 LOAD_FAST                1 (con)
                       96 LOAD_METHOD              4 (execute)
                      118 LOAD_FAST                2 (statement)
                      120 LOAD_GLOBAL             11 (NULL + asdict)
                      132 LOAD_FAST                0 (checkpoint)
                      134 PRECALL                  1
                      138 CALL                     1
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
          
-         108         164 LOAD_FAST                1 (con)
+         109         164 LOAD_FAST                1 (con)
                      166 LOAD_METHOD              6 (commit)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 POP_TOP
          
-         100         204 LOAD_CONST               0 (None)
+         101         204 LOAD_CONST               0 (None)
                      206 LOAD_CONST               0 (None)
                      208 LOAD_CONST               0 (None)
                      210 PRECALL                  2
                      214 CALL                     2
                      224 POP_TOP
                      226 JUMP_FORWARD            11 (to 250)
                  >>  228 PUSH_EXC_INFO
@@ -792,31 +851,529 @@
                      238 POP_EXCEPT
                      240 RERAISE                  1
                  >>  242 POP_TOP
                      244 POP_EXCEPT
                      246 POP_TOP
                      248 POP_TOP
          
-         109     >>  250 LOAD_FAST                0 (checkpoint)
+         110     >>  250 LOAD_FAST                0 (checkpoint)
                      252 RETURN_VALUE
          ExceptionTable:
            52 to 202 -> 228 [1] lasti
            228 to 234 -> 236 [3] lasti
            242 to 242 -> 236 [3] lasti
          consts
             None
             '\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            '
          names      ('db', 'connect', 'sqlalchemy', 'text', 'execute', 'asdict', 'commit')
          varnames   ('checkpoint', 'con', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_checkpoint'
-         firstlineno 99
+         firstlineno 100
          lnotab 0x02013401160102ff1006460128f82e09
+      'domains'
+      'search_uid'
+      'actor_key'
+      code
+         argcount  : 3
+         nlocals   : 6
+         stacksize : 10
+         flags     : 3
+         code
+            0x97007401000000000000000000007c01ac01a6010000ab010000000000
+            0000007d03740200000000000000000000a0020000000000000000000000
+            000000000000000000a6000000ab00000000000000000035007d047c0044
+            0090015d157d057c05a00300000000000000000000000000000000000000
+            00a6000000ab000000000000000000a00400000000000000000000000000
+            00000000000000a6000000ab000000000000000000a00500000000000000
+            0000000000000000000000000064026403a6020000ab0200000000000000
+            00a005000000000000000000000000000000000000000064046403a60200
+            00ab020000000000000000a0050000000000000000000000000000000000
+            00000064046403a6020000ab0200000000000000007d057c036405190000
+            000000000000006a060000000000000000a0070000000000000000000000
+            0000000000000000007c05a6010000ab010000000000000000a008000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            00721474130000000000000000000064067c059b0064079d03a6010000ab
+            01000000000000000001008cab74130000000000000000000064087c059b
+            0064099d03a6010000ab01000000000000000001007c04a00a0000000000
+            0000000000000000000000000000007417000000000000000000006a0c00
+            00000000000000640aa6010000ab01000000000000000064057c056901a6
+            020000ab02000000000000000001007c04a00a0000000000000000000000
+            0000000000000000007417000000000000000000006a0c00000000000000
+            00640ba6010000ab0100000000000000007c017c027c05640c640d9c04a6
+            020000ab020000000000000000010090018c177c04a00a00000000000000
+            000000000000000000000000007417000000000000000000006a0c000000
+            0000000000640ea6010000ab010000000000000000a6010000ab01000000
+            000000000001007c04a00d00000000000000000000000000000000000000
+            00a6000000ab0000000000000000000100640f640f640fa6020000ab0200
+            000000000000000100640f53002300310073047702780359007701010059
+            0001000100640f5300
+         113           0 RESUME                   0
+         
+         121           2 LOAD_GLOBAL              1 (NULL + target)
+                      14 LOAD_FAST                1 (search_uid)
+                      16 KW_NAMES                 1
+                      18 PRECALL                  1
+                      22 CALL                     1
+                      32 STORE_FAST               3 (targets)
+         
+         122          34 LOAD_GLOBAL              2 (db)
+                      46 LOAD_METHOD              2 (connect)
+                      68 PRECALL                  0
+                      72 CALL                     0
+                      82 BEFORE_WITH
+                      84 STORE_FAST               4 (con)
+         
+         123          86 LOAD_FAST                0 (domains)
+                      88 GET_ITER
+                 >>   90 EXTENDED_ARG             1
+                      92 FOR_ITER               277 (to 648)
+                      94 STORE_FAST               5 (domain)
+         
+         126          96 LOAD_FAST                5 (domain)
+                      98 LOAD_METHOD              3 (lower)
+                     120 PRECALL                  0
+                     124 CALL                     0
+         
+         127         134 LOAD_METHOD              4 (strip)
+                     156 PRECALL                  0
+                     160 CALL                     0
+         
+         128         170 LOAD_METHOD              5 (replace)
+                     192 LOAD_CONST               2 ('www.')
+                     194 LOAD_CONST               3 ('')
+                     196 PRECALL                  2
+                     200 CALL                     2
+         
+         129         210 LOAD_METHOD              5 (replace)
+                     232 LOAD_CONST               4 ('https://')
+                     234 LOAD_CONST               3 ('')
+                     236 PRECALL                  2
+                     240 CALL                     2
+         
+         130         250 LOAD_METHOD              5 (replace)
+                     272 LOAD_CONST               4 ('https://')
+                     274 LOAD_CONST               3 ('')
+                     276 PRECALL                  2
+                     280 CALL                     2
+         
+         125         290 STORE_FAST               5 (domain)
+         
+         132         292 LOAD_FAST                3 (targets)
+                     294 LOAD_CONST               5 ('domain')
+                     296 BINARY_SUBSCR
+                     306 LOAD_ATTR                6 (str)
+                     316 LOAD_METHOD              7 (contains)
+                     338 LOAD_FAST                5 (domain)
+                     340 PRECALL                  1
+                     344 CALL                     1
+                     354 LOAD_METHOD              8 (any)
+                     376 PRECALL                  0
+                     380 CALL                     0
+                     390 POP_JUMP_FORWARD_IF_FALSE    20 (to 432)
+         
+         133         392 LOAD_GLOBAL             19 (NULL + print)
+                     404 LOAD_CONST               6 ('Skipping ')
+                     406 LOAD_FAST                5 (domain)
+                     408 FORMAT_VALUE             0
+                     410 LOAD_CONST               7 (' as already a target')
+                     412 BUILD_STRING             3
+                     414 PRECALL                  1
+                     418 CALL                     1
+                     428 POP_TOP
+         
+         134         430 JUMP_BACKWARD          171 (to 90)
+         
+         136     >>  432 LOAD_GLOBAL             19 (NULL + print)
+                     444 LOAD_CONST               8 ('Adding ')
+                     446 LOAD_FAST                5 (domain)
+                     448 FORMAT_VALUE             0
+                     450 LOAD_CONST               9 (' as target')
+                     452 BUILD_STRING             3
+                     454 PRECALL                  1
+                     458 CALL                     1
+                     468 POP_TOP
+         
+         138         470 LOAD_FAST                4 (con)
+                     472 LOAD_METHOD             10 (execute)
+         
+         139         494 LOAD_GLOBAL             23 (NULL + sqlalchemy)
+                     506 LOAD_ATTR               12 (text)
+         
+         140         516 LOAD_CONST              10 ('\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    ')
+         
+         139         518 PRECALL                  1
+                     522 CALL                     1
+         
+         146         532 LOAD_CONST               5 ('domain')
+                     534 LOAD_FAST                5 (domain)
+                     536 BUILD_MAP                1
+         
+         138         538 PRECALL                  2
+                     542 CALL                     2
+                     552 POP_TOP
+         
+         149         554 LOAD_FAST                4 (con)
+                     556 LOAD_METHOD             10 (execute)
+         
+         150         578 LOAD_GLOBAL             23 (NULL + sqlalchemy)
+                     590 LOAD_ATTR               12 (text)
+         
+         151         600 LOAD_CONST              11 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ')
+         
+         150         602 PRECALL                  1
+                     606 CALL                     1
+         
+         157         616 LOAD_FAST                1 (search_uid)
+         
+         158         618 LOAD_FAST                2 (actor_key)
+         
+         159         620 LOAD_FAST                5 (domain)
+         
+         160         622 LOAD_CONST              12 ('advance')
+         
+         156         624 LOAD_CONST              13 (('search_uid', 'actor_key', 'domain', 'type'))
+                     626 BUILD_CONST_KEY_MAP      4
+         
+         149         628 PRECALL                  2
+                     632 CALL                     2
+                     642 POP_TOP
+                     644 EXTENDED_ARG             1
+                     646 JUMP_BACKWARD          279 (to 90)
+         
+         163     >>  648 LOAD_FAST                4 (con)
+                     650 LOAD_METHOD             10 (execute)
+                     672 LOAD_GLOBAL             23 (NULL + sqlalchemy)
+                     684 LOAD_ATTR               12 (text)
+                     694 LOAD_CONST              14 ('REFRESH MATERIALIZED VIEW target')
+                     696 PRECALL                  1
+                     700 CALL                     1
+                     710 PRECALL                  1
+                     714 CALL                     1
+                     724 POP_TOP
+         
+         164         726 LOAD_FAST                4 (con)
+                     728 LOAD_METHOD             13 (commit)
+                     750 PRECALL                  0
+                     754 CALL                     0
+                     764 POP_TOP
+         
+         122         766 LOAD_CONST              15 (None)
+                     768 LOAD_CONST              15 (None)
+                     770 LOAD_CONST              15 (None)
+                     772 PRECALL                  2
+                     776 CALL                     2
+                     786 POP_TOP
+                     788 LOAD_CONST              15 (None)
+                     790 RETURN_VALUE
+                 >>  792 PUSH_EXC_INFO
+                     794 WITH_EXCEPT_START
+                     796 POP_JUMP_FORWARD_IF_TRUE     4 (to 806)
+                     798 RERAISE                  2
+                 >>  800 COPY                     3
+                     802 POP_EXCEPT
+                     804 RERAISE                  1
+                 >>  806 POP_TOP
+                     808 POP_EXCEPT
+                     810 POP_TOP
+                     812 POP_TOP
+                     814 LOAD_CONST              15 (None)
+                     816 RETURN_VALUE
+         ExceptionTable:
+           84 to 764 -> 792 [1] lasti
+           792 to 798 -> 800 [3] lasti
+           806 to 806 -> 800 [3] lasti
+         consts
+            '\n    Takes in domains, inserts targets into a review stage, where they will\n    try to be enriched on process event\n\n    '
+            ('search_uid',)
+            'www.'
+            ''
+            'https://'
+            'domain'
+            'Skipping '
+            ' as already a target'
+            'Adding '
+            ' as target'
+            '\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    '
+            '\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    '
+            'advance'
+            ('search_uid', 'actor_key', 'domain', 'type')
+            'REFRESH MATERIALIZED VIEW target'
+            None
+         names      ('target', 'db', 'connect', 'lower', 'strip', 'replace', 'str', 'contains', 'any', 'print', 'execute', 'sqlalchemy', 'text', 'commit')
+         varnames   ('domains', 'search_uid', 'actor_key', 'targets', 'con', 'domain')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+         name       'insert_and_advance_targets_from_domains'
+         firstlineno 113
+         lnotab
+            0x0208200134010a03260124012801280128fb0207640126010202260218
+            01160102ff0e0706f8100b1801160102ff0e0702010201020102fc04f914
+            0e4e0128d6
+      'companies'
+      code
+         argcount  : 3
+         nlocals   : 6
+         stacksize : 10
+         flags     : 3
+         code
+            0x97007401000000000000000000007c01ac01a6010000ab010000000000
+            0000007d03740200000000000000000000a0020000000000000000000000
+            000000000000000000a6000000ab00000000000000000035007d047c0044
+            0090015d3c7d057c05a00300000000000000000000000000000000000000
+            006402a6010000ab01000000000000000080147409000000000000000000
+            0064037c059b0064049d03a6010000ab01000000000000000001008c2c7c
+            036402190000000000000000006a050000000000000000a0060000000000
+            0000000000000000000000000000007c05640219000000000000000000a6
+            010000ab010000000000000000a007000000000000000000000000000000
+            0000000000a6000000ab000000000000000000721a740900000000000000
+            00000064057c056402190000000000000000009b0064069d03a6010000ab
+            01000000000000000001008c7e74090000000000000000000064077c0564
+            02190000000000000000009b0064089d03a6010000ab0100000000000000
+            0001007c04a0080000000000000000000000000000000000000000741300
+            0000000000000000006a0a00000000000000006409a6010000ab01000000
+            00000000007c05a003000000000000000000000000000000000000000064
+            02a6010000ab0100000000000000007c05a0030000000000000000000000
+            000000000000000000640aa6010000ab0100000000000000007c05a00300
+            00000000000000000000000000000000000000640ba6010000ab01000000
+            0000000000640c9c03a6020000ab02000000000000000001007c04a00800
+            000000000000000000000000000000000000007413000000000000000000
+            006a0a0000000000000000640da6010000ab0100000000000000007c017c
+            027c05a00300000000000000000000000000000000000000006402a60100
+            00ab010000000000000000640e640f9c04a6020000ab0200000000000000
+            00010090018c3e7c04a00800000000000000000000000000000000000000
+            007413000000000000000000006a0a00000000000000006410a6010000ab
+            010000000000000000a6010000ab01000000000000000001007c04a00b00
+            00000000000000000000000000000000000000a6000000ab000000000000
+            0000000100640064006400a6020000ab0200000000000000000100640053
+            002300310073047702780359007701010059000100010064005300
+         167           0 RESUME                   0
+         
+         170           2 LOAD_GLOBAL              1 (NULL + target)
+                      14 LOAD_FAST                1 (search_uid)
+                      16 KW_NAMES                 1
+                      18 PRECALL                  1
+                      22 CALL                     1
+                      32 STORE_FAST               3 (targets)
+         
+         171          34 LOAD_GLOBAL              2 (db)
+                      46 LOAD_METHOD              2 (connect)
+                      68 PRECALL                  0
+                      72 CALL                     0
+                      82 BEFORE_WITH
+                      84 STORE_FAST               4 (con)
+         
+         172          86 LOAD_FAST                0 (companies)
+                      88 GET_ITER
+                 >>   90 EXTENDED_ARG             1
+                      92 FOR_ITER               316 (to 726)
+                      94 STORE_FAST               5 (company)
+         
+         173          96 LOAD_FAST                5 (company)
+                      98 LOAD_METHOD              3 (get)
+                     120 LOAD_CONST               2 ('domain')
+                     122 PRECALL                  1
+                     126 CALL                     1
+                     136 POP_JUMP_FORWARD_IF_NOT_NONE    20 (to 178)
+         
+         174         138 LOAD_GLOBAL              9 (NULL + print)
+                     150 LOAD_CONST               3 ('Missing domain: ')
+                     152 LOAD_FAST                5 (company)
+                     154 FORMAT_VALUE             0
+                     156 LOAD_CONST               4 ('. Skipping')
+                     158 BUILD_STRING             3
+                     160 PRECALL                  1
+                     164 CALL                     1
+                     174 POP_TOP
+         
+         175         176 JUMP_BACKWARD           44 (to 90)
+         
+         178     >>  178 LOAD_FAST                3 (targets)
+                     180 LOAD_CONST               2 ('domain')
+                     182 BINARY_SUBSCR
+                     192 LOAD_ATTR                5 (str)
+                     202 LOAD_METHOD              6 (contains)
+                     224 LOAD_FAST                5 (company)
+                     226 LOAD_CONST               2 ('domain')
+                     228 BINARY_SUBSCR
+                     238 PRECALL                  1
+                     242 CALL                     1
+                     252 LOAD_METHOD              7 (any)
+                     274 PRECALL                  0
+                     278 CALL                     0
+                     288 POP_JUMP_FORWARD_IF_FALSE    26 (to 342)
+         
+         179         290 LOAD_GLOBAL              9 (NULL + print)
+                     302 LOAD_CONST               5 ('Skipping ')
+                     304 LOAD_FAST                5 (company)
+                     306 LOAD_CONST               2 ('domain')
+                     308 BINARY_SUBSCR
+                     318 FORMAT_VALUE             0
+                     320 LOAD_CONST               6 (' as already a target')
+                     322 BUILD_STRING             3
+                     324 PRECALL                  1
+                     328 CALL                     1
+                     338 POP_TOP
+         
+         180         340 JUMP_BACKWARD          126 (to 90)
+         
+         182     >>  342 LOAD_GLOBAL              9 (NULL + print)
+                     354 LOAD_CONST               7 ('Adding ')
+                     356 LOAD_FAST                5 (company)
+                     358 LOAD_CONST               2 ('domain')
+                     360 BINARY_SUBSCR
+                     370 FORMAT_VALUE             0
+                     372 LOAD_CONST               8 (' as target')
+                     374 BUILD_STRING             3
+                     376 PRECALL                  1
+                     380 CALL                     1
+                     390 POP_TOP
+         
+         184         392 LOAD_FAST                4 (con)
+                     394 LOAD_METHOD              8 (execute)
+         
+         185         416 LOAD_GLOBAL             19 (NULL + sqlalchemy)
+                     428 LOAD_ATTR               10 (text)
+         
+         186         438 LOAD_CONST               9 ('\n                    INSERT INTO company (domain, name, description) \n                    VALUES(:domain, :name, :description)\n                    ON CONFLICT DO NOTHING\n                    ')
+         
+         185         440 PRECALL                  1
+                     444 CALL                     1
+         
+         193         454 LOAD_FAST                5 (company)
+                     456 LOAD_METHOD              3 (get)
+                     478 LOAD_CONST               2 ('domain')
+                     480 PRECALL                  1
+                     484 CALL                     1
+         
+         194         494 LOAD_FAST                5 (company)
+                     496 LOAD_METHOD              3 (get)
+                     518 LOAD_CONST              10 ('name')
+                     520 PRECALL                  1
+                     524 CALL                     1
+         
+         195         534 LOAD_FAST                5 (company)
+                     536 LOAD_METHOD              3 (get)
+                     558 LOAD_CONST              11 ('description')
+                     560 PRECALL                  1
+                     564 CALL                     1
+         
+         192         574 LOAD_CONST              12 (('domain', 'name', 'description'))
+                     576 BUILD_CONST_KEY_MAP      3
+         
+         184         578 PRECALL                  2
+                     582 CALL                     2
+                     592 POP_TOP
+         
+         199         594 LOAD_FAST                4 (con)
+                     596 LOAD_METHOD              8 (execute)
+         
+         200         618 LOAD_GLOBAL             19 (NULL + sqlalchemy)
+                     630 LOAD_ATTR               10 (text)
+         
+         201         640 LOAD_CONST              13 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ')
+         
+         200         642 PRECALL                  1
+                     646 CALL                     1
+         
+         207         656 LOAD_FAST                1 (search_uid)
+         
+         208         658 LOAD_FAST                2 (actor_key)
+         
+         209         660 LOAD_FAST                5 (company)
+                     662 LOAD_METHOD              3 (get)
+                     684 LOAD_CONST               2 ('domain')
+                     686 PRECALL                  1
+                     690 CALL                     1
+         
+         210         700 LOAD_CONST              14 ('create')
+         
+         206         702 LOAD_CONST              15 (('search_uid', 'actor_key', 'domain', 'type'))
+                     704 BUILD_CONST_KEY_MAP      4
+         
+         199         706 PRECALL                  2
+                     710 CALL                     2
+                     720 POP_TOP
+                     722 EXTENDED_ARG             1
+                     724 JUMP_BACKWARD          318 (to 90)
+         
+         214     >>  726 LOAD_FAST                4 (con)
+                     728 LOAD_METHOD              8 (execute)
+                     750 LOAD_GLOBAL             19 (NULL + sqlalchemy)
+                     762 LOAD_ATTR               10 (text)
+                     772 LOAD_CONST              16 ('REFRESH MATERIALIZED VIEW target')
+                     774 PRECALL                  1
+                     778 CALL                     1
+                     788 PRECALL                  1
+                     792 CALL                     1
+                     802 POP_TOP
+         
+         215         804 LOAD_FAST                4 (con)
+                     806 LOAD_METHOD             11 (commit)
+                     828 PRECALL                  0
+                     832 CALL                     0
+                     842 POP_TOP
+         
+         171         844 LOAD_CONST               0 (None)
+                     846 LOAD_CONST               0 (None)
+                     848 LOAD_CONST               0 (None)
+                     850 PRECALL                  2
+                     854 CALL                     2
+                     864 POP_TOP
+                     866 LOAD_CONST               0 (None)
+                     868 RETURN_VALUE
+                 >>  870 PUSH_EXC_INFO
+                     872 WITH_EXCEPT_START
+                     874 POP_JUMP_FORWARD_IF_TRUE     4 (to 884)
+                     876 RERAISE                  2
+                 >>  878 COPY                     3
+                     880 POP_EXCEPT
+                     882 RERAISE                  1
+                 >>  884 POP_TOP
+                     886 POP_EXCEPT
+                     888 POP_TOP
+                     890 POP_TOP
+                     892 LOAD_CONST               0 (None)
+                     894 RETURN_VALUE
+         ExceptionTable:
+           84 to 842 -> 870 [1] lasti
+           870 to 876 -> 878 [3] lasti
+           884 to 884 -> 878 [3] lasti
+         consts
+            None
+            ('search_uid',)
+            'domain'
+            'Missing domain: '
+            '. Skipping'
+            'Skipping '
+            ' as already a target'
+            'Adding '
+            ' as target'
+            '\n                    INSERT INTO company (domain, name, description) \n                    VALUES(:domain, :name, :description)\n                    ON CONFLICT DO NOTHING\n                    '
+            'name'
+            'description'
+            ('domain', 'name', 'description')
+            '\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    '
+            'create'
+            ('search_uid', 'actor_key', 'domain', 'type')
+            'REFRESH MATERIALIZED VIEW target'
+         names      ('target', 'db', 'connect', 'get', 'print', 'str', 'contains', 'any', 'execute', 'sqlalchemy', 'text', 'commit')
+         varnames   ('companies', 'search_uid', 'actor_key', 'targets', 'con', 'company')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+         name       'insert_companies_as_targets'
+         firstlineno 167
+         lnotab
+            0x0203200134010a012a012601020370013201020232021801160102ff0e
+            082801280128fd04f8100f1801160102ff0e0702010201280102fc04f914
+            0f4e0128d4
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
@@ -825,52 +1382,52 @@
             006a0400000000000000006401a6010000ab010000000000000000a60100
             00ab0100000000000000007d01740b000000000000000000006a06000000
             00000000007c01a0070000000000000000000000000000000000000000a6
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d02640064006400a6020000ab02000000000000000001
             006e0b230031007304770278035900770101005900010001007c025300
-         115           0 RESUME                   0
+         221           0 RESUME                   0
          
-         116           2 LOAD_GLOBAL              0 (db)
+         222           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         117          54 LOAD_FAST                0 (conn)
+         223          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         118          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         224          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
                      100 LOAD_CONST               1 ("SELECT *, meta->>'group' as group FROM search")
                      102 PRECALL                  1
                      106 CALL                     1
          
-         117         116 PRECALL                  1
+         223         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         120         132 LOAD_GLOBAL             11 (NULL + pd)
+         226         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         116         248 LOAD_CONST               0 (None)
+         222         248 LOAD_CONST               0 (None)
                      250 LOAD_CONST               0 (None)
                      252 LOAD_CONST               0 (None)
                      254 PRECALL                  2
                      258 CALL                     2
                      268 POP_TOP
                      270 JUMP_FORWARD            11 (to 294)
                  >>  272 PUSH_EXC_INFO
@@ -881,15 +1438,15 @@
                      282 POP_EXCEPT
                      284 RERAISE                  1
                  >>  286 POP_TOP
                      288 POP_EXCEPT
                      290 POP_TOP
                      292 POP_TOP
          
-         121     >>  294 LOAD_FAST                2 (df)
+         227     >>  294 LOAD_FAST                2 (df)
                      296 RETURN_VALUE
          ExceptionTable:
            52 to 246 -> 272 [1] lasti
            272 to 278 -> 280 [3] lasti
            286 to 286 -> 280 [3] lasti
          consts
             None
@@ -897,17 +1454,16 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search'
-         firstlineno 115
+         firstlineno 221
          lnotab 0x02013401180126ff100374fc2e05
-      'search_uid'
       'last_event_type'
       code
          argcount  : 2
          nlocals   : 8
          stacksize : 7
          flags     : 3
          code
@@ -930,84 +1486,84 @@
             17000000000000000000007c00a6010000ab0100000000000000007d077c
             05a00c00000000000000000000000000000000000000007c076a0d000000
             0000000000a00e0000000000000000000000000000000000000000640964
             06a6020000ab0200000000000000007c076a0d0000000000000000a00e00
             00000000000000000000000000000000000000640aa6010000ab01000000
             0000000000640b6b0200000000ac0ca6020000ab0200000000000000007d
             057c055300
-         124           0 RESUME                   0
+         230           0 RESUME                   0
          
-         125           2 LOAD_GLOBAL              0 (db)
+         231           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               2 (conn)
          
-         126          54 LOAD_FAST                1 (last_event_type)
+         232          54 LOAD_FAST                1 (last_event_type)
                       56 POP_JUMP_FORWARD_IF_NONE    46 (to 150)
          
-         127          58 LOAD_CONST               1 ('SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type')
+         233          58 LOAD_CONST               1 ('SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type')
                       60 STORE_FAST               3 (statement)
          
-         128          62 LOAD_FAST                2 (conn)
+         234          62 LOAD_FAST                2 (conn)
                       64 LOAD_METHOD              2 (execute)
          
-         129          86 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         235          86 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       98 LOAD_ATTR                4 (text)
                      108 LOAD_FAST                3 (statement)
                      110 PRECALL                  1
                      114 CALL                     1
          
-         130         124 LOAD_FAST                0 (search_uid)
+         236         124 LOAD_FAST                0 (search_uid)
                      126 LOAD_FAST                1 (last_event_type)
                      128 LOAD_CONST               2 (('search_uid', 'last_event_type'))
                      130 BUILD_CONST_KEY_MAP      2
          
-         128         132 PRECALL                  2
+         234         132 PRECALL                  2
                      136 CALL                     2
                      146 STORE_FAST               4 (result)
                      148 JUMP_FORWARD            44 (to 238)
          
-         134     >>  150 LOAD_CONST               3 ('SELECT * FROM target WHERE search_uid = :search_uid')
+         240     >>  150 LOAD_CONST               3 ('SELECT * FROM target WHERE search_uid = :search_uid')
                      152 STORE_FAST               3 (statement)
          
-         135         154 LOAD_FAST                2 (conn)
+         241         154 LOAD_FAST                2 (conn)
                      156 LOAD_METHOD              2 (execute)
          
-         136         178 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         242         178 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      190 LOAD_ATTR                4 (text)
                      200 LOAD_FAST                3 (statement)
                      202 PRECALL                  1
                      206 CALL                     1
          
-         137         216 LOAD_CONST               4 ('search_uid')
+         243         216 LOAD_CONST               4 ('search_uid')
                      218 LOAD_FAST                0 (search_uid)
                      220 BUILD_MAP                1
          
-         135         222 PRECALL                  2
+         241         222 PRECALL                  2
                      226 CALL                     2
                      236 STORE_FAST               4 (result)
          
-         140     >>  238 LOAD_GLOBAL             11 (NULL + pd)
+         246     >>  238 LOAD_GLOBAL             11 (NULL + pd)
                      250 LOAD_ATTR                6 (DataFrame)
                      260 LOAD_FAST                4 (result)
                      262 LOAD_METHOD              7 (fetchall)
                      284 PRECALL                  0
                      288 CALL                     0
                      298 LOAD_FAST                4 (result)
                      300 LOAD_METHOD              8 (keys)
                      322 PRECALL                  0
                      326 CALL                     0
                      336 KW_NAMES                 5
                      338 PRECALL                  2
                      342 CALL                     2
                      352 STORE_FAST               5 (targets)
          
-         125         354 LOAD_CONST               0 (None)
+         231         354 LOAD_CONST               0 (None)
                      356 LOAD_CONST               0 (None)
                      358 LOAD_CONST               0 (None)
                      360 PRECALL                  2
                      364 CALL                     2
                      374 POP_TOP
                      376 JUMP_FORWARD            11 (to 400)
                  >>  378 PUSH_EXC_INFO
@@ -1018,62 +1574,62 @@
                      388 POP_EXCEPT
                      390 RERAISE                  1
                  >>  392 POP_TOP
                      394 POP_EXCEPT
                      396 POP_TOP
                      398 POP_TOP
          
-         142     >>  400 LOAD_GLOBAL             19 (NULL + comment_by_domain)
+         248     >>  400 LOAD_GLOBAL             19 (NULL + comment_by_domain)
                      412 LOAD_FAST                0 (search_uid)
                      414 PRECALL                  1
                      418 CALL                     1
                      428 STORE_FAST               6 (comments)
          
-         143         430 LOAD_FAST                5 (targets)
+         249         430 LOAD_FAST                5 (targets)
                      432 LOAD_METHOD             10 (merge)
                      454 LOAD_FAST                6 (comments)
                      456 LOAD_CONST               6 ('domain')
                      458 LOAD_CONST               7 ('left')
                      460 KW_NAMES                 8
                      462 PRECALL                  3
                      466 CALL                     3
                      476 STORE_FAST               5 (targets)
          
-         146         478 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
+         252         478 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
                      490 LOAD_FAST                0 (search_uid)
                      492 PRECALL                  1
                      496 CALL                     1
                      506 STORE_FAST               7 (search)
          
-         147         508 LOAD_FAST                5 (targets)
+         253         508 LOAD_FAST                5 (targets)
                      510 LOAD_METHOD             12 (sort_values)
          
-         148         532 LOAD_FAST                7 (search)
+         254         532 LOAD_FAST                7 (search)
                      534 LOAD_ATTR               13 (sort)
                      544 LOAD_METHOD             14 (get)
                      566 LOAD_CONST               9 ('field')
                      568 LOAD_CONST               6 ('domain')
                      570 PRECALL                  2
                      574 CALL                     2
          
-         149         584 LOAD_FAST                7 (search)
+         255         584 LOAD_FAST                7 (search)
                      586 LOAD_ATTR               13 (sort)
                      596 LOAD_METHOD             14 (get)
                      618 LOAD_CONST              10 ('order')
                      620 PRECALL                  1
                      624 CALL                     1
                      634 LOAD_CONST              11 ('asc')
                      636 COMPARE_OP               2 (==)
          
-         147         642 KW_NAMES                12
+         253         642 KW_NAMES                12
                      644 PRECALL                  2
                      648 CALL                     2
                      658 STORE_FAST               5 (targets)
          
-         152         660 LOAD_FAST                5 (targets)
+         258         660 LOAD_FAST                5 (targets)
                      662 RETURN_VALUE
          ExceptionTable:
            52 to 352 -> 378 [1] lasti
            378 to 384 -> 386 [3] lasti
            392 to 392 -> 386 [3] lasti
          consts
             None
@@ -1091,15 +1647,15 @@
             ('by', 'ascending')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'comment_by_domain', 'merge', 'find_search_by_uid', 'sort_values', 'sort', 'get')
          varnames   ('search_uid', 'last_event_type', 'conn', 'statement', 'result', 'targets', 'comments', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target'
-         firstlineno 124
+         firstlineno 230
          lnotab
             0x02013401040104011801260108fe120604011801260106fe100574f12e
             111e0130031e01180134013afe1205
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
@@ -1112,59 +1668,59 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         155           0 RESUME                   0
+         261           0 RESUME                   0
          
-         156           2 LOAD_GLOBAL              0 (db)
+         262           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         157          54 LOAD_CONST               1 ('\n                SELECT last_event_type, count(*)\n                FROM target\n                WHERE search_uid = :search_uid\n                GROUP BY last_event_type\n            ')
+         263          54 LOAD_CONST               1 ('\n                SELECT last_event_type, count(*)\n                FROM target\n                WHERE search_uid = :search_uid\n                GROUP BY last_event_type\n            ')
                       56 STORE_FAST               2 (statement)
          
-         163          58 LOAD_FAST                1 (conn)
+         269          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         164          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         270          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         165         120 LOAD_CONST               2 ('search_uid')
+         271         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         163         126 PRECALL                  2
+         269         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         167         142 LOAD_GLOBAL             11 (NULL + pd)
+         273         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         156         258 LOAD_CONST               0 (None)
+         262         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -1175,15 +1731,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         168     >>  304 LOAD_FAST                4 (df)
+         274     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -1192,15 +1748,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target_count'
-         firstlineno 155
+         firstlineno 261
          lnotab 0x0201340104061801260106fe100474f52e0c
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -1211,56 +1767,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         171           0 RESUME                   0
+         277           0 RESUME                   0
          
-         172           2 LOAD_GLOBAL              0 (db)
+         278           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         173          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         279          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         178          58 LOAD_FAST                1 (conn)
+         284          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         179         142 LOAD_GLOBAL             11 (NULL + pd)
+         285         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         172         258 LOAD_CONST               0 (None)
+         278         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -1271,15 +1827,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         180     >>  304 LOAD_FAST                4 (df)
+         286     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -1288,15 +1844,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 171
+         firstlineno 277
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -1307,53 +1863,53 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d03640064006400a6020000ab020000000000
             00000001006e0b230031007304770278035900770101005900010001007c
             035300
-         183           0 RESUME                   0
+         289           0 RESUME                   0
          
-         184           2 LOAD_GLOBAL              0 (db)
+         290           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         185          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
+         291          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
                       56 STORE_FAST               1 (statement)
          
-         189          58 LOAD_FAST                0 (conn)
+         295          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         190         136 LOAD_GLOBAL             11 (NULL + pd)
+         296         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         184         252 LOAD_CONST               0 (None)
+         290         252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 LOAD_CONST               0 (None)
                      258 PRECALL                  2
                      262 CALL                     2
                      272 POP_TOP
                      274 JUMP_FORWARD            11 (to 298)
                  >>  276 PUSH_EXC_INFO
@@ -1364,15 +1920,15 @@
                      286 POP_EXCEPT
                      288 RERAISE                  1
                  >>  290 POP_TOP
                      292 POP_EXCEPT
                      294 POP_TOP
                      296 POP_TOP
          
-         191     >>  298 LOAD_FAST                3 (df)
+         297     >>  298 LOAD_FAST                3 (df)
                      300 RETURN_VALUE
          ExceptionTable:
            52 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
@@ -1380,15 +1936,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'company'
-         firstlineno 183
+         firstlineno 289
          lnotab 0x0201340104044e0174fa2e07
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -1399,56 +1955,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         194           0 RESUME                   0
+         300           0 RESUME                   0
          
-         195           2 LOAD_GLOBAL              0 (db)
+         301           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         196          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n                JOIN event ON checkpoint.event_id = event.id\n                WHERE search_uid = :search_uid\n            ')
+         302          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n                JOIN event ON checkpoint.event_id = event.id\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         202          58 LOAD_FAST                1 (conn)
+         308          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         203         142 LOAD_GLOBAL             11 (NULL + pd)
+         309         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         195         258 LOAD_CONST               0 (None)
+         301         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -1459,15 +2015,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         204     >>  304 LOAD_FAST                4 (df)
+         310     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -1476,15 +2032,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'checkpoint'
-         firstlineno 194
+         firstlineno 300
          lnotab 0x020134010406540174f82e09
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -1499,59 +2055,59 @@
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c04a009000000000000000000000000000000000000000064
             04a6010000ab010000000000000000a00a00000000000000000000000000
             000000000000006405640684006901a6010000ab010000000000000000a0
             0b0000000000000000000000000000000000000000a6000000ab00000000
             00000000005300
-         207           0 RESUME                   0
+         313           0 RESUME                   0
          
-         208           2 LOAD_GLOBAL              0 (db)
+         314           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         209          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
+         315          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
                       56 STORE_FAST               2 (statement)
          
-         216          58 LOAD_FAST                1 (conn)
+         322          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         217          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         323          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         218         120 LOAD_CONST               2 ('search_uid')
+         324         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         216         126 PRECALL                  2
+         322         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         220         142 LOAD_GLOBAL             11 (NULL + pd)
+         326         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         208         258 LOAD_CONST               0 (None)
+         314         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -1562,22 +2118,22 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         222     >>  304 LOAD_FAST                4 (df)
+         328     >>  304 LOAD_FAST                4 (df)
                      306 LOAD_METHOD              9 (groupby)
                      328 LOAD_CONST               4 ('domain')
                      330 PRECALL                  1
                      334 CALL                     1
                      344 LOAD_METHOD             10 (agg)
                      366 LOAD_CONST               5 ('comment')
-                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 222>)
+                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 328>)
                      370 MAKE_FUNCTION            0
                      372 BUILD_MAP                1
                      374 PRECALL                  1
                      378 CALL                     1
                      388 LOAD_METHOD             11 (reset_index)
                      410 PRECALL                  0
                      414 CALL                     0
@@ -1597,37 +2153,37 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-               222           0 RESUME                   0
+               328           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('list',)
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<lambda>'
-               firstlineno 222
+               firstlineno 328
                lnotab 0x
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'groupby', 'agg', 'reset_index')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'comment_by_domain'
-         firstlineno 207
+         firstlineno 313
          lnotab 0x0201340104071801260106fe100474f42e0e
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
@@ -1640,41 +2196,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         228           0 RESUME                   0
+         334           0 RESUME                   0
          
-         229           2 LOAD_GLOBAL              0 (db)
+         335           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         230          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
+         336          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         235          58 LOAD_FAST                1 (conn)
+         341          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         229         142 LOAD_CONST               0 (None)
+         335         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -1685,24 +2241,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         237     >>  188 LOAD_FAST                3 (result)
+         343     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         238         210 LOAD_CONST               0 (None)
+         344         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         240     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         346     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -1710,15 +2266,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         241         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         347         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Search)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -1731,15 +2287,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Search')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_uid'
-         firstlineno 228
+         firstlineno 334
          lnotab 0x02013401040554fa2e08160104028201
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -1753,41 +2309,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         244           0 RESUME                   0
+         350           0 RESUME                   0
          
-         245           2 LOAD_GLOBAL              0 (db)
+         351           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         246          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         352          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         251          58 LOAD_FAST                1 (conn)
+         357          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('domain')
                      122 LOAD_FAST                0 (domain)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         245         142 LOAD_CONST               0 (None)
+         351         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -1798,24 +2354,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         253     >>  188 LOAD_FAST                3 (result)
+         359     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         254         210 LOAD_CONST               0 (None)
+         360         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         256     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         362     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -1823,15 +2379,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         257         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         363         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -1844,15 +2400,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 244
+         firstlineno 350
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -1866,41 +2422,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         260           0 RESUME                   0
+         366           0 RESUME                   0
          
-         261           2 LOAD_GLOBAL              0 (db)
+         367           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         262          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         368          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         267          58 LOAD_FAST                1 (conn)
+         373          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('event_id')
                      122 LOAD_FAST                0 (event_id)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         261         142 LOAD_CONST               0 (None)
+         367         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -1911,24 +2467,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         269     >>  188 LOAD_FAST                3 (result)
+         375     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         270         210 LOAD_CONST               0 (None)
+         376         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         272     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         378     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -1936,15 +2492,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         273         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         379         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -1957,15 +2513,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 260
+         firstlineno 366
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 10
          flags     : 3
          code
@@ -1979,76 +2535,76 @@
             020000ab02000000000000000001007c01a0020000000000000000000000
             0000000000000000007407000000000000000000006a0400000000000000
             006403a6010000ab010000000000000000a6010000ab0100000000000000
             0001007c01a00b0000000000000000000000000000000000000000a60000
             00ab0000000000000000000100640064006400a6020000ab020000000000
             000000010064005300230031007304770278035900770101005900010001
             0064005300
-         278           0 RESUME                   0
+         385           0 RESUME                   0
          
-         279           2 LOAD_GLOBAL              0 (db)
+         386           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         280          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            ')
+         387          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         289          58 LOAD_FAST                1 (conn)
+         396          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         290          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         397          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         292         120 LOAD_FAST                0 (company)
+         399         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (name)
          
-         293         132 LOAD_FAST                0 (company)
+         400         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (description)
          
-         294         144 LOAD_FAST                0 (company)
+         401         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (domain)
          
-         295         156 LOAD_GLOBAL             17 (NULL + json)
+         402         156 LOAD_GLOBAL             17 (NULL + json)
                      168 LOAD_ATTR                9 (dumps)
                      178 LOAD_FAST                0 (company)
                      180 LOAD_ATTR               10 (meta)
                      190 PRECALL                  1
                      194 CALL                     1
          
-         291         204 LOAD_CONST               2 (('name', 'description', 'domain', 'meta'))
+         398         204 LOAD_CONST               2 (('name', 'description', 'domain', 'meta'))
                      206 BUILD_CONST_KEY_MAP      4
          
-         289         208 PRECALL                  2
+         396         208 PRECALL                  2
                      212 CALL                     2
                      222 POP_TOP
          
-         298         224 LOAD_FAST                1 (conn)
+         405         224 LOAD_FAST                1 (conn)
                      226 LOAD_METHOD              2 (execute)
                      248 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      260 LOAD_ATTR                4 (text)
                      270 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW target')
                      272 PRECALL                  1
                      276 CALL                     1
                      286 PRECALL                  1
                      290 CALL                     1
                      300 POP_TOP
          
-         299         302 LOAD_FAST                1 (conn)
+         406         302 LOAD_FAST                1 (conn)
                      304 LOAD_METHOD             11 (commit)
                      326 PRECALL                  0
                      330 CALL                     0
                      340 POP_TOP
          
-         279         342 LOAD_CONST               0 (None)
+         386         342 LOAD_CONST               0 (None)
                      344 LOAD_CONST               0 (None)
                      346 LOAD_CONST               0 (None)
                      348 PRECALL                  2
                      352 CALL                     2
                      362 POP_TOP
                      364 LOAD_CONST               0 (None)
                      366 RETURN_VALUE
@@ -2076,15 +2632,15 @@
             'REFRESH MATERIALIZED VIEW target'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'name', 'description', 'domain', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 278
+         firstlineno 385
          lnotab 0x020134010409180126020c010c010c0130fc04fe10094e0128ec
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 9
          flags     : 3
          code
@@ -2097,72 +2653,72 @@
             000000000000007c006a080000000000000000a6010000ab010000000000
             000000740b000000000000000000006a0600000000000000007c006a0900
             00000000000000a6010000ab0100000000000000007c006a0a0000000000
             00000064029c04a6020000ab02000000000000000001007c01a00b000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             000100640064006400a6020000ab02000000000000000001006400530023
             00310073047702780359007701010059000100010064005300
-         302           0 RESUME                   0
+         409           0 RESUME                   0
          
-         303           2 LOAD_GLOBAL              0 (db)
+         410           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         304          54 LOAD_FAST                1 (conn)
+         411          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         305          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         412          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         306         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                ')
+         413         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                ')
          
-         305         102 PRECALL                  1
+         412         102 PRECALL                  1
                      106 CALL                     1
          
-         316         116 LOAD_GLOBAL             11 (NULL + json)
+         423         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (sort)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         317         164 LOAD_GLOBAL             11 (NULL + json)
+         424         164 LOAD_GLOBAL             11 (NULL + json)
                      176 LOAD_ATTR                6 (dumps)
                      186 LOAD_FAST                0 (search)
                      188 LOAD_ATTR                8 (inclusion)
                      198 PRECALL                  1
                      202 CALL                     1
          
-         318         212 LOAD_GLOBAL             11 (NULL + json)
+         425         212 LOAD_GLOBAL             11 (NULL + json)
                      224 LOAD_ATTR                6 (dumps)
                      234 LOAD_FAST                0 (search)
                      236 LOAD_ATTR                9 (exclusion)
                      246 PRECALL                  1
                      250 CALL                     1
          
-         319         260 LOAD_FAST                0 (search)
+         426         260 LOAD_FAST                0 (search)
                      262 LOAD_ATTR               10 (uid)
          
-         315         272 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'uid'))
+         422         272 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'uid'))
                      274 BUILD_CONST_KEY_MAP      4
          
-         304         276 PRECALL                  2
+         411         276 PRECALL                  2
                      280 CALL                     2
                      290 POP_TOP
          
-         322         292 LOAD_FAST                1 (conn)
+         429         292 LOAD_FAST                1 (conn)
                      294 LOAD_METHOD             11 (commit)
                      316 PRECALL                  0
                      320 CALL                     0
                      330 POP_TOP
          
-         303         332 LOAD_CONST               0 (None)
+         410         332 LOAD_CONST               0 (None)
                      334 LOAD_CONST               0 (None)
                      336 LOAD_CONST               0 (None)
                      338 PRECALL                  2
                      342 CALL                     2
                      352 POP_TOP
                      354 LOAD_CONST               0 (None)
                      356 RETURN_VALUE
@@ -2189,20 +2745,22 @@
             ('sort', 'inclusion', 'exclusion', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'sort', 'inclusion', 'exclusion', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 302
+         firstlineno 409
          lnotab 0x020134011801160102ff0e0b3001300130010cfc04f5101228ed
       (None,)
-   names      ('json', 'pandas', 'pd', 'dataclasses', 'asdict', 'dacite', 'from_dict', 'gandai.models', 'Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint', 'sqlalchemy', 'google.cloud.sql.connector', 'Connector', 'dotenv', 'load_dotenv', 'gandai.db', 'connect_with_connector', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'search', 'int', 'str', 'target', 'DataFrame', 'target_count', 'event', 'company', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'find_event_by_id', 'update_company', 'update_search')
+   names      ('json', 'pandas', 'pd', 'typing', 'List', 'Any', 'dataclasses', 'asdict', 'dacite', 'from_dict', 'gandai.models', 'Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint', 'sqlalchemy', 'google.cloud.sql.connector', 'Connector', 'dotenv', 'load_dotenv', 'gandai.db', 'connect_with_connector', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'str', 'int', 'insert_and_advance_targets_from_domains', 'insert_companies_as_targets', 'search', 'target', 'DataFrame', 'target_count', 'event', 'company', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'find_event_by_id', 'update_company', 'update_search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010c010c01200a08020c010c0214020c0214060c0e10
-      15100f101310100609121f1a101a0c160b1a0d1a151010101010121018
+      0x00ff02010801080110010c010c01200a08020c010c0214020c0214060c
+      0e1015100f1013100d02010eff020102ff020102ff020202fe083602010e
+      ff020102ff020102ff020202fe08360609121f1a101a0c160b1a0d1a1510
+      10101010131018
```

### Comparing `gandai-1.1.9/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.2.0/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.9/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.2.0/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,183 +1,161 @@
 magic:    0xa70d0d0a
-moddate:  0xd24b6164 (Sun May 14 21:00:02 2023 UTC)
-files sz: 5497
+moddate:  0x56777f64 (Tue Jun  6 18:13:42 2023 UTC)
+files sz: 5534
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c045a04640064036c055a05640064046c066d075a07010002006507a6
-      000000ab000000000000000000010002004700640584006406a6020000ab
-      0200000000000000005a0802004700640784006408a6020000ab02000000
-      00000000005a0964035300
+      036c045a0402004700640484006405a6020000ab0200000000000000005a
+      0502004700640684006407a6020000ab0200000000000000005a06640353
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('query',))
-                 6 IMPORT_NAME              0 (gandai)
-                 8 IMPORT_FROM              1 (query)
-                10 STORE_NAME               1 (query)
+                 4 LOAD_CONST               1 (('access_secret_version',))
+                 6 IMPORT_NAME              0 (gandai.secrets)
+                 8 IMPORT_FROM              1 (access_secret_version)
+                10 STORE_NAME               1 (access_secret_version)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
                 16 LOAD_CONST               2 (('Search',))
                 18 IMPORT_NAME              2 (gandai.models)
                 20 IMPORT_FROM              3 (Search)
                 22 STORE_NAME               3 (Search)
                 24 POP_TOP
    
-     3          26 LOAD_CONST               0 (0)
+     4          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               3 (None)
                 30 IMPORT_NAME              4 (requests)
                 32 STORE_NAME               4 (requests)
    
-     4          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               3 (None)
-                38 IMPORT_NAME              5 (os)
-                40 STORE_NAME               5 (os)
+     6          34 PUSH_NULL
+                36 LOAD_BUILD_CLASS
+                38 LOAD_CONST               4 (<code object GrataWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 6>)
+                40 MAKE_FUNCTION            0
+                42 LOAD_CONST               5 ('GrataWrapper')
+                44 PRECALL                  2
+                48 CALL                     2
+                58 STORE_NAME               5 (GrataWrapper)
    
-     5          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               4 (('load_dotenv',))
-                46 IMPORT_NAME              6 (dotenv)
-                48 IMPORT_FROM              7 (load_dotenv)
-                50 STORE_NAME               7 (load_dotenv)
-                52 POP_TOP
-   
-     7          54 PUSH_NULL
-                56 LOAD_NAME                7 (load_dotenv)
-                58 PRECALL                  0
-                62 CALL                     0
-                72 POP_TOP
-   
-    10          74 PUSH_NULL
-                76 LOAD_BUILD_CLASS
-                78 LOAD_CONST               5 (<code object GrataWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 10>)
-                80 MAKE_FUNCTION            0
-                82 LOAD_CONST               6 ('GrataWrapper')
-                84 PRECALL                  2
-                88 CALL                     2
-                98 STORE_NAME               8 (GrataWrapper)
-   
-   166         100 PUSH_NULL
-               102 LOAD_BUILD_CLASS
-               104 LOAD_CONST               7 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 166>)
-               106 MAKE_FUNCTION            0
-               108 LOAD_CONST               8 ('SourceScrubWrapper')
-               110 PRECALL                  2
-               114 CALL                     2
-               124 STORE_NAME               9 (SourceScrubWrapper)
-               126 LOAD_CONST               3 (None)
-               128 RETURN_VALUE
+   163          60 PUSH_NULL
+                62 LOAD_BUILD_CLASS
+                64 LOAD_CONST               6 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 163>)
+                66 MAKE_FUNCTION            0
+                68 LOAD_CONST               7 ('SourceScrubWrapper')
+                70 PRECALL                  2
+                74 CALL                     2
+                84 STORE_NAME               6 (SourceScrubWrapper)
+                86 LOAD_CONST               3 (None)
+                88 RETURN_VALUE
    consts
       0
-      ('query',)
+      ('access_secret_version',)
       ('Search',)
       None
-      ('load_dotenv',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
-            0x970065005a0164005a02020065036a0400000000000000006401a60100
-            00ab010000000000000000640264039c025a05640484005a006405650664
-            066507640765086606640884045a09640665076407650a6604640984045a
-            0b640565066407650a6604640a84045a0c640665076407650a6604640b84
-            045a0d640c5300
-          10           0 RESUME                   0
+            0x970065005a0164005a02020065036401a6010000ab0100000000000000
+            00640264039c025a04640484005a00640565056406650664076507660664
+            0884045a0864066506640765096604640984045a0a640565056407650966
+            04640a84045a0b64066506640765096604640b84045a0c640c5300
+           6           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GrataWrapper')
                        8 STORE_NAME               2 (__qualname__)
          
-          12          10 PUSH_NULL
-                      12 LOAD_NAME                3 (os)
-                      14 LOAD_ATTR                4 (getenv)
-                      24 LOAD_CONST               1 ('GRATA_API_TOKEN')
-                      26 PRECALL                  1
-                      30 CALL                     1
+           8          10 PUSH_NULL
+                      12 LOAD_NAME                3 (access_secret_version)
+                      14 LOAD_CONST               1 ('GRATA_API_TOKEN')
+                      16 PRECALL                  1
+                      20 CALL                     1
          
-          13          40 LOAD_CONST               2 ('application/json')
+           9          30 LOAD_CONST               2 ('application/json')
          
-          11          42 LOAD_CONST               3 (('Authorization', 'Content-Type'))
-                      44 BUILD_CONST_KEY_MAP      2
-                      46 STORE_NAME               5 (HEADERS)
+           7          32 LOAD_CONST               3 (('Authorization', 'Content-Type'))
+                      34 BUILD_CONST_KEY_MAP      2
+                      36 STORE_NAME               4 (HEADERS)
          
-          16          48 LOAD_CONST               4 (<code object __name__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 16>)
-                      50 MAKE_FUNCTION            0
-                      52 STORE_NAME               0 (__name__)
+          12          38 LOAD_CONST               4 (<code object __name__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 12>)
+                      40 MAKE_FUNCTION            0
+                      42 STORE_NAME               0 (__name__)
          
-          19          54 LOAD_CONST               5 ('domain')
-                      56 LOAD_NAME                6 (str)
-                      58 LOAD_CONST               6 ('search')
-                      60 LOAD_NAME                7 (Search)
-                      62 LOAD_CONST               7 ('return')
-                      64 LOAD_NAME                8 (list)
-                      66 BUILD_TUPLE              6
-                      68 LOAD_CONST               8 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 19>)
-                      70 MAKE_FUNCTION            4 (annotations)
-                      72 STORE_NAME               9 (find_similar)
+          15          44 LOAD_CONST               5 ('domain')
+                      46 LOAD_NAME                5 (str)
+                      48 LOAD_CONST               6 ('search')
+                      50 LOAD_NAME                6 (Search)
+                      52 LOAD_CONST               7 ('return')
+                      54 LOAD_NAME                7 (list)
+                      56 BUILD_TUPLE              6
+                      58 LOAD_CONST               8 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 15>)
+                      60 MAKE_FUNCTION            4 (annotations)
+                      62 STORE_NAME               8 (find_similar)
          
-          36          74 LOAD_CONST               6 ('search')
-                      76 LOAD_NAME                7 (Search)
-                      78 LOAD_CONST               7 ('return')
-                      80 LOAD_NAME               10 (dict)
-                      82 BUILD_TUPLE              4
-                      84 LOAD_CONST               9 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 36>)
-                      86 MAKE_FUNCTION            4 (annotations)
-                      88 STORE_NAME              11 (find_by_criteria)
+          32          64 LOAD_CONST               6 ('search')
+                      66 LOAD_NAME                6 (Search)
+                      68 LOAD_CONST               7 ('return')
+                      70 LOAD_NAME                9 (dict)
+                      72 BUILD_TUPLE              4
+                      74 LOAD_CONST               9 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 32>)
+                      76 MAKE_FUNCTION            4 (annotations)
+                      78 STORE_NAME              10 (find_by_criteria)
          
-          54          90 LOAD_CONST               5 ('domain')
-                      92 LOAD_NAME                6 (str)
-                      94 LOAD_CONST               7 ('return')
-                      96 LOAD_NAME               10 (dict)
-                      98 BUILD_TUPLE              4
-                     100 LOAD_CONST              10 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 54>)
-                     102 MAKE_FUNCTION            4 (annotations)
-                     104 STORE_NAME              12 (enrich)
+          50          80 LOAD_CONST               5 ('domain')
+                      82 LOAD_NAME                5 (str)
+                      84 LOAD_CONST               7 ('return')
+                      86 LOAD_NAME                9 (dict)
+                      88 BUILD_TUPLE              4
+                      90 LOAD_CONST              10 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 50>)
+                      92 MAKE_FUNCTION            4 (annotations)
+                      94 STORE_NAME              11 (enrich)
          
-          64         106 LOAD_CONST               6 ('search')
-                     108 LOAD_NAME                7 (Search)
-                     110 LOAD_CONST               7 ('return')
-                     112 LOAD_NAME               10 (dict)
-                     114 BUILD_TUPLE              4
-                     116 LOAD_CONST              11 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 64>)
-                     118 MAKE_FUNCTION            4 (annotations)
-                     120 STORE_NAME              13 (_get_api_filter)
-                     122 LOAD_CONST              12 (None)
-                     124 RETURN_VALUE
+          61          96 LOAD_CONST               6 ('search')
+                      98 LOAD_NAME                6 (Search)
+                     100 LOAD_CONST               7 ('return')
+                     102 LOAD_NAME                9 (dict)
+                     104 BUILD_TUPLE              4
+                     106 LOAD_CONST              11 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 61>)
+                     108 MAKE_FUNCTION            4 (annotations)
+                     110 STORE_NAME              12 (_get_api_filter)
+                     112 LOAD_CONST              12 (None)
+                     114 RETURN_VALUE
          consts
             'GrataWrapper'
             'GRATA_API_TOKEN'
             'application/json'
             ('Authorization', 'Content-Type')
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064015300
-                16           0 RESUME                   0
+                12           0 RESUME                   0
                
-                17           2 LOAD_CONST               1 ('GrataWrapper')
+                13           2 LOAD_CONST               1 ('GrataWrapper')
                              4 RETURN_VALUE
                consts
                   None
                   'GrataWrapper'
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       '__name__'
-               firstlineno 16
+               firstlineno 12
                lnotab 0x0201
             'domain'
             'search'
             'return'
             code
                argcount  : 2
                nlocals   : 5
@@ -190,73 +168,73 @@
                   006a0400000000000000007c007c026402190000000000000000007c0264
                   031900000000000000000064049c03ac05a6030000ab0300000000000000
                   007d037c03a0050000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d04740d0000000000000000000064067c04a6
                   020000ab02000000000000000001007c04a0070000000000000000000000
                   00000000000000000064076700a6020000ab0200000000000000007c0464
                   083c0000007c046408190000000000000000005300
-                19           0 RESUME                   0
+                15           0 RESUME                   0
                
-                20           2 LOAD_GLOBAL              0 (GrataWrapper)
+                16           2 LOAD_GLOBAL              0 (GrataWrapper)
                             14 LOAD_METHOD              1 (_get_api_filter)
                             36 LOAD_FAST                1 (search)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               2 (api_filters)
                
-                21          54 LOAD_GLOBAL              5 (NULL + requests)
+                17          54 LOAD_GLOBAL              5 (NULL + requests)
                             66 LOAD_ATTR                3 (post)
                
-                22          76 LOAD_CONST               1 ('https://search.grata.com/api/v1/search-similar/')
+                18          76 LOAD_CONST               1 ('https://search.grata.com/api/v1/search-similar/')
                
-                23          78 LOAD_GLOBAL              0 (GrataWrapper)
+                19          78 LOAD_GLOBAL              0 (GrataWrapper)
                             90 LOAD_ATTR                4 (HEADERS)
                
-                25         100 LOAD_FAST                0 (domain)
+                21         100 LOAD_FAST                0 (domain)
                
-                26         102 LOAD_FAST                2 (api_filters)
+                22         102 LOAD_FAST                2 (api_filters)
                            104 LOAD_CONST               2 ('employees_range')
                            106 BINARY_SUBSCR
                
-                27         116 LOAD_FAST                2 (api_filters)
+                23         116 LOAD_FAST                2 (api_filters)
                            118 LOAD_CONST               3 ('headquarters')
                            120 BINARY_SUBSCR
                
-                24         130 LOAD_CONST               4 (('domain', 'employees_range', 'headquarters'))
+                20         130 LOAD_CONST               4 (('domain', 'employees_range', 'headquarters'))
                            132 BUILD_CONST_KEY_MAP      3
                
-                21         134 KW_NAMES                 5
+                17         134 KW_NAMES                 5
                            136 PRECALL                  3
                            140 CALL                     3
                            150 STORE_FAST               3 (response)
                
-                30         152 LOAD_FAST                3 (response)
+                26         152 LOAD_FAST                3 (response)
                            154 LOAD_METHOD              5 (json)
                            176 PRECALL                  0
                            180 CALL                     0
                            190 STORE_FAST               4 (data)
                
-                31         192 LOAD_GLOBAL             13 (NULL + print)
+                27         192 LOAD_GLOBAL             13 (NULL + print)
                            204 LOAD_CONST               6 ('find_similar:')
                            206 LOAD_FAST                4 (data)
                            208 PRECALL                  2
                            212 CALL                     2
                            222 POP_TOP
                
-                32         224 LOAD_FAST                4 (data)
+                28         224 LOAD_FAST                4 (data)
                            226 LOAD_METHOD              7 (get)
                            248 LOAD_CONST               7 ('results')
                            250 BUILD_LIST               0
                            252 PRECALL                  2
                            256 CALL                     2
                            266 LOAD_FAST                4 (data)
                            268 LOAD_CONST               8 ('companies')
                            270 STORE_SUBSCR
                
-                34         274 LOAD_FAST                4 (data)
+                30         274 LOAD_FAST                4 (data)
                            276 LOAD_CONST               8 ('companies')
                            278 BINARY_SUBSCR
                            288 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1/search-similar/'
                   'employees_range'
@@ -268,15 +246,15 @@
                   'companies'
                names      ('GrataWrapper', '_get_api_filter', 'requests', 'post', 'HEADERS', 'json', 'print', 'get')
                varnames   ('domain', 'search', 'api_filters', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
-               firstlineno 19
+               firstlineno 15
                lnotab 0x0201340116010201160202010e010efd04fd1209280120013202
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 11
                flags     : 3
                code
@@ -287,77 +265,77 @@
                   000000000000007c006a0600000000000000006403190000000000000000
                   007c016404190000000000000000007c016405190000000000000000007c
                   0164061900000000000000000064079c06ac08a6030000ab030000000000
                   0000007d027c02a0070000000000000000000000000000000000000000a6
                   000000ab0000000000000000007d0374110000000000000000000064097c
                   03a6020000ab02000000000000000001007c03640a190000000000000000
                   005300
-                36           0 RESUME                   0
+                32           0 RESUME                   0
                
-                37           2 LOAD_GLOBAL              0 (GrataWrapper)
+                33           2 LOAD_GLOBAL              0 (GrataWrapper)
                             14 LOAD_METHOD              1 (_get_api_filter)
                             36 LOAD_FAST                0 (search)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               1 (api_filters)
                
-                38          54 LOAD_GLOBAL              5 (NULL + requests)
+                34          54 LOAD_GLOBAL              5 (NULL + requests)
                             66 LOAD_ATTR                3 (post)
                
-                39          76 LOAD_CONST               1 ('https://search.grata.com/api/v1/search/')
+                35          76 LOAD_CONST               1 ('https://search.grata.com/api/v1/search/')
                
-                40          78 LOAD_GLOBAL              0 (GrataWrapper)
+                36          78 LOAD_GLOBAL              0 (GrataWrapper)
                             90 LOAD_ATTR                4 (HEADERS)
                
-                42         100 LOAD_CONST               2 ('any')
+                38         100 LOAD_CONST               2 ('any')
                
-                43         102 LOAD_FAST                0 (search)
+                39         102 LOAD_FAST                0 (search)
                            104 LOAD_ATTR                5 (inclusion)
                            114 LOAD_CONST               3 ('keywords')
                            116 BINARY_SUBSCR
                
-                44         126 LOAD_FAST                0 (search)
+                40         126 LOAD_FAST                0 (search)
                            128 LOAD_ATTR                6 (exclusion)
                            138 LOAD_CONST               3 ('keywords')
                            140 BINARY_SUBSCR
                
-                45         150 LOAD_FAST                1 (api_filters)
+                41         150 LOAD_FAST                1 (api_filters)
                            152 LOAD_CONST               4 ('employees_range')
                            154 BINARY_SUBSCR
                
-                46         164 LOAD_FAST                1 (api_filters)
+                42         164 LOAD_FAST                1 (api_filters)
                            166 LOAD_CONST               5 ('ownership')
                            168 BINARY_SUBSCR
                
-                47         178 LOAD_FAST                1 (api_filters)
+                43         178 LOAD_FAST                1 (api_filters)
                            180 LOAD_CONST               6 ('headquarters')
                            182 BINARY_SUBSCR
                
-                41         192 LOAD_CONST               7 (('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters'))
+                37         192 LOAD_CONST               7 (('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters'))
                            194 BUILD_CONST_KEY_MAP      6
                
-                38         196 KW_NAMES                 8
+                34         196 KW_NAMES                 8
                            198 PRECALL                  3
                            202 CALL                     3
                            212 STORE_FAST               2 (response)
                
-                50         214 LOAD_FAST                2 (response)
+                46         214 LOAD_FAST                2 (response)
                            216 LOAD_METHOD              7 (json)
                            238 PRECALL                  0
                            242 CALL                     0
                            252 STORE_FAST               3 (data)
                
-                51         254 LOAD_GLOBAL             17 (NULL + print)
+                47         254 LOAD_GLOBAL             17 (NULL + print)
                            266 LOAD_CONST               9 ('find_by_criteria: ')
                            268 LOAD_FAST                3 (data)
                            270 PRECALL                  2
                            274 CALL                     2
                            284 POP_TOP
                
-                52         286 LOAD_FAST                3 (data)
+                48         286 LOAD_FAST                3 (data)
                            288 LOAD_CONST              10 ('companies')
                            290 BINARY_SUBSCR
                            300 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1/search/'
                   'any'
@@ -371,81 +349,94 @@
                   'companies'
                names      ('GrataWrapper', '_get_api_filter', 'requests', 'post', 'HEADERS', 'inclusion', 'exclusion', 'json', 'print')
                varnames   ('search', 'api_filters', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_by_criteria'
-               firstlineno 36
+               firstlineno 32
                lnotab
                   0x020134011601020116020201180118010e010e010efa04fd120c280120
                   01
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000006401740400
                   0000000000000000006a03000000000000000064027c006901ac03a60300
                   00ab0300000000000000007d017c01a00400000000000000000000000000
                   00000000000000a6000000ab0000000000000000007d027c02a005000000
                   00000000000000000000000000000000006404a6010000ab010000000000
-                  0000007c0264053c0000007c025300
-                54           0 RESUME                   0
+                  0000007c0264053c0000007c02a005000000000000000000000000000000
+                  00000000006406a6010000ab0100000000000000007c0264073c0000007c
+                  025300
+                50           0 RESUME                   0
                
-                55           2 LOAD_GLOBAL              1 (NULL + requests)
+                51           2 LOAD_GLOBAL              1 (NULL + requests)
                             14 LOAD_ATTR                1 (post)
                
-                56          24 LOAD_CONST               1 ('https://search.grata.com/api/v1/enrich/')
+                52          24 LOAD_CONST               1 ('https://search.grata.com/api/v1/enrich/')
                
-                57          26 LOAD_GLOBAL              4 (GrataWrapper)
+                53          26 LOAD_GLOBAL              4 (GrataWrapper)
                             38 LOAD_ATTR                3 (HEADERS)
                
-                58          48 LOAD_CONST               2 ('domain')
+                54          48 LOAD_CONST               2 ('domain')
                             50 LOAD_FAST                0 (domain)
                             52 BUILD_MAP                1
                
-                55          54 KW_NAMES                 3
+                51          54 KW_NAMES                 3
                             56 PRECALL                  3
                             60 CALL                     3
                             70 STORE_FAST               1 (response)
                
-                60          72 LOAD_FAST                1 (response)
+                56          72 LOAD_FAST                1 (response)
                             74 LOAD_METHOD              4 (json)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 STORE_FAST               2 (data)
                
-                61         112 LOAD_FAST                2 (data)
+                57         112 LOAD_FAST                2 (data)
                            114 LOAD_METHOD              5 (get)
                            136 LOAD_CONST               4 ('social_linkedin')
                            138 PRECALL                  1
                            142 CALL                     1
                            152 LOAD_FAST                2 (data)
                            154 LOAD_CONST               5 ('linkedin')
                            156 STORE_SUBSCR
                
-                62         160 LOAD_FAST                2 (data)
-                           162 RETURN_VALUE
+                58         160 LOAD_FAST                2 (data)
+                           162 LOAD_METHOD              5 (get)
+                           184 LOAD_CONST               6 ('ownership_status')
+                           186 PRECALL                  1
+                           190 CALL                     1
+                           200 LOAD_FAST                2 (data)
+                           202 LOAD_CONST               7 ('ownership')
+                           204 STORE_SUBSCR
+               
+                59         208 LOAD_FAST                2 (data)
+                           210 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1/enrich/'
                   'domain'
                   ('headers', 'json')
                   'social_linkedin'
                   'linkedin'
+                  'ownership_status'
+                  'ownership'
                names      ('requests', 'post', 'GrataWrapper', 'HEADERS', 'json', 'get')
                varnames   ('domain', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 54
-               lnotab 0x020116010201160106fd120528013001
+               firstlineno 50
+               lnotab 0x020116010201160106fd1205280130013001
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 8
                flags     : 3
                code
                   0x8700870487059700690064016402930164036404930164056406930164
@@ -470,359 +461,359 @@
                   000000000002007c01a6000000ab00000000000000000002007c02a60000
                   00ab00000000000000000002007c03a6000000ab00000000000000000064
                   719c0264729c065300
                              0 MAKE_CELL                0 (search)
                              2 MAKE_CELL                4 (COUNTRIES)
                              4 MAKE_CELL                5 (STATES)
                
-                64           6 RESUME                   0
+                61           6 RESUME                   0
                
-                65           8 BUILD_MAP                0
+                62           8 BUILD_MAP                0
                
-                66          10 LOAD_CONST               1 ('AL')
+                63          10 LOAD_CONST               1 ('AL')
                             12 LOAD_CONST               2 ('Alabama')
                
-                65          14 MAP_ADD                  1
+                62          14 MAP_ADD                  1
                
-                67          16 LOAD_CONST               3 ('AK')
+                64          16 LOAD_CONST               3 ('AK')
                             18 LOAD_CONST               4 ('Alaska')
                
-                65          20 MAP_ADD                  1
+                62          20 MAP_ADD                  1
                
-                68          22 LOAD_CONST               5 ('AZ')
+                65          22 LOAD_CONST               5 ('AZ')
                             24 LOAD_CONST               6 ('Arizona')
                
-                65          26 MAP_ADD                  1
+                62          26 MAP_ADD                  1
                
-                69          28 LOAD_CONST               7 ('AR')
+                66          28 LOAD_CONST               7 ('AR')
                             30 LOAD_CONST               8 ('Arkansas')
                
-                65          32 MAP_ADD                  1
+                62          32 MAP_ADD                  1
                
-                70          34 LOAD_CONST               9 ('CA')
+                67          34 LOAD_CONST               9 ('CA')
                             36 LOAD_CONST              10 ('California')
                
-                65          38 MAP_ADD                  1
+                62          38 MAP_ADD                  1
                
-                71          40 LOAD_CONST              11 ('CO')
+                68          40 LOAD_CONST              11 ('CO')
                             42 LOAD_CONST              12 ('Colorado')
                
-                65          44 MAP_ADD                  1
+                62          44 MAP_ADD                  1
                
-                72          46 LOAD_CONST              13 ('CT')
+                69          46 LOAD_CONST              13 ('CT')
                             48 LOAD_CONST              14 ('Connecticut')
                
-                65          50 MAP_ADD                  1
+                62          50 MAP_ADD                  1
                
-                73          52 LOAD_CONST              15 ('DE')
+                70          52 LOAD_CONST              15 ('DE')
                             54 LOAD_CONST              16 ('Delaware')
                
-                65          56 MAP_ADD                  1
+                62          56 MAP_ADD                  1
                
-                74          58 LOAD_CONST              17 ('FL')
+                71          58 LOAD_CONST              17 ('FL')
                             60 LOAD_CONST              18 ('Florida')
                
-                65          62 MAP_ADD                  1
+                62          62 MAP_ADD                  1
                
-                75          64 LOAD_CONST              19 ('GA')
+                72          64 LOAD_CONST              19 ('GA')
                             66 LOAD_CONST              20 ('Georgia')
                
-                65          68 MAP_ADD                  1
+                62          68 MAP_ADD                  1
                
-                76          70 LOAD_CONST              21 ('HI')
+                73          70 LOAD_CONST              21 ('HI')
                             72 LOAD_CONST              22 ('Hawaii')
                
-                65          74 MAP_ADD                  1
+                62          74 MAP_ADD                  1
                
-                77          76 LOAD_CONST              23 ('ID')
+                74          76 LOAD_CONST              23 ('ID')
                             78 LOAD_CONST              24 ('Idaho')
                
-                65          80 MAP_ADD                  1
+                62          80 MAP_ADD                  1
                
-                78          82 LOAD_CONST              25 ('IL')
+                75          82 LOAD_CONST              25 ('IL')
                             84 LOAD_CONST              26 ('Illinois')
                
-                65          86 MAP_ADD                  1
+                62          86 MAP_ADD                  1
                
-                79          88 LOAD_CONST              27 ('IN')
+                76          88 LOAD_CONST              27 ('IN')
                             90 LOAD_CONST              28 ('Indiana')
                
-                65          92 MAP_ADD                  1
+                62          92 MAP_ADD                  1
                
-                80          94 LOAD_CONST              29 ('IA')
+                77          94 LOAD_CONST              29 ('IA')
                             96 LOAD_CONST              30 ('Iowa')
                
-                65          98 MAP_ADD                  1
+                62          98 MAP_ADD                  1
                
-                81         100 LOAD_CONST              31 ('KS')
+                78         100 LOAD_CONST              31 ('KS')
                            102 LOAD_CONST              32 ('Kansas')
                
-                65         104 MAP_ADD                  1
+                62         104 MAP_ADD                  1
                
-                82         106 LOAD_CONST              33 ('KY')
+                79         106 LOAD_CONST              33 ('KY')
                            108 LOAD_CONST              34 ('Kentucky')
                
-                65         110 MAP_ADD                  1
+                62         110 MAP_ADD                  1
                            112 BUILD_MAP                0
                
-                83         114 LOAD_CONST              35 ('LA')
+                80         114 LOAD_CONST              35 ('LA')
                            116 LOAD_CONST              36 ('Louisiana')
                
-                65         118 MAP_ADD                  1
+                62         118 MAP_ADD                  1
                
-                84         120 LOAD_CONST              37 ('ME')
+                81         120 LOAD_CONST              37 ('ME')
                            122 LOAD_CONST              38 ('Maine')
                
-                65         124 MAP_ADD                  1
+                62         124 MAP_ADD                  1
                
-                85         126 LOAD_CONST              39 ('MD')
+                82         126 LOAD_CONST              39 ('MD')
                            128 LOAD_CONST              40 ('Maryland')
                
-                65         130 MAP_ADD                  1
+                62         130 MAP_ADD                  1
                
-                86         132 LOAD_CONST              41 ('MA')
+                83         132 LOAD_CONST              41 ('MA')
                            134 LOAD_CONST              42 ('Massachusetts')
                
-                65         136 MAP_ADD                  1
+                62         136 MAP_ADD                  1
                
-                87         138 LOAD_CONST              43 ('MI')
+                84         138 LOAD_CONST              43 ('MI')
                            140 LOAD_CONST              44 ('Michigan')
                
-                65         142 MAP_ADD                  1
+                62         142 MAP_ADD                  1
                
-                88         144 LOAD_CONST              45 ('MN')
+                85         144 LOAD_CONST              45 ('MN')
                            146 LOAD_CONST              46 ('Minnesota')
                
-                65         148 MAP_ADD                  1
+                62         148 MAP_ADD                  1
                
-                89         150 LOAD_CONST              47 ('MS')
+                86         150 LOAD_CONST              47 ('MS')
                            152 LOAD_CONST              48 ('Mississippi')
                
-                65         154 MAP_ADD                  1
+                62         154 MAP_ADD                  1
                
-                90         156 LOAD_CONST              49 ('MO')
+                87         156 LOAD_CONST              49 ('MO')
                            158 LOAD_CONST              50 ('Missouri')
                
-                65         160 MAP_ADD                  1
+                62         160 MAP_ADD                  1
                
-                91         162 LOAD_CONST              51 ('MT')
+                88         162 LOAD_CONST              51 ('MT')
                            164 LOAD_CONST              52 ('Montana')
                
-                65         166 MAP_ADD                  1
+                62         166 MAP_ADD                  1
                
-                92         168 LOAD_CONST              53 ('NE')
+                89         168 LOAD_CONST              53 ('NE')
                            170 LOAD_CONST              54 ('Nebraska')
                
-                65         172 MAP_ADD                  1
+                62         172 MAP_ADD                  1
                
-                93         174 LOAD_CONST              55 ('NV')
+                90         174 LOAD_CONST              55 ('NV')
                            176 LOAD_CONST              56 ('Nevada')
                
-                65         178 MAP_ADD                  1
+                62         178 MAP_ADD                  1
                
-                94         180 LOAD_CONST              57 ('NH')
+                91         180 LOAD_CONST              57 ('NH')
                            182 LOAD_CONST              58 ('New Hampshire')
                
-                65         184 MAP_ADD                  1
+                62         184 MAP_ADD                  1
                
-                95         186 LOAD_CONST              59 ('NJ')
+                92         186 LOAD_CONST              59 ('NJ')
                            188 LOAD_CONST              60 ('New Jersey')
                
-                65         190 MAP_ADD                  1
+                62         190 MAP_ADD                  1
                
-                96         192 LOAD_CONST              61 ('NM')
+                93         192 LOAD_CONST              61 ('NM')
                            194 LOAD_CONST              62 ('New Mexico')
                
-                65         196 MAP_ADD                  1
+                62         196 MAP_ADD                  1
                
-                97         198 LOAD_CONST              63 ('NY')
+                94         198 LOAD_CONST              63 ('NY')
                            200 LOAD_CONST              64 ('New York')
                
-                65         202 MAP_ADD                  1
+                62         202 MAP_ADD                  1
                
-                98         204 LOAD_CONST              65 ('NC')
+                95         204 LOAD_CONST              65 ('NC')
                            206 LOAD_CONST              66 ('North Carolina')
                
-                65         208 MAP_ADD                  1
+                62         208 MAP_ADD                  1
                
-                99         210 LOAD_CONST              67 ('ND')
+                96         210 LOAD_CONST              67 ('ND')
                            212 LOAD_CONST              68 ('North Dakota')
                
-                65         214 MAP_ADD                  1
+                62         214 MAP_ADD                  1
                            216 DICT_UPDATE              1
                            218 BUILD_MAP                0
                
-               100         220 LOAD_CONST              69 ('OH')
+                97         220 LOAD_CONST              69 ('OH')
                            222 LOAD_CONST              70 ('Ohio')
                
-                65         224 MAP_ADD                  1
+                62         224 MAP_ADD                  1
                
-               101         226 LOAD_CONST              71 ('OK')
+                98         226 LOAD_CONST              71 ('OK')
                            228 LOAD_CONST              72 ('Oklahoma')
                
-                65         230 MAP_ADD                  1
+                62         230 MAP_ADD                  1
                
-               102         232 LOAD_CONST              73 ('OR')
+                99         232 LOAD_CONST              73 ('OR')
                            234 LOAD_CONST              74 ('Oregon')
                
-                65         236 MAP_ADD                  1
+                62         236 MAP_ADD                  1
                
-               103         238 LOAD_CONST              75 ('PA')
+               100         238 LOAD_CONST              75 ('PA')
                            240 LOAD_CONST              76 ('Pennsylvania')
                
-                65         242 MAP_ADD                  1
+                62         242 MAP_ADD                  1
                
-               104         244 LOAD_CONST              77 ('RI')
+               101         244 LOAD_CONST              77 ('RI')
                            246 LOAD_CONST              78 ('Rhode Island')
                
-                65         248 MAP_ADD                  1
+                62         248 MAP_ADD                  1
                
-               105         250 LOAD_CONST              79 ('SC')
+               102         250 LOAD_CONST              79 ('SC')
                            252 LOAD_CONST              80 ('South Carolina')
                
-                65         254 MAP_ADD                  1
+                62         254 MAP_ADD                  1
                
-               106         256 LOAD_CONST              81 ('SD')
+               103         256 LOAD_CONST              81 ('SD')
                            258 LOAD_CONST              82 ('South Dakota')
                
-                65         260 MAP_ADD                  1
+                62         260 MAP_ADD                  1
                
-               107         262 LOAD_CONST              83 ('TN')
+               104         262 LOAD_CONST              83 ('TN')
                            264 LOAD_CONST              84 ('Tennessee')
                
-                65         266 MAP_ADD                  1
+                62         266 MAP_ADD                  1
                
-               108         268 LOAD_CONST              85 ('TX')
+               105         268 LOAD_CONST              85 ('TX')
                            270 LOAD_CONST              86 ('Texas')
                
-                65         272 MAP_ADD                  1
+                62         272 MAP_ADD                  1
                
-               109         274 LOAD_CONST              87 ('UT')
+               106         274 LOAD_CONST              87 ('UT')
                            276 LOAD_CONST              88 ('Utah')
                
-                65         278 MAP_ADD                  1
+                62         278 MAP_ADD                  1
                
-               110         280 LOAD_CONST              89 ('VT')
+               107         280 LOAD_CONST              89 ('VT')
                            282 LOAD_CONST              90 ('Vermont')
                
-                65         284 MAP_ADD                  1
+                62         284 MAP_ADD                  1
                
-               111         286 LOAD_CONST              91 ('VA')
+               108         286 LOAD_CONST              91 ('VA')
                            288 LOAD_CONST              92 ('Virginia')
                
-                65         290 MAP_ADD                  1
+                62         290 MAP_ADD                  1
                
-               112         292 LOAD_CONST              93 ('WA')
+               109         292 LOAD_CONST              93 ('WA')
                            294 LOAD_CONST              94 ('Washington')
                
-                65         296 MAP_ADD                  1
+                62         296 MAP_ADD                  1
                
-               113         298 LOAD_CONST              95 ('WV')
+               110         298 LOAD_CONST              95 ('WV')
                            300 LOAD_CONST              96 ('West Virginia')
                
-                65         302 MAP_ADD                  1
+                62         302 MAP_ADD                  1
                
-               114         304 LOAD_CONST              97 ('WI')
+               111         304 LOAD_CONST              97 ('WI')
                            306 LOAD_CONST              98 ('Wisconsin')
                
-                65         308 MAP_ADD                  1
+                62         308 MAP_ADD                  1
                
-               115         310 LOAD_CONST              99 ('WY')
+               112         310 LOAD_CONST              99 ('WY')
                            312 LOAD_CONST             100 ('Wyoming')
                
-                65         314 MAP_ADD                  1
+                62         314 MAP_ADD                  1
                            316 DICT_UPDATE              1
                            318 STORE_DEREF              5 (STATES)
                
-               119         320 LOAD_CONST             101 ('United States')
+               116         320 LOAD_CONST             101 ('United States')
                
-               120         322 LOAD_CONST             102 ('Canada')
+               117         322 LOAD_CONST             102 ('Canada')
                
-               121         324 LOAD_CONST             103 ('Mexico')
+               118         324 LOAD_CONST             103 ('Mexico')
                
-               122         326 LOAD_CONST             104 ('United Kingdom')
+               119         326 LOAD_CONST             104 ('United Kingdom')
                
-               118         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
+               115         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
                            330 BUILD_CONST_KEY_MAP      4
                            332 STORE_DEREF              4 (COUNTRIES)
                
-               125         334 LOAD_CONST             106 ('return')
+               122         334 LOAD_CONST             106 ('return')
                            336 LOAD_GLOBAL              0 (dict)
                            348 BUILD_TUPLE              2
                            350 LOAD_CLOSURE             0 (search)
                            352 BUILD_TUPLE              1
-                           354 LOAD_CONST             107 (<code object _ownership_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 125>)
+                           354 LOAD_CONST             107 (<code object _ownership_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 122>)
                            356 MAKE_FUNCTION           12 (annotations, closure)
                            358 STORE_FAST               1 (_ownership_filter)
                
-               138         360 LOAD_CONST             106 ('return')
+               135         360 LOAD_CONST             106 ('return')
                            362 LOAD_GLOBAL              2 (list)
                            374 BUILD_TUPLE              2
                            376 LOAD_CLOSURE             4 (COUNTRIES)
                            378 LOAD_CLOSURE             5 (STATES)
                            380 LOAD_CLOSURE             0 (search)
                            382 BUILD_TUPLE              3
-                           384 LOAD_CONST             108 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 138>)
+                           384 LOAD_CONST             108 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 135>)
                            386 MAKE_FUNCTION           12 (annotations, closure)
                            388 STORE_FAST               2 (_hq_include)
                
-               147         390 LOAD_CONST             106 ('return')
+               144         390 LOAD_CONST             106 ('return')
                            392 LOAD_GLOBAL              2 (list)
                            404 BUILD_TUPLE              2
                            406 LOAD_CLOSURE             0 (search)
                            408 BUILD_TUPLE              1
-                           410 LOAD_CONST             109 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 147>)
+                           410 LOAD_CONST             109 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 144>)
                            412 MAKE_FUNCTION           12 (annotations, closure)
                            414 STORE_FAST               3 (_hq_exclude)
                
-               154         416 LOAD_CONST             110 ('any')
+               151         416 LOAD_CONST             110 ('any')
                
-               155         418 LOAD_DEREF               0 (search)
+               152         418 LOAD_DEREF               0 (search)
                            420 LOAD_ATTR                2 (inclusion)
                            430 LOAD_METHOD              3 (get)
                            452 LOAD_CONST             111 ('keywords')
                            454 BUILD_LIST               0
                            456 PRECALL                  2
                            460 CALL                     2
                
-               156         470 LOAD_DEREF               0 (search)
+               153         470 LOAD_DEREF               0 (search)
                            472 LOAD_ATTR                4 (exclusion)
                            482 LOAD_METHOD              3 (get)
                            504 LOAD_CONST             111 ('keywords')
                            506 BUILD_LIST               0
                            508 PRECALL                  2
                            512 CALL                     2
                
-               157         522 LOAD_DEREF               0 (search)
+               154         522 LOAD_DEREF               0 (search)
                            524 LOAD_ATTR                2 (inclusion)
                            534 LOAD_METHOD              3 (get)
                            556 LOAD_CONST             112 ('employees_range')
                            558 BUILD_LIST               0
                            560 PRECALL                  2
                            564 CALL                     2
                
-               158         574 PUSH_NULL
+               155         574 PUSH_NULL
                            576 LOAD_FAST                1 (_ownership_filter)
                            578 PRECALL                  0
                            582 CALL                     0
                
-               160         592 PUSH_NULL
+               157         592 PUSH_NULL
                            594 LOAD_FAST                2 (_hq_include)
                            596 PRECALL                  0
                            600 CALL                     0
                
-               161         610 PUSH_NULL
+               158         610 PUSH_NULL
                            612 LOAD_FAST                3 (_hq_exclude)
                            614 PRECALL                  0
                            618 CALL                     0
                
-               159         628 LOAD_CONST             113 (('include', 'exclude'))
+               156         628 LOAD_CONST             113 (('include', 'exclude'))
                            630 BUILD_CONST_KEY_MAP      2
                
-               153         632 LOAD_CONST             114 (('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters'))
+               150         632 LOAD_CONST             114 (('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters'))
                            634 BUILD_CONST_KEY_MAP      6
                            636 RETURN_VALUE
                consts
                   None
                   'AL'
                   'Alabama'
                   'AK'
@@ -939,22 +930,22 @@
                         000000000000007c00a6010000ab01000000000000000074030000000000
                         000000000089016a020000000000000000a0030000000000000000000000
                         00000000000000000064026700a6020000ab020000000000000000a60100
                         00ab0100000000000000007a0a0000a6010000ab01000000000000000053
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     125           2 RESUME                   0
+                     122           2 RESUME                   0
                      
-                     127           4 BUILD_LIST               0
+                     124           4 BUILD_LIST               0
                                    6 LOAD_CONST               1 (('bootstrapped', 'investor_backed', 'public', 'public_subsidiary', 'private_subsidiary', 'private_equity', 'private_equity_add_on'))
                                    8 LIST_EXTEND              1
                                   10 STORE_FAST               0 (OWNERSHIP)
                      
-                     136          12 LOAD_GLOBAL              1 (NULL + list)
+                     133          12 LOAD_GLOBAL              1 (NULL + list)
                                   24 LOAD_GLOBAL              3 (NULL + set)
                                   36 LOAD_FAST                0 (OWNERSHIP)
                                   38 PRECALL                  1
                                   42 CALL                     1
                                   52 LOAD_GLOBAL              3 (NULL + set)
                                   64 LOAD_DEREF               1 (search)
                                   66 LOAD_ATTR                2 (exclusion)
@@ -975,15 +966,15 @@
                         'ownership'
                      names      ('list', 'set', 'exclusion', 'get')
                      varnames   ('OWNERSHIP',)
                      freevars   ('search',)
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_ownership_filter'
-                     firstlineno 125
+                     firstlineno 122
                      lnotab 0x04020809
                   code
                      argcount  : 0
                      nlocals   : 3
                      stacksize : 6
                      flags     : 19
                      code
@@ -994,202 +985,202 @@
                         00000001008c2089056a000000000000000000a001000000000000000000
                         000000000000000000000064026700a6020000ab02000000000000000044
                         005d1f7d027c00a002000000000000000000000000000000000000000064
                         0289037c02190000000000000000006901a6010000ab0100000000000000
                         0001008c207c005300
                                    0 COPY_FREE_VARS           3
                      
-                     138           2 RESUME                   0
+                     135           2 RESUME                   0
                      
-                     139           4 BUILD_LIST               0
+                     136           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (include)
                      
-                     140           8 LOAD_DEREF               5 (search)
+                     137           8 LOAD_DEREF               5 (search)
                                   10 LOAD_ATTR                0 (inclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('state')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 GET_ITER
                              >>   62 FOR_ITER                31 (to 126)
                                   64 STORE_FAST               1 (state)
                      
-                     142          66 LOAD_FAST                0 (include)
+                     139          66 LOAD_FAST                0 (include)
                                   68 LOAD_METHOD              2 (append)
                                   90 LOAD_CONST               1 ('state')
                                   92 LOAD_DEREF               4 (STATES)
                                   94 LOAD_FAST                1 (state)
                                   96 BINARY_SUBSCR
                                  106 BUILD_MAP                1
                                  108 PRECALL                  1
                                  112 CALL                     1
                                  122 POP_TOP
                                  124 JUMP_BACKWARD           32 (to 62)
                      
-                     143     >>  126 LOAD_DEREF               5 (search)
+                     140     >>  126 LOAD_DEREF               5 (search)
                                  128 LOAD_ATTR                0 (inclusion)
                                  138 LOAD_METHOD              1 (get)
                                  160 LOAD_CONST               2 ('country')
                                  162 BUILD_LIST               0
                                  164 PRECALL                  2
                                  168 CALL                     2
                                  178 GET_ITER
                              >>  180 FOR_ITER                31 (to 244)
                                  182 STORE_FAST               2 (country)
                      
-                     144         184 LOAD_FAST                0 (include)
+                     141         184 LOAD_FAST                0 (include)
                                  186 LOAD_METHOD              2 (append)
                                  208 LOAD_CONST               2 ('country')
                                  210 LOAD_DEREF               3 (COUNTRIES)
                                  212 LOAD_FAST                2 (country)
                                  214 BINARY_SUBSCR
                                  224 BUILD_MAP                1
                                  226 PRECALL                  1
                                  230 CALL                     1
                                  240 POP_TOP
                                  242 JUMP_BACKWARD           32 (to 180)
                      
-                     145     >>  244 LOAD_FAST                0 (include)
+                     142     >>  244 LOAD_FAST                0 (include)
                                  246 RETURN_VALUE
                      consts
                         None
                         'state'
                         'country'
                      names      ('inclusion', 'get', 'append')
                      varnames   ('include', 'state', 'country')
                      freevars   ('COUNTRIES', 'STATES', 'search')
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_include'
-                     firstlineno 138
+                     firstlineno 135
                      lnotab 0x040104013a023c013a013c01
                   code
                      argcount  : 0
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007d0089026a000000000000000000a00100000000000000
                         0000000000000000000000000064016700a6020000ab0200000000000000
                         0044005d197d017c00a00200000000000000000000000000000000000000
                         0064017c016901a6010000ab01000000000000000001008c1a7c005300
                                    0 COPY_FREE_VARS           1
                      
-                     147           2 RESUME                   0
+                     144           2 RESUME                   0
                      
-                     148           4 BUILD_LIST               0
+                     145           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (exclude)
                      
-                     149           8 LOAD_DEREF               2 (search)
+                     146           8 LOAD_DEREF               2 (search)
                                   10 LOAD_ATTR                0 (exclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('state')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 GET_ITER
                              >>   62 FOR_ITER                25 (to 114)
                                   64 STORE_FAST               1 (state)
                      
-                     150          66 LOAD_FAST                0 (exclude)
+                     147          66 LOAD_FAST                0 (exclude)
                                   68 LOAD_METHOD              2 (append)
                                   90 LOAD_CONST               1 ('state')
                                   92 LOAD_FAST                1 (state)
                                   94 BUILD_MAP                1
                                   96 PRECALL                  1
                                  100 CALL                     1
                                  110 POP_TOP
                                  112 JUMP_BACKWARD           26 (to 62)
                      
-                     151     >>  114 LOAD_FAST                0 (exclude)
+                     148     >>  114 LOAD_FAST                0 (exclude)
                                  116 RETURN_VALUE
                      consts
                         None
                         'state'
                      names      ('exclusion', 'get', 'append')
                      varnames   ('exclude', 'state')
                      freevars   ('search',)
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_exclude'
-                     firstlineno 147
+                     firstlineno 144
                      lnotab 0x040104013a013001
                   'any'
                   'keywords'
                   'employees_range'
                   ('include', 'exclude')
                   ('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters')
                names      ('dict', 'list', 'inclusion', 'get', 'exclusion')
                varnames   ('search', '_ownership_filter', '_hq_include', '_hq_exclude')
                freevars   ()
                cellvars   ('search', 'COUNTRIES', 'STATES')
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       '_get_api_filter'
-               firstlineno 64
+               firstlineno 61
                lnotab
                   0x0801020104ff020204fe020304fd020404fc020504fb020604fa020704
                   f9020804f8020904f7020a04f6020b04f5020c04f4020d04f3020e04f202
                   0f04f1021004f0021104ef041204ee021304ed021404ec021504eb021604
                   ea021704e9021804e8021904e7021a04e6021b04e5021c04e4021d04e302
                   1e04e2021f04e1022004e0022104df022204de062304dd022404dc022504
                   db022604da022704d9022804d8022904d7022a04d6022b04d5022c04d402
                   2d04d3022e04d2022f04d1023004d0023104cf023204ce06360201020102
                   0102fc06071a0d1e091a0702013401340134011202120112fe04fa
             None
-         names      ('__name__', '__module__', '__qualname__', 'os', 'getenv', 'HEADERS', 'str', 'Search', 'list', 'find_similar', 'dict', 'find_by_criteria', 'enrich', '_get_api_filter')
+         names      ('__name__', '__module__', '__qualname__', 'access_secret_version', 'HEADERS', 'str', 'Search', 'list', 'find_similar', 'dict', 'find_by_criteria', 'enrich', '_get_api_filter')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'GrataWrapper'
-         firstlineno 10
-         lnotab 0x0a021e0102fe0605060314111012100a
+         firstlineno 6
+         lnotab 0x0a02140102fe0605060314111012100b
       'GrataWrapper'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a026401650364026504640365056606640484045a
             0664026504640365056604640584045a0764016503640365056604640684
             045a0864075300
-         166           0 RESUME                   0
+         163           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SourceScrubWrapper')
                        8 STORE_NAME               2 (__qualname__)
          
-         167          10 LOAD_CONST               1 ('domain')
+         164          10 LOAD_CONST               1 ('domain')
                       12 LOAD_NAME                3 (str)
                       14 LOAD_CONST               2 ('search')
                       16 LOAD_NAME                4 (Search)
                       18 LOAD_CONST               3 ('return')
                       20 LOAD_NAME                5 (dict)
                       22 BUILD_TUPLE              6
-                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 167>)
+                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 164>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               6 (find_similar)
          
-         170          30 LOAD_CONST               2 ('search')
+         167          30 LOAD_CONST               2 ('search')
                       32 LOAD_NAME                4 (Search)
                       34 LOAD_CONST               3 ('return')
                       36 LOAD_NAME                5 (dict)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 170>)
+                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 167>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_NAME               7 (find_by_criteria)
          
-         173          46 LOAD_CONST               1 ('domain')
+         170          46 LOAD_CONST               1 ('domain')
                       48 LOAD_NAME                3 (str)
                       50 LOAD_CONST               3 ('return')
                       52 LOAD_NAME                5 (dict)
                       54 BUILD_TUPLE              4
-                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 173>)
+                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 170>)
                       58 MAKE_FUNCTION            4 (annotations)
                       60 STORE_NAME               8 (enrich)
                       62 LOAD_CONST               7 (None)
                       64 RETURN_VALUE
          consts
             'SourceScrubWrapper'
             'domain'
@@ -1197,79 +1188,79 @@
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               167           0 RESUME                   0
+               164           0 RESUME                   0
                
-               168           2 LOAD_CONST               0 (None)
+               165           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain', 'search')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
-               firstlineno 167
+               firstlineno 164
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               170           0 RESUME                   0
+               167           0 RESUME                   0
                
-               171           2 LOAD_CONST               0 (None)
+               168           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('search',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_by_criteria'
-               firstlineno 170
+               firstlineno 167
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               173           0 RESUME                   0
+               170           0 RESUME                   0
                
-               174           2 LOAD_CONST               0 (None)
+               171           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 173
+               firstlineno 170
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'str', 'Search', 'dict', 'find_similar', 'find_by_criteria', 'enrich')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'SourceScrubWrapper'
-         firstlineno 166
+         firstlineno 163
          lnotab 0x0a0114031003
       'SourceScrubWrapper'
-   names      ('gandai', 'query', 'gandai.models', 'Search', 'requests', 'os', 'dotenv', 'load_dotenv', 'GrataWrapper', 'SourceScrubWrapper')
+   names      ('gandai.secrets', 'access_secret_version', 'gandai.models', 'Search', 'requests', 'GrataWrapper', 'SourceScrubWrapper')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c01080108010c0214031a7f001d
+   lnotab 0x00ff02010c010c0208021a7f001e
```

### Comparing `gandai-1.1.9/gandai/datastore.py` & `gandai-1.2.0/gandai/datastore.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 import json
 import os
 from concurrent.futures import ThreadPoolExecutor
 
 from typing import Any, Dict, List
 from google.cloud import storage
 import os
-# from dotenv import load_dotenv
-# load_dotenv()
+from dotenv import load_dotenv
+load_dotenv()
 
 class Cloudstore:
     def __init__(self):
-        GCP_PROJECT = os.getenv("GCP_PROJECT", "gandai-prod")
-        GCP_STAGE = os.getenv("GCP_STAGE", "prod")
-        self.BUCKET_NAME = f"{GCP_PROJECT}-{GCP_STAGE}"
+        GCP_PROJECT = os.getenv("PROJECT_ID")
+        self.BUCKET_NAME = f"{GCP_PROJECT}"
         self.client = storage.Client(project=GCP_PROJECT)
         self.bucket = self.client.get_bucket(self.BUCKET_NAME)
 
     def keys(self, prefix="") -> List[str]:
         keys = [
             blob.name
             for blob in self.client.list_blobs(self.BUCKET_NAME, prefix=prefix)
```

### Comparing `gandai-1.1.9/gandai/main.py` & `gandai-1.2.0/gandai/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,90 @@
 import pandas as pd
 from dacite import from_dict
 from dataclasses import dataclass, field
 from concurrent.futures import ThreadPoolExecutor
+from time import time
+
 
 from gandai.models import Event, Company, Checkpoint
 from gandai import query
-
 from gandai.sources import GrataWrapper as grata
 
 
 def process_event(event_id: int) -> None:
     """
     May trigger additional targets adding to inbox, or something else
     (e.g. a notification)
     """
-
-    def _insert_companies(companies: list, existing_domains: list) -> None:
-        # rewrite this in less db txns
-        for company in companies:
-            if company.get("domain") is None:
-                print(f"Missing domain: {company}. Skipping")
-                continue
-
-            if company["domain"] in existing_domains:
-                print(f"Skipping {company['domain']} as already a target")
-                continue
-            print(f"Adding {company['domain']} as target")
-            query.insert_company(
-                Company(
-                    domain=company["domain"],
-                    name=company.get("name"),
-                    description=company.get("description"),
-                )
-            )
-            query.insert_event(
-                Event(
-                    search_uid=search_uid,
-                    domain=company.get("domain"),
-                    actor_key="grata",
-                    type="create",
-                )
-            )
-
-    # sets up better to do this threaded
+    
     e = query.find_event_by_id(event_id)
     search_uid = e.search_uid
+
     if e.type == "create":
         pass
     elif e.type == "advance":
         # enrich the company
         company = query.find_company_by_domain(e.domain)
-        # might consider a check here to see if the company is already enriched
-        resp = grata.enrich(company.domain)
-        if resp.get("status") == 404:
-            print(f"{company} not found")
+        
+        if len(company.meta.keys()) < 10:
+            # adding this check to mitigate API usage
+            # revisit this number
+            resp = grata.enrich(company.domain)
+            if resp.get("status") == 404:
+                print(f"{company} not found") # are we charged for "not found"?
+            else:
+                print(resp)
+                company.name = resp.get("name")
+                company.description = resp.get("description")
+                company.meta = {**company.meta, **resp}  # merge 3.5+
+                query.update_company(company)
         else:
-            print(resp)
-            company.name = resp.get("name")
-            company.description = resp.get("description")
-            company.meta = {**company.meta, **resp}  # merge 3.5+
-            query.update_company(company)
+            print(f"{company} already enriched.")
 
     elif e.type == "validate":
         search = query.find_search_by_uid(search_uid)
-        _insert_companies(
-            companies=grata.find_similar(domain=e.domain, search=search),
-            existing_domains=query.target(search_uid=search_uid)["domain"].tolist(),
+        grata_companies = grata.find_similar(domain=e.domain, search=search)
+        query.insert_companies_as_targets(
+            companies=grata_companies, search_uid=search_uid, actor_key="grata"
         )
+        # subscribers (which could be a virtual) could get a notification here
     elif e.type == "send":
         pass
     elif e.type == "accept":
         pass
     elif e.type == "reject":
         pass
     elif e.type == "conflict":
         pass
     elif e.type == "criteria":
-        print("criteria search here we gooo")
+        print(f"criteria search for {search_uid}")
         search = query.find_search_by_uid(search_uid)
-        _insert_companies(
-            companies=grata.find_by_criteria(search),
-            existing_domains=query.target(search_uid=search_uid)["domain"].tolist(),
+        grata_companies = grata.find_by_criteria(search)
+        query.insert_companies_as_targets(
+            companies=grata_companies, search_uid=search_uid, actor_key="grata"
         )
-
+        
     # finally, record we processed the event
+    # could make these async
     query.insert_checkpoint(Checkpoint(event_id=e.id))
     print(f"processed: {e}")
 
 
 def process_events(search_uid: int) -> int:
     """
     Process all events for a given search
     """
 
     events = query.event(search_uid=search_uid)
     checkpoints = query.checkpoint(search_uid=search_uid)
 
     q = list(set(events["id"].tolist()) - set(checkpoints["event_id"].tolist()))
-    
+
     for event_id in q:
         print(event_id)
         process_event(event_id)
+
+    # 
     # with ThreadPoolExecutor(max_workers=4) as executor:
     #     executor.map(process_event, q)
-    
+
     return len(q)
```

### Comparing `gandai-1.1.9/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.2.0/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x391c6164 (Sun May 14 17:36:57 2023 UTC)
+moddate:  0x5ba76c64 (Tue May 23 11:45:31 2023 UTC)
 files sz: 3257
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `gandai-1.1.9/gandai/migrations/db_seed.py` & `gandai-1.2.0/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.9/gandai/migrations/dealcloud.py` & `gandai-1.2.0/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.9/gandai/migrations/sql/schema.sql` & `gandai-1.2.0/gandai/migrations/sql/schema.sql`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 CREATE INDEX idx_event_search_uid ON event(search_uid);
 ALTER TABLE event ADD CONSTRAINT unique_event_type_domain_search_uid_created UNIQUE (type, domain, search_uid, created);
 
 
 CREATE TABLE IF NOT EXISTS checkpoint (
     id SERIAL PRIMARY KEY,
-    event_id INTEGER NOT NULL REFERENCES event(id),
+    event_id INTEGER NOT NULL REFERENCES event(id) ON DELETE CASCADE,
     created BIGINT NOT NULL DEFAULT FLOOR(EXTRACT(EPOCH FROM NOW()))
 );
 
 CREATE MATERIALIZED VIEW IF NOT EXISTS target AS
 SELECT 
     e.id, 
     e.search_uid, 
@@ -62,15 +62,15 @@
     e.type AS last_event_type, 
     e.created AS last_event_dt,
     c.name as name,
     c.uid as dealcloud_id,
     c.description as description,
     c.meta as meta,
     (c.meta->>'employees') AS employees,
-    (c.meta->>'ownership_status') AS ownership,
+    (c.meta->>'ownership') AS ownership,
     (c.meta->>'linkedin') AS linkedin,    
     (r.data->>'rating') AS rating
 FROM (
     SELECT 
         domain, 
         MAX(created) AS max_created
     FROM
```

### Comparing `gandai-1.1.9/gandai/models.py` & `gandai-1.2.0/gandai/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @dataclass(order=True)
 class Company:
     domain: str  # unique
     name: Optional[str] = None
     description: Optional[str] = None
     meta: dict = field(default_factory=dict)
     id: int = field(default=None)  # primary key
-    uid: int = field(default=None)  # foreign key
+    uid: Optional[int] = field(default=None)  # foreign key
 
 
 class EventType(str, Enum):
     CREATE = auto()
     ADVANCE = auto()
     VALIDATE = auto()
     SEND = auto()
```

### Comparing `gandai-1.1.9/gandai/query.py` & `gandai-1.2.0/gandai/query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import pandas as pd
+from typing import List, Any
 from dataclasses import asdict
 from dacite import from_dict
 from gandai.models import (
     Event,
     Company,
     EventType,
     Actor,
@@ -105,14 +106,119 @@
             """
         )
         con.execute(statement, asdict(checkpoint))
         con.commit()
     return checkpoint
 
 
+def insert_and_advance_targets_from_domains(
+    domains: List[str], search_uid: int, actor_key: str
+) -> None:
+    """
+    Takes in domains, inserts targets into a review stage, where they will
+    try to be enriched on process event
+
+    """
+    targets = target(search_uid=search_uid)
+    with db.connect() as con:
+        for domain in domains:
+            # consider upstream formatter/validator
+            domain = (
+                domain.lower()
+                .strip()
+                .replace("www.", "")
+                .replace("https://", "")
+                .replace("https://", "")
+            )
+            if targets['domain'].str.contains(domain).any():
+                print(f"Skipping {domain} as already a target")
+                continue
+            else:
+                print(f"Adding {domain} as target")
+
+            con.execute(
+                sqlalchemy.text(
+                    """
+                    INSERT INTO company (domain) 
+                    VALUES(:domain)
+                    ON CONFLICT DO NOTHING
+                    """
+                ),
+                {"domain": domain},
+            )
+
+            con.execute(
+                sqlalchemy.text(
+                    """
+                    INSERT INTO event (search_uid, domain, actor_key, type) 
+                    VALUES(:search_uid, :domain, :actor_key, :type)
+                    """
+                ),
+                {
+                    "search_uid": search_uid,
+                    "actor_key": actor_key,
+                    "domain": domain,
+                    "type": "advance",
+                },
+            )
+        con.execute(sqlalchemy.text("REFRESH MATERIALIZED VIEW target"))
+        con.commit()
+
+
+def insert_companies_as_targets(
+    companies: List[Any], search_uid: int, actor_key: str
+) -> None:
+    targets = target(search_uid=search_uid)
+    with db.connect() as con:
+        for company in companies:
+            if company.get("domain") is None:
+                print(f"Missing domain: {company}. Skipping")
+                continue
+
+            # elif company["domain"] in targets["domain"]:
+            elif targets['domain'].str.contains(company['domain']).any():
+                print(f"Skipping {company['domain']} as already a target")
+                continue
+            else:
+                print(f"Adding {company['domain']} as target")
+
+            con.execute(
+                sqlalchemy.text(
+                    """
+                    INSERT INTO company (domain, name, description) 
+                    VALUES(:domain, :name, :description)
+                    ON CONFLICT DO NOTHING
+                    """
+                ),
+                {
+                    "domain": company.get("domain"),
+                    "name": company.get("name"),
+                    "description": company.get("description"),
+                },
+            )
+
+            con.execute(
+                sqlalchemy.text(
+                    """
+                    INSERT INTO event (search_uid, domain, actor_key, type) 
+                    VALUES(:search_uid, :domain, :actor_key, :type)
+                    """
+                ),
+                {
+                    "search_uid": search_uid,
+                    "actor_key": actor_key,
+                    "domain": company.get("domain"),
+                    "type": "create",
+                },
+            )
+        
+        con.execute(sqlalchemy.text("REFRESH MATERIALIZED VIEW target"))
+        con.commit()
+
+
 ### READS ###
 
 
 def search():
     with db.connect() as conn:
         result = conn.execute(
             sqlalchemy.text("SELECT *, meta->>'group' as group FROM search")
@@ -268,14 +374,15 @@
         # obj = dict(zip(result.keys(), result.fetchone()))
     if result.rowcount == 0:
         return None
     else:
         obj = dict(zip(result.keys(), result.fetchone()))
         return from_dict(Event, obj)
 
+
 ### UPDATE ###
 
 
 def update_company(company: Company) -> None:
     with db.connect() as conn:
         statement = """
             UPDATE company
```

### Comparing `gandai-1.1.9/gandai/sources.py` & `gandai-1.2.0/gandai/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from gandai import query
+from gandai.secrets import access_secret_version
 from gandai.models import Search
-import requests
-import os
-from dotenv import load_dotenv
-
-load_dotenv()
 
+import requests
 
 class GrataWrapper:
     HEADERS = {
-        "Authorization": os.getenv("GRATA_API_TOKEN"),
+        "Authorization": access_secret_version("GRATA_API_TOKEN"),
         "Content-Type": "application/json",
     }
 
     def __name__(self):
         return "GrataWrapper"
 
     def find_similar(domain: str, search: Search) -> list:
```

### Comparing `gandai-1.1.9/gandai.egg-info/SOURCES.txt` & `gandai-1.2.0/gandai.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 gandai/__init__.py
 gandai/auth.py
 gandai/datastore.py
 gandai/db.py
 gandai/main.py
 gandai/models.py
 gandai/query.py
+gandai/secrets.py
 gandai/sources.py
 gandai.egg-info/PKG-INFO
 gandai.egg-info/SOURCES.txt
 gandai.egg-info/dependency_links.txt
 gandai.egg-info/top_level.txt
 gandai/__pycache__/__init__.cpython-311.pyc
 gandai/__pycache__/adapters.cpython-311.pyc
 gandai/__pycache__/auth.cpython-311.pyc
 gandai/__pycache__/datastore.cpython-311.pyc
 gandai/__pycache__/db.cpython-311.pyc
 gandai/__pycache__/grata.cpython-311.pyc
 gandai/__pycache__/main.cpython-311.pyc
 gandai/__pycache__/models.cpython-311.pyc
 gandai/__pycache__/query.cpython-311.pyc
+gandai/__pycache__/secrets.cpython-311.pyc
 gandai/__pycache__/services.cpython-311.pyc
 gandai/__pycache__/sources.cpython-311.pyc
 gandai/migrations/__init__.py
 gandai/migrations/db_create.py
 gandai/migrations/db_seed.py
 gandai/migrations/dealcloud.py
 gandai/migrations/__pycache__/__init__.cpython-311.pyc
 gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+gandai/migrations/sql/2305023-alter.sql
 gandai/migrations/sql/schema.sql
```

