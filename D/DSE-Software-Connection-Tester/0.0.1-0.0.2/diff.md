# Comparing `tmp/DSE Software Connection Tester-0.0.1.tar.gz` & `tmp/DSE Software Connection Tester-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DSE Software Connection Tester-0.0.1.tar", last modified: Mon Jun  5 14:40:47 2023, max compression
+gzip compressed data, was "DSE Software Connection Tester-0.0.2.tar", last modified: Tue Jun  6 12:04:46 2023, max compression
```

## Comparing `DSE Software Connection Tester-0.0.1.tar` & `DSE Software Connection Tester-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 14:40:47.257286 DSE Software Connection Tester-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-05 14:40:47.241693 DSE Software Connection Tester-0.0.1/DSE_Software_Connection_Tester.egg-info/
--rw-rw-rw-   0        0        0      791 2023-06-05 14:40:47.000000 DSE Software Connection Tester-0.0.1/DSE_Software_Connection_Tester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-06-05 14:40:47.000000 DSE Software Connection Tester-0.0.1/DSE_Software_Connection_Tester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 14:40:47.000000 DSE Software Connection Tester-0.0.1/DSE_Software_Connection_Tester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-05 14:40:47.000000 DSE Software Connection Tester-0.0.1/DSE_Software_Connection_Tester.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-05 12:50:28.000000 DSE Software Connection Tester-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      791 2023-06-05 14:40:47.257286 DSE Software Connection Tester-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-05 12:50:42.000000 DSE Software Connection Tester-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 14:40:47.257286 DSE Software Connection Tester-0.0.1/dseconnectiontester/
--rw-rw-rw-   0        0        0     7462 2023-06-05 14:32:52.000000 DSE Software Connection Tester-0.0.1/dseconnectiontester/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-05 14:40:47.257286 DSE Software Connection Tester-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-06-05 14:40:42.000000 DSE Software Connection Tester-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:04:46.866714 DSE Software Connection Tester-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-06 12:04:46.866714 DSE Software Connection Tester-0.0.2/DSE_Software_Connection_Tester.egg-info/
+-rw-rw-rw-   0        0        0      791 2023-06-06 12:04:46.000000 DSE Software Connection Tester-0.0.2/DSE_Software_Connection_Tester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-06-06 12:04:46.000000 DSE Software Connection Tester-0.0.2/DSE_Software_Connection_Tester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 12:04:46.000000 DSE Software Connection Tester-0.0.2/DSE_Software_Connection_Tester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-06 12:04:46.000000 DSE Software Connection Tester-0.0.2/DSE_Software_Connection_Tester.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-05 12:50:28.000000 DSE Software Connection Tester-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      791 2023-06-06 12:04:46.866714 DSE Software Connection Tester-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-05 12:50:42.000000 DSE Software Connection Tester-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 12:04:46.866714 DSE Software Connection Tester-0.0.2/dseconnectiontester/
+-rw-rw-rw-   0        0        0     8460 2023-06-06 12:03:32.000000 DSE Software Connection Tester-0.0.2/dseconnectiontester/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 12:04:46.866714 DSE Software Connection Tester-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2023-06-06 12:03:51.000000 DSE Software Connection Tester-0.0.2/setup.py
```

### Comparing `DSE Software Connection Tester-0.0.1/DSE_Software_Connection_Tester.egg-info/PKG-INFO` & `DSE Software Connection Tester-0.0.2/DSE_Software_Connection_Tester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DSE-Software-Connection-Tester
-Version: 0.0.1
+Version: 0.0.2
 Summary: A connection testing package.
 Author: Gabi Barrientos de Reus
 Author-email: gabi@dsesoftware.nl
 Keywords: DSE Software,connection,dns,resolve,ping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `DSE Software Connection Tester-0.0.1/PKG-INFO` & `DSE Software Connection Tester-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DSE Software Connection Tester
-Version: 0.0.1
+Version: 0.0.2
 Summary: A connection testing package.
 Author: Gabi Barrientos de Reus
 Author-email: gabi@dsesoftware.nl
 Keywords: DSE Software,connection,dns,resolve,ping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `DSE Software Connection Tester-0.0.1/dseconnectiontester/__init__.py` & `DSE Software Connection Tester-0.0.2/dseconnectiontester/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import abc
 import subprocess
 from os.path import exists
 from typing import List
 import logging
 import http.client
 from enum import Enum
 
@@ -150,38 +151,68 @@
         self.resolvable: bool = False
         self.pingable: bool = False
         self.domain = domain
         self.ip = ip
         self.recordType = record_type
 
 
-class FileParser:
+class ParserInterface(abc.ABC):
+    @abc.abstractmethod
+    def parse_dns(self) -> List[DnsEntry]:
+        pass
+
+    def parse_row(self, row: str, logger: CustomLogger) -> DnsEntry:
+        if logger:
+            logger.info(f'Parsing row `{row.strip()}`.')
+        entry_parts = row.strip().split(' ')
+        return DnsEntry(entry_parts[0], entry_parts[1], DnsRecordType[entry_parts[2]])
+
+
+class StringParser(ParserInterface):
+    def __init__(self, content: str, logger: CustomLogger | None):
+        self.content = content
+        self.logger = logger.instance(
+            caller=self.__class__.__name__,
+            log_level=logger.log_level,
+            date_format=logger.date_format,
+            filename=logger.filename
+        )
+
+    def parse_dns(self) -> List[DnsEntry]:
+        entries: List[DnsEntry] = list()
+        if self.logger:
+            self.logger.info(f'Trying to parse string.')
+        for dns_entry in self.content.splitlines():
+            entries.append(self.parse_row(dns_entry, self.logger))
+        if self.logger:
+            self.logger.info(f'Parsed a total of {len(entries)} rows.')
+        return entries
+
+
+class FileParser(ParserInterface):
     def __init__(self, file: str, logger: CustomLogger | None):
         self.file = file
         self.logger = logger.instance(
             caller=self.__class__.__name__,
             log_level=logger.log_level,
             date_format=logger.date_format,
             filename=logger.filename
         )
-
-    def parse_dns_entries(self) -> List[DnsEntry]:
         if not exists(self.file):
             if self.logger:
                 self.logger.critical(f'File `{self.file}` does not exist.')
             raise IOError(f'File {self.file} does not exist.')
+
+    def parse_dns(self) -> List[DnsEntry]:
         entries: List[DnsEntry] = list()
         if self.logger:
             self.logger.info(f'Trying to parse file `{self.file}`.')
         with open(self.file) as dns_entries:
             for dns_entry in dns_entries:
-                if self.logger:
-                    self.logger.info(f'Parsing row `{dns_entry.strip()}`.')
-                entry_parts = dns_entry.strip().split(' ')
-                entries.append(DnsEntry(entry_parts[0], entry_parts[1], DnsRecordType[entry_parts[2]]))
+                entries.append(self.parse_row(dns_entry, self.logger))
         if self.logger:
             self.logger.info(f'Parsed a total of {len(entries)} rows.')
         return entries
 
 
 class ConnectionTester:
     def __init__(self, logger: CustomLogger | None):
```

### Comparing `DSE Software Connection Tester-0.0.1/setup.py` & `DSE Software Connection Tester-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 NAME = 'DSE Software Connection Tester'
 DESCRIPTION = 'A connection testing package.'
 LONG_DESCRIPTION = 'A package that allows for testing the resolvability of a domain name ' \
                    'and the accessibility of an ip address.'
 AUTHOR = 'Gabi Barrientos de Reus'
 AUTHOR_EMAIL = 'gabi@dsesoftware.nl'
```

