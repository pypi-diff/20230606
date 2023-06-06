# Comparing `tmp/skulk-2.0.2-py2.py3-none-any.whl.zip` & `tmp/skulk-2.0.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8945 bytes, number of entries: 10
--rw-r--r--  2.0 unx        5 b- defN 23-May-31 20:30 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-May-31 20:30 skulk/__init__.py
--rw-r--r--  2.0 unx     9548 b- defN 23-May-31 20:30 skulk/bumper.py
--rw-r--r--  2.0 unx     8984 b- defN 23-May-31 20:30 skulk/skulk.py
--rw-r--r--  2.0 unx     3128 b- defN 23-May-31 20:30 skulk/util.py
--rw-r--r--  2.0 unx      646 b- defN 23-May-31 20:30 skulk-2.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-31 20:30 skulk-2.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-May-31 20:30 skulk-2.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-31 20:30 skulk-2.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      733 b- defN 23-May-31 20:30 skulk-2.0.2.dist-info/RECORD
-10 files, 23204 bytes uncompressed, 7703 bytes compressed:  66.8%
+Zip file size: 9241 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-06 16:13 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 16:12 skulk/__init__.py
+-rw-r--r--  2.0 unx     9548 b- defN 23-Jun-06 16:12 skulk/bumper.py
+-rw-r--r--  2.0 unx     9801 b- defN 23-Jun-06 16:12 skulk/skulk.py
+-rw-r--r--  2.0 unx     3363 b- defN 23-Jun-06 16:12 skulk/util.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Jun-06 16:13 skulk-2.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-06 16:13 skulk-2.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-06 16:13 skulk-2.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-06 16:13 skulk-2.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      733 b- defN 23-Jun-06 16:13 skulk-2.0.3.dist-info/RECORD
+10 files, 24256 bytes uncompressed, 7999 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-2.0.2.dist-info/METADATA
+Filename: skulk-2.0.3.dist-info/METADATA
 Comment: 
 
-Filename: skulk-2.0.2.dist-info/WHEEL
+Filename: skulk-2.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-2.0.2.dist-info/entry_points.txt
+Filename: skulk-2.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-2.0.2.dist-info/top_level.txt
+Filename: skulk-2.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-2.0.2.dist-info/RECORD
+Filename: skulk-2.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-2.0.2
+2.0.3
```

## skulk/skulk.py

```diff
@@ -57,15 +57,15 @@
         self.changelog_addition = ""
 
     def run(self):
         """
         Guide the user to ensure version and changelog are valid.
         """
 
-        # wizard.check_pre_push_hook()
+        self.check_pre_push_hook()
         self.check_clean()
         self.bumper = Bumper(self.repo, self.pip_name)
         if self.ask_do_tag_release():
             self.bumper.run()
 
         self.ask_changelog_additions()
 
@@ -247,14 +247,31 @@
             if line.startswith("## Unreleased"):
                 return False
             elif line.startswith("## Version"):
                 return True
         return True
 
 
+
+    def check_pre_push_hook(self):
+        """Check if there is a legacy pre-push hook and delete it."""
+        hook_detection_line = "skulk.run_pre_push_checks()"
+        delete_hook = False
+        if os.path.exists( self.hook_filename):
+            with open( self.hook_filename, "r", encoding="utf-8") as f:
+                for line in f:
+                    if line.strip() == hook_detection_line:
+                        delete_hook = True
+        if delete_hook:
+            print(f"Found legacy pre-push hook '{self.hook_filename}' - Deleting ...")
+            try:
+                os.unlink( self.hook_filename)
+            except IOError as ex:
+                print(f"Error deleting '{self.hook_filename}': {ex}")
+                util.enter_to_continue_or_exit("Please delete it manually, then press enter")
 def main():
     """Run the wizard."""
     wizard = Skulk()
     wizard.run()
 
 
 if __name__ == "__main__":
```

## skulk/util.py

```diff
@@ -111,7 +111,17 @@
             break
     result = []
     for c in repo.iter_commits(rev=branch):
         result.append(c)
         if c.hexsha == master_tag_sha:
             break
     return result
+
+def enter_to_continue_or_exit(cont_message):
+    cont = input(
+        green(
+            "f{cont_message}. Type 'exit' to exit."
+        )
+    )
+    if cont.lower() == "exit":
+        sys.stderr.write("Exited.\n")
+        sys.exit(0)
```

## Comparing `skulk-2.0.2.dist-info/METADATA` & `skulk-2.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 2.0.2
+Version: 2.0.3
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

