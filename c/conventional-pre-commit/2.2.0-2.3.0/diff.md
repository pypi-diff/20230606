# Comparing `tmp/conventional_pre_commit-2.2.0.tar.gz` & `tmp/conventional_pre_commit-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conventional_pre_commit-2.2.0.tar", last modified: Fri Apr 21 21:47:21 2023, max compression
+gzip compressed data, was "conventional_pre_commit-2.3.0.tar", last modified: Tue Jun  6 16:32:04 2023, max compression
```

## Comparing `conventional_pre_commit-2.2.0.tar` & `conventional_pre_commit-2.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/conventional_pre_commit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/conventional_pre_commit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/conventional_pre_commit/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/conventional_pre_commit/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/tests/test_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:32:04.895924 conventional_pre_commit-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 16:31:55.000000 conventional_pre_commit-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-06-06 16:32:04.895924 conventional_pre_commit-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-06 16:31:55.000000 conventional_pre_commit-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:32:04.891924 conventional_pre_commit-2.3.0/conventional_pre_commit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:31:55.000000 conventional_pre_commit-2.3.0/conventional_pre_commit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-06 16:31:55.000000 conventional_pre_commit-2.3.0/conventional_pre_commit/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-06 16:31:55.000000 conventional_pre_commit-2.3.0/conventional_pre_commit/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:32:04.891924 conventional_pre_commit-2.3.0/conventional_pre_commit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-06-06 16:32:04.000000 conventional_pre_commit-2.3.0/conventional_pre_commit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 16:32:04.000000 conventional_pre_commit-2.3.0/conventional_pre_commit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:32:04.000000 conventional_pre_commit-2.3.0/conventional_pre_commit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-06 16:32:04.000000 conventional_pre_commit-2.3.0/conventional_pre_commit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-06 16:32:04.000000 conventional_pre_commit-2.3.0/conventional_pre_commit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-06 16:32:04.000000 conventional_pre_commit-2.3.0/conventional_pre_commit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-06 16:31:55.000000 conventional_pre_commit-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:32:04.895924 conventional_pre_commit-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:32:04.895924 conventional_pre_commit-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-06 16:31:55.000000 conventional_pre_commit-2.3.0/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-06 16:31:55.000000 conventional_pre_commit-2.3.0/tests/test_hook.py
```

### Comparing `conventional_pre_commit-2.2.0/LICENSE` & `conventional_pre_commit-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conventional_pre_commit-2.2.0/PKG-INFO` & `conventional_pre_commit-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conventional_pre_commit
-Version: 2.2.0
+Version: 2.3.0
 Summary: A pre-commit hook that checks commit messages for Conventional Commits formatting.
 Author-email: Compiler LLC <dev@compiler.la>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `conventional_pre_commit-2.2.0/README.md` & `conventional_pre_commit-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `conventional_pre_commit-2.2.0/conventional_pre_commit/format.py` & `conventional_pre_commit-2.3.0/conventional_pre_commit/format.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,20 @@
 
 
 def r_types(types):
     """Join types with pipe "|" to form regex ORs."""
     return "|".join(types)
 
 
-def r_scope():
+def r_scope(optional=True):
     """Regex str for an optional (scope)."""
-    return r"(\([\w \/:-]+\))?"
+    if optional:
+        return r"(\([\w \/:-]+\))?"
+    else:
+        return r"(\([\w \/:-]+\))"
 
 
 def r_delim():
     """Regex str for optional breaking change indicator and colon delimiter."""
     return r"!?:"
 
 
@@ -39,19 +42,19 @@
 def conventional_types(types=[]):
     """Return a list of Conventional Commits types merged with the given types."""
     if set(types) & set(CONVENTIONAL_TYPES) == set():
         return CONVENTIONAL_TYPES + types
     return types
 
 
-def is_conventional(input, types=DEFAULT_TYPES):
+def is_conventional(input, types=DEFAULT_TYPES, optional_scope=True):
     """
     Returns True if input matches Conventional Commits formatting
     https://www.conventionalcommits.org
 
     Optionally provide a list of additional custom types.
     """
     types = conventional_types(types)
-    pattern = f"^({r_types(types)}){r_scope()}{r_delim()}{r_subject()}$"
+    pattern = f"^({r_types(types)}){r_scope(optional_scope)}{r_delim()}{r_subject()}$"
     regex = re.compile(pattern, re.DOTALL)
 
     return bool(regex.match(input))
```

### Comparing `conventional_pre_commit-2.2.0/conventional_pre_commit/hook.py` & `conventional_pre_commit-2.3.0/conventional_pre_commit/hook.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 def main(argv=[]):
     parser = argparse.ArgumentParser(
         prog="conventional-pre-commit", description="Check a git commit message for Conventional Commits formatting."
     )
     parser.add_argument("types", type=str, nargs="*", default=format.DEFAULT_TYPES, help="Optional list of types to support")
     parser.add_argument("input", type=str, help="A file containing a git commit message")
+    parser.add_argument(
+        "--force-scope", action="store_false", default=True, dest="optional_scope", help="Force commit to have scope defined."
+    )
 
     if len(argv) < 1:
         argv = sys.argv[1:]
 
     try:
         args = parser.parse_args(argv)
     except SystemExit:
@@ -40,15 +43,15 @@
 {Colors.YELLOW}conventional-pre-commit couldn't decode your commit message.{Colors.RESTORE}
 {Colors.YELLOW}UTF-8{Colors.RESTORE} encoding is assumed, please configure git to write commit messages in UTF-8.
 See {Colors.LBLUE}https://git-scm.com/docs/git-commit/#_discussion{Colors.RESTORE} for more.
         """
         )
         return RESULT_FAIL
 
-    if format.is_conventional(message, args.types):
+    if format.is_conventional(message, args.types, args.optional_scope):
         return RESULT_SUCCESS
     else:
         print(
             f"""
         {Colors.LRED}[Bad Commit message] >>{Colors.RESTORE} {message}
         {Colors.YELLOW}Your commit message does not follow Conventional Commits formatting
         {Colors.LBLUE}https://www.conventionalcommits.org/{Colors.YELLOW}
@@ -62,15 +65,15 @@
 
             feat: implement new API
 
         {Colors.YELLOW}Example commit message fixing an issue:{Colors.RESTORE}
 
             fix: remove infinite loop
 
-        {Colors.YELLOW}Optionally, include a scope in parentheses after the type for more context:{Colors.RESTORE}
+        {Colors.YELLOW}Example commit with scope in parentheses after the type for more context:{Colors.RESTORE}
 
             fix(account): remove infinite loop"""
         )
         return RESULT_FAIL
 
 
 if __name__ == "__main__":
```

### Comparing `conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/PKG-INFO` & `conventional_pre_commit-2.3.0/conventional_pre_commit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conventional-pre-commit
-Version: 2.2.0
+Version: 2.3.0
 Summary: A pre-commit hook that checks commit messages for Conventional Commits formatting.
 Author-email: Compiler LLC <dev@compiler.la>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `conventional_pre_commit-2.2.0/pyproject.toml` & `conventional_pre_commit-2.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "conventional_pre_commit"
-version = "2.2.0"
+version = "2.3.0"
 description = "A pre-commit hook that checks commit messages for Conventional Commits formatting."
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["Programming Language :: Python :: 3 :: Only"]
 keywords = ["git", "pre-commit", "conventional-commits"]
 authors = [
     { name = "Compiler LLC", email = "dev@compiler.la" }
```

### Comparing `conventional_pre_commit-2.2.0/tests/test_format.py` & `conventional_pre_commit-2.3.0/tests/test_format.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 
 import pytest
 
 from conventional_pre_commit import format
 
-
 CUSTOM_TYPES = ["one", "two"]
 
 
 def test_r_types():
     result = format.r_types(CUSTOM_TYPES)
     regex = re.compile(result)
 
@@ -19,14 +18,22 @@
 def test_r_scope__optional():
     result = format.r_scope()
     regex = re.compile(result)
 
     assert regex.match("")
 
 
+def test_r_scope__not_optional():
+    result = format.r_scope(optional=False)
+    regex = re.compile(result)
+
+    # Assert not optional anymore
+    assert not regex.match("")
+
+
 def test_r_scope__parenthesis_required():
     result = format.r_scope()
     regex = re.compile(result)
 
     # without parens produces a match object with a 0 span
     # since the (scope) is optional
     without_parens = regex.match("something")
@@ -183,11 +190,23 @@
 
 def test_is_conventional__scope_space():
     input = "feat(scope) : message"
 
     assert not format.is_conventional(input)
 
 
+def test_is_conventional__scope_not_optional():
+    input = "feat: message"
+
+    assert not format.is_conventional(input, optional_scope=False)
+
+
+def test_is_conventional__scope_not_optional_empty_parenthesis():
+    input = "feat(): message"
+
+    assert not format.is_conventional(input, optional_scope=False)
+
+
 def test_is_conventional__missing_delimiter():
     input = "feat message"
 
     assert not format.is_conventional(input)
```

### Comparing `conventional_pre_commit-2.2.0/tests/test_hook.py` & `conventional_pre_commit-2.3.0/tests/test_hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,7 +88,19 @@
     assert result == RESULT_SUCCESS
 
 
 def test_main_fail__conventional_gbk(conventional_gbk_commit_path):
     result = main([conventional_gbk_commit_path])
 
     assert result == RESULT_FAIL
+
+
+def test_main_fail__conventional_with_scope(cmd, conventional_commit_path):
+    result = subprocess.call((cmd, "--force-scope", conventional_commit_path))
+
+    assert result == RESULT_FAIL
+
+
+def test_main_success__conventional_with_scope(cmd, conventional_commit_with_scope_path):
+    result = subprocess.call((cmd, "--force-scope", conventional_commit_with_scope_path))
+
+    assert result == RESULT_SUCCESS
```

