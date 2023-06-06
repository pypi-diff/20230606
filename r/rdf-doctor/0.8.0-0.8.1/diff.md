# Comparing `tmp/rdf_doctor-0.8.0-py3-none-any.whl.zip` & `tmp/rdf_doctor-0.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 38528 bytes, number of entries: 29
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 08:08 doctor/__init__.py
+Zip file size: 38559 bytes, number of entries: 29
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-06 06:47 doctor/__init__.py
 -rw-r--r--  2.0 unx      631 b- defN 23-Jun-05 08:08 doctor/consts.py
--rw-r--r--  2.0 unx    26420 b- defN 23-Jun-05 08:08 doctor/doctor.py
+-rw-r--r--  2.0 unx    26669 b- defN 23-Jun-06 06:47 doctor/doctor.py
 -rw-r--r--  2.0 unx    20305 b- defN 23-Jun-05 06:43 doctor/reference/correct-prefixes.tsv
 -rw-r--r--  2.0 unx    36944 b- defN 23-Jun-05 06:43 doctor/reference/rdf-config-prefixes.tsv
 -rw-r--r--  2.0 unx    21257 b- defN 23-Jun-05 06:43 doctor/reference/rdf-config-prefixes.yaml
 -rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 06:43 doctor/reference/refine-classes.tsv
 -rw-r--r--  2.0 unx      679 b- defN 23-Jun-05 06:43 doctor/reference/refine-prefixes.tsv
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 06:43 tests/__init__.py
 -rw-r--r--  2.0 unx      754 b- defN 23-Jun-05 06:43 tests/consts.py
@@ -18,14 +18,14 @@
 -rw-r--r--  2.0 unx      745 b- defN 23-Jun-05 06:43 tests/test_get_input_format.py
 -rw-r--r--  2.0 unx     2617 b- defN 23-Jun-05 06:43 tests/test_get_input_prefixes.py
 -rw-r--r--  2.0 unx     2831 b- defN 23-Jun-05 06:43 tests/test_get_markdown_result.py
 -rw-r--r--  2.0 unx      964 b- defN 23-Jun-05 06:43 tests/test_get_prefix_comparison_result.py
 -rw-r--r--  2.0 unx     1396 b- defN 23-Jun-05 06:43 tests/test_get_prefix_reuse_percentage.py
 -rw-r--r--  2.0 unx     4936 b- defN 23-Jun-05 06:43 tests/test_get_suggested_qname.py
 -rw-r--r--  2.0 unx    15594 b- defN 23-Jun-05 06:43 tests/test_validate_command_line_args.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6694 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/RECORD
-29 files, 159640 bytes uncompressed, 34398 bytes compressed:  78.5%
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6694 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/RECORD
+29 files, 159889 bytes uncompressed, 34429 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -63,26 +63,26 @@
 
 Filename: tests/test_get_suggested_qname.py
 Comment: 
 
 Filename: tests/test_validate_command_line_args.py
 Comment: 
 
-Filename: rdf_doctor-0.8.0.dist-info/LICENSE
+Filename: rdf_doctor-0.8.1.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-0.8.0.dist-info/METADATA
+Filename: rdf_doctor-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-0.8.0.dist-info/WHEEL
+Filename: rdf_doctor-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-0.8.0.dist-info/entry_points.txt
+Filename: rdf_doctor-0.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.0.dist-info/top_level.txt
+Filename: rdf_doctor-0.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.0.dist-info/RECORD
+Filename: rdf_doctor-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.8.0"
+__version__ = "0.8.1"
```

## doctor/doctor.py

```diff
@@ -238,15 +238,21 @@
 
 
     return True, None
 
 
 # Processing when the report format is "shex"
 def get_shex_result(args, input_format, compression_mode):
-    input_prefixes = get_input_prefixes_from_multi_files(args.input, compression_mode)
+
+    # Get Prefix when input file is turtle format
+    if input_format == TURTLE:
+        input_prefixes = get_input_prefixes_from_multi_files(args.input, compression_mode)
+    else:
+        input_prefixes = []
+
     shaper_result = get_shaper_result(args, input_format, compression_mode, input_prefixes)
 
     # Suggest QName based on URI of validation expression output by sheXer and correct-prefixes.tsv
     result_suggested_qname = []
     correct_prefixes = get_correct_prefixes()
     suggested_qname = get_suggested_qname(shaper_result, input_prefixes, correct_prefixes)
     if len(suggested_qname) != 0:
@@ -264,17 +270,22 @@
     return shex_final_result
 
 
 # Processing when the report format is "md/markdown"
 def get_markdown_result(input_file, input_format, compression_mode, classes, prefix_dict, class_dict):
 
     # Processing related to prefixes ------------------
+    # Get Prefix when input file is turtle format
+    if input_format == TURTLE:
+        input_prefixes = get_input_prefixes(input_file, compression_mode)
+    else:
+        input_prefixes = []
+
     # Get list for result output about prefix reuse rate
     result_prefix_reuse_percentage = []
-    input_prefixes = get_input_prefixes(input_file, compression_mode)
     result_prefix_reuse_percentage.append("## Prefix reuse percentage ([?](" + HELP_LINK_URL + "))\n")
     result_prefix_reuse_percentage.append("Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.\n")
     prefix_reuse_percentage = get_prefix_reuse_percentage(input_prefixes)
     if prefix_reuse_percentage == None:
         result_prefix_reuse_percentage.append("```\n")
         result_prefix_reuse_percentage.append("Not calculated because there is no prefix defined.\n")
         result_prefix_reuse_percentage.append("```\n\n")
```

## Comparing `rdf_doctor-0.8.0.dist-info/LICENSE` & `rdf_doctor-0.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-0.8.0.dist-info/METADATA` & `rdf_doctor-0.8.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 0.8.0
+Version: 0.8.1
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `rdf_doctor-0.8.0.dist-info/RECORD` & `rdf_doctor-0.8.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-doctor/__init__.py,sha256=iPlYCcIzuzW7T2HKDkmYlMkRI51dBLfNRxPPiWrfw9U,22
+doctor/__init__.py,sha256=Ocl79hbbH8_jdr5dGC90VR1cAvZc05Rc0tkZttUnMjo,22
 doctor/consts.py,sha256=jo_-yPRv-Z7OoTYeIEed4RNsKR6nzrm64wVJPmI8vww,631
-doctor/doctor.py,sha256=1QcVgQN7qqZbZo_60aEWGfq9qZkjOnHZt3dxU5tLFl4,26420
+doctor/doctor.py,sha256=nyA9dHEhP16Ey93-VvVU1QQsEdTZ9STw59sah-CxzBo,26669
 doctor/reference/correct-prefixes.tsv,sha256=2IAy3-9YwmWbG9JgoB8R2fxW7T-U-Qr59PzqMApUbpI,20305
 doctor/reference/rdf-config-prefixes.tsv,sha256=vAUFO7WZhRrCA4ESBc-xq17uFIx7XqIjYCa-8Q_-nN4,36944
 doctor/reference/rdf-config-prefixes.yaml,sha256=WllZLfDVchyqIYi0uSUC5JQ3h52UlCb2Ek4P-YdM8ds,21257
 doctor/reference/refine-classes.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
 doctor/reference/refine-prefixes.tsv,sha256=B5iok0_4VqdBNLn4_Auwx5gSwAnxgIh6OoQ4cgebERY,679
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/consts.py,sha256=FekU8wajsGMDbTWx0nV14s7KL3RQJsyMfXEtjDtLqCs,754
@@ -17,13 +17,13 @@
 tests/test_get_input_format.py,sha256=dMzc0qm4rHChxLDq7bzvEF701lf9mDpZ8VgF5kiyvbE,745
 tests/test_get_input_prefixes.py,sha256=ltnPhPbBstmeiExt2o1Hy9djtnoyGTYMKTd7hQ2lHMw,2617
 tests/test_get_markdown_result.py,sha256=DiZTV83XLXBSHK5yiKLITF6EKCev8ig4D7WPd5j6wQ0,2831
 tests/test_get_prefix_comparison_result.py,sha256=u3J543zQMX8IxdfGB1QF9KScq-spZz-OSW2Q5cQGYVE,964
 tests/test_get_prefix_reuse_percentage.py,sha256=2rVMIMipBSUy34NMStEp9sGimB8j9mAA32NVUjVUCSk,1396
 tests/test_get_suggested_qname.py,sha256=ELPLwv0PDsve2m63xkI0CVWjUAnJ4381Wbyg2stFx58,4936
 tests/test_validate_command_line_args.py,sha256=0UXMSClVMGwjg_h6YbmcSqwzTgUq5ECvznfC5bzZr-g,15594
-rdf_doctor-0.8.0.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
-rdf_doctor-0.8.0.dist-info/METADATA,sha256=k6WBW_kIRujPcyvKuNycCsjscs5LePrF42OG7GhQm8c,6694
-rdf_doctor-0.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rdf_doctor-0.8.0.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
-rdf_doctor-0.8.0.dist-info/top_level.txt,sha256=ypiEwVeuDnH4vVv0LSX0AUO7DU05HXE7eun4aW7Zvow,13
-rdf_doctor-0.8.0.dist-info/RECORD,,
+rdf_doctor-0.8.1.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
+rdf_doctor-0.8.1.dist-info/METADATA,sha256=TTRbKZa49maWM6IPVY9QuCWBz_dwXMwqwHN6jmPuVqk,6694
+rdf_doctor-0.8.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rdf_doctor-0.8.1.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
+rdf_doctor-0.8.1.dist-info/top_level.txt,sha256=ypiEwVeuDnH4vVv0LSX0AUO7DU05HXE7eun4aW7Zvow,13
+rdf_doctor-0.8.1.dist-info/RECORD,,
```

