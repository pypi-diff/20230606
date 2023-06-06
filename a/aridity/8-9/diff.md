# Comparing `tmp/aridity-8.tar.gz` & `tmp/aridity-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aridity-8.tar", last modified: Wed Nov 13 16:21:50 2019, max compression
+gzip compressed data, was "dist/aridity-9.tar", last modified: Sun Nov 17 11:26:57 2019, max compression
```

## Comparing `aridity-8.tar` & `aridity-9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 arc       (1000) arc       (1000)        0 2019-11-13 16:21:50.000000 aridity-8/
--rw-r--r--   0 arc       (1000) arc       (1000)      399 2019-11-13 16:21:50.000000 aridity-8/PKG-INFO
--rw-r--r--   0 arc       (1000) arc       (1000)      132 2019-11-13 15:09:55.000000 aridity-8/README.md
--rwxr-xr-x   0 arc       (1000) arc       (1000)       63 2019-09-23 10:46:29.000000 aridity-8/arid-config
--rw-r--r--   0 arc       (1000) arc       (1000)     1228 2019-09-23 10:46:29.000000 aridity-8/arid_config.py
-drwxr-xr-x   0 arc       (1000) arc       (1000)        0 2019-11-13 16:21:50.000000 aridity-8/aridimpl/
--rw-r--r--   0 arc       (1000) arc       (1000)      689 2019-09-23 10:46:29.000000 aridity-8/aridimpl/__init__.py
--rw-r--r--   0 arc       (1000) arc       (1000)     6370 2019-11-13 16:15:22.000000 aridity-8/aridimpl/context.py
--rw-r--r--   0 arc       (1000) arc       (1000)     2782 2019-09-23 10:46:29.000000 aridity-8/aridimpl/directives.py
--rw-r--r--   0 arc       (1000) arc       (1000)     4157 2019-09-23 10:46:29.000000 aridity-8/aridimpl/functions.py
--rw-r--r--   0 arc       (1000) arc       (1000)     4393 2019-09-23 10:46:29.000000 aridity-8/aridimpl/grammar.py
--rw-r--r--   0 arc       (1000) arc       (1000)     6384 2019-09-23 10:46:29.000000 aridity-8/aridimpl/model.py
--rw-r--r--   0 arc       (1000) arc       (1000)     3098 2019-09-23 10:46:29.000000 aridity-8/aridimpl/repl.py
--rw-r--r--   0 arc       (1000) arc       (1000)    12799 2019-11-13 15:26:47.000000 aridity-8/aridimpl/test_context.py
--rw-r--r--   0 arc       (1000) arc       (1000)     5852 2019-09-23 10:46:29.000000 aridity-8/aridimpl/test_grammar.py
--rw-r--r--   0 arc       (1000) arc       (1000)     3239 2019-09-23 10:46:29.000000 aridity-8/aridimpl/test_model.py
--rw-r--r--   0 arc       (1000) arc       (1000)     2905 2019-09-23 10:46:29.000000 aridity-8/aridimpl/test_repl.py
--rw-r--r--   0 arc       (1000) arc       (1000)     1104 2019-09-23 10:46:29.000000 aridity-8/aridimpl/test_util.py
--rw-r--r--   0 arc       (1000) arc       (1000)     2306 2019-09-23 10:46:29.000000 aridity-8/aridimpl/util.py
-drwxr-xr-x   0 arc       (1000) arc       (1000)        0 2019-11-13 16:21:50.000000 aridity-8/aridity.egg-info/
--rw-r--r--   0 arc       (1000) arc       (1000)      399 2019-11-13 16:21:50.000000 aridity-8/aridity.egg-info/PKG-INFO
--rw-r--r--   0 arc       (1000) arc       (1000)      495 2019-11-13 16:21:50.000000 aridity-8/aridity.egg-info/SOURCES.txt
--rw-r--r--   0 arc       (1000) arc       (1000)        1 2019-11-13 16:21:50.000000 aridity-8/aridity.egg-info/dependency_links.txt
--rw-r--r--   0 arc       (1000) arc       (1000)       10 2019-11-13 16:21:50.000000 aridity-8/aridity.egg-info/requires.txt
--rw-r--r--   0 arc       (1000) arc       (1000)       29 2019-11-13 16:21:50.000000 aridity-8/aridity.egg-info/top_level.txt
--rwxr-xr-x   0 arc       (1000) arc       (1000)     1076 2019-09-23 10:46:29.000000 aridity-8/aridity.py
--rw-r--r--   0 arc       (1000) arc       (1000)       67 2019-11-13 16:21:50.000000 aridity-8/setup.cfg
--rw-r--r--   0 arc       (1000) arc       (1000)      690 2019-11-13 16:21:49.000000 aridity-8/setup.py
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2019-11-17 11:26:57.000000 aridity-9/
+-rwxrwxr-x   0 arc       (1000) arc       (1000)       63 2019-11-03 21:11:31.000000 aridity-9/arid-config
+-rwxrwxr-x   0 arc       (1000) arc       (1000)     1076 2019-11-03 21:11:31.000000 aridity-9/aridity.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1228 2019-11-03 21:11:31.000000 aridity-9/arid_config.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      690 2019-11-17 11:26:56.000000 aridity-9/setup.py
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2019-11-17 11:26:57.000000 aridity-9/aridimpl/
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5852 2019-11-03 21:11:31.000000 aridity-9/aridimpl/test_grammar.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2782 2019-11-03 21:11:31.000000 aridity-9/aridimpl/directives.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2306 2019-11-03 21:11:31.000000 aridity-9/aridimpl/util.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     6370 2019-11-13 20:23:49.000000 aridity-9/aridimpl/context.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1104 2019-11-03 21:11:31.000000 aridity-9/aridimpl/test_util.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)    12799 2019-11-13 20:23:49.000000 aridity-9/aridimpl/test_context.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3239 2019-11-03 21:11:31.000000 aridity-9/aridimpl/test_model.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3098 2019-11-03 21:11:31.000000 aridity-9/aridimpl/repl.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     6384 2019-11-03 21:11:31.000000 aridity-9/aridimpl/model.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4409 2019-11-17 10:35:11.000000 aridity-9/aridimpl/grammar.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4157 2019-11-03 21:11:31.000000 aridity-9/aridimpl/functions.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2905 2019-11-03 21:11:31.000000 aridity-9/aridimpl/test_repl.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      689 2019-11-03 21:11:31.000000 aridity-9/aridimpl/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       67 2019-11-17 11:26:57.000000 aridity-9/setup.cfg
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2019-11-17 11:26:57.000000 aridity-9/aridity.egg-info/
+-rw-rw-r--   0 arc       (1000) arc       (1000)        1 2019-11-17 11:26:57.000000 aridity-9/aridity.egg-info/dependency_links.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       10 2019-11-17 11:26:57.000000 aridity-9/aridity.egg-info/requires.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      495 2019-11-17 11:26:57.000000 aridity-9/aridity.egg-info/SOURCES.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       29 2019-11-17 11:26:57.000000 aridity-9/aridity.egg-info/top_level.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      399 2019-11-17 11:26:57.000000 aridity-9/aridity.egg-info/PKG-INFO
+-rw-rw-r--   0 arc       (1000) arc       (1000)      132 2019-11-03 21:11:31.000000 aridity-9/README.md
+-rw-rw-r--   0 arc       (1000) arc       (1000)      399 2019-11-17 11:26:57.000000 aridity-9/PKG-INFO
```

### Comparing `aridity-8/arid_config.py` & `aridity-9/arid_config.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/__init__.py` & `aridity-9/aridimpl/__init__.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/context.py` & `aridity-9/aridimpl/context.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/directives.py` & `aridity-9/aridimpl/directives.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/functions.py` & `aridity-9/aridimpl/functions.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/grammar.py` & `aridity-9/aridimpl/grammar.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with aridity.  If not, see <http://www.gnu.org/licenses/>.
 
-from pyparsing import Forward, OneOrMore, Optional, Or, Regex, Suppress, ZeroOrMore, NoMatch, Literal
+from pyparsing import Forward, OneOrMore, Optional, MatchFirst, Regex, Suppress, ZeroOrMore, NoMatch, Literal
 from decimal import Decimal
 from .model import Text, Boolean, Number, Blank, Call, Concat, Boundary, Entry
 import re
 
 class AnyScalar:
 
     numberpattern = re.compile('^-?(?:[0-9]+|[0-9]*[.][0-9]+)$')
@@ -59,15 +59,15 @@
             for o, c in cls.bracketpairs:
                 yield (Suppress(Regex("lit|'")) + Suppress(o) + Regex("[^%s]*" % re.escape(c)) + Suppress(c)).setParseAction(Text.pa)
                 def getbrackets(blankpa, scalarpa):
                     optblank = cls.getoptblank(blankpa, '')
                     return Literal(o) + ZeroOrMore(optblank + cls.getarg(action, scalarpa, c)) + optblank + Literal(c)
                 yield (Suppress(Regex('pass|[.]')) + getbrackets(Text.pa, Text.pa)).setParseAction(Concat.strictpa)
                 yield (cls.identifier + getbrackets(Blank.pa, AnyScalar.pa)).setParseAction(Call.pa)
-        action << Suppress('$').leaveWhitespace() + Or(clauses()).leaveWhitespace()
+        action << Suppress('$').leaveWhitespace() + MatchFirst(clauses()).leaveWhitespace()
         return action
 
     @classmethod
     def getarg(cls, action, scalarpa, boundarychars):
         opttext = Optional(cls.gettext(Text.pa, boundarychars))
         return (OneOrMore(opttext + action) + opttext | cls.gettext(scalarpa, boundarychars)).setParseAction(Concat.smartpa)
```

### Comparing `aridity-8/aridimpl/model.py` & `aridity-9/aridimpl/model.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/repl.py` & `aridity-9/aridimpl/repl.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/test_context.py` & `aridity-9/aridimpl/test_context.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/test_grammar.py` & `aridity-9/aridimpl/test_grammar.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/test_model.py` & `aridity-9/aridimpl/test_model.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/test_repl.py` & `aridity-9/aridimpl/test_repl.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/test_util.py` & `aridity-9/aridimpl/test_util.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridimpl/util.py` & `aridity-9/aridimpl/util.py`

 * *Files identical despite different names*

### Comparing `aridity-8/aridity.py` & `aridity-9/aridity.py`

 * *Files identical despite different names*

