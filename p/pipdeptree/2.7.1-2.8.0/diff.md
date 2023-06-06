# Comparing `tmp/pipdeptree-2.7.1.tar.gz` & `tmp/pipdeptree-2.8.0.tar.gz`

## Comparing `pipdeptree-2.7.1.tar` & `pipdeptree-2.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.prettierrc.toml
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/CHANGES.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/tox.ini
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/whitelist.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.github/workflows/check.yml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.github/workflows/release.yml
--rw-r--r--   0        0        0    97568 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/docs/twine-pdt.png
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/docs/v2beta-opts.org
--rw-r--r--   0        0        0    35115 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/src/pipdeptree/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/src/pipdeptree/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/src/pipdeptree/version.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/tests/guess_version_setuptools.py
--rw-r--r--   0        0        0    24276 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/tests/test_pipdeptree.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/LICENSE
--rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/README.md
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/pyproject.toml
--rw-r--r--   0        0        0    15544 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.prettierrc.toml
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/CHANGES.md
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/tox.ini
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/whitelist.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.github/workflows/check.yml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0    97568 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/docs/twine-pdt.png
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/docs/v2beta-opts.org
+-rw-r--r--   0        0        0    37458 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/src/pipdeptree/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/src/pipdeptree/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/src/pipdeptree/version.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/tests/guess_version_setuptools.py
+-rw-r--r--   0        0        0    30300 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/tests/test_pipdeptree.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/LICENSE
+-rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/README.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0    15544 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/PKG-INFO
```

### Comparing `pipdeptree-2.7.1/.pre-commit-config.yaml` & `pipdeptree-2.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.1/CHANGES.md` & `pipdeptree-2.8.0/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.1/tox.ini` & `pipdeptree-2.8.0/tox.ini`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.1/.github/workflows/check.yml` & `pipdeptree-2.8.0/.github/workflows/check.yml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   test:
     name: test ${{ matrix.py }}
     runs-on: ubuntu-22.04
     strategy:
       fail-fast: false
       matrix:
         py:
-          - "3.12.0-alpha.7"
+          - "3.12.0-beta.1"
           - "3.11"
           - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
     steps:
       - name: Install OS dependencies
@@ -91,12 +91,12 @@
           python-version: "3.11"
       - name: install build
         run: python -m pip install build
       - uses: actions/checkout@v3
       - name: build package
         run: python -m build --sdist --wheel . -o dist
       - name: publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.5
+        uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           skip_existing: true
           user: __token__
           password: ${{ secrets.pypi_password }}
```

### Comparing `pipdeptree-2.7.1/.github/workflows/release.yml` & `pipdeptree-2.8.0/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         run: python -m pip install build
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Build package
         run: pyproject-build -s -w . -o dist
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.5
+        uses: pypa/gh-action-pypi-publish@v1.8.6
```

### Comparing `pipdeptree-2.7.1/docs/twine-pdt.png` & `pipdeptree-2.8.0/docs/twine-pdt.png`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.1/docs/v2beta-opts.org` & `pipdeptree-2.8.0/docs/v2beta-opts.org`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.1/src/pipdeptree/__init__.py` & `pipdeptree-2.8.0/src/pipdeptree/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -458,24 +458,98 @@
 def render_text(tree, list_all=True, frozen=False):
     """Print tree as text on console
 
     :param dict tree: the package tree
     :param bool list_all: whether to list all the pgks at the root level or only those that are the sub-dependencies
     :param bool frozen: show the names of the pkgs in the output that's favourable to pip --freeze
     :returns: None
-
     """
     tree = tree.sort()
     nodes = tree.keys()
     branch_keys = {r.key for r in chain.from_iterable(tree.values())}
-    use_bullets = not frozen
 
     if not list_all:
         nodes = [p for p in nodes if p.key not in branch_keys]
 
+    if sys.stdout.encoding.lower() in ("utf-8", "utf-16", "utf-32"):
+        _render_text_with_unicode(tree, nodes, frozen)
+    else:
+        _render_text_without_unicode(tree, nodes, frozen)
+
+
+def _render_text_with_unicode(tree, nodes, frozen):
+    use_bullets = not frozen
+
+    def aux(
+        node,
+        parent=None,
+        indent=0,
+        cur_chain=None,
+        prefix="",
+        depth=0,
+        has_grand_parent=False,
+        is_last_child=False,
+        parent_is_last_child=False,
+    ):
+        cur_chain = cur_chain or []
+        node_str = node.render(parent, frozen)
+        next_prefix = ""
+        next_indent = indent + 2
+
+        if parent:
+            bullet = "├── "
+            if is_last_child:
+                bullet = "└── "
+
+            line_char = "│"
+            if not use_bullets:
+                line_char = ""
+                # Add 2 spaces so direct dependencies to a project are indented
+                bullet = "  "
+
+            if has_grand_parent:
+                next_indent -= 1
+                if parent_is_last_child:
+                    offset = 0 if len(line_char) == 1 else 1
+                    prefix += " " * (indent + 1 - offset - depth)
+                else:
+                    prefix += line_char + " " * (indent - depth)
+                # Without this extra space, bullets will point to the space just before the project name
+                prefix += " " if use_bullets else ""
+            next_prefix = prefix
+            node_str = prefix + bullet + node_str
+        result = [node_str]
+
+        children = tree.get_children(node.key)
+        children_strings = [
+            aux(
+                c,
+                node,
+                indent=next_indent,
+                cur_chain=cur_chain + [c.project_name],
+                prefix=next_prefix,
+                depth=depth + 1,
+                has_grand_parent=parent is not None,
+                is_last_child=c is children[-1],
+                parent_is_last_child=is_last_child,
+            )
+            for c in children
+            if c.project_name not in cur_chain
+        ]
+
+        result += list(chain.from_iterable(children_strings))
+        return result
+
+    lines = chain.from_iterable([aux(p) for p in nodes])
+    print("\n".join(lines))
+
+
+def _render_text_without_unicode(tree, nodes, frozen):
+    use_bullets = not frozen
+
     def aux(node, parent=None, indent=0, cur_chain=None):
         cur_chain = cur_chain or []
         node_str = node.render(parent, frozen)
         if parent:
             prefix = " " * indent + ("- " if use_bullets else "")
             node_str = prefix + node_str
         result = [node_str]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pipdeptree-2.7.1/LICENSE` & `pipdeptree-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.1/README.md` & `pipdeptree-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.1/pyproject.toml` & `pipdeptree-2.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.1/PKG-INFO` & `pipdeptree-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipdeptree
-Version: 2.7.1
+Version: 2.8.0
 Summary: Command line utility to show dependency tree of packages.
 Project-URL: Changelog, https://github.com/tox-dev/pipdeptree/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/tox-dev/pipdeptree/blob/main/README.md#pipdeptree
 Project-URL: Homepage, https://github.com/tox-dev/pipdeptree
 Project-URL: Source, https://github.com/tox-dev/pipdeptree
 Project-URL: Tracker, https://github.com/tox-dev/pipdeptree/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Vineet Naik <naikvin@gmail.com>
```

