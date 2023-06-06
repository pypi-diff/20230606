# Comparing `tmp/sexpdata-1.0.0.tar.gz` & `tmp/sexpdata-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sexpdata-1.0.0.tar", last modified: Fri Mar  3 10:11:02 2023, max compression
+gzip compressed data, was "sexpdata-1.0.1.tar", last modified: Tue Jun  6 18:18:37 2023, max compression
```

## Comparing `sexpdata-1.0.0.tar` & `sexpdata-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,14 @@
-drwxrwxr-x   0 jdboyd    (1000) jdboyd    (1000)        0 2023-03-03 10:11:02.493781 sexpdata-1.0.0/
--rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)     2029 2023-03-03 10:11:02.493781 sexpdata-1.0.0/PKG-INFO
--rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)      843 2021-12-25 06:38:58.610580 sexpdata-1.0.0/README.rst
--rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)     1264 2023-03-03 10:05:11.486509 sexpdata-1.0.0/setup.py
--rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)    22600 2023-03-03 10:05:11.486509 sexpdata-1.0.0/sexpdata.py
+drwxrwxr-x   0 jdboyd    (1000) jdboyd    (1000)        0 2023-06-06 18:18:37.229969 sexpdata-1.0.1/
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)     1331 2021-12-25 06:38:58.000000 sexpdata-1.0.1/LICENSE
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)       19 2021-12-25 06:38:58.000000 sexpdata-1.0.1/MANIFEST.in
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)     1578 2023-06-06 18:18:37.229969 sexpdata-1.0.1/PKG-INFO
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)      843 2021-12-25 06:38:58.000000 sexpdata-1.0.1/README.rst
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)     1019 2023-06-06 18:16:55.000000 sexpdata-1.0.1/pyproject.toml
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)       38 2023-06-06 18:18:37.229969 sexpdata-1.0.1/setup.cfg
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)      986 2023-06-06 18:16:47.000000 sexpdata-1.0.1/setup.py
+drwxrwxr-x   0 jdboyd    (1000) jdboyd    (1000)        0 2023-06-06 18:18:37.229969 sexpdata-1.0.1/sexpdata.egg-info/
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)     1578 2023-06-06 18:18:37.000000 sexpdata-1.0.1/sexpdata.egg-info/PKG-INFO
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)      194 2023-06-06 18:18:37.000000 sexpdata-1.0.1/sexpdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)        1 2023-06-06 18:18:37.000000 sexpdata-1.0.1/sexpdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)        9 2023-06-06 18:18:37.000000 sexpdata-1.0.1/sexpdata.egg-info/top_level.txt
+-rw-rw-r--   0 jdboyd    (1000) jdboyd    (1000)    22999 2023-06-06 18:16:40.000000 sexpdata-1.0.1/sexpdata.py
```

### Comparing `sexpdata-1.0.0/README.rst` & `sexpdata-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `sexpdata-1.0.0/setup.py` & `sexpdata-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 import sys
 
-from distutils.core import setup
+from setuptools import setup
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='sexpdata',
-    version='1.0.0',
+    version='1.0.1',
     py_modules=['sexpdata'],
     author='Joshua D. Boyd, Takafumi Arakaki',
     author_email='jdboyd@jdboyd.net',
     url='https://github.com/jd-boyd/sexpdata',
     license='BSD License',
     description='S-expression parser for Python',
     long_description=long_description,
     keywords='s-expression, lisp, parser',
     classifiers=[
         "Development Status :: 3 - Alpha",
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         "Programming Language :: Lisp",
         "Programming Language :: Emacs-Lisp",
         # see: http://pypi.python.org/pypi?%3Aaction=list_classifiers
     ],
-    install_requires=[
-        "singledispatch; python_version < '3.4'",
-    ],
 )
```

### Comparing `sexpdata-1.0.0/sexpdata.py` & `sexpdata-1.0.1/sexpdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 # LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 # DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 # THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 __author__ = 'Joshua D. Boyd, Takafumi Arakaki'
 __license__ = 'BSD License'
 __all__ = [
     # API functions:
     'load', 'loads', 'dump', 'dumps', 'parse',
     # Utility functions:
     'car', 'cdr',
@@ -82,16 +82,14 @@
     from collections.abc import Iterable, Mapping, Sequence
 except ImportError:
     # Python < 3.3
     from collections import Iterable, Mapping, Sequence
 from itertools import chain
 from string import whitespace
 
-BRACKETS = {'(': ')', '[': ']'}
-
 
 ### PEP fallbacks
 
 try:
     from functools import singledispatch
 except ImportError:
     from singledispatch import singledispatch
@@ -491,20 +489,21 @@
 
 class Symbol(String):
 
     _lisp_quoted_specials = [
         ('\\', '\\\\'),    # must come first to avoid doubly quoting "\"
         ("'", r"\'"), ("`", r"\`"), ('"', r'\"'),
         ('(', r'\('), (')', r'\)'), ('[', r'\['), (']', r'\]'),
-        (' ', r'\ '), ('.', r'\.'), (',', r'\,'), ('?', r'\?'),
+        (' ', r'\ '), (',', r'\,'), ('?', r'\?'),
         (';', r'\;'), ('#', r'\#'),
     ]
 
     _lisp_quoted_to_raw = dict((q, r) for (r, q) in _lisp_quoted_specials)
 
+
 @tosexp.register(Symbol)
 def _(obj, **kwds):
     return Symbol.quote(obj)
 
 
 class Quoted(namedtuple('Quoted', 'x')):
 
@@ -537,14 +536,18 @@
     def from_opener(opener, val):
         cls_map = dict((cls.opener, cls) for cls in Delimiters.__subclasses__())
         if opener in cls_map.keys():
             return cls_map[opener](val)
         else:
             raise TypeError
 
+    @staticmethod
+    def get_brackets():
+        return {cls.opener: cls.closer for cls in Delimiters.__subclasses__()}
+
 @tosexp.register(Delimiters)
 def _(self, **kwds):
     # Don't break up expressions produced by certain overloads of tosexp
     dont_break = all(tosexp.dispatch(type(x)) not in DONT_BREAK_OVERLOADS for x in self.I)
 
     if "pretty_print" in kwds and kwds["pretty_print"] and not dont_break:
         expr_separator = "\n"
@@ -632,34 +635,44 @@
         super(ExpectSExp, self).__init__(
             'No s-exp is found after an apostrophe'
             ' at position {0}'.format(pos))
 
 
 class Parser(object):
 
-    closing_brackets = set(BRACKETS.values())
-    _atom_end_basic = \
-        set(BRACKETS) | set(closing_brackets) | set('"\'') | set(whitespace)
-    _atom_end_basic_or_escape_regexp = "|".join(map(re.escape,
-                                                    _atom_end_basic | set('\\')))
-    quote_or_escape_re = re.compile(r'"|\\')
+    brackets: dict
+    closing_brackets: set
+    _atom_end_basic: set
+    _atom_end_basic_or_escape_regexp: str
+
 
     def __init__(self, string, string_to=None, nil='nil', true='t', false=None,
                  line_comment=';'):
         self.string = string
         self.nil = nil
         self.true = true
         self.false = false
         self.string_to = (lambda x: x) if string_to is None else string_to
         self.line_comment = line_comment
+
+        # Compute brackets from delimiter
+        self.brackets = Delimiters.get_brackets()
+        self.closing_brackets = set(self.brackets.values())
+        self._atom_end_basic = \
+            set(self.brackets) | set(self.closing_brackets) | \
+            set('"') | set(whitespace)
+        self._atom_end_basic_or_escape_regexp = "|".join(map(re.escape,
+                                                         self._atom_end_basic | set('\\')))
+        self.quote_or_escape_re = re.compile(r'"|\\')
         self.atom_end = set([line_comment]) | self._atom_end_basic
         self.atom_end_or_escape_re = \
             re.compile("{0}|{1}".format(self._atom_end_basic_or_escape_regexp,
                                         re.escape(line_comment)))
 
+
     def parse_str(self, i):
         string = self.string
         chars = []
         append = chars.append
         search = self.quote_or_escape_re.search
 
         assert string[i] == '"'  # never fail
@@ -730,16 +743,16 @@
             c = string[i]
             if c == '"':
                 (i, subsexp) = self.parse_str(i)
                 append(self.string_to(subsexp))
             elif c in whitespace:
                 i += 1
                 continue
-            elif c in BRACKETS:
-                close = BRACKETS[c]
+            elif c in self.brackets:
+                close = self.brackets[c]
                 (i, subsexp) = self.parse_sexp(i + 1)
                 append(bracket(subsexp, c))
                 try:
                     nc = string[i]
                 except IndexError:
                     nc = None
                 if nc != close:
@@ -781,8 +794,9 @@
     [Symbol('a')]
     >>> parse("(a 'b)")
     [[Symbol('a'), Quoted(Symbol('b'))]]
     >>> parse("(a '(b))")
     [[Symbol('a'), Quoted([Symbol('b')])]]
 
     """
+    assert type(string)==str
     return Parser(string, **kwds).parse()
```

