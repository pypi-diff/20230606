# Comparing `tmp/mkpkg-2023.5.4.tar.gz` & `tmp/mkpkg-2023.6.1.tar.gz`

## Comparing `mkpkg-2023.5.4.tar` & `mkpkg-2023.6.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.coveragerc
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.readthedocs.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/codecov.yml
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/noxfile.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/test-requirements.in
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/test-requirements.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.github/SECURITY.md
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.github/release.yml
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/Makefile
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/conf.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/index.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/requirements.in
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/__main__.py
--rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/_cli.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.coveragerc.j2
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/COPYING.j2
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/README.rst.j2
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/codecov.yml
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/noxfile.py.j2
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/pyproject.toml.j2
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/tests.py.j2 -> package/tests/test_integration.py.j2
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.github/FUNDING.yml
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.github/SECURITY.md.j2
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.github/release.yml
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.github/workflows/ci.yml.j2
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/docs/conf.py.j2
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/docs/index.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/docs/requirements.in.j2
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/package/__init__.py.j2
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/package/__main__.py.j2
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/package/_build.py.j2
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/package/_cli.py.j2
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/package/tests/test_integration.py.j2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/tests/__init__.py
--rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/tests/test_integration.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/COPYING
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/README.rst
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/pyproject.toml
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/.coveragerc
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/.readthedocs.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/codecov.yml
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/noxfile.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/test-requirements.in
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/test-requirements.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/.github/release.yml
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/docs/Makefile
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/docs/conf.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/docs/index.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/docs/requirements.in
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/__main__.py
+-rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/_cli.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/.coveragerc.j2
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/COPYING.j2
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/README.rst.j2
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/codecov.yml
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/noxfile.py.j2
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/pyproject.toml.j2
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/tests.py.j2 -> package/tests/test_integration.py.j2
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/.github/FUNDING.yml
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/.github/SECURITY.md.j2
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/.github/release.yml
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/.github/workflows/ci.yml.j2
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/docs/conf.py.j2
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/docs/index.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/docs/requirements.in.j2
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/package/__init__.py.j2
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/package/__main__.py.j2
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/package/_build.py.j2
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/package/_cli.py.j2
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/template/package/tests/test_integration.py.j2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/tests/__init__.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/mkpkg/tests/test_integration.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/COPYING
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/README.rst
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 mkpkg-2023.6.1/PKG-INFO
```

### Comparing `mkpkg-2023.5.4/.pre-commit-config.yaml` & `mkpkg-2023.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/noxfile.py` & `mkpkg-2023.6.1/noxfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from tempfile import TemporaryDirectory
 import os
 
 import nox
 
 ROOT = Path(__file__).parent
 PYPROJECT = ROOT / "pyproject.toml"
 DOCS = ROOT / "docs"
@@ -53,25 +54,18 @@
 def audit(session):
     session.install("pip-audit", ROOT)
     session.run("python", "-m", "pip_audit")
 
 
 @session(tags=["build"])
 def build(session):
-    session.install("build")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-
-
-@session(tags=["style"])
-def readme(session):
     session.install("build", "twine")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-    session.run("twine", "check", "--strict", tmpdir + "/mkpkg*")
+    with TemporaryDirectory() as tmpdir:
+        session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
+        session.run("twine", "check", "--strict", tmpdir + "/*")
 
 
 @session()
 def secrets(session):
     session.install("detect-secrets")
     session.run("detect-secrets", "scan", ROOT)
 
@@ -100,28 +94,29 @@
             "man",
             "spelling",
         ]
     ],
 )
 def docs(session, builder):
     session.install("-r", DOCS / "requirements.txt")
-    tmpdir = Path(session.create_tmp())
-    argv = ["-n", "-T", "-W"]
-    if builder != "spelling":
-        argv += ["-q"]
-    session.run(
-        "python",
-        "-m",
-        "sphinx",
-        "-b",
-        builder,
-        DOCS,
-        tmpdir / builder,
-        *argv,
-    )
+    with TemporaryDirectory() as tmpdir_str:
+        tmpdir = Path(tmpdir_str)
+        argv = ["-n", "-T", "-W"]
+        if builder != "spelling":
+            argv += ["-q"]
+        session.run(
+            "python",
+            "-m",
+            "sphinx",
+            "-b",
+            builder,
+            DOCS,
+            tmpdir / builder,
+            *argv,
+        )
 
 
 @session(tags=["docs", "style"], name="docs(style)")
 def docs_style(session):
     session.install(
         "doc8",
         "pygments",
```

### Comparing `mkpkg-2023.5.4/test-requirements.txt` & `mkpkg-2023.6.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/.github/SECURITY.md` & `mkpkg-2023.6.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/.github/workflows/ci.yml` & `mkpkg-2023.6.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/docs/Makefile` & `mkpkg-2023.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/docs/conf.py` & `mkpkg-2023.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/docs/requirements.txt` & `mkpkg-2023.6.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/mkpkg/_cli.py` & `mkpkg-2023.6.1/mkpkg/_cli.py`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/mkpkg/template/.pre-commit-config.yaml` & `mkpkg-2023.6.1/mkpkg/template/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/mkpkg/template/COPYING.j2` & `mkpkg-2023.6.1/mkpkg/template/COPYING.j2`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/mkpkg/template/README.rst.j2` & `mkpkg-2023.6.1/mkpkg/template/README.rst.j2`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/mkpkg/template/noxfile.py.j2` & `mkpkg-2023.6.1/mkpkg/template/noxfile.py.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from tempfile import TemporaryDirectory
 import os
 
 import nox
 
 ROOT = Path(__file__).parent
 PYPROJECT = ROOT / "pyproject.toml"
 DOCS = ROOT / "docs"
@@ -53,25 +54,18 @@
 def audit(session):
     session.install("pip-audit", ROOT)
     session.run("python", "-m", "pip_audit")
 
 
 @session(tags=["build"])
 def build(session):
-    session.install("build")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-
-
-@session(tags=["style"])
-def readme(session):
     session.install("build", "twine")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-    session.run("twine", "check", "--strict", tmpdir + "/{{ package_name }}*")
+    with TemporaryDirectory() as tmpdir:
+        session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
+        session.run("twine", "check", "--strict", tmpdir + "/*")
 
 
 @session()
 def secrets(session):
     session.install("detect-secrets")
     session.run("detect-secrets", "scan", ROOT)
 
@@ -100,28 +94,29 @@
             "man",
             "spelling",
         ]
     ],
 )
 def docs(session, builder):
     session.install("-r", DOCS / "requirements.txt")
-    tmpdir = Path(session.create_tmp())
-    argv = ["-n", "-T", "-W"]
-    if builder != "spelling":
-        argv += ["-q"]
-    session.run(
-        "python",
-        "-m",
-        "sphinx",
-        "-b",
-        builder,
-        DOCS,
-        tmpdir / builder,
-        *argv,
-    )
+    with TemporaryDirectory() as tmpdir_str:
+        tmpdir = Path(tmpdir_str)
+        argv = ["-n", "-T", "-W"]
+        if builder != "spelling":
+            argv += ["-q"]
+        session.run(
+            "python",
+            "-m",
+            "sphinx",
+            "-b",
+            builder,
+            DOCS,
+            tmpdir / builder,
+            *argv,
+        )
 
 
 @session(tags=["docs", "style"], name="docs(style)")
 def docs_style(session):
     session.install(
         "doc8",
         "pygments",
```

### Comparing `mkpkg-2023.5.4/mkpkg/template/pyproject.toml.j2` & `mkpkg-2023.6.1/mkpkg/template/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/mkpkg/template/.github/SECURITY.md.j2` & `mkpkg-2023.6.1/mkpkg/template/.github/SECURITY.md.j2`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/mkpkg/template/.github/workflows/ci.yml.j2` & `mkpkg-2023.6.1/mkpkg/template/.github/workflows/ci.yml.j2`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/mkpkg/template/docs/conf.py.j2` & `mkpkg-2023.6.1/mkpkg/template/docs/conf.py.j2`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/mkpkg/tests/test_integration.py` & `mkpkg-2023.6.1/mkpkg/tests/test_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,14 @@
                 "tests-3.8",
                 "tests-3.9",
                 "tests-3.10",
                 "tests-3.11",
                 "tests-pypy3",
                 "audit",
                 "build",
-                "readme",
                 "secrets",
                 "style",
                 "typing",
             },
         )
 
     def test_docs_envs(self):
@@ -111,15 +110,14 @@
                 "tests-3.8",
                 "tests-3.9",
                 "tests-3.10",
                 "tests-3.11",
                 "tests-pypy3",
                 "audit",
                 "build",
-                "readme",
                 "secrets",
                 "style",
                 "typing",
                 "docs(dirhtml)",
                 "docs(doctest)",
                 "docs(linkcheck)",
                 "docs(man)",
```

### Comparing `mkpkg-2023.5.4/COPYING` & `mkpkg-2023.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/README.rst` & `mkpkg-2023.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/pyproject.toml` & `mkpkg-2023.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.4/PKG-INFO` & `mkpkg-2023.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkpkg
-Version: 2023.5.4
+Version: 2023.6.1
 Summary: A package @Julian uses to create Python packages.
 Project-URL: Homepage, https://github.com/Julian/mkpkg
 Project-URL: Documentation, https://mkpkg.readthedocs.io/
 Project-URL: Issues, https://github.com/Julian/mkpkg/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/Julian/mkpkg
 Author: Julian Berman
```

