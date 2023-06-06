# Comparing `tmp/inkscape_figure_manager-0.0.3.tar.gz` & `tmp/inkscape_figure_manager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inkscape_figure_manager-0.0.3.tar", last modified: Wed Apr 19 04:08:39 2023, max compression
+gzip compressed data, was "inkscape_figure_manager-0.0.4.tar", last modified: Tue Jun  6 19:30:31 2023, max compression
```

## Comparing `inkscape_figure_manager-0.0.3.tar` & `inkscape_figure_manager-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       50 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.3/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/LICENSE
--rw-r--r--   0        0        0       55 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.3/MANIFEST.in
--rw-r--r--   0        0        0      224 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/Pipfile
--rw-r--r--   0        0        0    28263 2023-04-19 04:06:10.275214 inkscape_figure_manager-0.0.3/Pipfile.lock
--rw-r--r--   0        0        0     1038 2023-04-15 21:12:40.220852 inkscape_figure_manager-0.0.3/README.md
--rw-r--r--   0        0        0      709 2023-04-19 04:06:56.711626 inkscape_figure_manager-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/__init__.py
--rw-r--r--   0        0        0     7922 2023-04-19 04:05:37.378728 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/__main__.py
--rw-r--r--   0        0        0     4022 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/daemon.py
--rw-r--r--   0        0        0     1427 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/picker.py
--rw-r--r--   0        0        0     1892 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/template.svg
--rw-r--r--   0        0        0     3354 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/watcher.py
--rw-r--r--   0        0        0     2504 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/watcher_daemon.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 inkscape_figure_manager-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1081 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/LICENSE
+-rw-r--r--   0        0        0       55 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.4/MANIFEST.in
+-rw-r--r--   0        0        0      224 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/Pipfile
+-rw-r--r--   0        0        0    28263 2023-04-19 04:06:10.275214 inkscape_figure_manager-0.0.4/Pipfile.lock
+-rw-r--r--   0        0        0     1038 2023-04-15 21:12:40.220852 inkscape_figure_manager-0.0.4/README.md
+-rw-r--r--   0        0        0      709 2023-06-06 19:29:51.936382 inkscape_figure_manager-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/__init__.py
+-rw-r--r--   0        0        0     7777 2023-06-06 19:20:41.239737 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/__main__.py
+-rw-r--r--   0        0        0     4022 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/daemon.py
+-rw-r--r--   0        0        0     1427 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/picker.py
+-rw-r--r--   0        0        0     1989 2023-04-19 20:08:36.387298 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/template.svg
+-rw-r--r--   0        0        0     3354 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/watcher.py
+-rw-r--r--   0        0        0     2504 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/watcher_daemon.py
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 inkscape_figure_manager-0.0.4/PKG-INFO
```

### Comparing `inkscape_figure_manager-0.0.3/LICENSE` & `inkscape_figure_manager-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.3/Pipfile.lock` & `inkscape_figure_manager-0.0.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.3/README.md` & `inkscape_figure_manager-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.3/pyproject.toml` & `inkscape_figure_manager-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = 'inkscape_figure_manager'
-version = '0.0.3'
+version = '0.0.4'
 authors = [
   { name="Silas Waxter" },
   { name="Gille Castel" },
 ]
 description = "An API for managing inkscape figures."
 readme = "README.md"
 classifiers = [
```

### Comparing `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/__main__.py` & `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from inkscape_figure_manager.watcher import EXPORT_EXTENSTION_NO_DOT, Watcher
 from inkscape_figure_manager.watcher_daemon import WatcherDaemon
 
 APPLICATION_NAME = "inkscape-figure-manager"
 # os-agnostic path to current user's configuration directory for this
 # application
 APP_USER_CONFIG_DIR = Path(user_config_dir(APPLICATION_NAME, False))
-ROOT_FILE_PATH = APP_USER_CONFIG_DIR / 'roots'
 TEMPLATE_FILE_PATH = APP_USER_CONFIG_DIR / 'template.svg'
 # error codes:
 ERROR_CODE_CREATED_FILE_ALREADY_EXISTS = 1
 ERROR_CODE_EDITED_FILE_PATH_DOES_NOT_EXIST = 2
 ERROR_CODE_GIT_REPO_DNE = 3
 ERROR_CODE_BAD_DIR_TO_WATCH = 4
 
@@ -133,15 +132,14 @@
     if relative_from.is_relative_to(figure_dir):
         up_dir_steps = Path('')  # will contain multiple '..'
         while (relative_from / up_dir_steps).resolve() != figure_dir:
             up_dir_steps = up_dir_steps / '..'
         relative_path = up_dir_steps
     else:
         relative_path = figure_dir.relative_to(relative_from)
-        print(relative_path)
 
     relative_figure = relative_path / figure_file_name
     relative_figure_exported = relative_path / figure_file_name_exported
     absolute_figure = (relative_from / relative_figure).absolute()
 
     # Ensure figure does not exist
     if relative_figure.exists():
@@ -210,17 +208,14 @@
 def ensure_init():
     """
     Ensures the configuration directories and a figure template exist.
     """
     if not APP_USER_CONFIG_DIR.is_dir():
         APP_USER_CONFIG_DIR.mkdir()
 
-    if not ROOT_FILE_PATH.is_file():
-        ROOT_FILE_PATH.touch()
-
     # if template file does not exist, copy it from the template file in this
     # directory
     if not TEMPLATE_FILE_PATH.is_file():
         copy(str(Path(__file__).parent / 'template.svg'),
              str(TEMPLATE_FILE_PATH))
```

### Comparing `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/daemon.py` & `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/daemon.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/picker.py` & `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/picker.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/template.svg` & `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/template.svg`

 * *Files 8% similar despite different names*

```diff
@@ -1,119 +1,125 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
 00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
 00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
 00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
 00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
-00000070: 0a0a 3c73 7667 0a20 2020 786d 6c6e 733a  ..<svg.   xmlns:
-00000080: 6463 3d22 6874 7470 3a2f 2f70 7572 6c2e  dc="http://purl.
-00000090: 6f72 672f 6463 2f65 6c65 6d65 6e74 732f  org/dc/elements/
-000000a0: 312e 312f 220a 2020 2078 6d6c 6e73 3a63  1.1/".   xmlns:c
-000000b0: 633d 2268 7474 703a 2f2f 6372 6561 7469  c="http://creati
-000000c0: 7665 636f 6d6d 6f6e 732e 6f72 672f 6e73  vecommons.org/ns
-000000d0: 2322 0a20 2020 786d 6c6e 733a 7264 663d  #".   xmlns:rdf=
-000000e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
-000000f0: 7267 2f31 3939 392f 3032 2f32 322d 7264  rg/1999/02/22-rd
-00000100: 662d 7379 6e74 6178 2d6e 7323 220a 2020  f-syntax-ns#".  
-00000110: 2078 6d6c 6e73 3a73 7667 3d22 6874 7470   xmlns:svg="http
-00000120: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
-00000130: 3030 2f73 7667 220a 2020 2078 6d6c 6e73  00/svg".   xmlns
-00000140: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-00000150: 6f72 672f 3230 3030 2f73 7667 220a 2020  org/2000/svg".  
-00000160: 2078 6d6c 6e73 3a73 6f64 6970 6f64 693d   xmlns:sodipodi=
-00000170: 2268 7474 703a 2f2f 736f 6469 706f 6469  "http://sodipodi
-00000180: 2e73 6f75 7263 6566 6f72 6765 2e6e 6574  .sourceforge.net
-00000190: 2f44 5444 2f73 6f64 6970 6f64 692d 302e  /DTD/sodipodi-0.
-000001a0: 6474 6422 0a20 2020 786d 6c6e 733a 696e  dtd".   xmlns:in
-000001b0: 6b73 6361 7065 3d22 6874 7470 3a2f 2f77  kscape="http://w
-000001c0: 7777 2e69 6e6b 7363 6170 652e 6f72 672f  ww.inkscape.org/
-000001d0: 6e61 6d65 7370 6163 6573 2f69 6e6b 7363  namespaces/inksc
-000001e0: 6170 6522 0a20 2020 7769 6474 683d 2232  ape".   width="2
-000001f0: 3430 6d6d 220a 2020 2068 6569 6768 743d  40mm".   height=
-00000200: 2231 3230 6d6d 220a 2020 2076 6965 7742  "120mm".   viewB
-00000210: 6f78 3d22 3020 3020 3234 3020 3132 3022  ox="0 0 240 120"
-00000220: 0a20 2020 7665 7273 696f 6e3d 2231 2e31  .   version="1.1
-00000230: 220a 2020 2069 643d 2273 7667 3822 0a20  ".   id="svg8". 
-00000240: 2020 696e 6b73 6361 7065 3a76 6572 7369    inkscape:versi
-00000250: 6f6e 3d22 302e 3932 2e34 2028 756e 6b6e  on="0.92.4 (unkn
-00000260: 6f77 6e29 220a 2020 2073 6f64 6970 6f64  own)".   sodipod
-00000270: 693a 646f 636e 616d 653d 2266 6967 7572  i:docname="figur
-00000280: 652e 7376 6722 3e0a 2020 3c64 6566 730a  e.svg">.  <defs.
-00000290: 2020 2020 2069 643d 2264 6566 7332 2220       id="defs2" 
-000002a0: 2f3e 0a20 203c 736f 6469 706f 6469 3a6e  />.  <sodipodi:n
-000002b0: 616d 6564 7669 6577 0a20 2020 2020 6964  amedview.     id
-000002c0: 3d22 6261 7365 220a 2020 2020 2070 6167  ="base".     pag
-000002d0: 6563 6f6c 6f72 3d22 2366 6666 6666 6622  ecolor="#ffffff"
-000002e0: 0a20 2020 2020 626f 7264 6572 636f 6c6f  .     bordercolo
-000002f0: 723d 2223 3636 3636 3636 220a 2020 2020  r="#666666".    
-00000300: 2062 6f72 6465 726f 7061 6369 7479 3d22   borderopacity="
-00000310: 312e 3022 0a20 2020 2020 696e 6b73 6361  1.0".     inksca
-00000320: 7065 3a70 6167 656f 7061 6369 7479 3d22  pe:pageopacity="
-00000330: 302e 3022 0a20 2020 2020 696e 6b73 6361  0.0".     inksca
-00000340: 7065 3a70 6167 6573 6861 646f 773d 2232  pe:pageshadow="2
-00000350: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-00000360: 7a6f 6f6d 3d22 302e 3939 3433 3733 3838  zoom="0.99437388
-00000370: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-00000380: 6378 3d22 3238 342e 3237 3632 3722 0a20  cx="284.27627". 
-00000390: 2020 2020 696e 6b73 6361 7065 3a63 793d      inkscape:cy=
-000003a0: 2231 3832 2e37 3230 3535 220a 2020 2020  "182.72055".    
-000003b0: 2069 6e6b 7363 6170 653a 646f 6375 6d65   inkscape:docume
-000003c0: 6e74 2d75 6e69 7473 3d22 6d6d 220a 2020  nt-units="mm".  
-000003d0: 2020 2069 6e6b 7363 6170 653a 6375 7272     inkscape:curr
-000003e0: 656e 742d 6c61 7965 723d 226c 6179 6572  ent-layer="layer
-000003f0: 3122 0a20 2020 2020 7368 6f77 6772 6964  1".     showgrid
-00000400: 3d22 6661 6c73 6522 0a20 2020 2020 7368  ="false".     sh
-00000410: 6f77 626f 7264 6572 3d22 7472 7565 220a  owborder="true".
-00000420: 2020 2020 2077 6964 7468 3d22 3230 306d       width="200m
-00000430: 6d22 0a20 2020 2020 7368 6f77 6775 6964  m".     showguid
-00000440: 6573 3d22 7472 7565 220a 2020 2020 2069  es="true".     i
-00000450: 6e6b 7363 6170 653a 6775 6964 652d 6262  nkscape:guide-bb
-00000460: 6f78 3d22 7472 7565 220a 2020 2020 2069  ox="true".     i
-00000470: 6e6b 7363 6170 653a 7769 6e64 6f77 2d77  nkscape:window-w
-00000480: 6964 7468 3d22 3235 3230 220a 2020 2020  idth="2520".    
-00000490: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
-000004a0: 2d68 6569 6768 743d 2239 3935 220a 2020  -height="995".  
-000004b0: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
-000004c0: 6f77 2d78 3d22 3230 220a 2020 2020 2069  ow-x="20".     i
-000004d0: 6e6b 7363 6170 653a 7769 6e64 6f77 2d79  nkscape:window-y
-000004e0: 3d22 3635 220a 2020 2020 2069 6e6b 7363  ="65".     inksc
-000004f0: 6170 653a 7769 6e64 6f77 2d6d 6178 696d  ape:window-maxim
-00000500: 697a 6564 3d22 3122 3e0a 2020 2020 3c69  ized="1">.    <i
-00000510: 6e6b 7363 6170 653a 6772 6964 0a20 2020  nkscape:grid.   
-00000520: 2020 2020 7479 7065 3d22 7879 6772 6964      type="xygrid
-00000530: 220a 2020 2020 2020 2069 643d 2267 7269  ".       id="gri
-00000540: 6438 3135 220a 2020 2020 2020 2075 6e69  d815".       uni
-00000550: 7473 3d22 6d6d 220a 2020 2020 2020 2073  ts="mm".       s
-00000560: 7061 6369 6e67 783d 2231 3022 0a20 2020  pacingx="10".   
-00000570: 2020 2020 7370 6163 696e 6779 3d22 3130      spacingy="10
-00000580: 220a 2020 2020 2020 2065 6d70 7370 6163  ".       empspac
-00000590: 696e 673d 2234 220a 2020 2020 2020 2064  ing="4".       d
-000005a0: 6f74 7465 643d 2266 616c 7365 2220 2f3e  otted="false" />
-000005b0: 0a20 203c 2f73 6f64 6970 6f64 693a 6e61  .  </sodipodi:na
-000005c0: 6d65 6476 6965 773e 0a20 203c 6d65 7461  medview>.  <meta
-000005d0: 6461 7461 0a20 2020 2020 6964 3d22 6d65  data.     id="me
-000005e0: 7461 6461 7461 3522 3e0a 2020 2020 3c72  tadata5">.    <r
-000005f0: 6466 3a52 4446 3e0a 2020 2020 2020 3c63  df:RDF>.      <c
-00000600: 633a 576f 726b 0a20 2020 2020 2020 2020  c:Work.         
-00000610: 7264 663a 6162 6f75 743d 2222 3e0a 2020  rdf:about="">.  
-00000620: 2020 2020 2020 3c64 633a 666f 726d 6174        <dc:format
-00000630: 3e69 6d61 6765 2f73 7667 2b78 6d6c 3c2f  >image/svg+xml</
-00000640: 6463 3a66 6f72 6d61 743e 0a20 2020 2020  dc:format>.     
-00000650: 2020 203c 6463 3a74 7970 650a 2020 2020     <dc:type.    
-00000660: 2020 2020 2020 2072 6466 3a72 6573 6f75         rdf:resou
-00000670: 7263 653d 2268 7474 703a 2f2f 7075 726c  rce="http://purl
-00000680: 2e6f 7267 2f64 632f 6463 6d69 7479 7065  .org/dc/dcmitype
-00000690: 2f53 7469 6c6c 496d 6167 6522 202f 3e0a  /StillImage" />.
-000006a0: 2020 2020 2020 2020 3c64 633a 7469 746c          <dc:titl
-000006b0: 6520 2f3e 0a20 2020 2020 203c 2f63 633a  e />.      </cc:
-000006c0: 576f 726b 3e0a 2020 2020 3c2f 7264 663a  Work>.    </rdf:
-000006d0: 5244 463e 0a20 203c 2f6d 6574 6164 6174  RDF>.  </metadat
-000006e0: 613e 0a20 203c 670a 2020 2020 2069 6e6b  a>.  <g.     ink
-000006f0: 7363 6170 653a 6c61 6265 6c3d 224c 6179  scape:label="Lay
-00000700: 6572 2031 220a 2020 2020 2069 6e6b 7363  er 1".     inksc
-00000710: 6170 653a 6772 6f75 706d 6f64 653d 226c  ape:groupmode="l
-00000720: 6179 6572 220a 2020 2020 2069 643d 226c  ayer".     id="l
-00000730: 6179 6572 3122 0a20 2020 2020 7472 616e  ayer1".     tran
-00000740: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-00000750: 2830 2c2d 3137 3729 2220 2f3e 0a3c 2f73  (0,-177)" />.</s
-00000760: 7667 3e0a                                vg>.
+00000070: 0a0a 3c73 7667 0a20 2020 7769 6474 683d  ..<svg.   width=
+00000080: 2232 3430 6d6d 220a 2020 2068 6569 6768  "240mm".   heigh
+00000090: 743d 2231 3230 6d6d 220a 2020 2076 6965  t="120mm".   vie
+000000a0: 7742 6f78 3d22 3020 3020 3234 3020 3132  wBox="0 0 240 12
+000000b0: 3022 0a20 2020 7665 7273 696f 6e3d 2231  0".   version="1
+000000c0: 2e31 220a 2020 2069 643d 2273 7667 3822  .1".   id="svg8"
+000000d0: 0a20 2020 696e 6b73 6361 7065 3a76 6572  .   inkscape:ver
+000000e0: 7369 6f6e 3d22 312e 322e 3220 2862 3061  sion="1.2.2 (b0a
+000000f0: 3834 3836 3534 312c 2032 3032 322d 3132  8486541, 2022-12
+00000100: 2d30 3129 220a 2020 2073 6f64 6970 6f64  -01)".   sodipod
+00000110: 693a 646f 636e 616d 653d 2274 656d 706c  i:docname="templ
+00000120: 6174 652e 7376 6722 0a20 2020 786d 6c6e  ate.svg".   xmln
+00000130: 733a 696e 6b73 6361 7065 3d22 6874 7470  s:inkscape="http
+00000140: 3a2f 2f77 7777 2e69 6e6b 7363 6170 652e  ://www.inkscape.
+00000150: 6f72 672f 6e61 6d65 7370 6163 6573 2f69  org/namespaces/i
+00000160: 6e6b 7363 6170 6522 0a20 2020 786d 6c6e  nkscape".   xmln
+00000170: 733a 736f 6469 706f 6469 3d22 6874 7470  s:sodipodi="http
+00000180: 3a2f 2f73 6f64 6970 6f64 692e 736f 7572  ://sodipodi.sour
+00000190: 6365 666f 7267 652e 6e65 742f 4454 442f  ceforge.net/DTD/
+000001a0: 736f 6469 706f 6469 2d30 2e64 7464 220a  sodipodi-0.dtd".
+000001b0: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
+000001c0: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
+000001d0: 2f73 7667 220a 2020 2078 6d6c 6e73 3a73  /svg".   xmlns:s
+000001e0: 7667 3d22 6874 7470 3a2f 2f77 7777 2e77  vg="http://www.w
+000001f0: 332e 6f72 672f 3230 3030 2f73 7667 220a  3.org/2000/svg".
+00000200: 2020 2078 6d6c 6e73 3a72 6466 3d22 6874     xmlns:rdf="ht
+00000210: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000220: 3139 3939 2f30 322f 3232 2d72 6466 2d73  1999/02/22-rdf-s
+00000230: 796e 7461 782d 6e73 2322 0a20 2020 786d  yntax-ns#".   xm
+00000240: 6c6e 733a 6363 3d22 6874 7470 3a2f 2f63  lns:cc="http://c
+00000250: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
+00000260: 7267 2f6e 7323 220a 2020 2078 6d6c 6e73  rg/ns#".   xmlns
+00000270: 3a64 633d 2268 7474 703a 2f2f 7075 726c  :dc="http://purl
+00000280: 2e6f 7267 2f64 632f 656c 656d 656e 7473  .org/dc/elements
+00000290: 2f31 2e31 2f22 3e0a 2020 3c64 6566 730a  /1.1/">.  <defs.
+000002a0: 2020 2020 2069 643d 2264 6566 7332 2220       id="defs2" 
+000002b0: 2f3e 0a20 203c 736f 6469 706f 6469 3a6e  />.  <sodipodi:n
+000002c0: 616d 6564 7669 6577 0a20 2020 2020 6964  amedview.     id
+000002d0: 3d22 6261 7365 220a 2020 2020 2070 6167  ="base".     pag
+000002e0: 6563 6f6c 6f72 3d22 2366 6666 6666 6622  ecolor="#ffffff"
+000002f0: 0a20 2020 2020 626f 7264 6572 636f 6c6f  .     bordercolo
+00000300: 723d 2223 3636 3636 3636 220a 2020 2020  r="#666666".    
+00000310: 2062 6f72 6465 726f 7061 6369 7479 3d22   borderopacity="
+00000320: 312e 3022 0a20 2020 2020 696e 6b73 6361  1.0".     inksca
+00000330: 7065 3a70 6167 656f 7061 6369 7479 3d22  pe:pageopacity="
+00000340: 3122 0a20 2020 2020 696e 6b73 6361 7065  1".     inkscape
+00000350: 3a70 6167 6573 6861 646f 773d 2232 220a  :pageshadow="2".
+00000360: 2020 2020 2069 6e6b 7363 6170 653a 7a6f       inkscape:zo
+00000370: 6f6d 3d22 302e 3939 3433 3733 3838 220a  om="0.99437388".
+00000380: 2020 2020 2069 6e6b 7363 6170 653a 6378       inkscape:cx
+00000390: 3d22 3238 342e 3630 3132 220a 2020 2020  ="284.6012".    
+000003a0: 2069 6e6b 7363 6170 653a 6379 3d22 3138   inkscape:cy="18
+000003b0: 332e 3032 3937 3522 0a20 2020 2020 696e  3.02975".     in
+000003c0: 6b73 6361 7065 3a64 6f63 756d 656e 742d  kscape:document-
+000003d0: 756e 6974 733d 226d 6d22 0a20 2020 2020  units="mm".     
+000003e0: 696e 6b73 6361 7065 3a63 7572 7265 6e74  inkscape:current
+000003f0: 2d6c 6179 6572 3d22 6c61 7965 7231 220a  -layer="layer1".
+00000400: 2020 2020 2073 686f 7767 7269 643d 2266       showgrid="f
+00000410: 616c 7365 220a 2020 2020 2073 686f 7762  alse".     showb
+00000420: 6f72 6465 723d 2274 7275 6522 0a20 2020  order="true".   
+00000430: 2020 7769 6474 683d 2232 3030 6d6d 220a    width="200mm".
+00000440: 2020 2020 2073 686f 7767 7569 6465 733d       showguides=
+00000450: 2274 7275 6522 0a20 2020 2020 696e 6b73  "true".     inks
+00000460: 6361 7065 3a67 7569 6465 2d62 626f 783d  cape:guide-bbox=
+00000470: 2274 7275 6522 0a20 2020 2020 696e 6b73  "true".     inks
+00000480: 6361 7065 3a77 696e 646f 772d 7769 6474  cape:window-widt
+00000490: 683d 2231 3731 3822 0a20 2020 2020 696e  h="1718".     in
+000004a0: 6b73 6361 7065 3a77 696e 646f 772d 6865  kscape:window-he
+000004b0: 6967 6874 3d22 3134 3036 220a 2020 2020  ight="1406".    
+000004c0: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
+000004d0: 2d78 3d22 3336 3430 220a 2020 2020 2069  -x="3640".     i
+000004e0: 6e6b 7363 6170 653a 7769 6e64 6f77 2d79  nkscape:window-y
+000004f0: 3d22 3332 220a 2020 2020 2069 6e6b 7363  ="32".     inksc
+00000500: 6170 653a 7769 6e64 6f77 2d6d 6178 696d  ape:window-maxim
+00000510: 697a 6564 3d22 3122 0a20 2020 2020 696e  ized="1".     in
+00000520: 6b73 6361 7065 3a73 686f 7770 6167 6573  kscape:showpages
+00000530: 6861 646f 773d 2232 220a 2020 2020 2069  hadow="2".     i
+00000540: 6e6b 7363 6170 653a 7061 6765 6368 6563  nkscape:pagechec
+00000550: 6b65 7262 6f61 7264 3d22 3022 0a20 2020  kerboard="0".   
+00000560: 2020 696e 6b73 6361 7065 3a64 6573 6b63    inkscape:deskc
+00000570: 6f6c 6f72 3d22 2364 3164 3164 3122 3e0a  olor="#d1d1d1">.
+00000580: 2020 2020 3c69 6e6b 7363 6170 653a 6772      <inkscape:gr
+00000590: 6964 0a20 2020 2020 2020 7479 7065 3d22  id.       type="
+000005a0: 7879 6772 6964 220a 2020 2020 2020 2069  xygrid".       i
+000005b0: 643d 2267 7269 6438 3135 220a 2020 2020  d="grid815".    
+000005c0: 2020 2075 6e69 7473 3d22 6d6d 220a 2020     units="mm".  
+000005d0: 2020 2020 2073 7061 6369 6e67 783d 2231       spacingx="1
+000005e0: 3022 0a20 2020 2020 2020 7370 6163 696e  0".       spacin
+000005f0: 6779 3d22 3130 220a 2020 2020 2020 2065  gy="10".       e
+00000600: 6d70 7370 6163 696e 673d 2234 220a 2020  mpspacing="4".  
+00000610: 2020 2020 2064 6f74 7465 643d 2266 616c       dotted="fal
+00000620: 7365 2220 2f3e 0a20 203c 2f73 6f64 6970  se" />.  </sodip
+00000630: 6f64 693a 6e61 6d65 6476 6965 773e 0a20  odi:namedview>. 
+00000640: 203c 6d65 7461 6461 7461 0a20 2020 2020   <metadata.     
+00000650: 6964 3d22 6d65 7461 6461 7461 3522 3e0a  id="metadata5">.
+00000660: 2020 2020 3c72 6466 3a52 4446 3e0a 2020      <rdf:RDF>.  
+00000670: 2020 2020 3c63 633a 576f 726b 0a20 2020      <cc:Work.   
+00000680: 2020 2020 2020 7264 663a 6162 6f75 743d        rdf:about=
+00000690: 2222 3e0a 2020 2020 2020 2020 3c64 633a  "">.        <dc:
+000006a0: 666f 726d 6174 3e69 6d61 6765 2f73 7667  format>image/svg
+000006b0: 2b78 6d6c 3c2f 6463 3a66 6f72 6d61 743e  +xml</dc:format>
+000006c0: 0a20 2020 2020 2020 203c 6463 3a74 7970  .        <dc:typ
+000006d0: 650a 2020 2020 2020 2020 2020 2072 6466  e.           rdf
+000006e0: 3a72 6573 6f75 7263 653d 2268 7474 703a  :resource="http:
+000006f0: 2f2f 7075 726c 2e6f 7267 2f64 632f 6463  //purl.org/dc/dc
+00000700: 6d69 7479 7065 2f53 7469 6c6c 496d 6167  mitype/StillImag
+00000710: 6522 202f 3e0a 2020 2020 2020 3c2f 6363  e" />.      </cc
+00000720: 3a57 6f72 6b3e 0a20 2020 203c 2f72 6466  :Work>.    </rdf
+00000730: 3a52 4446 3e0a 2020 3c2f 6d65 7461 6461  :RDF>.  </metada
+00000740: 7461 3e0a 2020 3c67 0a20 2020 2020 696e  ta>.  <g.     in
+00000750: 6b73 6361 7065 3a6c 6162 656c 3d22 4c61  kscape:label="La
+00000760: 7965 7220 3122 0a20 2020 2020 696e 6b73  yer 1".     inks
+00000770: 6361 7065 3a67 726f 7570 6d6f 6465 3d22  cape:groupmode="
+00000780: 6c61 7965 7222 0a20 2020 2020 6964 3d22  layer".     id="
+00000790: 6c61 7965 7231 220a 2020 2020 2074 7261  layer1".     tra
+000007a0: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+000007b0: 6528 302c 2d31 3737 2922 202f 3e0a 3c2f  e(0,-177)" />.</
+000007c0: 7376 673e 0a                             svg>.
```

### Comparing `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/watcher.py` & `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/watcher.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/watcher_daemon.py` & `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/watcher_daemon.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.3/PKG-INFO` & `inkscape_figure_manager-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkscape_figure_manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: An API for managing inkscape figures.
 Author: Silas Waxter, Gille Castel
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Dist: click
 Requires-Dist: appdirs
```

