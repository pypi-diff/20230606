# Comparing `tmp/makenote-1.6-py3-none-any.whl.zip` & `tmp/makenote-1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17695 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       20 b- defN 23-May-26 22:48 makenote/__init__.py
--rwxrwxr-x  2.0 unx    10718 b- defN 23-May-26 22:48 makenote-1.6.data/scripts/makenote
--rw-rw-r--  2.0 unx    35099 b- defN 23-May-26 22:48 makenote-1.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3022 b- defN 23-May-26 22:48 makenote-1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-26 22:48 makenote-1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-26 22:48 makenote-1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      548 b- defN 23-May-26 22:48 makenote-1.6.dist-info/RECORD
-7 files, 49508 bytes uncompressed, 16725 bytes compressed:  66.2%
+Zip file size: 17799 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jun-06 15:05 makenote/__init__.py
+-rwxrwxr-x  2.0 unx    11325 b- defN 23-Jun-06 15:05 makenote-1.7.data/scripts/makenote
+-rw-rw-r--  2.0 unx    35099 b- defN 23-Jun-06 15:05 makenote-1.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3022 b- defN 23-Jun-06 15:05 makenote-1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 15:05 makenote-1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-06 15:05 makenote-1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      548 b- defN 23-Jun-06 15:05 makenote-1.7.dist-info/RECORD
+7 files, 50115 bytes uncompressed, 16829 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: makenote/__init__.py
 Comment: 
 
-Filename: makenote-1.6.data/scripts/makenote
+Filename: makenote-1.7.data/scripts/makenote
 Comment: 
 
-Filename: makenote-1.6.dist-info/LICENSE
+Filename: makenote-1.7.dist-info/LICENSE
 Comment: 
 
-Filename: makenote-1.6.dist-info/METADATA
+Filename: makenote-1.7.dist-info/METADATA
 Comment: 
 
-Filename: makenote-1.6.dist-info/WHEEL
+Filename: makenote-1.7.dist-info/WHEEL
 Comment: 
 
-Filename: makenote-1.6.dist-info/top_level.txt
+Filename: makenote-1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: makenote-1.6.dist-info/RECORD
+Filename: makenote-1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## makenote/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.6"
+__version__ = "1.7"
```

## Comparing `makenote-1.6.data/scripts/makenote` & `makenote-1.7.data/scripts/makenote`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,17 @@
                     help="list tables", default=None, action="store_true")
 parser.add_argument("-t", "--table", dest="table_name", help="table for notes",
                     default=default_table_name)
 parser.add_argument("-m", "--merge",  help="merge two databases",
                     default=None, nargs=3, metavar=('FIRST','SECOND','OUTPUT'))
 parser.add_argument("-x", "--export",  help="export database into file",
                     default=None, metavar='FILENAME')
+parser.add_argument("-i", "--import",  help="import database",
+                    default=None, dest='import_file', metavar='FILENAME')
+
 parser.add_argument("text",  help="text", default=None, nargs='*')
 
 parser.add_argument("-u", "--update",  help="edit note. add entry number",
                     default=None, metavar='note_id', type=int)
 
 args = parser.parse_args()
 
@@ -75,15 +78,15 @@
 def tail_show_table(sqlite_cursor, table_name, limit):
     try:
         # get records from sqlite
         sqlite_cursor.execute(f"SELECT count(*) FROM {table_name}")
         N = sqlite_cursor.fetchone()[0]
         records = sqlite_cursor.execute(f"SELECT * FROM {table_name} LIMIT {N - limit}, {limit};")
         # print them all
-        i = 0
+        i = N - limit 
         for r in records:
             i += 1
             print(i, end="  ")
 
             # if style number 1 is selected
             if show_style == 1:
                 # replace that utf representation of نیم‌فاصله with itself
@@ -210,14 +213,20 @@
         else:
             add_table(cursor1, cursor_out, table_name[0])
     
     for table_name in tables_2:
         if table_name not in tables_1:
             add_table(cursor2, cursor_out, table_name[0])
 
+def sql_to_csv(sqlite_cursor: sqlite3.Cursor):
+    records = sqlite_cursor.execute(
+        'SELECT name from sqlite_master where type= "table"')
+    # print them
+    tables = [r[0] for r in records]
+    
 
 def merge_databases_by_name(firstdb_filename:str, seconddb_filename:str, outdb_filename:str):
 
     con1 = sqlite3.connect(firstdb_filename)
     cur1 = con1.cursor()
 
     con2 = sqlite3.connect(seconddb_filename)
@@ -236,14 +245,21 @@
     
     con3.commit()
     con3.close()
 
     print('done merging databases')
 
 
+def import_database(db_filename: str, outdb_filename:str):
+
+    merge_databases_by_name(outdb_filename, db_filename, outdb_filename)
+    print('done importing your database')
+
+
+
 if sys.stdout.isatty() == True:
     # this number is like an option for how the show record output is styled
     show_style = 2
 else:
     show_style = 1
 
 os.makedirs(os.path.dirname(diaryFileName), exist_ok=True)
@@ -259,14 +275,17 @@
 elif args.list_tables:
     list_tables(cur)
 elif args.create_table:
     make_table(cur, args.create_table)
 elif args.export:
     shutil.copy(diaryFileName, args.export)
     print(f'exported to {os.path.realpath(args.export)}')
+elif args.import_file:
+    import_database(args.import_file, diaryFileName)
+
 elif args.merge:
     firstdb, seconddb, outdb = args.merge
     merge_databases_by_name(firstdb, seconddb, outdb)
 # elif args.default:
 #     default_table_name = args.default
 #     table_name = args.default
```

## Comparing `makenote-1.6.dist-info/LICENSE` & `makenote-1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `makenote-1.6.dist-info/METADATA` & `makenote-1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makenote
-Version: 1.6
+Version: 1.7
 Summary: command line tool for quickly writing journals
 Home-page: https://github.com/ekm507/makenote
 Author: Erfan Kheirollahi
 Author-email: ekm507@gmail.com
 License: UNKNOWN
 Keywords: makenote
 Platform: UNKNOWN
```

## Comparing `makenote-1.6.dist-info/RECORD` & `makenote-1.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-makenote/__init__.py,sha256=8psuJD1S_9CzZhv5UYeBf0WEXuW-U5N-vMFk3UwhuMI,20
-makenote-1.6.data/scripts/makenote,sha256=5lpFIP-Q0wtcxese4ohAkIfWSXQ-xUzP9K2HR_kQLvo,10718
-makenote-1.6.dist-info/LICENSE,sha256=EDNKolfZwqzjwV8uF_EmpqT-ZnS1b1mue9J8MVdQ-VA,35099
-makenote-1.6.dist-info/METADATA,sha256=gb8FhZLAcQ-HnG5Z3fkcSE11s3lmeurEB-Yqp3YFs7I,3022
-makenote-1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-makenote-1.6.dist-info/top_level.txt,sha256=C9KLIKlcZbG1d-Rhpmu0_Q-Eb7GIWp9OX1ekrqewXVg,9
-makenote-1.6.dist-info/RECORD,,
+makenote/__init__.py,sha256=0oYt-duoMe9LZv2io7u2SnwQBPHKTfh4Fvu-S_0QMSQ,20
+makenote-1.7.data/scripts/makenote,sha256=QAnjRAwo7YFeXIv9TvaapAwgRSB3QLzhALjGc4qQm8o,11325
+makenote-1.7.dist-info/LICENSE,sha256=EDNKolfZwqzjwV8uF_EmpqT-ZnS1b1mue9J8MVdQ-VA,35099
+makenote-1.7.dist-info/METADATA,sha256=iaX8LR7KHSPk9HoKcspBSgS1dkFmKRAtsAdWmizawQc,3022
+makenote-1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+makenote-1.7.dist-info/top_level.txt,sha256=C9KLIKlcZbG1d-Rhpmu0_Q-Eb7GIWp9OX1ekrqewXVg,9
+makenote-1.7.dist-info/RECORD,,
```

