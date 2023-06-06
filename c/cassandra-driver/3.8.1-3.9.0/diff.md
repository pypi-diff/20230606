# Comparing `tmp/cassandra-driver-3.8.1.tar.gz` & `tmp/cassandra-driver-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cassandra-driver-3.8.1.tar", last modified: Thu Mar 16 18:10:37 2017, max compression
+gzip compressed data, was "dist/cassandra-driver-3.9.0.tar", last modified: Tue Apr 11 18:11:22 2017, max compression
```

## Comparing `cassandra-driver-3.8.1.tar` & `cassandra-driver-3.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 mambocab  (1000) mambocab  (1000)        0 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    10174 2017-02-15 15:28:44.000000 cassandra-driver-3.8.1/LICENSE
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     5970 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/PKG-INFO
-drwxrwxr-x   0 mambocab  (1000) mambocab  (1000)        0 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/cassandra_driver.egg-info/
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)       16 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/cassandra_driver.egg-info/top_level.txt
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     5970 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/cassandra_driver.egg-info/PKG-INFO
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1653 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/cassandra_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)       18 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/cassandra_driver.egg-info/requires.txt
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)        1 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/cassandra_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)       38 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/setup.cfg
-drwxrwxr-x   0 mambocab  (1000) mambocab  (1000)        0 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/cassandra/
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2053 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/row_parser.pyx
-drwxrwxr-x   0 mambocab  (1000) mambocab  (1000)        0 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/cassandra/io/
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     4998 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/io/eventletreactor.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    11912 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/io/libevreactor.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    22348 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/io/libevwrapper.c
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    12125 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/io/asyncorereactor.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     4303 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/io/geventreactor.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     7996 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/io/twistedreactor.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      580 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/io/__init__.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    35173 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqltypes.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     9437 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/concurrent.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)   170900 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cluster.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1591 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/tuple.pxd
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    28846 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/pool.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2062 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cython_utils.pyx
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     5865 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/numpy_parser.pyx
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2994 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/obj_parser.pyx
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2387 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/murmur3.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1951 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/type_codes.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     6548 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/metrics.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)       50 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/numpyFlags.h
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    16441 2017-03-16 17:54:22.000000 cassandra-driver-3.8.1/cassandra/__init__.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     6526 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cmurmur3.c
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1648 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/ioutils.pyx
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    38213 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/util.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     6151 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/auth.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1711 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/bytesio.pyx
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    16927 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/deserializers.pyx
-drwxrwxr-x   0 mambocab  (1000) mambocab  (1000)        0 2017-03-16 18:10:37.000000 cassandra-driver-3.8.1/cassandra/cqlengine/
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     4727 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/named.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    30209 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/columns.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    22842 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/management.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     6862 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/usertype.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      983 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/__init__.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    38099 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/models.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2362 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/operators.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    13509 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/connection.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    53834 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/query.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    28541 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/statements.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     3934 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cqlengine/functions.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      977 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/type_codes.pxd
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2450 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cython_marshal.pyx
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    42216 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/connection.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    38153 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/query.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      220 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cython_deps.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     7889 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/encoder.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1819 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/buffer.pxd
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      753 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/bytesio.pxd
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     3918 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/timestamps.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1693 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/deserializers.pxd
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    35030 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/policies.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    42525 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/protocol.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     4391 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/marshal.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1433 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/parsing.pyx
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    96852 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/metadata.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1048 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/parsing.pxd
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)       80 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/cassandra/cython_utils.pxd
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    16451 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/setup.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      195 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/MANIFEST.in
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     8596 2017-01-13 16:49:18.000000 cassandra-driver-3.8.1/ez_setup.py
--rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     4338 2017-03-16 17:39:48.000000 cassandra-driver-3.8.1/README.rst
+drwxrwxr-x   0 mambocab  (1000) mambocab  (1000)        0 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    10174 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/LICENSE
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     5970 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/PKG-INFO
+drwxrwxr-x   0 mambocab  (1000) mambocab  (1000)        0 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/cassandra_driver.egg-info/
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)       16 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/cassandra_driver.egg-info/top_level.txt
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     5970 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/cassandra_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1653 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/cassandra_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)       18 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/cassandra_driver.egg-info/requires.txt
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)        1 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/cassandra_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)       38 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/setup.cfg
+drwxrwxr-x   0 mambocab  (1000) mambocab  (1000)        0 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/cassandra/
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2053 2017-03-31 19:23:02.000000 cassandra-driver-3.9.0/cassandra/row_parser.pyx
+drwxrwxr-x   0 mambocab  (1000) mambocab  (1000)        0 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/cassandra/io/
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     5201 2017-03-31 19:33:53.000000 cassandra-driver-3.9.0/cassandra/io/eventletreactor.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    11912 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/io/libevreactor.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    22348 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/io/libevwrapper.c
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    12125 2017-03-31 19:23:02.000000 cassandra-driver-3.9.0/cassandra/io/asyncorereactor.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     4303 2017-03-31 19:33:53.000000 cassandra-driver-3.9.0/cassandra/io/geventreactor.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     7996 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/io/twistedreactor.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      580 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/io/__init__.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    35173 2017-04-06 14:05:50.000000 cassandra-driver-3.9.0/cassandra/cqltypes.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     9437 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/concurrent.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)   172307 2017-04-11 17:54:07.000000 cassandra-driver-3.9.0/cassandra/cluster.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1591 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/tuple.pxd
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    28846 2017-03-31 19:33:53.000000 cassandra-driver-3.9.0/cassandra/pool.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2062 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cython_utils.pyx
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     5865 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/numpy_parser.pyx
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2994 2017-03-31 19:23:02.000000 cassandra-driver-3.9.0/cassandra/obj_parser.pyx
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2387 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/murmur3.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1951 2017-03-31 19:23:02.000000 cassandra-driver-3.9.0/cassandra/type_codes.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     6548 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/metrics.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)       50 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/numpyFlags.h
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    16441 2017-04-11 18:00:02.000000 cassandra-driver-3.9.0/cassandra/__init__.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     6526 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cmurmur3.c
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1648 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/ioutils.pyx
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    38213 2017-03-31 19:33:53.000000 cassandra-driver-3.9.0/cassandra/util.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     6151 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/auth.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1711 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/bytesio.pyx
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    16927 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/deserializers.pyx
+drwxrwxr-x   0 mambocab  (1000) mambocab  (1000)        0 2017-04-11 18:11:22.000000 cassandra-driver-3.9.0/cassandra/cqlengine/
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     4727 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cqlengine/named.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    30729 2017-04-05 21:24:49.000000 cassandra-driver-3.9.0/cassandra/cqlengine/columns.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    22842 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cqlengine/management.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     6862 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cqlengine/usertype.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      983 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cqlengine/__init__.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    38505 2017-04-11 17:54:07.000000 cassandra-driver-3.9.0/cassandra/cqlengine/models.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2362 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cqlengine/operators.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    13612 2017-03-31 19:33:53.000000 cassandra-driver-3.9.0/cassandra/cqlengine/connection.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    54581 2017-04-05 21:24:49.000000 cassandra-driver-3.9.0/cassandra/cqlengine/query.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    28947 2017-04-04 18:17:14.000000 cassandra-driver-3.9.0/cassandra/cqlengine/statements.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     3934 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cqlengine/functions.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      977 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/type_codes.pxd
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     2450 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cython_marshal.pyx
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    42216 2017-03-31 19:23:02.000000 cassandra-driver-3.9.0/cassandra/connection.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    38153 2017-03-31 19:23:02.000000 cassandra-driver-3.9.0/cassandra/query.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      220 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cython_deps.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     7889 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/encoder.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1819 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/buffer.pxd
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      753 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/bytesio.pxd
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     3919 2017-03-31 19:33:53.000000 cassandra-driver-3.9.0/cassandra/timestamps.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1693 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/deserializers.pxd
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    35030 2017-03-31 19:23:02.000000 cassandra-driver-3.9.0/cassandra/policies.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    42525 2017-03-31 19:23:02.000000 cassandra-driver-3.9.0/cassandra/protocol.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     4391 2017-03-31 19:33:53.000000 cassandra-driver-3.9.0/cassandra/marshal.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1433 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/parsing.pyx
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    96852 2017-03-31 19:33:53.000000 cassandra-driver-3.9.0/cassandra/metadata.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     1048 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/parsing.pxd
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)       80 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/cassandra/cython_utils.pxd
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)    16451 2017-03-31 19:23:02.000000 cassandra-driver-3.9.0/setup.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)      195 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/MANIFEST.in
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     8596 2017-03-16 18:36:02.000000 cassandra-driver-3.9.0/ez_setup.py
+-rw-rw-r--   0 mambocab  (1000) mambocab  (1000)     4338 2017-03-31 19:23:02.000000 cassandra-driver-3.9.0/README.rst
```

### Comparing `cassandra-driver-3.8.1/LICENSE` & `cassandra-driver-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/PKG-INFO` & `cassandra-driver-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cassandra-driver
-Version: 3.8.1
+Version: 3.9.0
 Summary: Python driver for Cassandra
 Home-page: http://github.com/datastax/python-driver
 Author: Tyler Hobbs
 Author-email: tyler@datastax.com
 License: UNKNOWN
 Description: DataStax Python Driver for Apache Cassandra
         ===========================================
```

### Comparing `cassandra-driver-3.8.1/cassandra_driver.egg-info/PKG-INFO` & `cassandra-driver-3.9.0/cassandra_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cassandra-driver
-Version: 3.8.1
+Version: 3.9.0
 Summary: Python driver for Cassandra
 Home-page: http://github.com/datastax/python-driver
 Author: Tyler Hobbs
 Author-email: tyler@datastax.com
 License: UNKNOWN
 Description: DataStax Python Driver for Apache Cassandra
         ===========================================
```

### Comparing `cassandra-driver-3.8.1/cassandra_driver.egg-info/SOURCES.txt` & `cassandra-driver-3.9.0/cassandra_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/row_parser.pyx` & `cassandra-driver-3.9.0/cassandra/row_parser.pyx`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/io/eventletreactor.py` & `cassandra-driver-3.9.0/cassandra/io/eventletreactor.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 # Originally derived from MagnetoDB source:
 #   https://github.com/stackforge/magnetodb/blob/2015.1.0b1/magnetodb/common/cassandra/io/eventletreactor.py
 
 import eventlet
 from eventlet.green import socket
 from eventlet.queue import Queue
+from greenlet import GreenletExit
 import logging
 from threading import Event
 import time
 
 from six.moves import xrange
 
 from cassandra.connection import Connection, ConnectionShutdown, Timer, TimerManager
@@ -76,15 +77,14 @@
             next_end = timer_manager.service_timeouts()
             sleep_time = max(next_end - time.time(), 0) if next_end else 10000
             cls._new_timer.wait(sleep_time)
             cls._new_timer.clear()
 
     def __init__(self, *args, **kwargs):
         Connection.__init__(self, *args, **kwargs)
-
         self._write_queue = Queue()
 
         self._connect_socket()
 
         self._read_watcher = eventlet.spawn(lambda: self.handle_read())
         self._write_watcher = eventlet.spawn(lambda: self.handle_write())
         self._send_options_message()
@@ -122,25 +122,29 @@
             try:
                 next_msg = self._write_queue.get()
                 self._socket.sendall(next_msg)
             except socket.error as err:
                 log.debug("Exception during socket send for %s: %s", self, err)
                 self.defunct(err)
                 return  # Leave the write loop
+            except GreenletExit:  # graceful greenthread exit
+                return
 
     def handle_read(self):
         while True:
             try:
                 buf = self._socket.recv(self.in_buffer_size)
                 self._iobuf.write(buf)
             except socket.error as err:
                 log.debug("Exception during socket recv for %s: %s",
                           self, err)
                 self.defunct(err)
                 return  # leave the read loop
+            except GreenletExit:  # graceful greenthread exit
+                return
 
             if buf and self._iobuf.tell():
                 self.process_io_buffer()
             else:
                 log.debug("Connection %s closed by server", self)
                 self.close()
                 return
```

### Comparing `cassandra-driver-3.8.1/cassandra/io/libevreactor.py` & `cassandra-driver-3.9.0/cassandra/io/libevreactor.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/io/libevwrapper.c` & `cassandra-driver-3.9.0/cassandra/io/libevwrapper.c`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/io/asyncorereactor.py` & `cassandra-driver-3.9.0/cassandra/io/asyncorereactor.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/io/geventreactor.py` & `cassandra-driver-3.9.0/cassandra/io/geventreactor.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/io/twistedreactor.py` & `cassandra-driver-3.9.0/cassandra/io/twistedreactor.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/io/__init__.py` & `cassandra-driver-3.9.0/cassandra/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/cqltypes.py` & `cassandra-driver-3.9.0/cassandra/cqltypes.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/concurrent.py` & `cassandra-driver-3.9.0/cassandra/concurrent.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/cluster.py` & `cassandra-driver-3.9.0/cassandra/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1971,14 +1971,20 @@
             if future:
                 self._initial_connect_futures.add(future)
 
         futures = wait_futures(self._initial_connect_futures, return_when=FIRST_COMPLETED)
         while futures.not_done and not any(f.result() for f in futures.done):
             futures = wait_futures(futures.not_done, return_when=FIRST_COMPLETED)
 
+        if not any(f.result() for f in self._initial_connect_futures):
+            msg = "Unable to connect to any servers"
+            if self.keyspace:
+                msg += " using keyspace '%s'" % self.keyspace
+            raise NoHostAvailable(msg, [h.address for h in hosts])
+
     def execute(self, query, parameters=None, timeout=_NOT_SET, trace=False, custom_payload=None, execution_profile=EXEC_PROFILE_DEFAULT, paging_state=None):
         """
         Execute the given query and synchronously wait for the response.
 
         If an error is encountered while executing the query, an Exception
         will be raised.
 
@@ -3718,34 +3724,49 @@
     def _set_final_result(self, response):
         self._cancel_timer()
         if self._metrics is not None:
             self._metrics.request_timer.addValue(time.time() - self._start_time)
 
         with self._callback_lock:
             self._final_result = response
+            # save off current callbacks inside lock for execution outside it
+            # -- prevents case where _final_result is set, then a callback is
+            # added and executed on the spot, then executed again as a
+            # registered callback
+            to_call = tuple(
+                partial(fn, response, *args, **kwargs)
+                for (fn, args, kwargs) in self._callbacks
+            )
 
         self._event.set()
 
         # apply each callback
-        for callback in self._callbacks:
-            fn, args, kwargs = callback
-            fn(response, *args, **kwargs)
+        for callback_partial in to_call:
+            callback_partial()
 
     def _set_final_exception(self, response):
         self._cancel_timer()
         if self._metrics is not None:
             self._metrics.request_timer.addValue(time.time() - self._start_time)
 
         with self._callback_lock:
             self._final_exception = response
+            # save off current errbacks inside lock for execution outside it --
+            # prevents case where _final_exception is set, then an errback is
+            # added and executed on the spot, then executed again as a
+            # registered errback
+            to_call = tuple(
+                partial(fn, response, *args, **kwargs)
+                for (fn, args, kwargs) in self._errbacks
+            )
         self._event.set()
 
-        for errback in self._errbacks:
-            fn, args, kwargs = errback
-            fn(response, *args, **kwargs)
+        # apply each callback
+        for callback_partial in to_call:
+            callback_partial()
 
     def _retry(self, reuse_connection, consistency_level, host):
         if self._final_exception:
             # the connection probably broke while we were waiting
             # to retry the operation
             return
 
@@ -3871,34 +3892,38 @@
 
             >>> future = session.execute_async("SELECT * FROM users")
             >>> future.add_callback(handle_results, time.time(), should_log=True)
 
         """
         run_now = False
         with self._callback_lock:
+            # Always add fn to self._callbacks, even when we're about to
+            # execute it, to prevent races with functions like
+            # start_fetching_next_page that reset _final_result
+            self._callbacks.append((fn, args, kwargs))
             if self._final_result is not _NOT_SET:
                 run_now = True
-            else:
-                self._callbacks.append((fn, args, kwargs))
         if run_now:
             fn(self._final_result, *args, **kwargs)
         return self
 
     def add_errback(self, fn, *args, **kwargs):
         """
         Like :meth:`.add_callback()`, but handles error cases.
         An Exception instance will be passed as the first positional argument
         to `fn`.
         """
         run_now = False
         with self._callback_lock:
+            # Always add fn to self._errbacks, even when we're about to execute
+            # it, to prevent races with functions like start_fetching_next_page
+            # that reset _final_exception
+            self._errbacks.append((fn, args, kwargs))
             if self._final_exception:
                 run_now = True
-            else:
-                self._errbacks.append((fn, args, kwargs))
         if run_now:
             fn(self._final_exception, *args, **kwargs)
         return self
 
     def add_callbacks(self, callback, errback,
                       callback_args=(), callback_kwargs=None,
                       errback_args=(), errback_kwargs=None):
```

### Comparing `cassandra-driver-3.8.1/cassandra/tuple.pxd` & `cassandra-driver-3.9.0/cassandra/tuple.pxd`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/pool.py` & `cassandra-driver-3.9.0/cassandra/pool.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/cython_utils.pyx` & `cassandra-driver-3.9.0/cassandra/cython_utils.pyx`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/numpy_parser.pyx` & `cassandra-driver-3.9.0/cassandra/numpy_parser.pyx`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/obj_parser.pyx` & `cassandra-driver-3.9.0/cassandra/obj_parser.pyx`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/murmur3.py` & `cassandra-driver-3.9.0/cassandra/murmur3.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/type_codes.py` & `cassandra-driver-3.9.0/cassandra/type_codes.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/metrics.py` & `cassandra-driver-3.9.0/cassandra/metrics.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/__init__.py` & `cassandra-driver-3.9.0/cassandra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class NullHandler(logging.Handler):
 
     def emit(self, record):
         pass
 
 logging.getLogger('cassandra').addHandler(NullHandler())
 
-__version_info__ = (3, 8, 1)
+__version_info__ = (3, 9, 0)
 __version__ = '.'.join(map(str, __version_info__))
 
 
 class ConsistencyLevel(object):
     """
     Spcifies how many replicas must respond for an operation to be considered
     a success.  By default, ``ONE`` is used for all operations.
```

### Comparing `cassandra-driver-3.8.1/cassandra/cmurmur3.c` & `cassandra-driver-3.9.0/cassandra/cmurmur3.c`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/ioutils.pyx` & `cassandra-driver-3.9.0/cassandra/ioutils.pyx`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/util.py` & `cassandra-driver-3.9.0/cassandra/util.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/auth.py` & `cassandra-driver-3.9.0/cassandra/auth.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/bytesio.pyx` & `cassandra-driver-3.9.0/cassandra/bytesio.pyx`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/deserializers.pyx` & `cassandra-driver-3.9.0/cassandra/deserializers.pyx`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/named.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/named.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/columns.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,34 +33,47 @@
         self.column = column
         self.value = value
         self.previous_value = None
         self.explicit = False
 
     @property
     def deleted(self):
-        return self.column._val_is_null(self.value) and (self.explicit or self.previous_value is not None)
+        return self.column._val_is_null(self.value) and (self.explicit or not self.column._val_is_null(self.previous_value))
 
     @property
     def changed(self):
         """
         Indicates whether or not this value has changed.
 
         :rtype: boolean
 
         """
-        return self.value != self.previous_value
+        if self.explicit:
+            return self.value != self.previous_value
+
+        if isinstance(self.column, BaseContainerColumn):
+            default_value = self.column.get_default()
+            if self.column._val_is_null(default_value):
+                return not self.column._val_is_null(self.value) and self.value != self.previous_value
+            elif self.previous_value is None:
+                return self.value != default_value
+
+            return self.value != self.previous_value
+
+        return False
 
     def reset_previous_value(self):
         self.previous_value = deepcopy(self.value)
 
     def getval(self):
         return self.value
 
     def setval(self, val):
         self.value = val
+        self.explicit = True
 
     def delval(self):
         self.value = None
 
     def get_property(self):
         _get = lambda slf: self.getval()
         _set = lambda slf, val: self.setval(val)
```

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/management.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/management.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/usertype.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/usertype.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/__init__.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/models.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,20 +480,22 @@
 
             values = dict((k, v) for k, v in values.items() if k in klass._columns.keys())
 
         else:
             klass = cls
 
         instance = klass(**values)
-        instance._set_persisted()
+        instance._set_persisted(force=True)
         return instance
 
-    def _set_persisted(self):
-        for v in self._values.values():
+    def _set_persisted(self, force=False):
+        # ensure we don't modify to any values not affected by the last save/update
+        for v in [v for v in self._values.values() if v.changed or force]:
             v.reset_previous_value()
+            v.explicit = False
         self._is_persisted = True
 
     def _can_update(self):
         """
         Called by the save function to check if this should be
         persisted with update or insert
 
@@ -584,24 +586,28 @@
                     cf_name = cf_name[-48:]
                     cf_name = cf_name.lower()
                     cf_name = re.sub(r'^_+', '', cf_name)
                     cls._table_name = cf_name
 
         return cls._table_name
 
+    def _set_column_value(self, name, value):
+        """Function to change a column value without changing the value manager states"""
+        self._values[name].value = value  # internal assignement, skip the main setter
+
     def validate(self):
         """
         Cleans and validates the field values
         """
         for name, col in self._columns.items():
             v = getattr(self, name)
             if v is None and not self._values[name].explicit and col.has_default:
                 v = col.get_default()
             val = col.validate(v)
-            setattr(self, name, val)
+            self._set_column_value(name, val)
 
     # Let an instance be used like a dict of its columns keys/values
     def __iter__(self):
         """ Iterate over column ids. """
         for column_id in self._columns.keys():
             yield column_id
```

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/operators.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/operators.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/connection.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from collections import defaultdict
 import logging
 import six
 import threading
 
-from cassandra.cluster import Cluster, _NOT_SET, NoHostAvailable, UserTypeDoesNotExist
+from cassandra.cluster import Cluster, _NOT_SET, NoHostAvailable, UserTypeDoesNotExist, ConsistencyLevel
 from cassandra.query import SimpleStatement, dict_factory
 
 from cassandra.cqlengine import CQLEngineException
 from cassandra.cqlengine.statements import BaseCQLStatement
 
 
 log = logging.getLogger(__name__)
@@ -180,14 +180,16 @@
         if invalid_config_args:
             raise CQLEngineException(
                 "Session configuration arguments and 'session' argument are mutually exclusive"
             )
         conn = Connection.from_session(name, session=session)
         conn.setup_session()
     else:  # use hosts argument
+        if consistency is None:
+            consistency = ConsistencyLevel.LOCAL_ONE
         conn = Connection(
             name, hosts=hosts,
             consistency=consistency, lazy_connect=lazy_connect,
             retry_connect=retry_connect, cluster_options=cluster_options
         )
         conn.setup()
```

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/query.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1248,14 +1248,17 @@
 
         - `update`: adds the given keys/values to the columns, creating new entries if they didn't exist, and overwriting old ones if they did
 
         .. code-block:: python
 
             # add items to a map
             Row.objects(row_id=5).update(map_column__update={1: 2, 3: 4})
+
+            # remove items from a map
+            Row.objects(row_id=5).update(map_column__remove={1, 2})
         """
         if not values:
             return
 
         nulled_columns = set()
         updated_columns = set()
         us = UpdateStatement(self.column_family_name, where=self._where, ttl=self._ttl,
@@ -1266,16 +1269,22 @@
             # check for nonexistant columns
             if col is None:
                 raise ValidationError("{0}.{1} has no column named: {2}".format(self.__module__, self.model.__name__, col_name))
             # check for primary key update attempts
             if col.is_primary_key:
                 raise ValidationError("Cannot apply update to primary key '{0}' for {1}.{2}".format(col_name, self.__module__, self.model.__name__))
 
-            # we should not provide default values in this use case.
-            val = col.validate(val)
+            if col_op == 'remove' and isinstance(col, columns.Map):
+                if not isinstance(val, set):
+                    raise ValidationError(
+                        "Cannot apply update operation '{0}' on column '{1}' with value '{2}'. A set is required.".format(col_op, col_name, val))
+                val = {v: None for v in val}
+            else:
+                # we should not provide default values in this use case.
+                val = col.validate(val)
 
             if val is None:
                 nulled_columns.add(col_name)
                 continue
 
             us.add_update(col, val, operation=col_op)
             updated_columns.add(col_name)
@@ -1444,14 +1453,17 @@
                 if static_save_only and not col.static and not col.partition_key:
                     continue
                 val = getattr(self.instance, name, None)
                 if col._val_is_null(val):
                     if self.instance._values[name].changed:
                         nulled_fields.add(col.db_field_name)
                     continue
+                if col.has_default and not self.instance._values[name].changed:
+                    # Ensure default columns included in a save() are marked as explicit, to get them *persisted* properly
+                    self.instance._values[name].explicit = True
                 insert.add_assignment(col, getattr(self.instance, name, None))
 
         # skip query execution if it's empty
         # caused by pointless update queries
         if not insert.is_empty:
             self._execute(insert)
         # delete any nulled columns
```

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/statements.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,53 +355,61 @@
 
 class MapUpdateClause(ContainerUpdateClause):
     """ updates a map collection """
 
     col_type = columns.Map
 
     _updates = None
+    _removals = None
 
     def _analyze(self):
         if self._operation == "update":
             self._updates = self.value.keys()
+        elif self._operation == "remove":
+            self._removals = {v for v in self.value.keys()}
         else:
             if self.previous is None:
                 self._updates = sorted([k for k, v in self.value.items()])
             else:
                 self._updates = sorted([k for k, v in self.value.items() if v != self.previous.get(k)]) or None
         self._analyzed = True
 
     def get_context_size(self):
         if self.is_assignment:
             return 1
-        return len(self._updates or []) * 2
+        return int((len(self._updates or []) * 2) + int(bool(self._removals)))
 
     def update_context(self, ctx):
         ctx_id = self.context_id
         if self.is_assignment:
             ctx[str(ctx_id)] = {}
+        elif self._removals is not None:
+            ctx[str(ctx_id)] = self._removals
         else:
             for key in self._updates or []:
                 val = self.value.get(key)
                 ctx[str(ctx_id)] = key
                 ctx[str(ctx_id + 1)] = val
                 ctx_id += 2
 
     @property
     def is_assignment(self):
         if not self._analyzed:
             self._analyze()
-        return self.previous is None and not self._updates
+        return self.previous is None and not self._updates and not self._removals
 
     def __unicode__(self):
         qs = []
 
         ctx_id = self.context_id
         if self.is_assignment:
             qs += ['"{0}" = %({1})s'.format(self.field, ctx_id)]
+        elif self._removals is not None:
+            qs += ['"{0}" = "{0}" - %({1})s'.format(self.field, ctx_id)]
+            ctx_id += 1
         else:
             for _ in self._updates or []:
                 qs += ['"{0}"[%({1})s] = %({2})s'.format(self.field, ctx_id, ctx_id + 1)]
                 ctx_id += 2
 
         return ', '.join(qs)
```

### Comparing `cassandra-driver-3.8.1/cassandra/cqlengine/functions.py` & `cassandra-driver-3.9.0/cassandra/cqlengine/functions.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/type_codes.pxd` & `cassandra-driver-3.9.0/cassandra/type_codes.pxd`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/cython_marshal.pyx` & `cassandra-driver-3.9.0/cassandra/cython_marshal.pyx`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/connection.py` & `cassandra-driver-3.9.0/cassandra/connection.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/query.py` & `cassandra-driver-3.9.0/cassandra/query.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/encoder.py` & `cassandra-driver-3.9.0/cassandra/encoder.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/buffer.pxd` & `cassandra-driver-3.9.0/cassandra/buffer.pxd`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/bytesio.pxd` & `cassandra-driver-3.9.0/cassandra/bytesio.pxd`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/timestamps.py` & `cassandra-driver-3.9.0/cassandra/timestamps.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     warning_interval = 1
     """
     This object will only issue warnings every ``warning_interval`` seconds.
     Defaults to 1 second.
     """
 
-    def __init__(self, warn_on_drift=True, warning_threshold=0, warning_interval=0):
+    def __init__(self, warn_on_drift=True, warning_threshold=1, warning_interval=1):
         self.lock = Lock()
         with self.lock:
             self.last = 0
             self._last_warn = 0
         self.warn_on_drift = warn_on_drift
         self.warning_threshold = warning_threshold
         self.warning_interval = warning_interval
@@ -93,15 +93,15 @@
 
     def _maybe_warn(self, now):
         # should be called from inside the self.lock.
         diff = self.last - now
         since_last_warn = now - self._last_warn
 
         warn = (self.warn_on_drift and
-                (diff > self.warning_threshold * 1e6) and
+                (diff >= self.warning_threshold * 1e6) and
                 (since_last_warn >= self.warning_interval * 1e6))
         if warn:
             log.warn(
                 "Clock skew detected: current tick ({now}) was {diff} "
                 "microseconds behind the last generated timestamp "
                 "({last}), returned timestamps will be artificially "
                 "incremented to guarantee monotonicity.".format(
```

### Comparing `cassandra-driver-3.8.1/cassandra/deserializers.pxd` & `cassandra-driver-3.9.0/cassandra/deserializers.pxd`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/policies.py` & `cassandra-driver-3.9.0/cassandra/policies.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/protocol.py` & `cassandra-driver-3.9.0/cassandra/protocol.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/marshal.py` & `cassandra-driver-3.9.0/cassandra/marshal.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/parsing.pyx` & `cassandra-driver-3.9.0/cassandra/parsing.pyx`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/metadata.py` & `cassandra-driver-3.9.0/cassandra/metadata.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/cassandra/parsing.pxd` & `cassandra-driver-3.9.0/cassandra/parsing.pxd`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/setup.py` & `cassandra-driver-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/ez_setup.py` & `cassandra-driver-3.9.0/ez_setup.py`

 * *Files identical despite different names*

### Comparing `cassandra-driver-3.8.1/README.rst` & `cassandra-driver-3.9.0/README.rst`

 * *Files identical despite different names*

