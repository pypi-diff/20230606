# Comparing `tmp/giskard-client-0.0.1.tar.gz` & `tmp/giskard_client-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/giskard-client-0.0.1.tar", last modified: Fri Jun  2 13:44:49 2023, max compression
+gzip compressed data, was "giskard_client-0.1.0b1.tar", last modified: Tue Jun  6 09:16:45 2023, max compression
```

## Comparing `giskard-client-0.0.1.tar` & `giskard_client-0.1.0b1.tar`

### file list

```diff
@@ -1,11 +1,3 @@
-drwxr-xr-x   0 alexcombessie   (502) staff       (20)        0 2023-06-02 13:44:49.000000 giskard-client-0.0.1/
--rw-r--r--   0 alexcombessie   (502) staff       (20)      203 2023-06-02 13:44:49.000000 giskard-client-0.0.1/PKG-INFO
--rw-r--r--   0 alexcombessie   (502) staff       (20)       52 2023-06-02 13:44:49.000000 giskard-client-0.0.1/README.md
--rw-r--r--   0 alexcombessie   (502) staff       (20)       26 2023-06-02 13:44:49.000000 giskard-client-0.0.1/giskard-client.py
-drwxr-xr-x   0 alexcombessie   (502) staff       (20)        0 2023-06-02 13:44:49.000000 giskard-client-0.0.1/giskard_client.egg-info/
--rw-r--r--   0 alexcombessie   (502) staff       (20)      203 2023-06-02 13:44:49.000000 giskard-client-0.0.1/giskard_client.egg-info/PKG-INFO
--rw-r--r--   0 alexcombessie   (502) staff       (20)      188 2023-06-02 13:44:49.000000 giskard-client-0.0.1/giskard_client.egg-info/SOURCES.txt
--rw-r--r--   0 alexcombessie   (502) staff       (20)        1 2023-06-02 13:44:49.000000 giskard-client-0.0.1/giskard_client.egg-info/dependency_links.txt
--rw-r--r--   0 alexcombessie   (502) staff       (20)       15 2023-06-02 13:44:49.000000 giskard-client-0.0.1/giskard_client.egg-info/top_level.txt
--rw-r--r--   0 alexcombessie   (502) staff       (20)       38 2023-06-02 13:44:49.000000 giskard-client-0.0.1/setup.cfg
--rw-r--r--   0 alexcombessie   (502) staff       (20)      256 2023-06-02 13:44:49.000000 giskard-client-0.0.1/setup.py
+-rw-r--r--   0        0        0       38 2023-06-06 09:16:29.301964 giskard_client-0.1.0b1/README.md
+-rw-r--r--   0        0        0      327 2023-06-06 09:16:45.149387 giskard_client-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0      228 1970-01-01 00:00:00.000000 giskard_client-0.1.0b1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

