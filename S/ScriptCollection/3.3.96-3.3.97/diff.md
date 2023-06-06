# Comparing `tmp/ScriptCollection-3.3.96-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.3.97-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 59631 bytes, number of entries: 14
+Zip file size: 59634 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    18064 b- defN 23-Mar-05 15:39 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34151 b- defN 23-May-26 16:46 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6275 b- defN 23-May-26 16:46 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    90646 b- defN 23-Jun-03 11:06 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   133998 b- defN 23-Jun-03 11:06 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat    90693 b- defN 23-Jun-06 19:19 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   133998 b- defN 23-Jun-06 10:08 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7795 b- defN 23-Jun-03 11:07 ScriptCollection-3.3.96.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 11:07 ScriptCollection-3.3.96.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1968 b- defN 23-Jun-03 11:07 ScriptCollection-3.3.96.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-03 11:07 ScriptCollection-3.3.96.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1295 b- defN 23-Jun-03 11:07 ScriptCollection-3.3.96.dist-info/RECORD
-14 files, 307179 bytes uncompressed, 57439 bytes compressed:  81.3%
+-rw-rw-rw-  2.0 fat     7795 b- defN 23-Jun-06 19:19 ScriptCollection-3.3.97.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 19:19 ScriptCollection-3.3.97.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1968 b- defN 23-Jun-06 19:19 ScriptCollection-3.3.97.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-06 19:19 ScriptCollection-3.3.97.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1295 b- defN 23-Jun-06 19:19 ScriptCollection-3.3.97.dist-info/RECORD
+14 files, 307226 bytes uncompressed, 57442 bytes compressed:  81.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.3.96.dist-info/METADATA
+Filename: ScriptCollection-3.3.97.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.3.96.dist-info/WHEEL
+Filename: ScriptCollection-3.3.97.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.3.96.dist-info/entry_points.txt
+Filename: ScriptCollection-3.3.97.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.96.dist-info/top_level.txt
+Filename: ScriptCollection-3.3.97.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.96.dist-info/RECORD
+Filename: ScriptCollection-3.3.97.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -22,15 +22,15 @@
 from PyPDF2 import PdfFileMerger
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.3.96"
+version = "3.3.97"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
@@ -510,15 +510,15 @@
                     raise ValueError(f"Can not calculate corresponding commit for tag '{tag}'.")
                 commit_id_new = search_commit_result[1]
                 self.git_delete_tag(repository, tag)
                 self.git_create_tag(repository, commit_id_new, tag, sign, message)
 
     @GeneralUtilities.check_arguments
     def get_current_branch_has_tag(self, repository_folder: str) -> str:
-        result = self.run_program_argsasarray("git", ["describe", "--tags", "--abbrev=0"], repository_folder, verbosity=0)
+        result = self.run_program_argsasarray("git", ["describe", "--tags", "--abbrev=0"], repository_folder, verbosity=0, throw_exception_if_exitcode_is_not_zero=False)
         return result[0] == 0
 
     @GeneralUtilities.check_arguments
     def get_latest_tag(self, repository_folder: str) -> str:
         result = self.run_program_argsasarray("git", ["describe", "--tags", "--abbrev=0"], repository_folder, verbosity=0)
         result = result[1].replace("\r", "").replace("\n", "")
         return result
```

## Comparing `ScriptCollection-3.3.96.dist-info/METADATA` & `ScriptCollection-3.3.97.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.3.96
+Version: 3.3.97
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
```

## Comparing `ScriptCollection-3.3.96.dist-info/entry_points.txt` & `ScriptCollection-3.3.97.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.3.96.dist-info/RECORD` & `ScriptCollection-3.3.97.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ScriptCollection/Executables.py,sha256=kXTIX92KLeFuxnYOlsyFs5lkznsxkuoBMVrV3OU7FZU,18064
 ScriptCollection/GeneralUtilities.py,sha256=rRQPyyRNZ1U0UDEuAqKZl3lHj38_4KofM6ON6hXqyRA,34151
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=nIzY4dG6W-xEpkeoTbozwNZtFSIo-bU_W6t6u1AZKtE,6275
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=gge6WqnQBPQ5HEg-Aq8AKgeU7zL93yezHey5l5n3GH0,90646
+ScriptCollection/ScriptCollectionCore.py,sha256=1IRlwsjd62EYM0U5ocd-gXD1dGM5bjEx39djCpDN43Q,90693
 ScriptCollection/TasksForCommonProjectStructure.py,sha256=R641ijodm622j-BTdAFgZNTWJ1vXRN1Y7ZOEPEBIkRw,133998
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.3.96.dist-info/METADATA,sha256=IpLGAGMOMJAaNRqy-1j-AUnXFMFJshTeICKroaVdbs0,7795
-ScriptCollection-3.3.96.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ScriptCollection-3.3.96.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
-ScriptCollection-3.3.96.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.3.96.dist-info/RECORD,,
+ScriptCollection-3.3.97.dist-info/METADATA,sha256=McuUCTtysRWBw6qw7UFk2c5jH9B_VEGkZdIALfBrsjg,7795
+ScriptCollection-3.3.97.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ScriptCollection-3.3.97.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
+ScriptCollection-3.3.97.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.3.97.dist-info/RECORD,,
```

