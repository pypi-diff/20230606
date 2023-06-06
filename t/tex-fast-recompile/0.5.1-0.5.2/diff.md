# Comparing `tmp/tex-fast-recompile-0.5.1.tar.gz` & `tmp/tex-fast-recompile-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tex-fast-recompile-0.5.1.tar", last modified: Mon Jun  5 16:24:47 2023, max compression
+gzip compressed data, was "tex-fast-recompile-0.5.2.tar", last modified: Tue Jun  6 08:07:49 2023, max compression
```

## Comparing `tex-fast-recompile-0.5.1.tar` & `tex-fast-recompile-0.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 16:24:47.348035 tex-fast-recompile-0.5.1/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1799 2023-01-12 16:09:27.000000 tex-fast-recompile-0.5.1/.gitignore
--rw-r--r--   0 user202729  (1000) user202729  (1000)    19105 2023-01-12 16:09:42.000000 tex-fast-recompile-0.5.1/LICENSE
--rw-r--r--   0 user202729  (1000) user202729  (1000)     6678 2023-06-05 16:24:47.348035 tex-fast-recompile-0.5.1/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)     6214 2023-06-02 05:25:15.000000 tex-fast-recompile-0.5.1/README.md
--rw-r--r--   0 user202729  (1000) user202729  (1000)       45 2023-06-02 08:06:52.000000 tex-fast-recompile-0.5.1/pytest.ini
--rw-r--r--   0 user202729  (1000) user202729  (1000)        9 2023-01-12 17:26:41.000000 tex-fast-recompile-0.5.1/requirements.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)      738 2023-06-05 16:24:47.351368 tex-fast-recompile-0.5.1/setup.cfg
--rw-r--r--   0 user202729  (1000) user202729  (1000)       63 2023-01-12 16:30:18.000000 tex-fast-recompile-0.5.1/setup.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 16:24:47.344702 tex-fast-recompile-0.5.1/tests/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     5205 2023-06-05 16:22:47.000000 tex-fast-recompile-0.5.1/tests/test_main.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 16:24:47.344702 tex-fast-recompile-0.5.1/tex/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4033 2023-06-02 07:59:36.000000 tex-fast-recompile-0.5.1/tex/fastrecompile.sty
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 16:24:47.348035 tex-fast-recompile-0.5.1/tex_fast_recompile/
--rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-06-02 08:06:32.000000 tex-fast-recompile-0.5.1/tex_fast_recompile/__init__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)    21348 2023-06-05 16:23:08.000000 tex-fast-recompile-0.5.1/tex_fast_recompile/__main__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4113 2023-02-07 16:26:44.000000 tex-fast-recompile-0.5.1/tex_fast_recompile/latexmk.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-01-12 16:30:32.000000 tex-fast-recompile-0.5.1/tex_fast_recompile/py.typed
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1163 2023-06-02 08:39:53.000000 tex-fast-recompile-0.5.1/tex_fast_recompile/util.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 16:24:47.348035 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     6678 2023-06-05 16:24:46.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)      517 2023-06-05 16:24:47.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/SOURCES.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-06-05 16:24:46.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/dependency_links.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)      133 2023-06-05 16:24:46.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/entry_points.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)       30 2023-06-05 16:24:46.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/requires.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)       19 2023-06-05 16:24:46.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/top_level.txt
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-06 08:07:49.969072 tex-fast-recompile-0.5.2/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1799 2023-01-12 16:09:27.000000 tex-fast-recompile-0.5.2/.gitignore
+-rw-r--r--   0 user202729  (1000) user202729  (1000)    19105 2023-01-12 16:09:42.000000 tex-fast-recompile-0.5.2/LICENSE
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     7665 2023-06-06 08:07:49.969072 tex-fast-recompile-0.5.2/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     7201 2023-06-06 08:01:38.000000 tex-fast-recompile-0.5.2/README.md
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       45 2023-06-02 08:06:52.000000 tex-fast-recompile-0.5.2/pytest.ini
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        9 2023-01-12 17:26:41.000000 tex-fast-recompile-0.5.2/requirements.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      738 2023-06-06 08:07:49.969072 tex-fast-recompile-0.5.2/setup.cfg
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       79 2023-06-06 08:06:43.000000 tex-fast-recompile-0.5.2/setup.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-06 08:07:49.965739 tex-fast-recompile-0.5.2/tests/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     6820 2023-06-06 08:06:09.000000 tex-fast-recompile-0.5.2/tests/test_main.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-06 08:07:49.965739 tex-fast-recompile-0.5.2/tex/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     4033 2023-06-02 07:59:36.000000 tex-fast-recompile-0.5.2/tex/fastrecompile.sty
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-06 08:07:49.969072 tex-fast-recompile-0.5.2/tex_fast_recompile/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-06-02 08:06:32.000000 tex-fast-recompile-0.5.2/tex_fast_recompile/__init__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)    21920 2023-06-06 08:01:38.000000 tex-fast-recompile-0.5.2/tex_fast_recompile/__main__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     4113 2023-02-07 16:26:44.000000 tex-fast-recompile-0.5.2/tex_fast_recompile/latexmk.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-01-12 16:30:32.000000 tex-fast-recompile-0.5.2/tex_fast_recompile/py.typed
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1163 2023-06-02 08:39:53.000000 tex-fast-recompile-0.5.2/tex_fast_recompile/util.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-06 08:07:49.969072 tex-fast-recompile-0.5.2/tex_fast_recompile.egg-info/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     7665 2023-06-06 08:07:49.000000 tex-fast-recompile-0.5.2/tex_fast_recompile.egg-info/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      517 2023-06-06 08:07:49.000000 tex-fast-recompile-0.5.2/tex_fast_recompile.egg-info/SOURCES.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-06-06 08:07:49.000000 tex-fast-recompile-0.5.2/tex_fast_recompile.egg-info/dependency_links.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      133 2023-06-06 08:07:49.000000 tex-fast-recompile-0.5.2/tex_fast_recompile.egg-info/entry_points.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       30 2023-06-06 08:07:49.000000 tex-fast-recompile-0.5.2/tex_fast_recompile.egg-info/requires.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       19 2023-06-06 08:07:49.000000 tex-fast-recompile-0.5.2/tex_fast_recompile.egg-info/top_level.txt
```

### Comparing `tex-fast-recompile-0.5.1/.gitignore` & `tex-fast-recompile-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.1/LICENSE` & `tex-fast-recompile-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.1/PKG-INFO` & `tex-fast-recompile-0.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-Metadata-Version: 2.1
-Name: tex-fast-recompile
-Version: 0.5.1
-Summary: A Python module to speed up TeX compilation.
-Home-page: https://github.com/user202729/tex-fast-recompile
-Author: user202729
-License: LPPL 1.3c
-Classifier: License :: OSI Approved
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Text Processing :: Markup :: LaTeX
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # tex-fast-recompile
 
+[![PyPI](https://img.shields.io/pypi/v/tex-fast-recompile?style=flat)](https://pypi.python.org/pypi/tex-fast-recompile/)
+
 A Python module to speed up TeX compilation.
 
 This is similar to the [`mylatexformat` TeX package](https://ctan.org/pkg/mylatexformat) that it works by "speed up" some "preamble",
 but unlike using "precompiled preamble" i.e. custom TeX format,
 this package works with *every* package including package that executes some Lua code, or load OpenType font.
 
 ## Installation
@@ -28,21 +16,34 @@
 * https://github.com/user202729/tex-fast-recompile
 
 You also need to install the helper TeX package `fastrecompile.sty`, which can be found in the `tex/` directory.
 Refer to https://tex.stackexchange.com/q/1137/250119 for installation instruction.
 
 (currently the TeX package is not available on CTAN)
 
-## Usage
+### Manual installation from source (GitHub)
 
-### Note for Vim users
+In case I fix some bug in the latest version but forget to push to PyPI.
 
-If update performance appears slow, try disabling `writebackup`, or set `backupcopy=yes`.
-(this issue happened once for me, and I haven't been able to reproduce it so far. Alternatively just try
-restarting your computer.)
+Run from the command-line:
+
+```bash
+pip install git+https://github.com/user202729/tex-fast-recompile
+```
+
+or alternatively download the code from GitHub by clicking "Code ⯆" green button → "Download ZIP" (at the moment),
+then unzip the file and from within the folder,
+
+```bash
+pip install -e .
+```
+
+The `-e` is an "editable" install, that is if you modify the source code in the folder, you don't need to reinstall the package.
+
+## Usage
 
 ### Normal mode
 
 If installed properly, an executable `tex_fast_recompile` should be available on your command-line.
 
 Run `tex_fast_recompile --help` to view the available options.
 
@@ -65,14 +66,34 @@
 
 For VimTeX usage, putting the following configuration in `.vimrc` usually suffices:
 
 ```vim
 let g:vimtex_compiler_latexmk = { 'executable' : 'tex_fast_recompile_latexmk' }
 ```
 
+### Note for Windows users
+
+For yet-unknown reasons, file names containing non-ASCII characters are not supported. For example the following is invalid:
+
+```bash
+tex_fast_recompile pdflatex ≡.tex
+```
+
+As a workaround, the following appears to work:
+
+```bash
+python -m tex_fast_recompile pdflatex ≡.tex
+```
+
+### Note for Vim users
+
+If update performance appears slow, try disabling `writebackup`, or set `backupcopy=yes`.
+(this issue happened once for me, and I haven't been able to reproduce it so far. Alternatively just try
+restarting your computer.)
+
 ## Limitations
 
 * If VimTeX is used, the latexmk (emulation) is forcefully killed when compilation stops.
 In that case, the temporary directory is not cleaned, and over time it may clutter the temporary directory.
 
   (this has a partial workaround, that is new process spawned will clean up previous process' temporary directories)
 * Any file `\input` in the preamble must not be changed. (when the preamble changes, the program will automatically detect that)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tex-fast-recompile-0.5.1/README.md` & `tex-fast-recompile-0.5.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,25 @@
+Metadata-Version: 2.1
+Name: tex-fast-recompile
+Version: 0.5.2
+Summary: A Python module to speed up TeX compilation.
+Home-page: https://github.com/user202729/tex-fast-recompile
+Author: user202729
+License: LPPL 1.3c
+Classifier: License :: OSI Approved
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Text Processing :: Markup :: LaTeX
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # tex-fast-recompile
 
+[![PyPI](https://img.shields.io/pypi/v/tex-fast-recompile?style=flat)](https://pypi.python.org/pypi/tex-fast-recompile/)
+
 A Python module to speed up TeX compilation.
 
 This is similar to the [`mylatexformat` TeX package](https://ctan.org/pkg/mylatexformat) that it works by "speed up" some "preamble",
 but unlike using "precompiled preamble" i.e. custom TeX format,
 this package works with *every* package including package that executes some Lua code, or load OpenType font.
 
 ## Installation
@@ -14,21 +30,34 @@
 * https://github.com/user202729/tex-fast-recompile
 
 You also need to install the helper TeX package `fastrecompile.sty`, which can be found in the `tex/` directory.
 Refer to https://tex.stackexchange.com/q/1137/250119 for installation instruction.
 
 (currently the TeX package is not available on CTAN)
 
-## Usage
+### Manual installation from source (GitHub)
 
-### Note for Vim users
+In case I fix some bug in the latest version but forget to push to PyPI.
 
-If update performance appears slow, try disabling `writebackup`, or set `backupcopy=yes`.
-(this issue happened once for me, and I haven't been able to reproduce it so far. Alternatively just try
-restarting your computer.)
+Run from the command-line:
+
+```bash
+pip install git+https://github.com/user202729/tex-fast-recompile
+```
+
+or alternatively download the code from GitHub by clicking "Code ⯆" green button → "Download ZIP" (at the moment),
+then unzip the file and from within the folder,
+
+```bash
+pip install -e .
+```
+
+The `-e` is an "editable" install, that is if you modify the source code in the folder, you don't need to reinstall the package.
+
+## Usage
 
 ### Normal mode
 
 If installed properly, an executable `tex_fast_recompile` should be available on your command-line.
 
 Run `tex_fast_recompile --help` to view the available options.
 
@@ -51,14 +80,34 @@
 
 For VimTeX usage, putting the following configuration in `.vimrc` usually suffices:
 
 ```vim
 let g:vimtex_compiler_latexmk = { 'executable' : 'tex_fast_recompile_latexmk' }
 ```
 
+### Note for Windows users
+
+For yet-unknown reasons, file names containing non-ASCII characters are not supported. For example the following is invalid:
+
+```bash
+tex_fast_recompile pdflatex ≡.tex
+```
+
+As a workaround, the following appears to work:
+
+```bash
+python -m tex_fast_recompile pdflatex ≡.tex
+```
+
+### Note for Vim users
+
+If update performance appears slow, try disabling `writebackup`, or set `backupcopy=yes`.
+(this issue happened once for me, and I haven't been able to reproduce it so far. Alternatively just try
+restarting your computer.)
+
 ## Limitations
 
 * If VimTeX is used, the latexmk (emulation) is forcefully killed when compilation stops.
 In that case, the temporary directory is not cleaned, and over time it may clutter the temporary directory.
 
   (this has a partial workaround, that is new process spawned will clean up previous process' temporary directories)
 * Any file `\input` in the preamble must not be changed. (when the preamble changes, the program will automatically detect that)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tex-fast-recompile-0.5.1/setup.cfg` & `tex-fast-recompile-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tex-fast-recompile
-version = 0.5.1
+version = 0.5.2
 author = user202729
 description = A Python module to speed up TeX compilation.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = LPPL 1.3c
 url = https://github.com/user202729/tex-fast-recompile
 classifiers =
```

### Comparing `tex-fast-recompile-0.5.1/tests/test_main.py` & `tex-fast-recompile-0.5.2/tests/test_main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,79 @@
+from __future__ import annotations
+
 from threading import Timer
 import sys
+import os
 import pytest
 from pathlib import Path
 import textwrap
 import subprocess
 from typing import Callable
 import time
 import psutil  # type: ignore
 
 LinePredicate=Callable[[str], bool]
 line_predicates: list[LinePredicate]=[]
 
-def ensure_print_lines(process: subprocess.Popen, expects: list[LinePredicate], kill: bool=True)->None:
-	timer=Timer(1, process.kill)
+class Process:
+	def __init__(self, *args, **kwargs)->None:
+		self.args=args
+		self.kwargs=kwargs
+
+	def __enter__(self)->Process:
+		self.process=psutil.Popen(*self.args, **self.kwargs)
+		return self
+
+	def kill(self)->None:
+		process=self.process
+		if os.name=="nt":
+			try:
+				processes = [process] + process.children(recursive=True)
+			except psutil.NoSuchProcess:
+				return
+
+			for p in processes:
+				try: p.kill()
+				except psutil.NoSuchProcess: pass
+				p.wait()
+		else:
+			try: process.kill()
+			except psutil.NoSuchProcess: pass
+
+	def __exit__(self, exc_type, exc_value, traceback)->None:
+		self.kill()
+		
+
+def ensure_print_lines(process: Process, expects: list[LinePredicate])->None:
+	timer=Timer(5, process.kill)
 	timer.start()
 	expects=expects[::-1]
-	assert process.stdout is not None
+	assert process.process.stdout is not None
 	collected_lines=[]
-	for line in process.stdout:
+	for line in process.process.stdout:
 		collected_lines.append(line)
 		waiting_for=expects[-1]
 
 		assert waiting_for in line_predicates
 		for remaining in line_predicates:
-			if remaining!=waiting_for: assert not remaining(line), f"Unexpected line {line}"
+			if remaining!=waiting_for: assert not remaining(line), f"Unexpected line {line} -- seen lines are {collected_lines}"
 
 		if waiting_for(line):
 			expects.pop()
 			if not expects: break
 	else:
-		if not timer.is_alive():
+		if timer.is_alive():
+			assert False, f"Process exit voluntarily but some expected lines are never seen?? -- seen lines are {collected_lines}"
+		else:
 			assert False, f"Timeout without seeing some lines -- seen lines are {collected_lines}"
-		assert False, "Process exit voluntarily but some expected lines are never seen??"
+
+	if not timer.is_alive():
+		print("Warning: all expected lines are seen but process is killed anyway", file=sys.stderr)
+
 	timer.cancel()
-	if kill:
-		process.kill()
 
 
 def possible_line_content(f: LinePredicate)->LinePredicate:
 	line_predicates.append(f)
 	return f
 
 @possible_line_content
@@ -47,15 +82,15 @@
 
 @possible_line_content
 def expect_success(line: str)->bool:
 	return "========success" in line
 
 @possible_line_content
 def expect_rerunning(line: str)->bool:
-	return "Rerunning" in line
+	return "Rerunning" in line  # another LaTeX pass, something might have changed
 
 @possible_line_content
 def expect_preamble_changed(line: str)->bool:
 	return "Preamble changed" in line
 
 
 
@@ -65,20 +100,20 @@
 	txt_file.unlink(missing_ok=True)
 	subprocess.run(["pdftotext", pdf_file])
 	assert content in txt_file.read_text(encoding='u8')
 
 def ensure_pdf_content(folder: Path, content: str)->None:
 	ensure_pdf_content_file(folder/"output"/"a.txt", content)
 
-def prepare_process(tmp_path: Path, content: str, filename: str="a.tex", extra_args: list[str]=[])->tuple[Path, subprocess.Popen]:
+def prepare_process(tmp_path: Path, content: str, filename: str="a.tex", extra_args: list[str]=[])->tuple[Path, Process]:
 	tmp_file=tmp_path/filename
 	tmp_file.write_text(textwrap.dedent(content))
 	output_dir=tmp_path/"output"
 	output_dir.mkdir()
-	process=subprocess.Popen([
+	process=Process([
 		"tex_fast_recompile",
 		"--success-cmd=echo ========success",
 		"--failure-cmd=echo ========failure",
 		"--output-directory="+str(output_dir),
 		*extra_args,
 		"pdflatex", "--", filename], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, cwd=tmp_path)
 	return tmp_file, process
@@ -86,98 +121,115 @@
 
 def test_empty_output_pdf(tmp_path: Path)->None:
 	_, process=prepare_process(tmp_path, r"""
 	\documentclass{article}
 	\begin{document}
 	\end{document}
 	""")
-	ensure_print_lines(process, [expect_failure])
+	with process:
+		ensure_print_lines(process, [expect_failure])
 
 def test_tex_error(tmp_path: Path)->None:
 	_, process=prepare_process(tmp_path, r"""
 	\documentclass{article}
 	\begin{document}
 	123
 	\errmessage{hello world}
 	\end{document}
 	""")
-	ensure_print_lines(process, [expect_failure])
+	with process:
+		ensure_print_lines(process, [expect_failure])
 
 def test_recompile(tmp_path: Path)->None:
+	# in newer versions of LaTeX rerunfilecheck is not necessary
 	tmp_file, process=prepare_process(tmp_path, r"""
 	\documentclass{article}
+	\usepackage[mainaux]{rerunfilecheck}
 	\begin{document}
 	\label{abc}page[\pageref{abc}]
 	\end{document}
 	""")
-	ensure_print_lines(process, [expect_rerunning, expect_success], kill=False)
-	ensure_pdf_content(tmp_path, "page[1]")
-	tmp_file.write_text(textwrap.dedent(r"""
-	\documentclass{article}
-	\begin{document}
-	123\clearpage
-	\label{abc}page[\pageref{abc}]
-	\end{document}
-	"""))
-	ensure_print_lines(process, [expect_rerunning, expect_success])
-	ensure_pdf_content(tmp_path, "page[2]")
+	with process:
+		ensure_print_lines(process, [expect_rerunning, expect_success])
+		ensure_pdf_content(tmp_path, "page[1]")
+		tmp_file.write_text(textwrap.dedent(r"""
+		\documentclass{article}
+		\usepackage[mainaux]{rerunfilecheck}
+		\begin{document}
+		123\clearpage
+		\label{abc}page[\pageref{abc}]
+		\end{document}
+		"""))
+		ensure_print_lines(process, [expect_rerunning, expect_success])
+		ensure_pdf_content(tmp_path, "page[2]")
+
+skipif_windows=pytest.mark.skipif('os.name=="nt"')
 
 # note that `"` in file name is not supported
 @pytest.mark.parametrize("filename,valid", [
 	("{~", True),
-	("}|%", True),
-	("#  &^_\\:≡", True),
+	("}%", True),
+	pytest.param("%|", True, marks=skipif_windows),
+	("#  &^_", True),
+	pytest.param("≡", True, marks=skipif_windows),
+	pytest.param("\\?:", True, marks=skipif_windows),
 	("--help", True),
 
 	("$TEXMFHOME", False),
-	("|cat a.tex", False),
+	pytest.param("|cat a.tex", False, marks=skipif_windows),
 	("~", False),
-	("\"", False),
+	pytest.param("\"", False, marks=skipif_windows),
 	])
 @pytest.mark.parametrize("temp_output_directory", [True, False])
 def test_weird_file_name(tmp_path: Path, filename: str, valid: bool, temp_output_directory: bool)->None:
 	_, process=prepare_process(
 			tmp_path, r"""
 			\documentclass{article}
 			\begin{document}
 			helloworld
 			\end{document}
 			""",
 			filename=filename+".tex",
 			extra_args=["--temp-output-directory"] if temp_output_directory else [],
 			)
-	if not valid:
-		process.wait(timeout=2)
-		assert process.stderr
-		assert "AssertionError" in process.stderr.read()
-		return
-	ensure_print_lines(process, [expect_success])
-	process.kill()
-	ensure_pdf_content_file(tmp_path/"output"/(filename+".pdf"), "helloworld")
+	with process:
+		if not valid:
+			process.process.wait(timeout=2)
+			assert process.process.stderr
+			assert "AssertionError" in process.process.stderr.read()
+			return
+		ensure_print_lines(process, [expect_success])
+		ensure_pdf_content_file(tmp_path/"output"/(filename+".pdf"), "helloworld")
 
 def test_subprocess_killed_on_preamble_change(tmp_path: Path)->None:
 	file, process=prepare_process(tmp_path, r"""
 	\documentclass{article}
 	\begin{document}
 	helloworld
 	\end{document}
 	""")
-	ensure_print_lines(process, [expect_success], kill=False)
+	with process:
+		ensure_print_lines(process, [expect_success])
 
-	time.sleep(1)
-	assert count_child_processes(process)==1
-
-	file.write_text(textwrap.dedent(r"""
-	\documentclass{article}
-	\usepackage{amsmath}
-	\begin{document}
-	helloworld
-	\end{document}
-	"""))
-	ensure_print_lines(process, [expect_preamble_changed, expect_success], kill=False)
-	time.sleep(1)
-	assert count_child_processes(process)==1  # if this is 2 then there's the resource leak
-	process.kill()
+		time.sleep(1)
+		assert count_pdflatex_child_processes(process)==1, process.process.children(recursive=True)
 
-def count_child_processes(process: subprocess.Popen)->int:
-	return len(psutil.Process(process.pid).children(recursive=True))
+		file.write_text(textwrap.dedent(r"""
+		\documentclass{article}
+		\usepackage{amsmath}
+		\begin{document}
+		helloworld
+		\end{document}
+		"""))
+		ensure_print_lines(process, [expect_preamble_changed, expect_success])
+		time.sleep(1)
+		assert count_pdflatex_child_processes(process)==1, process.process.children(recursive=True)
+		# if this is 2 then there's the resource leak
+
+def count_pdflatex_child_processes(process: Process)->int:
+	return len([
+		x for x in process.process.children(recursive=True)
+		if Path(x.exe()).stem in ["pdftex", "pdflatex"]
+		# on Windows it's pdflatex (exe() returns symbolic link name)
+		# on Linux it's pdftex (exe() returns original executable name)
+		])
```

### Comparing `tex-fast-recompile-0.5.1/tex/fastrecompile.sty` & `tex-fast-recompile-0.5.2/tex/fastrecompile.sty`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.1/tex_fast_recompile/__main__.py` & `tex-fast-recompile-0.5.2/tex_fast_recompile/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import subprocess
 import threading
 import queue
 import shutil
 import sys
 import time
 import tempfile
+import traceback
 import os
 #import atexit
 import enum
 import psutil  # type: ignore
 from .util import *
 
 @dataclass
@@ -259,14 +260,19 @@
 		# wait for the process to finish
 		process.wait()
 
 		return process.returncode==0
 
 	def __exit__(self, exc_type, exc_value, traceback)->None:
 		self._process.kill()
+		try:
+			self._process.wait(timeout=1)  # on Windows this is needed to ensure process really exited -- #14
+		except subprocess.TimeoutExpired:
+			traceback.print_exc()
+			print("[Subprocess cannot be killed! Possible resource leak]")
 		if self._copy_stdout_thread is not None:
 			self._copy_stdout_thread.join()
 
 tmpdir=Path(tempfile.gettempdir())/".tex-fast-recompile-tmp"
 tmpdir.mkdir(parents=True, exist_ok=True)
 
 
@@ -348,16 +354,20 @@
 				shutil.copy2(file, self.output_directory)
 		# note: this is inefficient because it copies instead of moves
 		# note: currently files generated in subdirectories not supported
 		return result
 
 	def __exit__(self, exc_type, exc_value, traceback)->None:
 		self._daemon.__exit__(exc_type, exc_value, traceback)
-		shutil.rmtree(self._temp_output_dir_path)  # oddly cleanup() alone does not always remove the directory?
-		self._temp_output_dir.cleanup()
+		try:
+			shutil.rmtree(self._temp_output_dir_path)  # oddly cleanup() alone does not always remove the directory?
+			self._temp_output_dir.cleanup()
+		except:
+			traceback.print_exc()
+			print(f"[Cannot clean up temporary directory at {self._temp_output_dir_path}! Possible resource leak]")
 
 
 @dataclass
 class CompilationDaemon:
 	"""
 	Usage::
 
@@ -445,20 +455,17 @@
 
 					if no_preamble_error_instance is not None:
 						raise no_preamble_error_instance
 					return_0=daemon.finish()
 
 				self.finish_callback(return_0=return_0)
 
-				try:
-					log_text: bytes=(daemon.output_directory/args.jobname).with_suffix(".log").read_bytes()
-				except FileNotFoundError:
-					log_text=b""
+				log_text: bytes=(daemon.output_directory/args.jobname).with_suffix(".log").read_bytes()
 
-				if b"Rerun to get" in log_text:
+				if b"Rerun to get" in log_text or b"Rerun." in log_text:
 					print("Rerunning." + "\n"*args.num_separation_lines)
 					immediately_recompile=True
 					continue
 
 				if return_0 and (daemon.output_directory/args.jobname).with_suffix(".pdf").is_file():
 					if args.success_cmd:
 						subprocess.run(args.success_cmd, shell=True, check=True)
@@ -562,15 +569,23 @@
 	if not Path(args.filename).is_file():
 		raise FileNotFoundError(f"File {args.filename} not found (in directory {os.getcwd()}).")
 
 	daemon=CompilationDaemon(args)
 	daemon.recompile(False)
 
 	while True:
-		recompile_preamble=q.get()
+		if os.name=="nt":
+			# https://github.com/user202729/tex-fast-recompile/issues/15
+			while True:
+				try:
+					recompile_preamble=q.get(timeout=1)
+					break
+				except queue.Empty: continue
+		else:
+			recompile_preamble=q.get()
 		sys.stdout.write("\n"*args.num_separation_lines)
 
 		# wait for the specified delay
 		time.sleep(args.extra_delay)
 
 		# empty out the queue
 		while not q.empty():
```

### Comparing `tex-fast-recompile-0.5.1/tex_fast_recompile/latexmk.py` & `tex-fast-recompile-0.5.2/tex_fast_recompile/latexmk.py`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.1/tex_fast_recompile/util.py` & `tex-fast-recompile-0.5.2/tex_fast_recompile/util.py`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/PKG-INFO` & `tex-fast-recompile-0.5.2/tex_fast_recompile.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: tex-fast-recompile
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python module to speed up TeX compilation.
 Home-page: https://github.com/user202729/tex-fast-recompile
 Author: user202729
 License: LPPL 1.3c
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tex-fast-recompile
 
+[![PyPI](https://img.shields.io/pypi/v/tex-fast-recompile?style=flat)](https://pypi.python.org/pypi/tex-fast-recompile/)
+
 A Python module to speed up TeX compilation.
 
 This is similar to the [`mylatexformat` TeX package](https://ctan.org/pkg/mylatexformat) that it works by "speed up" some "preamble",
 but unlike using "precompiled preamble" i.e. custom TeX format,
 this package works with *every* package including package that executes some Lua code, or load OpenType font.
 
 ## Installation
@@ -28,21 +30,34 @@
 * https://github.com/user202729/tex-fast-recompile
 
 You also need to install the helper TeX package `fastrecompile.sty`, which can be found in the `tex/` directory.
 Refer to https://tex.stackexchange.com/q/1137/250119 for installation instruction.
 
 (currently the TeX package is not available on CTAN)
 
-## Usage
+### Manual installation from source (GitHub)
 
-### Note for Vim users
+In case I fix some bug in the latest version but forget to push to PyPI.
 
-If update performance appears slow, try disabling `writebackup`, or set `backupcopy=yes`.
-(this issue happened once for me, and I haven't been able to reproduce it so far. Alternatively just try
-restarting your computer.)
+Run from the command-line:
+
+```bash
+pip install git+https://github.com/user202729/tex-fast-recompile
+```
+
+or alternatively download the code from GitHub by clicking "Code ⯆" green button → "Download ZIP" (at the moment),
+then unzip the file and from within the folder,
+
+```bash
+pip install -e .
+```
+
+The `-e` is an "editable" install, that is if you modify the source code in the folder, you don't need to reinstall the package.
+
+## Usage
 
 ### Normal mode
 
 If installed properly, an executable `tex_fast_recompile` should be available on your command-line.
 
 Run `tex_fast_recompile --help` to view the available options.
 
@@ -65,14 +80,34 @@
 
 For VimTeX usage, putting the following configuration in `.vimrc` usually suffices:
 
 ```vim
 let g:vimtex_compiler_latexmk = { 'executable' : 'tex_fast_recompile_latexmk' }
 ```
 
+### Note for Windows users
+
+For yet-unknown reasons, file names containing non-ASCII characters are not supported. For example the following is invalid:
+
+```bash
+tex_fast_recompile pdflatex ≡.tex
+```
+
+As a workaround, the following appears to work:
+
+```bash
+python -m tex_fast_recompile pdflatex ≡.tex
+```
+
+### Note for Vim users
+
+If update performance appears slow, try disabling `writebackup`, or set `backupcopy=yes`.
+(this issue happened once for me, and I haven't been able to reproduce it so far. Alternatively just try
+restarting your computer.)
+
 ## Limitations
 
 * If VimTeX is used, the latexmk (emulation) is forcefully killed when compilation stops.
 In that case, the temporary directory is not cleaned, and over time it may clutter the temporary directory.
 
   (this has a partial workaround, that is new process spawned will clean up previous process' temporary directories)
 * Any file `\input` in the preamble must not be changed. (when the preamble changes, the program will automatically detect that)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/SOURCES.txt` & `tex-fast-recompile-0.5.2/tex_fast_recompile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

