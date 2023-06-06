# Comparing `tmp/logaut-0.1.1.tar.gz` & `tmp/logaut-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logaut-0.1.1.tar", last modified: Sun Jun 20 08:35:23 2021, max compression
+gzip compressed data, was "logaut-0.2.0.tar", max compression
```

## Comparing `logaut-0.1.1.tar` & `logaut-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0     7652 2021-06-08 09:19:21.847846 logaut-0.1.1/LICENSE
--rw-r--r--   0        0        0     5458 2021-06-20 08:35:14.129504 logaut-0.1.1/README.md
--rw-r--r--   0        0        0      891 2021-06-20 08:35:14.133504 logaut-0.1.1/logaut/__init__.py
--rw-r--r--   0        0        0     9049 2021-06-20 08:35:07.257510 logaut-0.1.1/logaut/_registry.py
--rw-r--r--   0        0        0     1409 2021-06-20 08:35:07.257510 logaut-0.1.1/logaut/backends/__init__.py
--rw-r--r--   0        0        0     4476 2021-06-20 08:35:07.261510 logaut-0.1.1/logaut/backends/base.py
--rw-r--r--   0        0        0      806 2021-06-20 08:35:07.261510 logaut-0.1.1/logaut/backends/common/__init__.py
--rw-r--r--   0        0        0     7245 2021-06-20 08:35:14.133504 logaut-0.1.1/logaut/backends/common/process_mona_output.py
--rw-r--r--   0        0        0      810 2021-06-20 08:35:07.265509 logaut-0.1.1/logaut/backends/ltlf2dfa/__init__.py
--rw-r--r--   0        0        0     4028 2021-06-20 08:35:07.269510 logaut-0.1.1/logaut/backends/ltlf2dfa/core.py
--rw-r--r--   0        0        0     4899 2021-06-20 08:35:07.269510 logaut-0.1.1/logaut/backends/ltlf2dfa/to_ltlf2dfa_formula.py
--rw-r--r--   0        0        0      807 2021-06-20 08:35:07.269510 logaut-0.1.1/logaut/backends/lydia/__init__.py
--rw-r--r--   0        0        0     2239 2021-06-20 08:35:07.273510 logaut-0.1.1/logaut/backends/lydia/_lydia_utils.py
--rw-r--r--   0        0        0     2787 2021-06-20 08:35:07.273510 logaut-0.1.1/logaut/backends/lydia/core.py
--rw-r--r--   0        0        0     7295 2021-06-20 08:35:07.273510 logaut-0.1.1/logaut/backends/lydia/to_lydia_grammar.py
--rw-r--r--   0        0        0     3484 2021-06-20 08:35:07.277510 logaut-0.1.1/logaut/core.py
--rw-r--r--   0        0        0     1503 2021-06-20 08:35:07.361509 logaut-0.1.1/logaut/exceptions.py
--rw-r--r--   0        0        0     1731 2021-06-20 08:35:07.361509 logaut-0.1.1/logaut/helpers.py
--rw-r--r--   0        0        0     1789 2021-06-20 08:35:14.141504 logaut-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6436 2021-06-20 08:35:23.154802 logaut-0.1.1/setup.py
--rw-r--r--   0        0        0     6602 2021-06-20 08:35:23.155136 logaut-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-06 11:41:10.682273 logaut-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5609 2023-06-06 11:41:10.682273 logaut-0.2.0/README.md
+-rw-r--r--   0        0        0      891 2023-06-06 11:41:10.682273 logaut-0.2.0/logaut/__init__.py
+-rw-r--r--   0        0        0     9049 2023-06-06 11:41:10.682273 logaut-0.2.0/logaut/_registry.py
+-rw-r--r--   0        0        0     1409 2023-06-06 11:41:10.682273 logaut-0.2.0/logaut/backends/__init__.py
+-rw-r--r--   0        0        0     4650 2023-06-06 11:41:10.682273 logaut-0.2.0/logaut/backends/base.py
+-rw-r--r--   0        0        0      806 2023-06-06 11:41:10.682273 logaut-0.2.0/logaut/backends/common/__init__.py
+-rw-r--r--   0        0        0      957 2023-06-06 11:41:10.682273 logaut-0.2.0/logaut/backends/common/find_atoms/__init__.py
+-rw-r--r--   0        0        0     2084 2023-06-06 11:41:10.682273 logaut-0.2.0/logaut/backends/common/find_atoms/base.py
+-rw-r--r--   0        0        0     1710 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/common/find_atoms/ldl.py
+-rw-r--r--   0        0        0     1269 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/common/find_atoms/ltl.py
+-rw-r--r--   0        0        0     7314 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/common/process_mona_output.py
+-rw-r--r--   0        0        0     1296 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/common/utils.py
+-rw-r--r--   0        0        0      810 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/ltlf2dfa/__init__.py
+-rw-r--r--   0        0        0     6424 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/ltlf2dfa/core.py
+-rw-r--r--   0        0        0     4899 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/ltlf2dfa/to_ltlf2dfa_formula.py
+-rw-r--r--   0        0        0      807 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/lydia/__init__.py
+-rw-r--r--   0        0        0     2357 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/lydia/_lydia_utils.py
+-rw-r--r--   0        0        0     3323 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/lydia/core.py
+-rw-r--r--   0        0        0     7295 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/backends/lydia/to_lydia_grammar.py
+-rw-r--r--   0        0        0     3484 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/core.py
+-rw-r--r--   0        0        0     1503 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/exceptions.py
+-rw-r--r--   0        0        0     2477 2023-06-06 11:41:10.686272 logaut-0.2.0/logaut/helpers.py
+-rw-r--r--   0        0        0     1830 2023-06-06 11:41:10.686272 logaut-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6854 1970-01-01 00:00:00.000000 logaut-0.2.0/PKG-INFO
```

### Comparing `logaut-0.1.1/LICENSE` & `logaut-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logaut-0.1.1/README.md` & `logaut-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,23 +77,31 @@
 ```
 docker pull whitemech/lydia:latest
 ```
 - Make the Docker image executable under the name `lydia`.
   On Linux and MacOS machines, the following commands should work:
 ```
 echo '#!/usr/bin/env sh' > lydia
-echo 'docker run -v$(pwd):/home/default whitemech/lydia lydia $@' >> lydia
+echo 'docker run -v$(pwd):/home/default whitemech/lydia lydia "$@"' >> lydia
 sudo chmod u+x lydia
 sudo mv lydia /usr/local/bin/
 ```
 
+
 This will install an alias to the inline Docker image execution
 in your system PATH. Instead of `/usr/local/bin/`
 you may use another path which is still in the `PATH` variable.
 
+On Windows, make a `.bat` file:
+```
+docker run --name lydia -v"%cd%":/home/default whitemech/lydia lydia %*
+```
+And add it to your PATH variable.
+
+
 ## Quickstart
 
 Now you are ready to go:
 ```python
 from logaut import ltl2dfa
 from pylogics.parsers import parse_ltl
 formula = parse_ltl("F(a)")
```

### Comparing `logaut-0.1.1/logaut/__init__.py` & `logaut-0.2.0/logaut/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with logaut.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 """From LOGics to AUTomata"""
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 from .core import fol2dfa, ldl2dfa, ltl2dfa, mso2dfa, pldl2dfa, pltl2dfa
```

### Comparing `logaut-0.1.1/logaut/_registry.py` & `logaut-0.2.0/logaut/_registry.py`

 * *Files identical despite different names*

### Comparing `logaut-0.1.1/logaut/backends/__init__.py` & `logaut-0.2.0/logaut/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `logaut-0.1.1/logaut/backends/base.py` & `logaut-0.2.0/logaut/backends/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,21 +84,28 @@
             setattr(class_, method_name, mcs._add_validation(method_obj))
         return class_
 
 
 class Backend(ABC, metaclass=_MetaBackend):
     """Logaut back-end interface."""
 
+    def __init__(self) -> None:
+        """Initialize the backend."""
+        self.init_checks()
+
     @classmethod
     def __not_supported_error(cls, operation: str) -> Exception:
         """Raise a not supported error."""
         return NotImplementedBackendFunction(
             f"operation '{operation}' is not supported by backend '{cls.__name__}'"
         )
 
+    def init_checks(self) -> None:
+        """Do initialization checks."""
+
     def ltl2dfa(self, formula: Formula) -> DFA:
         """
         Transform an LTL formula into a DFA.
 
         :param formula: an LTL formula
         :return: the equivalent DFA
         """
```

### Comparing `logaut-0.1.1/logaut/backends/common/__init__.py` & `logaut-0.2.0/logaut/backends/common/__init__.py`

 * *Files identical despite different names*

### Comparing `logaut-0.1.1/logaut/backends/common/process_mona_output.py` & `logaut-0.2.0/logaut/backends/common/process_mona_output.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 # along with logaut.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 """Parse Lydia output to produce a pythomata.DFA."""
 
 import re
 from dataclasses import dataclass
-from typing import Dict, Match, Set, Tuple, cast
+from typing import Dict, List, Match, Set, Tuple, Union, cast
 
 from pythomata.impl.symbolic import SymbolicDFA
 from sympy import And, Not, Or, Symbol, true
-from sympy.logic.boolalg import BooleanFunction
+from sympy.logic.boolalg import BooleanAtom, BooleanFunction
 
 
 @dataclass
 class MONAOutput:
     """
     Dataclass to represent the MONA DFA output.
 
@@ -188,15 +188,15 @@
 
     def _index_value_pair_to_literal(pair):
         index, value = pair
         value = bool(int(value))
         literal = Symbol(variable_names[index])
         return literal if value else Not(literal)
 
-    processed_guards = []
+    processed_guards: List[Union[BooleanFunction, BooleanAtom]] = []
     for guard in guards:
         if guard == "":
             processed_guards.append(true)
         else:
             filtered_guard = list(filter(lambda x: x[1] != "X", enumerate(guard)))
             clause = And(*map(_index_value_pair_to_literal, filtered_guard))
             processed_guards.append(clause)
```

### Comparing `logaut-0.1.1/logaut/backends/ltlf2dfa/__init__.py` & `logaut-0.2.0/logaut/backends/ltlf2dfa/__init__.py`

 * *Files identical despite different names*

### Comparing `logaut-0.1.1/logaut/backends/ltlf2dfa/core.py` & `logaut-0.2.0/logaut/backends/lydia/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,111 +16,86 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with logaut.  If not, see <https://www.gnu.org/licenses/>.
 #
 
-"""
-Implementation of the LTLf2DFA backend.
-
-Repository:
-
-    https://github.com/whitemech/LTLf2DFA/
-
-"""
-import re
+"""Implementation of the Lydia backend."""
 import shutil
-from typing import Match, Tuple, cast
+from typing import Tuple
 
-import ltlf2dfa
-from ltlf2dfa.parser.ltlf import LTLfParser
-from ltlf2dfa.parser.pltlf import PLTLfParser
-from pylogics.syntax.base import Formula, Logic
+from pylogics.syntax.base import Formula
 from pythomata.core import DFA
 from pythomata.impl.symbolic import SymbolicDFA
 
 from logaut.backends.base import Backend
 from logaut.backends.common.process_mona_output import (
     parse_automaton,
     parse_mona_output,
 )
-from logaut.backends.ltlf2dfa.to_ltlf2dfa_formula import to_string
+from logaut.backends.common.utils import _check_atoms_match_regex
+from logaut.backends.lydia._lydia_utils import call_lydia, postprocess_lydia_output
+from logaut.backends.lydia.to_lydia_grammar import to_string
+from logaut.helpers import temporary_directory
 
+# this is stricter than the actual regex used by lydia.
+_LYDIA_SYMBOL_REGEX = "[a-z_][a-z0-9_]*"
 
-class LTLf2DFABackend(Backend):
-    """The LTLf2DFA backend."""
+
+class LydiaBackend(Backend):
+    """The Lydia backend."""
 
     _LOWERBOUND_VERSION: Tuple[int, int, int] = (0, 1, 0)
     _UPPERBOUND_VERSION: Tuple[int, int, int] = (0, 2, 0)
 
     @classmethod
-    def __check_mona(cls):
-        """Check that the MONA CLI tool is available."""
-        is_mona_present = shutil.which("mona") is not None
-        if is_mona_present is None:
+    def __check_lydia(cls):
+        """Check that the Lydia CLI tool is available."""
+        is_lydia_present = shutil.which("lydia") is not None
+        if is_lydia_present is None:
             raise Exception(
-                "MONA binary is not installed. Please follow"
-                "the installation instructions at https://github.com/whitemech/MONA.\n"
+                "Lydia binary is not installed. Please follow"
+                "the installation instructions at https://github.com/whitemech/lydia.\n"
                 "If instead it is installed, please check that it is in the system PATH."
             )
+        # TODO: check Lydia version
 
-    @classmethod
-    def __check_ltlf2dfa(cls):
-        """Check that the LTLf2DFA package is at the right version."""
-        is_right_version = ltlf2dfa.__version__ == "1.0.1"
-        if not is_right_version:
-            raise Exception(
-                "LTLf2DFA needs to be at version 1.0.1. "
-                "Please install it manually using:"
-                "\n"
-                "\tpip install git+https://github.com/whitemech/LTLf2DFA.git@develop#egg=ltlf2dfa"
-            )
-
-    def __post_init__(self):
+    def init_checks(self):
         """Do post-initialization checks."""
-        self.__check_mona()
-        self.__check_ltlf2dfa()
+        self.__check_lydia()
 
-    def ltl2dfa(self, formula: Formula) -> DFA:
-        """From LTL to DFA."""
+    def ldl2dfa(self, formula: Formula) -> DFA:
+        """From LDL to DFA."""
         return _process_formula(formula)
 
-    def pltl2dfa(self, formula: Formula) -> DFA:
-        """From PLTL to DFA."""
+    def ltl2dfa(self, formula: Formula) -> DFA:
+        """From LTL to DFA."""
         return _process_formula(formula)
 
 
 def _process_formula(formula: Formula) -> SymbolicDFA:
     """
     Process a formula with Lydia.
 
     :param formula: the formula
     :return: the DFA
     """
-    logic = formula.logic
+    _check_atoms_match_regex(formula, _LYDIA_SYMBOL_REGEX, "Lydia")
     formula_str = to_string(formula)
-    parser = LTLfParser() if logic == Logic.LTL else PLTLfParser()
-    ltlf2dfa_formula = parser(formula_str)
-    mona_output_string = ltlf2dfa_formula.to_dfa(mona_dfa_out=True)
-    mona_output = parse_mona_output(postprocess_output(mona_output_string))
+
+    with temporary_directory() as tmpdir:
+        tmpfilename = "formula.txt"
+        tmpfile = tmpdir / tmpfilename
+        tmpfile = tmpfile.resolve()
+        tmpfile.write_text(formula_str)
+
+        output = call_lydia(
+            f"--logic={formula.logic.value}f",
+            f"--file={tmpfilename}",
+            "-p",
+            cwd=str(tmpdir),
+        )
+    mona_output_string = postprocess_lydia_output(output)
+    mona_output = parse_mona_output(mona_output_string)
     automaton = parse_automaton(mona_output)
     return automaton
-
-
-def postprocess_output(output: str) -> str:
-    """
-    Post-process MONA output.
-
-    Capture the output related to the MONA DFA transitions.
-
-    :param: the raw output from the LTLf2DFA tool.
-    :return: the output associated to the DFA.
-    """
-    regex = re.compile(
-        r".*(?=\nFormula is (valid|unsatisfiable)|A counter-example)",
-        flags=re.MULTILINE | re.DOTALL,
-    )
-    match = regex.search(output)
-    if match is None:
-        raise Exception("cannot find automaton description in MONA output.")
-    return cast(Match, regex.search(output)).group(0)
```

### Comparing `logaut-0.1.1/logaut/backends/ltlf2dfa/to_ltlf2dfa_formula.py` & `logaut-0.2.0/logaut/backends/ltlf2dfa/to_ltlf2dfa_formula.py`

 * *Files identical despite different names*

### Comparing `logaut-0.1.1/logaut/backends/lydia/__init__.py` & `logaut-0.2.0/logaut/backends/lydia/__init__.py`

 * *Files identical despite different names*

### Comparing `logaut-0.1.1/logaut/backends/lydia/_lydia_utils.py` & `logaut-0.2.0/logaut/backends/lydia/_lydia_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,33 +19,38 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with logaut.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 """This module contains utilities to call the Lydia tool from Python."""
 import re
 import subprocess
+import sys
 from typing import Match, cast
 
 from pylogics.helpers.misc import enforce
 
 from logaut.exceptions import LogautException
 
 
-def call_lydia(*args) -> str:
+def call_lydia(*args, cwd: str = ".") -> str:
     """Call the Lydia CLI tool with the arguments provided."""
-    command = ["lydia", *args]
+    command = ["lydia" if sys.platform != "win32" else "lydia.bat", *args]
+    output = ""
+    stderr = ""
     try:
-        result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        result = subprocess.run(
+            command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=cwd
+        )
         output = result.stdout.decode()
         stderr = result.stderr.decode()
         enforce(result.returncode == 0, exception_cls=LogautException)
         return output
     except LogautException:
         raise Exception(  # type: ignore
-            f"the Lydia command {' '.join(command)} failed.\nstdout={output}\nstderr={stderr}"  # type: ignore
+            f"the Lydia command {' '.join(command)} failed.\nstdout={output}\nstderr={stderr}"
         )
     except Exception as e:
         raise Exception(f"an error occurred while running lydia: {str(e)}") from e
 
 
 def postprocess_lydia_output(output: str) -> str:
     """
```

### Comparing `logaut-0.1.1/logaut/backends/lydia/to_lydia_grammar.py` & `logaut-0.2.0/logaut/backends/lydia/to_lydia_grammar.py`

 * *Files identical despite different names*

### Comparing `logaut-0.1.1/logaut/core.py` & `logaut-0.2.0/logaut/core.py`

 * *Files identical despite different names*

### Comparing `logaut-0.1.1/logaut/exceptions.py` & `logaut-0.2.0/logaut/exceptions.py`

 * *Files identical despite different names*

### Comparing `logaut-0.1.1/logaut/helpers.py` & `logaut-0.2.0/logaut/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,16 +17,19 @@
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with logaut.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 """Helpers module."""
-
+import contextlib
 import re
+import tempfile
+from pathlib import Path
+from typing import Generator
 
 
 class RegexConstrainedString(str):
     """
     A string that is constrained by a regex.
 
     The default behaviour is to match anything.
@@ -51,7 +54,28 @@
 
     def _handle_no_match(self):
         raise ValueError(
             "Value '{data}' does not match the regular expression {regex}".format(
                 data=self, regex=self.REGEX
             )
         )
+
+
+@contextlib.contextmanager
+def temporary_directory() -> Generator[Path, None, None]:
+    """
+    Create a temporary directory and clean up when done.
+
+    This function is a context manager that creates a temporary directory.
+    It wraps tempfile.TemporaryDirectory in order to make the clean up more robust
+    (e.g. managing a PermissionError in Windows: https://www.scivision.dev/python-tempfile-permission-error-windows/).
+    """
+    temp_dir = tempfile.TemporaryDirectory()
+    temp_path = Path(temp_dir.name)
+
+    yield temp_path
+
+    # when done with temporary directory
+    try:
+        temp_dir.cleanup()
+    except PermissionError:
+        pass
```

### Comparing `logaut-0.1.1/pyproject.toml` & `logaut-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "logaut"
-version = "0.1.1"
+version = "0.2.0"
 description = "From logic to automata."
-authors = ["Marco Favorito <favorito@diag.uniroma1.it>"]
+authors = ["Marco Favorito <marco.favorito@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://marcofavorito.me/logaut"
 repository = "https://github.com/whitemech/logaut.git"
 documentation = "https://marcofavorito.me/logaut"
 keywords = []
 classifiers = [
@@ -28,45 +28,47 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/whitemech/logaut/issues"
 "Pull Requests" = "https://github.com/whitemech/logaut/pulls"
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pylogics = "^0.1.0"
+python = "^3.8"
+pylogics = "^0.2.1"
 pythomata = "^0.3.2"
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.1"
-pytest-cov = "^2.10.1"
-pytest-randomly = "^3.5.0"
-tox = "^3.23.0"
-codecov = "^2.1.11"
-black = "==20.8b1"
-mypy = "^0.812"
-isort = "^5.7.0"
-flake8 = "^3.9.1"
-flake8-docstrings = "^1.5.0"
-flake8-bugbear = "^21.4.3"
-flake8-eradicate = "^1.0.0"
-flake8-isort = "^4.0.0"
-pylint = "^2.6.0"
-safety = "^1.10.1"
-vulture = "^2.1"
-bandit = "^1.7.0"
-mkdocs = "^1.1.2"
-markdown_include = "^0.6.0"
-mkdocs-material = "^7.1.1"
+
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.5"
+black = "^23.3.0"
+codecov = "^2.1.13"
+flake8 = "^5.0.4"
+flake8-bugbear = "^23.3.12"
+flake8-docstrings = "^1.7.0"
+flake8-eradicate = "^1.5.0"
+flake8-isort = "^6.0.0"
+hypothesis = "^6.76.0"
+hypothesis-pytest = "^0.19.0"
 ipython = "^7.18.1"
+isort = "^5.12.0"
 jupyter = "^1.0.0"
-mknotebooks = "^0.7.0"
-markdown = "^3.3.4"
-twine = "^3.3.0"
-hypothesis = "^6.10.0"
-hypothesis-pytest = "^0.19.0"
-ltlf2dfa = "^1.0.1"
+ltlf2dfa = "^1.0.2"
+markdown = "^3.3.0"
+markdown-include = "^0.8.1"
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.15"
+mknotebooks = "^0.7.1"
+mypy = "^1.3.0"
+pylint = "^2.17.4"
+pymdown-extensions = "^10.0.1"
+pytest = "^7.3.1"
+pytest-cov = "^4.1.0"
+pytest-randomly = "^3.12.0"
+safety = "^2.4.0b1"
+tox = "^4.4.12"
+twine = "^4.0.2"
+vulture = "^2.7"
 
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `logaut-0.1.1/setup.py` & `logaut-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,403 +1,429 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 276c 6f67 6175 7427 2c0a 2027   \.['logaut',. '
-00000050: 6c6f 6761 7574 2e62 6163 6b65 6e64 7327  logaut.backends'
-00000060: 2c0a 2027 6c6f 6761 7574 2e62 6163 6b65  ,. 'logaut.backe
-00000070: 6e64 732e 636f 6d6d 6f6e 272c 0a20 276c  nds.common',. 'l
-00000080: 6f67 6175 742e 6261 636b 656e 6473 2e6c  ogaut.backends.l
-00000090: 746c 6632 6466 6127 2c0a 2027 6c6f 6761  tlf2dfa',. 'loga
-000000a0: 7574 2e62 6163 6b65 6e64 732e 6c79 6469  ut.backends.lydi
-000000b0: 6127 5d0a 0a70 6163 6b61 6765 5f64 6174  a']..package_dat
-000000c0: 6120 3d20 5c0a 7b27 273a 205b 272a 275d  a = \.{'': ['*']
-000000d0: 7d0a 0a69 6e73 7461 6c6c 5f72 6571 7569  }..install_requi
-000000e0: 7265 7320 3d20 5c0a 5b27 7079 6c6f 6769  res = \.['pylogi
-000000f0: 6373 3e3d 302e 312e 302c 3c30 2e32 2e30  cs>=0.1.0,<0.2.0
-00000100: 272c 2027 7079 7468 6f6d 6174 613e 3d30  ', 'pythomata>=0
-00000110: 2e33 2e32 2c3c 302e 342e 3027 5d0a 0a73  .3.2,<0.4.0']..s
-00000120: 6574 7570 5f6b 7761 7267 7320 3d20 7b0a  etup_kwargs = {.
-00000130: 2020 2020 276e 616d 6527 3a20 276c 6f67      'name': 'log
-00000140: 6175 7427 2c0a 2020 2020 2776 6572 7369  aut',.    'versi
-00000150: 6f6e 273a 2027 302e 312e 3127 2c0a 2020  on': '0.1.1',.  
-00000160: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
-00000170: 2027 4672 6f6d 206c 6f67 6963 2074 6f20   'From logic to 
-00000180: 6175 746f 6d61 7461 2e27 2c0a 2020 2020  automata.',.    
-00000190: 276c 6f6e 675f 6465 7363 7269 7074 696f  'long_descriptio
-000001a0: 6e27 3a20 273c 6831 2061 6c69 676e 3d22  n': '<h1 align="
-000001b0: 6365 6e74 6572 223e 5c6e 2020 3c62 3e6c  center">\n  <b>l
-000001c0: 6f67 6175 743c 2f62 3e5c 6e3c 2f68 313e  ogaut</b>\n</h1>
-000001d0: 5c6e 5c6e 3c70 2061 6c69 676e 3d22 6365  \n\n<p align="ce
-000001e0: 6e74 6572 223e 5c6e 2020 3c61 2068 7265  nter">\n  <a hre
-000001f0: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
-00000200: 6f72 672f 7072 6f6a 6563 742f 6c6f 6761  org/project/loga
-00000210: 7574 223e 5c6e 2020 2020 3c69 6d67 2061  ut">\n    <img a
-00000220: 6c74 3d22 5079 5049 2220 7372 633d 2268  lt="PyPI" src="h
-00000230: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000240: 6473 2e69 6f2f 7079 7069 2f76 2f6c 6f67  ds.io/pypi/v/log
-00000250: 6175 7422 3e5c 6e20 203c 2f61 3e5c 6e20  aut">\n  </a>\n 
-00000260: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000270: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000280: 6374 2f6c 6f67 6175 7422 3e5c 6e20 2020  ct/logaut">\n   
-00000290: 203c 696d 6720 616c 743d 2250 7950 4920   <img alt="PyPI 
-000002a0: 2d20 5079 7468 6f6e 2056 6572 7369 6f6e  - Python Version
-000002b0: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-000002c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000002d0: 7069 2f70 7976 6572 7369 6f6e 732f 6c6f  pi/pyversions/lo
-000002e0: 6761 7574 2220 2f3e 5c6e 2020 3c2f 613e  gaut" />\n  </a>
-000002f0: 5c6e 2020 3c61 2068 7265 663d 2222 3e5c  \n  <a href="">\
-00000300: 6e20 2020 203c 696d 6720 616c 743d 2250  n    <img alt="P
-00000310: 7950 4920 2d20 5374 6174 7573 2220 7372  yPI - Status" sr
-00000320: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000330: 6869 656c 6473 2e69 6f2f 7079 7069 2f73  hields.io/pypi/s
-00000340: 7461 7475 732f 6c6f 6761 7574 2220 2f3e  tatus/logaut" />
-00000350: 5c6e 2020 3c2f 613e 5c6e 2020 3c61 2068  \n  </a>\n  <a h
-00000360: 7265 663d 2222 3e5c 6e20 2020 203c 696d  ref="">\n    <im
-00000370: 6720 616c 743d 2250 7950 4920 2d20 496d  g alt="PyPI - Im
-00000380: 706c 656d 656e 7461 7469 6f6e 2220 7372  plementation" sr
-00000390: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-000003a0: 6869 656c 6473 2e69 6f2f 7079 7069 2f69  hields.io/pypi/i
-000003b0: 6d70 6c65 6d65 6e74 6174 696f 6e2f 6c6f  mplementation/lo
-000003c0: 6761 7574 223e 5c6e 2020 3c2f 613e 5c6e  gaut">\n  </a>\n
-000003d0: 2020 3c61 2068 7265 663d 2222 3e5c 6e20    <a href="">\n 
-000003e0: 2020 203c 696d 6720 616c 743d 2250 7950     <img alt="PyP
-000003f0: 4920 2d20 5768 6565 6c22 2073 7263 3d22  I - Wheel" src="
-00000400: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000410: 6c64 732e 696f 2f70 7970 692f 7768 6565  lds.io/pypi/whee
-00000420: 6c2f 6c6f 6761 7574 223e 5c6e 2020 3c2f  l/logaut">\n  </
-00000430: 613e 5c6e 2020 3c61 2068 7265 663d 2268  a>\n  <a href="h
-00000440: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000450: 6d2f 7768 6974 656d 6563 682f 6c6f 6761  m/whitemech/loga
-00000460: 7574 2f62 6c6f 622f 6d61 7374 6572 2f4c  ut/blob/master/L
-00000470: 4943 454e 5345 223e 5c6e 2020 2020 3c69  ICENSE">\n    <i
-00000480: 6d67 2061 6c74 3d22 4769 7448 7562 2220  mg alt="GitHub" 
-00000490: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000004a0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-000004b0: 7562 2f6c 6963 656e 7365 2f6d 6172 636f  ub/license/marco
-000004c0: 6661 766f 7269 746f 2f6c 6f67 6175 7422  favorito/logaut"
-000004d0: 3e5c 6e20 203c 2f61 3e5c 6e3c 2f70 3e5c  >\n  </a>\n</p>\
-000004e0: 6e3c 7020 616c 6967 6e3d 2263 656e 7465  n<p align="cente
-000004f0: 7222 3e5c 6e20 203c 6120 6872 6566 3d22  r">\n  <a href="
-00000500: 223e 5c6e 2020 2020 3c69 6d67 2061 6c74  ">\n    <img alt
-00000510: 3d22 7465 7374 2220 7372 633d 2268 7474  ="test" src="htt
-00000520: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000530: 7768 6974 656d 6563 682f 6c6f 6761 7574  whitemech/logaut
-00000540: 2f77 6f72 6b66 6c6f 7773 2f74 6573 742f  /workflows/test/
-00000550: 6261 6467 652e 7376 6722 3e5c 6e20 203c  badge.svg">\n  <
-00000560: 2f61 3e5c 6e20 203c 6120 6872 6566 3d22  /a>\n  <a href="
-00000570: 223e 5c6e 2020 2020 3c69 6d67 2061 6c74  ">\n    <img alt
-00000580: 3d22 6c69 6e74 2220 7372 633d 2268 7474  ="lint" src="htt
-00000590: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000005a0: 7768 6974 656d 6563 682f 6c6f 6761 7574  whitemech/logaut
-000005b0: 2f77 6f72 6b66 6c6f 7773 2f6c 696e 742f  /workflows/lint/
-000005c0: 6261 6467 652e 7376 6722 3e5c 6e20 203c  badge.svg">\n  <
-000005d0: 2f61 3e5c 6e20 203c 6120 6872 6566 3d22  /a>\n  <a href="
-000005e0: 223e 5c6e 2020 2020 3c69 6d67 2061 6c74  ">\n    <img alt
-000005f0: 3d22 646f 6373 2220 7372 633d 2268 7474  ="docs" src="htt
-00000600: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000610: 7768 6974 656d 6563 682f 6c6f 6761 7574  whitemech/logaut
-00000620: 2f77 6f72 6b66 6c6f 7773 2f64 6f63 732f  /workflows/docs/
-00000630: 6261 6467 652e 7376 6722 3e5c 6e20 203c  badge.svg">\n  <
-00000640: 2f61 3e5c 6e20 203c 6120 6872 6566 3d22  /a>\n  <a href="
-00000650: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
-00000660: 696f 2f67 682f 6d61 7263 6f66 6176 6f72  io/gh/marcofavor
-00000670: 6974 6f2f 6c6f 6761 7574 223e 5c6e 2020  ito/logaut">\n  
-00000680: 2020 3c69 6d67 2061 6c74 3d22 636f 6465    <img alt="code
-00000690: 636f 7622 2073 7263 3d22 6874 7470 733a  cov" src="https:
-000006a0: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
-000006b0: 6d61 7263 6f66 6176 6f72 6974 6f2f 6c6f  marcofavorito/lo
-000006c0: 6761 7574 2f62 7261 6e63 682f 6d61 7374  gaut/branch/mast
-000006d0: 6572 2f67 7261 7068 2f62 6164 6765 2e73  er/graph/badge.s
-000006e0: 7667 3f74 6f6b 656e 3d46 4733 4154 4750  vg?token=FG3ATGP
-000006f0: 3550 3522 3e5c 6e20 203c 2f61 3e5c 6e3c  5P5">\n  </a>\n<
-00000700: 2f70 3e5c 6e3c 7020 616c 6967 6e3d 2263  /p>\n<p align="c
-00000710: 656e 7465 7222 3e5c 6e20 203c 6120 6872  enter">\n  <a hr
-00000720: 6566 3d22 6874 7470 733a 2f2f 696d 672e  ef="https://img.
-00000730: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000740: 2f66 6c61 6b65 382d 6368 6563 6b65 642d  /flake8-checked-
-00000750: 626c 7565 7669 6f6c 6574 223e 5c6e 2020  blueviolet">\n  
-00000760: 2020 3c69 6d67 2061 6c74 3d22 2220 7372    <img alt="" sr
-00000770: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000780: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000790: 666c 616b 6538 2d63 6865 636b 6564 2d62  flake8-checked-b
-000007a0: 6c75 6576 696f 6c65 7422 3e5c 6e20 203c  lueviolet">\n  <
-000007b0: 2f61 3e5c 6e20 203c 6120 6872 6566 3d22  /a>\n  <a href="
-000007c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000007d0: 6c64 732e 696f 2f62 6164 6765 2f6d 7970  lds.io/badge/myp
-000007e0: 792d 6368 6563 6b65 642d 626c 7565 223e  y-checked-blue">
-000007f0: 5c6e 2020 2020 3c69 6d67 2061 6c74 3d22  \n    <img alt="
-00000800: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000810: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000820: 6467 652f 6d79 7079 2d63 6865 636b 6564  dge/mypy-checked
-00000830: 2d62 6c75 6522 3e5c 6e20 203c 2f61 3e5c  -blue">\n  </a>\
-00000840: 6e20 203c 6120 6872 6566 3d22 6874 7470  n  <a href="http
-00000850: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000860: 696f 2f62 6164 6765 2f63 6f64 6525 3230  io/badge/code%20
-00000870: 7374 796c 652d 626c 6163 6b2d 626c 6163  style-black-blac
-00000880: 6b22 3e5c 6e20 2020 203c 696d 6720 616c  k">\n    <img al
-00000890: 743d 2262 6c61 636b 2220 7372 633d 2268  t="black" src="h
-000008a0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000008b0: 6473 2e69 6f2f 6261 6467 652f 636f 6465  ds.io/badge/code
-000008c0: 2532 3073 7479 6c65 2d62 6c61 636b 2d62  %20style-black-b
-000008d0: 6c61 636b 2220 2f3e 5c6e 2020 3c2f 613e  lack" />\n  </a>
-000008e0: 5c6e 2020 3c61 2068 7265 663d 2268 7474  \n  <a href="htt
-000008f0: 7073 3a2f 2f77 7777 2e6d 6b64 6f63 732e  ps://www.mkdocs.
-00000900: 6f72 672f 223e 5c6e 2020 2020 3c69 6d67  org/">\n    <img
-00000910: 2061 6c74 3d22 2220 7372 633d 2268 7474   alt="" src="htt
-00000920: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000930: 2e69 6f2f 6261 6467 652f 646f 6373 2d6d  .io/badge/docs-m
-00000940: 6b64 6f63 732d 3963 6622 3e5c 6e20 203c  kdocs-9cf">\n  <
-00000950: 2f61 3e5c 6e3c 2f70 3e5c 6e5c 6e5c 6e4c  /a>\n</p>\n\n\nL
-00000960: 4f47 6963 7320 666f 726d 616c 6973 6d73  OGics formalisms
-00000970: 2074 6f20 4155 546f 6d61 7461 5c6e 5c6e   to AUTomata\n\n
-00000980: 2323 2057 6861 7420 6973 2060 6c6f 6761  ## What is `loga
-00000990: 7574 605c 6e5c 6e4c 6f67 6175 7420 6973  ut`\n\nLogaut is
-000009a0: 2074 6f20 7468 6520 6c6f 6769 6373 2d74   to the logics-t
-000009b0: 6f2d 4446 4120 7072 6f62 6c65 6d5c 6e77  o-DFA problem\nw
-000009c0: 6861 7420 4b65 7261 7320 6973 2066 6f72  hat Keras is for
-000009d0: 2044 6565 7020 4c65 6172 6e69 6e67 3a5c   Deep Learning:\
-000009e0: 6e61 2077 7261 7070 6572 2074 6f20 7065  na wrapper to pe
-000009f0: 7266 6f72 6d61 6e74 2062 6163 6b2d 656e  rformant back-en
-00000a00: 6473 2c5c 6e62 7574 2077 6974 6820 6875  ds,\nbut with hu
-00000a10: 6d61 6e2d 6672 6965 6e64 6c79 2041 5049  man-friendly API
-00000a20: 732e 5c6e 5c6e 2323 2049 6e73 7461 6c6c  s.\n\n## Install
-00000a30: 5c6e 5c6e 546f 2069 6e73 7461 6c6c 2074  \n\nTo install t
-00000a40: 6865 2070 6163 6b61 6765 2066 726f 6d20  he package from 
-00000a50: 5079 5049 3a5c 6e60 6060 5c6e 7069 7020  PyPI:\n```\npip 
-00000a60: 696e 7374 616c 6c20 6c6f 6761 7574 5c6e  install logaut\n
-00000a70: 6060 605c 6e5c 6e4d 616b 6520 7375 7265  ```\n\nMake sure
-00000a80: 2074 6f20 6861 7665 205b 4c79 6469 615d   to have [Lydia]
-00000a90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000aa0: 636f 6d2f 7768 6974 656d 6563 682f 6c79  com/whitemech/ly
-00000ab0: 6469 6129 205c 6e69 6e73 7461 6c6c 6564  dia) \ninstalled
-00000ac0: 206f 6e20 796f 7572 206d 6163 6869 6e65   on your machine
-00000ad0: 2e5c 6e57 6520 7375 6767 6573 7420 7468  .\nWe suggest th
-00000ae0: 6520 666f 6c6c 6f77 696e 6720 7365 7475  e following setu
-00000af0: 703a 5c6e 5c6e 2d20 5b49 6e73 7461 6c6c  p:\n\n- [Install
-00000b00: 2044 6f63 6b65 725d 2868 7474 7073 3a2f   Docker](https:/
-00000b10: 2f77 7777 2e64 6f63 6b65 722e 636f 6d2f  /www.docker.com/
-00000b20: 6765 742d 7374 6172 7465 6429 5c6e 2d20  get-started)\n- 
-00000b30: 446f 776e 6c6f 6164 2074 6865 204c 7964  Download the Lyd
-00000b40: 6961 2044 6f63 6b65 7220 696d 6167 653a  ia Docker image:
-00000b50: 5c6e 6060 605c 6e64 6f63 6b65 7220 7075  \n```\ndocker pu
-00000b60: 6c6c 2077 6869 7465 6d65 6368 2f6c 7964  ll whitemech/lyd
-00000b70: 6961 3a6c 6174 6573 745c 6e60 6060 5c6e  ia:latest\n```\n
-00000b80: 2d20 4d61 6b65 2074 6865 2044 6f63 6b65  - Make the Docke
-00000b90: 7220 696d 6167 6520 6578 6563 7574 6162  r image executab
-00000ba0: 6c65 2075 6e64 6572 2074 6865 206e 616d  le under the nam
-00000bb0: 6520 606c 7964 6961 602e 5c6e 2020 4f6e  e `lydia`.\n  On
-00000bc0: 204c 696e 7578 2061 6e64 204d 6163 4f53   Linux and MacOS
-00000bd0: 206d 6163 6869 6e65 732c 2074 6865 2066   machines, the f
-00000be0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00000bf0: 7320 7368 6f75 6c64 2077 6f72 6b3a 5c6e  s should work:\n
-00000c00: 6060 605c 6e65 6368 6f20 5c27 2321 2f75  ```\necho \'#!/u
-00000c10: 7372 2f62 696e 2f65 6e76 2073 685c 2720  sr/bin/env sh\' 
-00000c20: 3e20 6c79 6469 615c 6e65 6368 6f20 5c27  > lydia\necho \'
-00000c30: 646f 636b 6572 2072 756e 202d 7624 2870  docker run -v$(p
-00000c40: 7764 293a 2f68 6f6d 652f 6465 6661 756c  wd):/home/defaul
-00000c50: 7420 7768 6974 656d 6563 682f 6c79 6469  t whitemech/lydi
-00000c60: 6120 6c79 6469 6120 2440 5c27 203e 3e20  a lydia $@\' >> 
-00000c70: 6c79 6469 615c 6e73 7564 6f20 6368 6d6f  lydia\nsudo chmo
-00000c80: 6420 752b 7820 6c79 6469 615c 6e73 7564  d u+x lydia\nsud
-00000c90: 6f20 6d76 206c 7964 6961 202f 7573 722f  o mv lydia /usr/
-00000ca0: 6c6f 6361 6c2f 6269 6e2f 5c6e 6060 605c  local/bin/\n```\
-00000cb0: 6e5c 6e54 6869 7320 7769 6c6c 2069 6e73  n\nThis will ins
-00000cc0: 7461 6c6c 2061 6e20 616c 6961 7320 746f  tall an alias to
-00000cd0: 2074 6865 2069 6e6c 696e 6520 446f 636b   the inline Dock
-00000ce0: 6572 2069 6d61 6765 2065 7865 6375 7469  er image executi
-00000cf0: 6f6e 5c6e 696e 2079 6f75 7220 7379 7374  on\nin your syst
-00000d00: 656d 2050 4154 482e 2049 6e73 7465 6164  em PATH. Instead
-00000d10: 206f 6620 602f 7573 722f 6c6f 6361 6c2f   of `/usr/local/
-00000d20: 6269 6e2f 605c 6e79 6f75 206d 6179 2075  bin/`\nyou may u
-00000d30: 7365 2061 6e6f 7468 6572 2070 6174 6820  se another path 
-00000d40: 7768 6963 6820 6973 2073 7469 6c6c 2069  which is still i
-00000d50: 6e20 7468 6520 6050 4154 4860 2076 6172  n the `PATH` var
-00000d60: 6961 626c 652e 5c6e 5c6e 2323 2051 7569  iable.\n\n## Qui
-00000d70: 636b 7374 6172 745c 6e5c 6e4e 6f77 2079  ckstart\n\nNow y
-00000d80: 6f75 2061 7265 2072 6561 6479 2074 6f20  ou are ready to 
-00000d90: 676f 3a5c 6e60 6060 7079 7468 6f6e 5c6e  go:\n```python\n
-00000da0: 6672 6f6d 206c 6f67 6175 7420 696d 706f  from logaut impo
-00000db0: 7274 206c 746c 3264 6661 5c6e 6672 6f6d  rt ltl2dfa\nfrom
-00000dc0: 2070 796c 6f67 6963 732e 7061 7273 6572   pylogics.parser
-00000dd0: 7320 696d 706f 7274 2070 6172 7365 5f6c  s import parse_l
-00000de0: 746c 5c6e 666f 726d 756c 6120 3d20 7061  tl\nformula = pa
-00000df0: 7273 655f 6c74 6c28 2246 2861 2922 295c  rse_ltl("F(a)")\
-00000e00: 6e64 6661 203d 206c 746c 3264 6661 2866  ndfa = ltl2dfa(f
-00000e10: 6f72 6d75 6c61 2c20 6261 636b 656e 643d  ormula, backend=
-00000e20: 226c 7964 6961 2229 5c6e 6060 605c 6e5c  "lydia")\n```\n\
-00000e30: 6e54 6865 2066 756e 6374 696f 6e20 606c  nThe function `l
-00000e40: 746c 3264 6661 6020 7461 6b65 7320 696e  tl2dfa` takes in
-00000e50: 2069 6e70 7574 2061 205c 6e5b 7079 6c6f   input a \n[pylo
-00000e60: 6769 6373 5d28 6874 7470 733a 2f2f 6769  gics](https://gi
-00000e70: 7468 7562 2e63 6f6d 2f77 6869 7465 6d65  thub.com/whiteme
-00000e80: 6368 2f70 796c 6f67 6963 7329 205c 6e60  ch/pylogics) \n`
-00000e90: 666f 726d 756c 6160 2061 6e64 2067 6976  formula` and giv
-00000ea0: 6573 2069 6e20 6f75 7470 7574 5c6e 6120  es in output\na 
-00000eb0: 5b70 7974 686f 6d61 7461 5d28 6874 7470  [pythomata](http
-00000ec0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f77  s://github.com/w
-00000ed0: 6869 7465 6d65 6368 2f70 7974 686f 6d61  hitemech/pythoma
-00000ee0: 7461 2920 4446 412e 5c6e 5c6e 5468 656e  ta) DFA.\n\nThen
-00000ef0: 2c20 796f 7520 6361 6e20 6d61 6e69 7075  , you can manipu
-00000f00: 6c61 7465 2074 6865 2044 4641 2061 7320  late the DFA as 
-00000f10: 646f 6e65 2077 6974 6820 5079 7468 6f6d  done with Pythom
-00000f20: 6174 612c 5c6e 652e 672e 2074 6f20 7072  ata,\ne.g. to pr
-00000f30: 696e 743a 5c6e 6060 605c 6e64 6661 2e74  int:\n```\ndfa.t
-00000f40: 6f5f 6772 6170 6876 697a 2829 2e72 656e  o_graphviz().ren
-00000f50: 6465 7228 2265 7665 6e74 7561 6c6c 792e  der("eventually.
-00000f60: 6466 6122 295c 6e60 6060 5c6e 5c6e 4375  dfa")\n```\n\nCu
-00000f70: 7272 656e 746c 792c 2074 6865 2060 6c79  rrently, the `ly
-00000f80: 6469 6160 2062 6163 6b65 6e64 206f 6e6c  dia` backend onl
-00000f90: 7920 7375 7070 6f72 7473 5c6e 7468 6520  y supports\nthe 
-00000fa0: 606c 746c 6020 616e 6420 606c 646c 6020  `ltl` and `ldl` 
-00000fb0: 6c6f 6769 6373 2e5c 6e5c 6e54 6865 2060  logics.\n\nThe `
-00000fc0: 6c74 6c66 3264 6661 602c 2062 6173 6564  ltlf2dfa`, based
-00000fd0: 206f 6e20 5c6e 5b4c 544c 6632 4446 415d   on \n[LTLf2DFA]
-00000fe0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000ff0: 636f 6d2f 7768 6974 656d 6563 682f 4c54  com/whitemech/LT
-00001000: 4c66 3244 4641 2f29 2c5c 6e73 7570 706f  Lf2DFA/),\nsuppo
-00001010: 7274 7320 606c 746c 6020 616e 6420 6070  rts `ltl` and `p
-00001020: 6c74 6c60 2e5c 6e46 6972 7374 2c20 696e  ltl`.\nFirst, in
-00001030: 7374 616c 6c20 6974 2061 7420 7665 7273  stall it at vers
-00001040: 696f 6e20 6031 2e30 2e31 603a 5c6e 6060  ion `1.0.1`:\n``
-00001050: 605c 6e70 6970 2069 6e73 7461 6c6c 2067  `\npip install g
-00001060: 6974 2b68 7474 7073 3a2f 2f67 6974 6875  it+https://githu
-00001070: 622e 636f 6d2f 7768 6974 656d 6563 682f  b.com/whitemech/
-00001080: 4c54 4c66 3244 4641 2e67 6974 4064 6576  LTLf2DFA.git@dev
-00001090: 656c 6f70 2365 6767 3d6c 746c 6632 6466  elop#egg=ltlf2df
-000010a0: 615c 6e60 6060 5c6e 5c6e 5468 656e 2c20  a\n```\n\nThen, 
-000010b0: 796f 7520 6361 6e20 7573 653a 5c6e 6060  you can use:\n``
-000010c0: 6070 7974 686f 6e5c 6e66 726f 6d20 6c6f  `python\nfrom lo
-000010d0: 6761 7574 2069 6d70 6f72 7420 706c 746c  gaut import pltl
-000010e0: 3264 6661 5c6e 6672 6f6d 2070 796c 6f67  2dfa\nfrom pylog
-000010f0: 6963 732e 7061 7273 6572 7320 696d 706f  ics.parsers impo
-00001100: 7274 2070 6172 7365 5f70 6c74 6c5c 6e66  rt parse_pltl\nf
-00001110: 6f72 6d75 6c61 203d 2070 6172 7365 5f70  ormula = parse_p
-00001120: 6c74 6c28 2261 2053 2062 2229 5c6e 6466  ltl("a S b")\ndf
-00001130: 6120 3d20 706c 746c 3264 6661 2866 6f72  a = pltl2dfa(for
-00001140: 6d75 6c61 2c20 6261 636b 656e 643d 226c  mula, backend="l
-00001150: 746c 6632 6466 6122 295c 6e60 6060 5c6e  tlf2dfa")\n```\n
-00001160: 5c6e 2323 2057 7269 7465 2079 6f75 7220  \n## Write your 
-00001170: 6f77 6e20 6261 636b 656e 645c 6e5c 6e59  own backend\n\nY
-00001180: 6f75 2063 616e 2077 7269 7465 2079 6f75  ou can write you
-00001190: 7220 6261 636b 2d65 6e64 2062 7920 696d  r back-end by im
-000011a0: 706c 656d 656e 7469 6e67 5c6e 7468 6520  plementing\nthe 
-000011b0: 6042 6163 6b65 6e64 6020 696e 7465 7266  `Backend` interf
-000011c0: 6163 653a 5c6e 5c6e 6060 6070 7974 686f  ace:\n\n```pytho
-000011d0: 6e5c 6e66 726f 6d20 6c6f 6761 7574 2e62  n\nfrom logaut.b
-000011e0: 6163 6b65 6e64 732e 6261 7365 2069 6d70  ackends.base imp
-000011f0: 6f72 7420 4261 636b 656e 645c 6e5c 6e63  ort Backend\n\nc
-00001200: 6c61 7373 204d 7942 6163 6b65 6e64 2842  lass MyBackend(B
-00001210: 6163 6b65 6e64 293a 5c6e 5c6e 2020 2020  ackend):\n\n    
-00001220: 6465 6620 6c74 6c32 6466 6128 7365 6c66  def ltl2dfa(self
-00001230: 2c20 666f 726d 756c 613a 2046 6f72 6d75  , formula: Formu
-00001240: 6c61 2920 2d3e 2044 4641 3a5c 6e20 2020  la) -> DFA:\n   
-00001250: 2020 2020 2022 2222 4672 6f6d 204c 544c       """From LTL
-00001260: 2074 6f20 4446 412e 2222 225c 6e5c 6e20   to DFA."""\n\n 
-00001270: 2020 2064 6566 206c 646c 3264 6661 2873     def ldl2dfa(s
-00001280: 656c 662c 2066 6f72 6d75 6c61 3a20 466f  elf, formula: Fo
-00001290: 726d 756c 6129 202d 3e20 4446 413a 5c6e  rmula) -> DFA:\n
-000012a0: 2020 2020 2020 2020 2222 2246 726f 6d20          """From 
-000012b0: 4c44 4c20 746f 2044 4641 2e22 2222 5c6e  LDL to DFA."""\n
-000012c0: 5c6e 2020 2020 6465 6620 706c 746c 3264  \n    def pltl2d
-000012d0: 6661 2873 656c 662c 2066 6f72 6d75 6c61  fa(self, formula
-000012e0: 3a20 466f 726d 756c 6129 202d 3e20 4446  : Formula) -> DF
-000012f0: 413a 5c6e 2020 2020 2020 2020 2222 2246  A:\n        """F
-00001300: 726f 6d20 504c 544c 2074 6f20 4446 412e  rom PLTL to DFA.
-00001310: 2222 225c 6e5c 6e20 2020 2064 6566 2070  """\n\n    def p
-00001320: 6c64 6c32 6466 6128 7365 6c66 2c20 666f  ldl2dfa(self, fo
-00001330: 726d 756c 613a 2046 6f72 6d75 6c61 2920  rmula: Formula) 
-00001340: 2d3e 2044 4641 3a5c 6e20 2020 2020 2020  -> DFA:\n       
-00001350: 2022 2222 4672 6f6d 2050 4c44 4c20 746f   """From PLDL to
-00001360: 2044 4641 2e22 2222 5c6e 2020 2020 2020   DFA."""\n      
-00001370: 2020 5c6e 2020 2020 6465 6620 666f 6c32    \n    def fol2
-00001380: 6466 6128 7365 6c66 2c20 666f 726d 756c  dfa(self, formul
-00001390: 613a 2046 6f72 6d75 6c61 2920 2d3e 2044  a: Formula) -> D
-000013a0: 4641 3a5c 6e20 2020 2020 2020 2022 2222  FA:\n        """
-000013b0: 4672 6f6d 2046 4f4c 2074 6f20 4446 412e  From FOL to DFA.
-000013c0: 2222 225c 6e5c 6e20 2020 2064 6566 206d  """\n\n    def m
-000013d0: 736f 3264 6661 2873 656c 662c 2066 6f72  so2dfa(self, for
-000013e0: 6d75 6c61 3a20 466f 726d 756c 6129 202d  mula: Formula) -
-000013f0: 3e20 4446 413a 5c6e 2020 2020 2020 2020  > DFA:\n        
-00001400: 2222 2246 726f 6d20 4d53 4f20 746f 2044  """From MSO to D
-00001410: 4641 2e22 2222 5c6e 6060 605c 6e5c 6e54  FA."""\n```\n\nT
-00001420: 6865 6e2c 2079 6f75 2063 616e 2072 6567  hen, you can reg
-00001430: 6973 7465 7220 7468 6520 6375 7374 6f6d  ister the custom
-00001440: 2062 6163 6b65 6e64 5c6e 636c 6173 7320   backend\nclass 
-00001450: 696e 2074 6865 206c 6962 7261 7279 3a5c  in the library:\
-00001460: 6e5c 6e60 6060 7079 7468 6f6e 5c6e 6672  n\n```python\nfr
-00001470: 6f6d 206c 6f67 6175 742e 6261 636b 656e  om logaut.backen
-00001480: 6473 2069 6d70 6f72 7420 7265 6769 7374  ds import regist
-00001490: 6572 5c6e 7265 6769 7374 6572 2869 645f  er\nregister(id_
-000014a0: 3d22 6d79 5f62 6163 6b65 6e64 222c 2065  ="my_backend", e
-000014b0: 6e74 7279 5f70 6f69 6e74 3d22 646f 7474  ntry_point="dott
-000014c0: 6564 2e70 6174 682e 746f 2e4d 7942 6163  ed.path.to.MyBac
-000014d0: 6b65 6e64 2229 5c6e 6060 605c 6e5c 6e41  kend")\n```\n\nA
-000014e0: 6e64 2074 6865 6e2c 2075 7365 2069 7420  nd then, use it 
-000014f0: 7468 726f 7567 6820 7468 6520 6d61 696e  through the main
-00001500: 2065 6e74 7279 2070 6f69 6e74 3a5c 6e60   entry point:\n`
-00001510: 6060 7079 7468 6f6e 5c6e 6466 6120 3d20  ``python\ndfa = 
-00001520: 6c74 6c32 6466 6128 666f 726d 756c 612c  ltl2dfa(formula,
-00001530: 2062 6163 6b65 6e64 3d22 6d79 5f62 6163   backend="my_bac
-00001540: 6b65 6e64 2229 5c6e 6060 605c 6e5c 6e23  kend")\n```\n\n#
-00001550: 2320 5465 7374 735c 6e5c 6e54 6f20 7275  # Tests\n\nTo ru
-00001560: 6e20 7465 7374 733a 2060 746f 7860 5c6e  n tests: `tox`\n
-00001570: 5c6e 546f 2072 756e 206f 6e6c 7920 7468  \nTo run only th
-00001580: 6520 636f 6465 2074 6573 7473 3a20 6074  e code tests: `t
-00001590: 6f78 202d 6520 7079 332e 3760 5c6e 5c6e  ox -e py3.7`\n\n
-000015a0: 546f 2072 756e 206f 6e6c 7920 7468 6520  To run only the 
-000015b0: 6c69 6e74 6572 733a 205c 6e2d 2060 746f  linters: \n- `to
-000015c0: 7820 2d65 2066 6c61 6b65 3860 5c6e 2d20  x -e flake8`\n- 
-000015d0: 6074 6f78 202d 6520 6d79 7079 605c 6e2d  `tox -e mypy`\n-
-000015e0: 2060 746f 7820 2d65 2062 6c61 636b 2d63   `tox -e black-c
-000015f0: 6865 636b 605c 6e2d 2060 746f 7820 2d65  heck`\n- `tox -e
-00001600: 2069 736f 7274 2d63 6865 636b 605c 6e5c   isort-check`\n\
-00001610: 6e50 6c65 6173 6520 6c6f 6f6b 2061 7420  nPlease look at 
-00001620: 7468 6520 6074 6f78 2e69 6e69 6020 6669  the `tox.ini` fi
-00001630: 6c65 2066 6f72 2074 6865 2066 756c 6c20  le for the full 
-00001640: 6c69 7374 206f 6620 7375 7070 6f72 7465  list of supporte
-00001650: 6420 636f 6d6d 616e 6473 2e20 5c6e 5c6e  d commands. \n\n
-00001660: 2323 2044 6f63 735c 6e5c 6e54 6f20 6275  ## Docs\n\nTo bu
-00001670: 696c 6420 7468 6520 646f 6373 3a20 606d  ild the docs: `m
-00001680: 6b64 6f63 7320 6275 696c 6460 5c6e 5c6e  kdocs build`\n\n
-00001690: 546f 2076 6965 7720 646f 6375 6d65 6e74  To view document
-000016a0: 6174 696f 6e20 696e 2061 2062 726f 7773  ation in a brows
-000016b0: 6572 3a20 606d 6b64 6f63 7320 7365 7276  er: `mkdocs serv
-000016c0: 6560 5c6e 616e 6420 7468 656e 2067 6f20  e`\nand then go 
-000016d0: 746f 205b 6874 7470 3a2f 2f6c 6f63 616c  to [http://local
-000016e0: 686f 7374 3a38 3030 305d 2868 7474 703a  host:8000](http:
-000016f0: 2f2f 6c6f 6361 6c68 6f73 743a 3830 3030  //localhost:8000
-00001700: 295c 6e5c 6e23 2320 4c69 6365 6e73 655c  )\n\n## License\
-00001710: 6e5c 6e6c 6f67 6175 7420 6973 2072 656c  n\nlogaut is rel
-00001720: 6561 7365 6420 756e 6465 7220 7468 6520  eased under the 
-00001730: 474e 5520 4c65 7373 6572 2047 656e 6572  GNU Lesser Gener
-00001740: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-00001750: 6520 7633 2e30 206f 7220 6c61 7465 7220  e v3.0 or later 
-00001760: 284c 4750 4c76 332b 292e 5c6e 5c6e 436f  (LGPLv3+).\n\nCo
-00001770: 7079 7269 6768 7420 3230 3231 2057 6869  pyright 2021 Whi
-00001780: 7465 4d65 6368 5c6e 5c6e 2323 2041 7574  teMech\n\n## Aut
-00001790: 686f 7273 5c6e 5c6e 2d20 5b4d 6172 636f  hors\n\n- [Marco
-000017a0: 2046 6176 6f72 6974 6f5d 2868 7474 7073   Favorito](https
-000017b0: 3a2f 2f6d 6172 636f 6661 766f 7269 746f  ://marcofavorito
-000017c0: 2e6d 652f 295c 6e27 2c0a 2020 2020 2761  .me/)\n',.    'a
-000017d0: 7574 686f 7227 3a20 274d 6172 636f 2046  uthor': 'Marco F
-000017e0: 6176 6f72 6974 6f27 2c0a 2020 2020 2761  avorito',.    'a
-000017f0: 7574 686f 725f 656d 6169 6c27 3a20 2766  uthor_email': 'f
-00001800: 6176 6f72 6974 6f40 6469 6167 2e75 6e69  avorito@diag.uni
-00001810: 726f 6d61 312e 6974 272c 0a20 2020 2027  roma1.it',.    '
-00001820: 6d61 696e 7461 696e 6572 273a 204e 6f6e  maintainer': Non
-00001830: 652c 0a20 2020 2027 6d61 696e 7461 696e  e,.    'maintain
-00001840: 6572 5f65 6d61 696c 273a 204e 6f6e 652c  er_email': None,
-00001850: 0a20 2020 2027 7572 6c27 3a20 2768 7474  .    'url': 'htt
-00001860: 7073 3a2f 2f6d 6172 636f 6661 766f 7269  ps://marcofavori
-00001870: 746f 2e6d 652f 6c6f 6761 7574 272c 0a20  to.me/logaut',. 
-00001880: 2020 2027 7061 636b 6167 6573 273a 2070     'packages': p
-00001890: 6163 6b61 6765 732c 0a20 2020 2027 7061  ackages,.    'pa
-000018a0: 636b 6167 655f 6461 7461 273a 2070 6163  ckage_data': pac
-000018b0: 6b61 6765 5f64 6174 612c 0a20 2020 2027  kage_data,.    '
-000018c0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-000018d0: 273a 2069 6e73 7461 6c6c 5f72 6571 7569  ': install_requi
-000018e0: 7265 732c 0a20 2020 2027 7079 7468 6f6e  res,.    'python
-000018f0: 5f72 6571 7569 7265 7327 3a20 273e 3d33  _requires': '>=3
-00001900: 2e37 2c3c 342e 3027 2c0a 7d0a 0a0a 7365  .7,<4.0',.}...se
-00001910: 7475 7028 2a2a 7365 7475 705f 6b77 6172  tup(**setup_kwar
-00001920: 6773 290a                                gs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6c6f 6761  : 2.1.Name: loga
+00000020: 7574 0a56 6572 7369 6f6e 3a20 302e 322e  ut.Version: 0.2.
+00000030: 300a 5375 6d6d 6172 793a 2046 726f 6d20  0.Summary: From 
+00000040: 6c6f 6769 6320 746f 2061 7574 6f6d 6174  logic to automat
+00000050: 612e 0a48 6f6d 652d 7061 6765 3a20 6874  a..Home-page: ht
+00000060: 7470 733a 2f2f 6d61 7263 6f66 6176 6f72  tps://marcofavor
+00000070: 6974 6f2e 6d65 2f6c 6f67 6175 740a 4c69  ito.me/logaut.Li
+00000080: 6365 6e73 653a 2047 504c 2d33 2e30 2d6f  cense: GPL-3.0-o
+00000090: 722d 6c61 7465 720a 4175 7468 6f72 3a20  r-later.Author: 
+000000a0: 4d61 7263 6f20 4661 766f 7269 746f 0a41  Marco Favorito.A
+000000b0: 7574 686f 722d 656d 6169 6c3a 206d 6172  uthor-email: mar
+000000c0: 636f 2e66 6176 6f72 6974 6f40 676d 6169  co.favorito@gmai
+000000d0: 6c2e 636f 6d0a 5265 7175 6972 6573 2d50  l.com.Requires-P
+000000e0: 7974 686f 6e3a 203e 3d33 2e38 2c3c 342e  ython: >=3.8,<4.
+000000f0: 300a 436c 6173 7369 6669 6572 3a20 4465  0.Classifier: De
+00000100: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000110: 203a 3a20 3220 2d20 5072 652d 416c 7068   :: 2 - Pre-Alph
+00000120: 610a 436c 6173 7369 6669 6572 3a20 496e  a.Classifier: In
+00000130: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000140: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
+00000150: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000160: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000170: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
+00000180: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+00000190: 7633 206f 7220 6c61 7465 7220 2847 504c  v3 or later (GPL
+000001a0: 7633 2b29 0a43 6c61 7373 6966 6965 723a  v3+).Classifier:
+000001b0: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+000001c0: 4170 7072 6f76 6564 203a 3a20 474e 5520  Approved :: GNU 
+000001d0: 4c65 7373 6572 2047 656e 6572 616c 2050  Lesser General P
+000001e0: 7562 6c69 6320 4c69 6365 6e73 6520 7633  ublic License v3
+000001f0: 206f 7220 6c61 7465 7220 284c 4750 4c76   or later (LGPLv
+00000200: 332b 290a 436c 6173 7369 6669 6572 3a20  3+).Classifier: 
+00000210: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
+00000220: 203a 3a20 456e 676c 6973 680a 436c 6173   :: English.Clas
+00000230: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000240: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000250: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
+00000260: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000270: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000280: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
+00000290: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000002a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002b0: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
+000002c0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000002d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002f0: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00000300: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000310: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000320: 2033 2e31 310a 436c 6173 7369 6669 6572   3.11.Classifier
+00000330: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000340: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000350: 203a 3a20 332e 370a 5265 7175 6972 6573   :: 3.7.Requires
+00000360: 2d44 6973 743a 2070 796c 6f67 6963 7320  -Dist: pylogics 
+00000370: 283e 3d30 2e32 2e31 2c3c 302e 332e 3029  (>=0.2.1,<0.3.0)
+00000380: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000390: 7079 7468 6f6d 6174 6120 283e 3d30 2e33  pythomata (>=0.3
+000003a0: 2e32 2c3c 302e 342e 3029 0a50 726f 6a65  .2,<0.4.0).Proje
+000003b0: 6374 2d55 524c 3a20 4275 6720 5472 6163  ct-URL: Bug Trac
+000003c0: 6b65 722c 2068 7474 7073 3a2f 2f67 6974  ker, https://git
+000003d0: 6875 622e 636f 6d2f 7768 6974 656d 6563  hub.com/whitemec
+000003e0: 682f 6c6f 6761 7574 2f69 7373 7565 730a  h/logaut/issues.
+000003f0: 5072 6f6a 6563 742d 5552 4c3a 2044 6f63  Project-URL: Doc
+00000400: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
+00000410: 733a 2f2f 6d61 7263 6f66 6176 6f72 6974  s://marcofavorit
+00000420: 6f2e 6d65 2f6c 6f67 6175 740a 5072 6f6a  o.me/logaut.Proj
+00000430: 6563 742d 5552 4c3a 2050 756c 6c20 5265  ect-URL: Pull Re
+00000440: 7175 6573 7473 2c20 6874 7470 733a 2f2f  quests, https://
+00000450: 6769 7468 7562 2e63 6f6d 2f77 6869 7465  github.com/white
+00000460: 6d65 6368 2f6c 6f67 6175 742f 7075 6c6c  mech/logaut/pull
+00000470: 730a 5072 6f6a 6563 742d 5552 4c3a 2052  s.Project-URL: R
+00000480: 6570 6f73 6974 6f72 792c 2068 7474 7073  epository, https
+00000490: 3a2f 2f67 6974 6875 622e 636f 6d2f 7768  ://github.com/wh
+000004a0: 6974 656d 6563 682f 6c6f 6761 7574 2e67  itemech/logaut.g
+000004b0: 6974 0a44 6573 6372 6970 7469 6f6e 2d43  it.Description-C
+000004c0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+000004d0: 742f 6d61 726b 646f 776e 0a0a 3c68 3120  t/markdown..<h1 
+000004e0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+000004f0: 2020 3c62 3e6c 6f67 6175 743c 2f62 3e0a    <b>logaut</b>.
+00000500: 3c2f 6831 3e0a 0a3c 7020 616c 6967 6e3d  </h1>..<p align=
+00000510: 2263 656e 7465 7222 3e0a 2020 3c61 2068  "center">.  <a h
+00000520: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+00000530: 692e 6f72 672f 7072 6f6a 6563 742f 6c6f  i.org/project/lo
+00000540: 6761 7574 223e 0a20 2020 203c 696d 6720  gaut">.    <img 
+00000550: 616c 743d 2250 7950 4922 2073 7263 3d22  alt="PyPI" src="
+00000560: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000570: 6c64 732e 696f 2f70 7970 692f 762f 6c6f  lds.io/pypi/v/lo
+00000580: 6761 7574 223e 0a20 203c 2f61 3e0a 2020  gaut">.  </a>.  
+00000590: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000005a0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+000005b0: 742f 6c6f 6761 7574 223e 0a20 2020 203c  t/logaut">.    <
+000005c0: 696d 6720 616c 743d 2250 7950 4920 2d20  img alt="PyPI - 
+000005d0: 5079 7468 6f6e 2056 6572 7369 6f6e 2220  Python Version" 
+000005e0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000005f0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000600: 2f70 7976 6572 7369 6f6e 732f 6c6f 6761  /pyversions/loga
+00000610: 7574 2220 2f3e 0a20 203c 2f61 3e0a 2020  ut" />.  </a>.  
+00000620: 3c61 2068 7265 663d 2222 3e0a 2020 2020  <a href="">.    
+00000630: 3c69 6d67 2061 6c74 3d22 5079 5049 202d  <img alt="PyPI -
+00000640: 2053 7461 7475 7322 2073 7263 3d22 6874   Status" src="ht
+00000650: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000660: 732e 696f 2f70 7970 692f 7374 6174 7573  s.io/pypi/status
+00000670: 2f6c 6f67 6175 7422 202f 3e0a 2020 3c2f  /logaut" />.  </
+00000680: 613e 0a20 203c 6120 6872 6566 3d22 223e  a>.  <a href="">
+00000690: 0a20 2020 203c 696d 6720 616c 743d 2250  .    <img alt="P
+000006a0: 7950 4920 2d20 496d 706c 656d 656e 7461  yPI - Implementa
+000006b0: 7469 6f6e 2220 7372 633d 2268 7474 7073  tion" src="https
+000006c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000006d0: 6f2f 7079 7069 2f69 6d70 6c65 6d65 6e74  o/pypi/implement
+000006e0: 6174 696f 6e2f 6c6f 6761 7574 223e 0a20  ation/logaut">. 
+000006f0: 203c 2f61 3e0a 2020 3c61 2068 7265 663d   </a>.  <a href=
+00000700: 2222 3e0a 2020 2020 3c69 6d67 2061 6c74  "">.    <img alt
+00000710: 3d22 5079 5049 202d 2057 6865 656c 2220  ="PyPI - Wheel" 
+00000720: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000730: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000740: 2f77 6865 656c 2f6c 6f67 6175 7422 3e0a  /wheel/logaut">.
+00000750: 2020 3c2f 613e 0a20 203c 6120 6872 6566    </a>.  <a href
+00000760: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000770: 2e63 6f6d 2f77 6869 7465 6d65 6368 2f6c  .com/whitemech/l
+00000780: 6f67 6175 742f 626c 6f62 2f6d 6173 7465  ogaut/blob/maste
+00000790: 722f 4c49 4345 4e53 4522 3e0a 2020 2020  r/LICENSE">.    
+000007a0: 3c69 6d67 2061 6c74 3d22 4769 7448 7562  <img alt="GitHub
+000007b0: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+000007c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+000007d0: 7468 7562 2f6c 6963 656e 7365 2f6d 6172  thub/license/mar
+000007e0: 636f 6661 766f 7269 746f 2f6c 6f67 6175  cofavorito/logau
+000007f0: 7422 3e0a 2020 3c2f 613e 0a3c 2f70 3e0a  t">.  </a>.</p>.
+00000800: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000810: 223e 0a20 203c 6120 6872 6566 3d22 223e  ">.  <a href="">
+00000820: 0a20 2020 203c 696d 6720 616c 743d 2274  .    <img alt="t
+00000830: 6573 7422 2073 7263 3d22 6874 7470 733a  est" src="https:
+00000840: 2f2f 6769 7468 7562 2e63 6f6d 2f77 6869  //github.com/whi
+00000850: 7465 6d65 6368 2f6c 6f67 6175 742f 776f  temech/logaut/wo
+00000860: 726b 666c 6f77 732f 7465 7374 2f62 6164  rkflows/test/bad
+00000870: 6765 2e73 7667 223e 0a20 203c 2f61 3e0a  ge.svg">.  </a>.
+00000880: 2020 3c61 2068 7265 663d 2222 3e0a 2020    <a href="">.  
+00000890: 2020 3c69 6d67 2061 6c74 3d22 6c69 6e74    <img alt="lint
+000008a0: 2220 7372 633d 2268 7474 7073 3a2f 2f67  " src="https://g
+000008b0: 6974 6875 622e 636f 6d2f 7768 6974 656d  ithub.com/whitem
+000008c0: 6563 682f 6c6f 6761 7574 2f77 6f72 6b66  ech/logaut/workf
+000008d0: 6c6f 7773 2f6c 696e 742f 6261 6467 652e  lows/lint/badge.
+000008e0: 7376 6722 3e0a 2020 3c2f 613e 0a20 203c  svg">.  </a>.  <
+000008f0: 6120 6872 6566 3d22 223e 0a20 2020 203c  a href="">.    <
+00000900: 696d 6720 616c 743d 2264 6f63 7322 2073  img alt="docs" s
+00000910: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+00000920: 7562 2e63 6f6d 2f77 6869 7465 6d65 6368  ub.com/whitemech
+00000930: 2f6c 6f67 6175 742f 776f 726b 666c 6f77  /logaut/workflow
+00000940: 732f 646f 6373 2f62 6164 6765 2e73 7667  s/docs/badge.svg
+00000950: 223e 0a20 203c 2f61 3e0a 2020 3c61 2068  ">.  </a>.  <a h
+00000960: 7265 663d 2268 7474 7073 3a2f 2f63 6f64  ref="https://cod
+00000970: 6563 6f76 2e69 6f2f 6768 2f6d 6172 636f  ecov.io/gh/marco
+00000980: 6661 766f 7269 746f 2f6c 6f67 6175 7422  favorito/logaut"
+00000990: 3e0a 2020 2020 3c69 6d67 2061 6c74 3d22  >.    <img alt="
+000009a0: 636f 6465 636f 7622 2073 7263 3d22 6874  codecov" src="ht
+000009b0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+000009c0: 2f67 682f 6d61 7263 6f66 6176 6f72 6974  /gh/marcofavorit
+000009d0: 6f2f 6c6f 6761 7574 2f62 7261 6e63 682f  o/logaut/branch/
+000009e0: 6d61 7374 6572 2f67 7261 7068 2f62 6164  master/graph/bad
+000009f0: 6765 2e73 7667 3f74 6f6b 656e 3d46 4733  ge.svg?token=FG3
+00000a00: 4154 4750 3550 3522 3e0a 2020 3c2f 613e  ATGP5P5">.  </a>
+00000a10: 0a3c 2f70 3e0a 3c70 2061 6c69 676e 3d22  .</p>.<p align="
+00000a20: 6365 6e74 6572 223e 0a20 203c 6120 6872  center">.  <a hr
+00000a30: 6566 3d22 6874 7470 733a 2f2f 696d 672e  ef="https://img.
+00000a40: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000a50: 2f66 6c61 6b65 382d 6368 6563 6b65 642d  /flake8-checked-
+00000a60: 626c 7565 7669 6f6c 6574 223e 0a20 2020  blueviolet">.   
+00000a70: 203c 696d 6720 616c 743d 2222 2073 7263   <img alt="" src
+00000a80: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000a90: 6965 6c64 732e 696f 2f62 6164 6765 2f66  ields.io/badge/f
+00000aa0: 6c61 6b65 382d 6368 6563 6b65 642d 626c  lake8-checked-bl
+00000ab0: 7565 7669 6f6c 6574 223e 0a20 203c 2f61  ueviolet">.  </a
+00000ac0: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+00000ad0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000ae0: 2e69 6f2f 6261 6467 652f 6d79 7079 2d63  .io/badge/mypy-c
+00000af0: 6865 636b 6564 2d62 6c75 6522 3e0a 2020  hecked-blue">.  
+00000b00: 2020 3c69 6d67 2061 6c74 3d22 2220 7372    <img alt="" sr
+00000b10: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000b20: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000b30: 6d79 7079 2d63 6865 636b 6564 2d62 6c75  mypy-checked-blu
+00000b40: 6522 3e0a 2020 3c2f 613e 0a20 203c 6120  e">.  </a>.  <a 
+00000b50: 6872 6566 3d22 6874 7470 733a 2f2f 696d  href="https://im
+00000b60: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000b70: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
+00000b80: 626c 6163 6b2d 626c 6163 6b22 3e0a 2020  black-black">.  
+00000b90: 2020 3c69 6d67 2061 6c74 3d22 626c 6163    <img alt="blac
+00000ba0: 6b22 2073 7263 3d22 6874 7470 733a 2f2f  k" src="https://
+00000bb0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000bc0: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
+00000bd0: 652d 626c 6163 6b2d 626c 6163 6b22 202f  e-black-black" /
+00000be0: 3e0a 2020 3c2f 613e 0a20 203c 6120 6872  >.  </a>.  <a hr
+00000bf0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
+00000c00: 6d6b 646f 6373 2e6f 7267 2f22 3e0a 2020  mkdocs.org/">.  
+00000c10: 2020 3c69 6d67 2061 6c74 3d22 2220 7372    <img alt="" sr
+00000c20: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000c30: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000c40: 646f 6373 2d6d 6b64 6f63 732d 3963 6622  docs-mkdocs-9cf"
+00000c50: 3e0a 2020 3c2f 613e 0a3c 2f70 3e0a 0a0a  >.  </a>.</p>...
+00000c60: 4c4f 4769 6373 2066 6f72 6d61 6c69 736d  LOGics formalism
+00000c70: 7320 746f 2041 5554 6f6d 6174 610a 0a23  s to AUTomata..#
+00000c80: 2320 5768 6174 2069 7320 606c 6f67 6175  # What is `logau
+00000c90: 7460 0a0a 4c6f 6761 7574 2069 7320 746f  t`..Logaut is to
+00000ca0: 2074 6865 206c 6f67 6963 732d 746f 2d44   the logics-to-D
+00000cb0: 4641 2070 726f 626c 656d 0a77 6861 7420  FA problem.what 
+00000cc0: 4b65 7261 7320 6973 2066 6f72 2044 6565  Keras is for Dee
+00000cd0: 7020 4c65 6172 6e69 6e67 3a0a 6120 7772  p Learning:.a wr
+00000ce0: 6170 7065 7220 746f 2070 6572 666f 726d  apper to perform
+00000cf0: 616e 7420 6261 636b 2d65 6e64 732c 0a62  ant back-ends,.b
+00000d00: 7574 2077 6974 6820 6875 6d61 6e2d 6672  ut with human-fr
+00000d10: 6965 6e64 6c79 2041 5049 732e 0a0a 2323  iendly APIs...##
+00000d20: 2049 6e73 7461 6c6c 0a0a 546f 2069 6e73   Install..To ins
+00000d30: 7461 6c6c 2074 6865 2070 6163 6b61 6765  tall the package
+00000d40: 2066 726f 6d20 5079 5049 3a0a 6060 600a   from PyPI:.```.
+00000d50: 7069 7020 696e 7374 616c 6c20 6c6f 6761  pip install loga
+00000d60: 7574 0a60 6060 0a0a 4d61 6b65 2073 7572  ut.```..Make sur
+00000d70: 6520 746f 2068 6176 6520 5b4c 7964 6961  e to have [Lydia
+00000d80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000d90: 2e63 6f6d 2f77 6869 7465 6d65 6368 2f6c  .com/whitemech/l
+00000da0: 7964 6961 2920 0a69 6e73 7461 6c6c 6564  ydia) .installed
+00000db0: 206f 6e20 796f 7572 206d 6163 6869 6e65   on your machine
+00000dc0: 2e0a 5765 2073 7567 6765 7374 2074 6865  ..We suggest the
+00000dd0: 2066 6f6c 6c6f 7769 6e67 2073 6574 7570   following setup
+00000de0: 3a0a 0a2d 205b 496e 7374 616c 6c20 446f  :..- [Install Do
+00000df0: 636b 6572 5d28 6874 7470 733a 2f2f 7777  cker](https://ww
+00000e00: 772e 646f 636b 6572 2e63 6f6d 2f67 6574  w.docker.com/get
+00000e10: 2d73 7461 7274 6564 290a 2d20 446f 776e  -started).- Down
+00000e20: 6c6f 6164 2074 6865 204c 7964 6961 2044  load the Lydia D
+00000e30: 6f63 6b65 7220 696d 6167 653a 0a60 6060  ocker image:.```
+00000e40: 0a64 6f63 6b65 7220 7075 6c6c 2077 6869  .docker pull whi
+00000e50: 7465 6d65 6368 2f6c 7964 6961 3a6c 6174  temech/lydia:lat
+00000e60: 6573 740a 6060 600a 2d20 4d61 6b65 2074  est.```.- Make t
+00000e70: 6865 2044 6f63 6b65 7220 696d 6167 6520  he Docker image 
+00000e80: 6578 6563 7574 6162 6c65 2075 6e64 6572  executable under
+00000e90: 2074 6865 206e 616d 6520 606c 7964 6961   the name `lydia
+00000ea0: 602e 0a20 204f 6e20 4c69 6e75 7820 616e  `..  On Linux an
+00000eb0: 6420 4d61 634f 5320 6d61 6368 696e 6573  d MacOS machines
+00000ec0: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
+00000ed0: 636f 6d6d 616e 6473 2073 686f 756c 6420  commands should 
+00000ee0: 776f 726b 3a0a 6060 600a 6563 686f 2027  work:.```.echo '
+00000ef0: 2321 2f75 7372 2f62 696e 2f65 6e76 2073  #!/usr/bin/env s
+00000f00: 6827 203e 206c 7964 6961 0a65 6368 6f20  h' > lydia.echo 
+00000f10: 2764 6f63 6b65 7220 7275 6e20 2d76 2428  'docker run -v$(
+00000f20: 7077 6429 3a2f 686f 6d65 2f64 6566 6175  pwd):/home/defau
+00000f30: 6c74 2077 6869 7465 6d65 6368 2f6c 7964  lt whitemech/lyd
+00000f40: 6961 206c 7964 6961 2022 2440 2227 203e  ia lydia "$@"' >
+00000f50: 3e20 6c79 6469 610a 7375 646f 2063 686d  > lydia.sudo chm
+00000f60: 6f64 2075 2b78 206c 7964 6961 0a73 7564  od u+x lydia.sud
+00000f70: 6f20 6d76 206c 7964 6961 202f 7573 722f  o mv lydia /usr/
+00000f80: 6c6f 6361 6c2f 6269 6e2f 0a60 6060 0a0a  local/bin/.```..
+00000f90: 0a54 6869 7320 7769 6c6c 2069 6e73 7461  .This will insta
+00000fa0: 6c6c 2061 6e20 616c 6961 7320 746f 2074  ll an alias to t
+00000fb0: 6865 2069 6e6c 696e 6520 446f 636b 6572  he inline Docker
+00000fc0: 2069 6d61 6765 2065 7865 6375 7469 6f6e   image execution
+00000fd0: 0a69 6e20 796f 7572 2073 7973 7465 6d20  .in your system 
+00000fe0: 5041 5448 2e20 496e 7374 6561 6420 6f66  PATH. Instead of
+00000ff0: 2060 2f75 7372 2f6c 6f63 616c 2f62 696e   `/usr/local/bin
+00001000: 2f60 0a79 6f75 206d 6179 2075 7365 2061  /`.you may use a
+00001010: 6e6f 7468 6572 2070 6174 6820 7768 6963  nother path whic
+00001020: 6820 6973 2073 7469 6c6c 2069 6e20 7468  h is still in th
+00001030: 6520 6050 4154 4860 2076 6172 6961 626c  e `PATH` variabl
+00001040: 652e 0a0a 4f6e 2057 696e 646f 7773 2c20  e...On Windows, 
+00001050: 6d61 6b65 2061 2060 2e62 6174 6020 6669  make a `.bat` fi
+00001060: 6c65 3a0a 6060 600a 646f 636b 6572 2072  le:.```.docker r
+00001070: 756e 202d 2d6e 616d 6520 6c79 6469 6120  un --name lydia 
+00001080: 2d76 2225 6364 2522 3a2f 686f 6d65 2f64  -v"%cd%":/home/d
+00001090: 6566 6175 6c74 2077 6869 7465 6d65 6368  efault whitemech
+000010a0: 2f6c 7964 6961 206c 7964 6961 2025 2a0a  /lydia lydia %*.
+000010b0: 6060 600a 416e 6420 6164 6420 6974 2074  ```.And add it t
+000010c0: 6f20 796f 7572 2050 4154 4820 7661 7269  o your PATH vari
+000010d0: 6162 6c65 2e0a 0a0a 2323 2051 7569 636b  able....## Quick
+000010e0: 7374 6172 740a 0a4e 6f77 2079 6f75 2061  start..Now you a
+000010f0: 7265 2072 6561 6479 2074 6f20 676f 3a0a  re ready to go:.
+00001100: 6060 6070 7974 686f 6e0a 6672 6f6d 206c  ```python.from l
+00001110: 6f67 6175 7420 696d 706f 7274 206c 746c  ogaut import ltl
+00001120: 3264 6661 0a66 726f 6d20 7079 6c6f 6769  2dfa.from pylogi
+00001130: 6373 2e70 6172 7365 7273 2069 6d70 6f72  cs.parsers impor
+00001140: 7420 7061 7273 655f 6c74 6c0a 666f 726d  t parse_ltl.form
+00001150: 756c 6120 3d20 7061 7273 655f 6c74 6c28  ula = parse_ltl(
+00001160: 2246 2861 2922 290a 6466 6120 3d20 6c74  "F(a)").dfa = lt
+00001170: 6c32 6466 6128 666f 726d 756c 612c 2062  l2dfa(formula, b
+00001180: 6163 6b65 6e64 3d22 6c79 6469 6122 290a  ackend="lydia").
+00001190: 6060 600a 0a54 6865 2066 756e 6374 696f  ```..The functio
+000011a0: 6e20 606c 746c 3264 6661 6020 7461 6b65  n `ltl2dfa` take
+000011b0: 7320 696e 2069 6e70 7574 2061 200a 5b70  s in input a .[p
+000011c0: 796c 6f67 6963 735d 2868 7474 7073 3a2f  ylogics](https:/
+000011d0: 2f67 6974 6875 622e 636f 6d2f 7768 6974  /github.com/whit
+000011e0: 656d 6563 682f 7079 6c6f 6769 6373 2920  emech/pylogics) 
+000011f0: 0a60 666f 726d 756c 6160 2061 6e64 2067  .`formula` and g
+00001200: 6976 6573 2069 6e20 6f75 7470 7574 0a61  ives in output.a
+00001210: 205b 7079 7468 6f6d 6174 615d 2868 7474   [pythomata](htt
+00001220: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001230: 7768 6974 656d 6563 682f 7079 7468 6f6d  whitemech/pythom
+00001240: 6174 6129 2044 4641 2e0a 0a54 6865 6e2c  ata) DFA...Then,
+00001250: 2079 6f75 2063 616e 206d 616e 6970 756c   you can manipul
+00001260: 6174 6520 7468 6520 4446 4120 6173 2064  ate the DFA as d
+00001270: 6f6e 6520 7769 7468 2050 7974 686f 6d61  one with Pythoma
+00001280: 7461 2c0a 652e 672e 2074 6f20 7072 696e  ta,.e.g. to prin
+00001290: 743a 0a60 6060 0a64 6661 2e74 6f5f 6772  t:.```.dfa.to_gr
+000012a0: 6170 6876 697a 2829 2e72 656e 6465 7228  aphviz().render(
+000012b0: 2265 7665 6e74 7561 6c6c 792e 6466 6122  "eventually.dfa"
+000012c0: 290a 6060 600a 0a43 7572 7265 6e74 6c79  ).```..Currently
+000012d0: 2c20 7468 6520 606c 7964 6961 6020 6261  , the `lydia` ba
+000012e0: 636b 656e 6420 6f6e 6c79 2073 7570 706f  ckend only suppo
+000012f0: 7274 730a 7468 6520 606c 746c 6020 616e  rts.the `ltl` an
+00001300: 6420 606c 646c 6020 6c6f 6769 6373 2e0a  d `ldl` logics..
+00001310: 0a54 6865 2060 6c74 6c66 3264 6661 602c  .The `ltlf2dfa`,
+00001320: 2062 6173 6564 206f 6e20 0a5b 4c54 4c66   based on .[LTLf
+00001330: 3244 4641 5d28 6874 7470 733a 2f2f 6769  2DFA](https://gi
+00001340: 7468 7562 2e63 6f6d 2f77 6869 7465 6d65  thub.com/whiteme
+00001350: 6368 2f4c 544c 6632 4446 412f 292c 0a73  ch/LTLf2DFA/),.s
+00001360: 7570 706f 7274 7320 606c 746c 6020 616e  upports `ltl` an
+00001370: 6420 6070 6c74 6c60 2e0a 4669 7273 742c  d `pltl`..First,
+00001380: 2069 6e73 7461 6c6c 2069 7420 6174 2076   install it at v
+00001390: 6572 7369 6f6e 2060 312e 302e 3160 3a0a  ersion `1.0.1`:.
+000013a0: 6060 600a 7069 7020 696e 7374 616c 6c20  ```.pip install 
+000013b0: 6769 742b 6874 7470 733a 2f2f 6769 7468  git+https://gith
+000013c0: 7562 2e63 6f6d 2f77 6869 7465 6d65 6368  ub.com/whitemech
+000013d0: 2f4c 544c 6632 4446 412e 6769 7440 6465  /LTLf2DFA.git@de
+000013e0: 7665 6c6f 7023 6567 673d 6c74 6c66 3264  velop#egg=ltlf2d
+000013f0: 6661 0a60 6060 0a0a 5468 656e 2c20 796f  fa.```..Then, yo
+00001400: 7520 6361 6e20 7573 653a 0a60 6060 7079  u can use:.```py
+00001410: 7468 6f6e 0a66 726f 6d20 6c6f 6761 7574  thon.from logaut
+00001420: 2069 6d70 6f72 7420 706c 746c 3264 6661   import pltl2dfa
+00001430: 0a66 726f 6d20 7079 6c6f 6769 6373 2e70  .from pylogics.p
+00001440: 6172 7365 7273 2069 6d70 6f72 7420 7061  arsers import pa
+00001450: 7273 655f 706c 746c 0a66 6f72 6d75 6c61  rse_pltl.formula
+00001460: 203d 2070 6172 7365 5f70 6c74 6c28 2261   = parse_pltl("a
+00001470: 2053 2062 2229 0a64 6661 203d 2070 6c74   S b").dfa = plt
+00001480: 6c32 6466 6128 666f 726d 756c 612c 2062  l2dfa(formula, b
+00001490: 6163 6b65 6e64 3d22 6c74 6c66 3264 6661  ackend="ltlf2dfa
+000014a0: 2229 0a60 6060 0a0a 2323 2057 7269 7465  ").```..## Write
+000014b0: 2079 6f75 7220 6f77 6e20 6261 636b 656e   your own backen
+000014c0: 640a 0a59 6f75 2063 616e 2077 7269 7465  d..You can write
+000014d0: 2079 6f75 7220 6261 636b 2d65 6e64 2062   your back-end b
+000014e0: 7920 696d 706c 656d 656e 7469 6e67 0a74  y implementing.t
+000014f0: 6865 2060 4261 636b 656e 6460 2069 6e74  he `Backend` int
+00001500: 6572 6661 6365 3a0a 0a60 6060 7079 7468  erface:..```pyth
+00001510: 6f6e 0a66 726f 6d20 6c6f 6761 7574 2e62  on.from logaut.b
+00001520: 6163 6b65 6e64 732e 6261 7365 2069 6d70  ackends.base imp
+00001530: 6f72 7420 4261 636b 656e 640a 0a63 6c61  ort Backend..cla
+00001540: 7373 204d 7942 6163 6b65 6e64 2842 6163  ss MyBackend(Bac
+00001550: 6b65 6e64 293a 0a0a 2020 2020 6465 6620  kend):..    def 
+00001560: 6c74 6c32 6466 6128 7365 6c66 2c20 666f  ltl2dfa(self, fo
+00001570: 726d 756c 613a 2046 6f72 6d75 6c61 2920  rmula: Formula) 
+00001580: 2d3e 2044 4641 3a0a 2020 2020 2020 2020  -> DFA:.        
+00001590: 2222 2246 726f 6d20 4c54 4c20 746f 2044  """From LTL to D
+000015a0: 4641 2e22 2222 0a0a 2020 2020 6465 6620  FA."""..    def 
+000015b0: 6c64 6c32 6466 6128 7365 6c66 2c20 666f  ldl2dfa(self, fo
+000015c0: 726d 756c 613a 2046 6f72 6d75 6c61 2920  rmula: Formula) 
+000015d0: 2d3e 2044 4641 3a0a 2020 2020 2020 2020  -> DFA:.        
+000015e0: 2222 2246 726f 6d20 4c44 4c20 746f 2044  """From LDL to D
+000015f0: 4641 2e22 2222 0a0a 2020 2020 6465 6620  FA."""..    def 
+00001600: 706c 746c 3264 6661 2873 656c 662c 2066  pltl2dfa(self, f
+00001610: 6f72 6d75 6c61 3a20 466f 726d 756c 6129  ormula: Formula)
+00001620: 202d 3e20 4446 413a 0a20 2020 2020 2020   -> DFA:.       
+00001630: 2022 2222 4672 6f6d 2050 4c54 4c20 746f   """From PLTL to
+00001640: 2044 4641 2e22 2222 0a0a 2020 2020 6465   DFA."""..    de
+00001650: 6620 706c 646c 3264 6661 2873 656c 662c  f pldl2dfa(self,
+00001660: 2066 6f72 6d75 6c61 3a20 466f 726d 756c   formula: Formul
+00001670: 6129 202d 3e20 4446 413a 0a20 2020 2020  a) -> DFA:.     
+00001680: 2020 2022 2222 4672 6f6d 2050 4c44 4c20     """From PLDL 
+00001690: 746f 2044 4641 2e22 2222 0a20 2020 2020  to DFA.""".     
+000016a0: 2020 200a 2020 2020 6465 6620 666f 6c32     .    def fol2
+000016b0: 6466 6128 7365 6c66 2c20 666f 726d 756c  dfa(self, formul
+000016c0: 613a 2046 6f72 6d75 6c61 2920 2d3e 2044  a: Formula) -> D
+000016d0: 4641 3a0a 2020 2020 2020 2020 2222 2246  FA:.        """F
+000016e0: 726f 6d20 464f 4c20 746f 2044 4641 2e22  rom FOL to DFA."
+000016f0: 2222 0a0a 2020 2020 6465 6620 6d73 6f32  ""..    def mso2
+00001700: 6466 6128 7365 6c66 2c20 666f 726d 756c  dfa(self, formul
+00001710: 613a 2046 6f72 6d75 6c61 2920 2d3e 2044  a: Formula) -> D
+00001720: 4641 3a0a 2020 2020 2020 2020 2222 2246  FA:.        """F
+00001730: 726f 6d20 4d53 4f20 746f 2044 4641 2e22  rom MSO to DFA."
+00001740: 2222 0a60 6060 0a0a 5468 656e 2c20 796f  "".```..Then, yo
+00001750: 7520 6361 6e20 7265 6769 7374 6572 2074  u can register t
+00001760: 6865 2063 7573 746f 6d20 6261 636b 656e  he custom backen
+00001770: 640a 636c 6173 7320 696e 2074 6865 206c  d.class in the l
+00001780: 6962 7261 7279 3a0a 0a60 6060 7079 7468  ibrary:..```pyth
+00001790: 6f6e 0a66 726f 6d20 6c6f 6761 7574 2e62  on.from logaut.b
+000017a0: 6163 6b65 6e64 7320 696d 706f 7274 2072  ackends import r
+000017b0: 6567 6973 7465 720a 7265 6769 7374 6572  egister.register
+000017c0: 2869 645f 3d22 6d79 5f62 6163 6b65 6e64  (id_="my_backend
+000017d0: 222c 2065 6e74 7279 5f70 6f69 6e74 3d22  ", entry_point="
+000017e0: 646f 7474 6564 2e70 6174 682e 746f 2e4d  dotted.path.to.M
+000017f0: 7942 6163 6b65 6e64 2229 0a60 6060 0a0a  yBackend").```..
+00001800: 416e 6420 7468 656e 2c20 7573 6520 6974  And then, use it
+00001810: 2074 6872 6f75 6768 2074 6865 206d 6169   through the mai
+00001820: 6e20 656e 7472 7920 706f 696e 743a 0a60  n entry point:.`
+00001830: 6060 7079 7468 6f6e 0a64 6661 203d 206c  ``python.dfa = l
+00001840: 746c 3264 6661 2866 6f72 6d75 6c61 2c20  tl2dfa(formula, 
+00001850: 6261 636b 656e 643d 226d 795f 6261 636b  backend="my_back
+00001860: 656e 6422 290a 6060 600a 0a23 2320 5465  end").```..## Te
+00001870: 7374 730a 0a54 6f20 7275 6e20 7465 7374  sts..To run test
+00001880: 733a 2060 746f 7860 0a0a 546f 2072 756e  s: `tox`..To run
+00001890: 206f 6e6c 7920 7468 6520 636f 6465 2074   only the code t
+000018a0: 6573 7473 3a20 6074 6f78 202d 6520 7079  ests: `tox -e py
+000018b0: 332e 3760 0a0a 546f 2072 756e 206f 6e6c  3.7`..To run onl
+000018c0: 7920 7468 6520 6c69 6e74 6572 733a 200a  y the linters: .
+000018d0: 2d20 6074 6f78 202d 6520 666c 616b 6538  - `tox -e flake8
+000018e0: 600a 2d20 6074 6f78 202d 6520 6d79 7079  `.- `tox -e mypy
+000018f0: 600a 2d20 6074 6f78 202d 6520 626c 6163  `.- `tox -e blac
+00001900: 6b2d 6368 6563 6b60 0a2d 2060 746f 7820  k-check`.- `tox 
+00001910: 2d65 2069 736f 7274 2d63 6865 636b 600a  -e isort-check`.
+00001920: 0a50 6c65 6173 6520 6c6f 6f6b 2061 7420  .Please look at 
+00001930: 7468 6520 6074 6f78 2e69 6e69 6020 6669  the `tox.ini` fi
+00001940: 6c65 2066 6f72 2074 6865 2066 756c 6c20  le for the full 
+00001950: 6c69 7374 206f 6620 7375 7070 6f72 7465  list of supporte
+00001960: 6420 636f 6d6d 616e 6473 2e20 0a0a 2323  d commands. ..##
+00001970: 2044 6f63 730a 0a54 6f20 6275 696c 6420   Docs..To build 
+00001980: 7468 6520 646f 6373 3a20 606d 6b64 6f63  the docs: `mkdoc
+00001990: 7320 6275 696c 6460 0a0a 546f 2076 6965  s build`..To vie
+000019a0: 7720 646f 6375 6d65 6e74 6174 696f 6e20  w documentation 
+000019b0: 696e 2061 2062 726f 7773 6572 3a20 606d  in a browser: `m
+000019c0: 6b64 6f63 7320 7365 7276 6560 0a61 6e64  kdocs serve`.and
+000019d0: 2074 6865 6e20 676f 2074 6f20 5b68 7474   then go to [htt
+000019e0: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3830  p://localhost:80
+000019f0: 3030 5d28 6874 7470 3a2f 2f6c 6f63 616c  00](http://local
+00001a00: 686f 7374 3a38 3030 3029 0a0a 2323 204c  host:8000)..## L
+00001a10: 6963 656e 7365 0a0a 6c6f 6761 7574 2069  icense..logaut i
+00001a20: 7320 7265 6c65 6173 6564 2075 6e64 6572  s released under
+00001a30: 2074 6865 2047 4e55 204c 6573 7365 7220   the GNU Lesser 
+00001a40: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
+00001a50: 6963 656e 7365 2076 332e 3020 6f72 206c  icense v3.0 or l
+00001a60: 6174 6572 2028 4c47 504c 7633 2b29 2e0a  ater (LGPLv3+)..
+00001a70: 0a43 6f70 7972 6967 6874 2032 3032 3120  .Copyright 2021 
+00001a80: 5768 6974 654d 6563 680a 0a23 2320 4175  WhiteMech..## Au
+00001a90: 7468 6f72 730a 0a2d 205b 4d61 7263 6f20  thors..- [Marco 
+00001aa0: 4661 766f 7269 746f 5d28 6874 7470 733a  Favorito](https:
+00001ab0: 2f2f 6d61 7263 6f66 6176 6f72 6974 6f2e  //marcofavorito.
+00001ac0: 6d65 2f29 0a0a                           me/)..
```

