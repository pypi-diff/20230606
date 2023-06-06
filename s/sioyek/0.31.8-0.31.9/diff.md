# Comparing `tmp/sioyek-0.31.8.tar.gz` & `tmp/sioyek-0.31.9.tar.gz`

## Comparing `sioyek-0.31.8.tar` & `sioyek-0.31.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sioyek-0.31.8/src/sioyek/__init__.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 sioyek-0.31.8/src/sioyek/add_text.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 sioyek-0.31.8/src/sioyek/dual_panelify.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 sioyek-0.31.8/src/sioyek/embed_annotations.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 sioyek-0.31.8/src/sioyek/extract_highlights.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 sioyek-0.31.8/src/sioyek/import_annotations.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 sioyek-0.31.8/src/sioyek/paper_downloader.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 sioyek-0.31.8/src/sioyek/remove_annotation.py
--rw-r--r--   0        0        0    45702 2020-02-02 00:00:00.000000 sioyek-0.31.8/src/sioyek/sioyek.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 sioyek-0.31.8/src/sioyek/translate.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sioyek-0.31.8/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sioyek-0.31.8/LICENSE.txt
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 sioyek-0.31.8/README.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sioyek-0.31.8/pyproject.toml
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 sioyek-0.31.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sioyek-0.31.9/src/sioyek/__init__.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 sioyek-0.31.9/src/sioyek/add_text.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 sioyek-0.31.9/src/sioyek/dual_panelify.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 sioyek-0.31.9/src/sioyek/embed_annotations.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 sioyek-0.31.9/src/sioyek/extract_highlights.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 sioyek-0.31.9/src/sioyek/import_annotations.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 sioyek-0.31.9/src/sioyek/paper_downloader.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 sioyek-0.31.9/src/sioyek/remove_annotation.py
+-rw-r--r--   0        0        0    45702 2020-02-02 00:00:00.000000 sioyek-0.31.9/src/sioyek/sioyek.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 sioyek-0.31.9/src/sioyek/translate.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sioyek-0.31.9/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sioyek-0.31.9/LICENSE.txt
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 sioyek-0.31.9/README.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sioyek-0.31.9/pyproject.toml
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 sioyek-0.31.9/PKG-INFO
```

### Comparing `sioyek-0.31.8/src/sioyek/add_text.py` & `sioyek-0.31.9/src/sioyek/add_text.py`

 * *Files identical despite different names*

### Comparing `sioyek-0.31.8/src/sioyek/dual_panelify.py` & `sioyek-0.31.9/src/sioyek/dual_panelify.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import datetime
 import fitz
 from copy import copy
 import numpy as np
 
 from .sioyek import Sioyek, clean_path
 
-from PyPDF2 import PdfWriter, PdfReader, PageObject
+from PyPDF2 import PdfWriter, PdfReader, PageObject, Transformation
 
 UPDATE_EVERY_SECONDS = 3
 SIDE_MARGIN = 25
 MIDDLE_MARGIN = 25
 sioyek = None
 
 def first_and_last_nonzero(arr):
@@ -102,49 +102,52 @@
 
     pdf_reader = PdfReader(single_panel_file_path)
     pdf_writer = PdfWriter()
 
     doc = fitz.open(single_panel_file_path)
     cropbox = get_document_cropbox(doc)
 
-    for i in range(pdf_reader.numPages // 2):
+    for i in range(len(pdf_reader.pages) // 2):
         if (datetime.datetime.now() - last_update_time).seconds > UPDATE_EVERY_SECONDS:
             last_update_time = datetime.datetime.now()
             # subprocess.run([sioyek_path, '--execute-command', 'set_status_string', '--execute-command-data', 'Dual panelifying {} / {}'.format((i+1) * 2, pdf_reader.numPages)])
-            sioyek.set_status_string('Dual panelifying {} / {}'.format((i+1) * 2, pdf_reader.numPages))
+            sioyek.set_status_string('Dual panelifying {} / {}'.format((i+1) * 2, len(pdf_reader.pages)))
 
-        page1 = copy(pdf_reader.getPage(2 * i))
-        page2 = copy(pdf_reader.getPage(2 * i+1))
+        page1 = copy(pdf_reader.pages[2 * i])
+        page2 = copy(pdf_reader.pages[2 * i+1])
 
-        original_width1 = page1.mediaBox.width
-        original_width2 = page2.mediaBox.width
+        original_width1 = page1.mediabox.width
+        original_width2 = page2.mediabox.width
 
-        page1.mediaBox.setLowerLeft(cropbox.bottom_left)
-        page1.mediaBox.setUpperRight(cropbox.top_right)
-        page2.mediaBox.setLowerLeft(cropbox.bottom_left)
-        page2.mediaBox.setUpperRight(cropbox.top_right)
-
-        page1.cropBox.setLowerLeft(cropbox.bottom_left)
-        page1.cropBox.setUpperRight(cropbox.top_right)
-        page2.cropBox.setLowerLeft(cropbox.bottom_left)
-        page2.cropBox.setUpperRight(cropbox.top_right)
+        llx = page1.cropbox.lower_right[0]
+        lly = page1.cropbox.lower_right[1]
+        page2.cropbox.lower_left = (llx, lly)
+
+        urx = page1.cropbox.lower_right[0] + page2.cropbox.lower_right[0]
+        ury = page2.cropbox.upper_right[1]
+        page2.cropbox.upper_right = (urx, ury)
 
 
         # total_width = original_width1 + original_width2
-        total_width = page1.mediaBox.width + page2.mediaBox.width + 2 * SIDE_MARGIN + MIDDLE_MARGIN
-        total_height = -max([page1.mediaBox.height, page2.mediaBox.height])
-        new_page = PageObject.createBlankPage(None, total_width, total_height)
-        # new_page.mergePage(page1)
-        new_page.mergeTranslatedPage(page1, -page1.mediaBox.left + SIDE_MARGIN, 0)
-        new_page.mergeTranslatedPage(page2, page1.mediaBox.width - page1.mediaBox.left + SIDE_MARGIN + MIDDLE_MARGIN, 0)
-        # new_page.mergeTranslatedPage(page2, page1.mediaBox.width - 200, 0)
+        total_width = page1.mediabox.width + page2.mediabox.width + 2 * SIDE_MARGIN + MIDDLE_MARGIN
+        total_height = max([page1.mediabox.height, page2.mediabox.height])
+        new_page = PageObject.create_blank_page(None, total_width, total_height)
+
+        # new_page.mergeTranslatedPage(page1, -page1.mediabox.left + SIDE_MARGIN, 0)
+        page1.add_transformation(Transformation().translate( SIDE_MARGIN, 0))
+        new_page.merge_page(page1)
+
+        # new_page.mergeTranslatedPage(page2, page1.mediabox.width - page1.mediabox.left + SIDE_MARGIN + MIDDLE_MARGIN, 0)
+        page2.add_transformation(Transformation().translate(page1.mediabox.width + SIDE_MARGIN + MIDDLE_MARGIN, 0))
+        new_page.merge_page(page2)
+
         pdf_writer.add_page(new_page)
     
-    if pdf_reader.numPages % 2 == 1:
-        pdf_writer.add_page(pdf_reader.getPage(pdf_reader.numPages - 1))
+    if len(pdf_reader.pages) % 2 == 1:
+        pdf_writer.add_page(pdf_reader.pages[len(pdf_reader.pages) - 1])
 
     sioyek.set_status_string('Writing new file to disk')
     with open(dual_panel_file_path, 'wb') as f:
         pdf_writer.write(f)
 
     sioyek.clear_status_string()
     subprocess.run([sioyek_path, '--new-window', dual_panel_file_path])
```

### Comparing `sioyek-0.31.8/src/sioyek/embed_annotations.py` & `sioyek-0.31.9/src/sioyek/embed_annotations.py`

 * *Files identical despite different names*

### Comparing `sioyek-0.31.8/src/sioyek/extract_highlights.py` & `sioyek-0.31.9/src/sioyek/extract_highlights.py`

 * *Files identical despite different names*

### Comparing `sioyek-0.31.8/src/sioyek/import_annotations.py` & `sioyek-0.31.9/src/sioyek/import_annotations.py`

 * *Files identical despite different names*

### Comparing `sioyek-0.31.8/src/sioyek/paper_downloader.py` & `sioyek-0.31.9/src/sioyek/paper_downloader.py`

 * *Files identical despite different names*

### Comparing `sioyek-0.31.8/src/sioyek/remove_annotation.py` & `sioyek-0.31.9/src/sioyek/remove_annotation.py`

 * *Files identical despite different names*

### Comparing `sioyek-0.31.8/src/sioyek/sioyek.py` & `sioyek-0.31.9/src/sioyek/sioyek.py`

 * *Files identical despite different names*

### Comparing `sioyek-0.31.8/LICENSE.txt` & `sioyek-0.31.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sioyek-0.31.8/pyproject.toml` & `sioyek-0.31.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sioyek"
-version = "0.31.8"
+version = "0.31.9"
 authors = [
   { name="Ali Mostafavi", email="a.hr.mostafavi@gmail.com" },
 ]
 description = "Python tools and extensions for sioyek PDF reader"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sioyek-0.31.8/PKG-INFO` & `sioyek-0.31.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7369 6f79  : 2.1.Name: sioy
 00000020: 656b 0a56 6572 7369 6f6e 3a20 302e 3331  ek.Version: 0.31
-00000030: 2e38 0a53 756d 6d61 7279 3a20 5079 7468  .8.Summary: Pyth
+00000030: 2e39 0a53 756d 6d61 7279 3a20 5079 7468  .9.Summary: Pyth
 00000040: 6f6e 2074 6f6f 6c73 2061 6e64 2065 7874  on tools and ext
 00000050: 656e 7369 6f6e 7320 666f 7220 7369 6f79  ensions for sioy
 00000060: 656b 2050 4446 2072 6561 6465 720a 5072  ek PDF reader.Pr
 00000070: 6f6a 6563 742d 5552 4c3a 2048 6f6d 6570  oject-URL: Homep
 00000080: 6167 652c 2068 7474 7073 3a2f 2f67 6974  age, https://git
 00000090: 6875 622e 636f 6d2f 6168 726d 2f73 696f  hub.com/ahrm/sio
 000000a0: 7965 6b2d 7079 7468 6f6e 2d65 7874 656e  yek-python-exten
@@ -200,35 +200,111 @@
 00000c70: 6563 7465 645f 7465 7874 7d22 0a6e 6577  ected_text}".new
 00000c80: 5f63 6f6d 6d61 6e64 205f 7472 616e 736c  _command _transl
 00000c90: 6174 655f 6375 7272 656e 745f 6c69 6e65  ate_current_line
 00000ca0: 5f74 6578 7420 7079 7468 6f6e 202d 6d20  _text python -m 
 00000cb0: 7369 6f79 656b 2e74 7261 6e73 6c61 7465  sioyek.translate
 00000cc0: 2022 257b 7369 6f79 656b 5f70 6174 687d   "%{sioyek_path}
 00000cd0: 2220 2225 7b6c 696e 655f 7465 7874 7d22  " "%{line_text}"
-00000ce0: 0a60 6060 0a0a 2323 2055 7365 7220 5363  .```..## User Sc
-00000cf0: 7269 7074 730a 4865 7265 2069 7320 6120  ripts.Here is a 
-00000d00: 6c69 7374 206f 6620 7363 7269 7074 7320  list of scripts 
-00000d10: 6372 6561 7465 6420 6279 2073 696f 7965  created by sioye
-00000d20: 6b20 7573 6572 733a 0a2a 2041 2073 6372  k users:.* A scr
-00000d30: 6970 7420 746f 2069 6d70 6f72 7420 616e  ipt to import an
-00000d40: 6e6f 7461 7469 6f6e 7320 666f 7220 6b6f  notations for ko
-00000d50: 7265 6164 6572 3a20 6874 7470 733a 2f2f  reader: https://
-00000d60: 6769 7468 7562 2e63 6f6d 2f62 6c6f 6234  github.com/blob4
-00000d70: 322f 6b6f 7265 6164 6572 2d73 696f 7965  2/koreader-sioye
-00000d80: 6b2d 696d 706f 7274 0a0a 2323 2044 6f6e  k-import..## Don
-00000d90: 6174 696f 6e0a 4966 2079 6f75 2065 6e6a  ation.If you enj
-00000da0: 6f79 2073 696f 7965 6b2c 2070 6c65 6173  oy sioyek, pleas
-00000db0: 6520 636f 6e73 6964 6572 2064 6f6e 6174  e consider donat
-00000dc0: 696e 6720 746f 2073 7570 706f 7274 2069  ing to support i
-00000dd0: 7473 2064 6576 656c 6f70 6d65 6e74 2e0a  ts development..
-00000de0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00000df0: 2f2f 7777 772e 6275 796d 6561 636f 6666  //www.buymeacoff
-00000e00: 6565 2e63 6f6d 2f61 6872 6d22 2074 6172  ee.com/ahrm" tar
-00000e10: 6765 743d 225f 626c 616e 6b22 3e3c 696d  get="_blank"><im
-00000e20: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
-00000e30: 646e 2e62 7579 6d65 6163 6f66 6665 652e  dn.buymeacoffee.
-00000e40: 636f 6d2f 6275 7474 6f6e 732f 6465 6661  com/buttons/defa
-00000e50: 756c 742d 6f72 616e 6765 2e70 6e67 2220  ult-orange.png" 
-00000e60: 616c 743d 2242 7579 204d 6520 4120 436f  alt="Buy Me A Co
-00000e70: 6666 6565 2220 6865 6967 6874 3d22 3431  ffee" height="41
-00000e80: 2220 7769 6474 683d 2231 3734 223e 3c2f  " width="174"></
-00000e90: 613e 0a                                  a>.
+00000ce0: 0a60 6060 0a0a 2323 2320 2d60 696d 706f  .```..### -`impo
+00000cf0: 7274 5f61 6e6e 6f74 6174 696f 6e73 600a  rt_annotations`.
+00000d00: 496d 706f 7274 2050 4446 2062 6f6f 6b6d  Import PDF bookm
+00000d10: 6172 6b73 2061 6e64 2068 6967 686c 6967  arks and highlig
+00000d20: 6874 7320 696e 746f 2073 696f 7965 6b20  hts into sioyek 
+00000d30: 736f 2074 6861 7420 7468 6579 2061 7265  so that they are
+00000d40: 2073 6561 7263 6861 626c 652e 0a0a 6874   searchable...ht
+00000d50: 7470 733a 2f2f 7573 6572 2d69 6d61 6765  tps://user-image
+00000d60: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
+00000d70: 656e 742e 636f 6d2f 3633 3932 3332 312f  ent.com/6392321/
+00000d80: 3230 3539 3330 3835 392d 3739 6235 6566  205930859-79b5ef
+00000d90: 6239 2d64 3135 392d 3464 3932 2d39 3338  b9-d159-4d92-938
+00000da0: 322d 3136 3431 6165 3363 6630 3164 2e6d  2-1641ae3cf01d.m
+00000db0: 7034 0a0a 436f 6e66 6967 3a0a 6060 600a  p4..Config:.```.
+00000dc0: 6e65 775f 636f 6d6d 616e 6420 5f69 6d70  new_command _imp
+00000dd0: 6f72 745f 616e 6e6f 7461 7469 6f6e 7320  ort_annotations 
+00000de0: 7079 7468 6f6e 202d 6d20 7369 6f79 656b  python -m sioyek
+00000df0: 2e69 6d70 6f72 745f 616e 6e6f 7461 7469  .import_annotati
+00000e00: 6f6e 7320 2225 7b73 696f 7965 6b5f 7061  ons "%{sioyek_pa
+00000e10: 7468 7d22 2022 257b 6c6f 6361 6c5f 6461  th}" "%{local_da
+00000e20: 7461 6261 7365 7d22 2022 257b 7368 6172  tabase}" "%{shar
+00000e30: 6564 5f64 6174 6162 6173 657d 2220 2225  ed_database}" "%
+00000e40: 7b66 696c 655f 7061 7468 7d22 0a60 6060  {file_path}".```
+00000e50: 0a0a 2323 2320 2d60 7265 6d6f 7665 5f61  ..### -`remove_a
+00000e60: 6e6e 6f74 6174 696f 6e60 0a52 656d 6f76  nnotation`.Remov
+00000e70: 6520 5044 4620 616e 6e6f 7461 7469 6f6e  e PDF annotation
+00000e80: 732e 0a0a 6874 7470 733a 2f2f 7573 6572  s...https://user
+00000e90: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+00000ea0: 6572 636f 6e74 656e 742e 636f 6d2f 3633  ercontent.com/63
+00000eb0: 3932 3332 312f 3230 3539 3331 3237 342d  92321/205931274-
+00000ec0: 6566 3262 3230 6535 2d30 6165 632d 3437  ef2b20e5-0aec-47
+00000ed0: 3863 2d39 6464 382d 6666 3833 6135 6261  8c-9dd8-ff83a5ba
+00000ee0: 3439 3862 2e6d 7034 0a0a 436f 6e66 6967  498b.mp4..Config
+00000ef0: 3a0a 6060 600a 6e65 775f 636f 6d6d 616e  :.```.new_comman
+00000f00: 6420 5f72 656d 6f76 655f 616e 6e6f 7461  d _remove_annota
+00000f10: 7469 6f6e 7320 7079 7468 6f6e 202d 6d20  tions python -m 
+00000f20: 7369 6f79 656b 2e72 656d 6f76 655f 616e  sioyek.remove_an
+00000f30: 6e6f 7461 7469 6f6e 2022 257b 7369 6f79  notation "%{sioy
+00000f40: 656b 5f70 6174 687d 2220 2225 7b6c 6f63  ek_path}" "%{loc
+00000f50: 616c 5f64 6174 6162 6173 657d 2220 2225  al_database}" "%
+00000f60: 7b73 6861 7265 645f 6461 7461 6261 7365  {shared_database
+00000f70: 7d22 2022 257b 6669 6c65 5f70 6174 687d  }" "%{file_path}
+00000f80: 2220 2225 7b73 656c 6563 7465 645f 7265  " "%{selected_re
+00000f90: 6374 7d22 0a60 6060 0a0a 2323 2320 2d60  ct}".```..### -`
+00000fa0: 6164 645f 7465 7874 600a 4164 6420 7465  add_text`.Add te
+00000fb0: 7874 2061 6e6e 6f74 6174 696f 6e20 746f  xt annotation to
+00000fc0: 2074 6865 2050 4446 2e0a 0a0a 0a68 7474   the PDF.....htt
+00000fd0: 7073 3a2f 2f75 7365 722d 696d 6167 6573  ps://user-images
+00000fe0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000ff0: 6e74 2e63 6f6d 2f36 3339 3233 3231 2f32  nt.com/6392321/2
+00001000: 3035 3933 3139 3338 2d39 3338 6461 3233  05931938-938da23
+00001010: 312d 3866 3263 2d34 6638 352d 3932 6133  1-8f2c-4f85-92a3
+00001020: 2d64 3761 6466 3332 3066 3566 322e 6d70  -d7adf320f5f2.mp
+00001030: 340a 0a0a 436f 6e66 6967 3a0a 6060 600a  4...Config:.```.
+00001040: 6e65 775f 636f 6d6d 616e 6420 5f61 6464  new_command _add
+00001050: 5f74 6578 7420 7079 7468 6f6e 202d 6d20  _text python -m 
+00001060: 7369 6f79 656b 2e61 6464 5f74 6578 7420  sioyek.add_text 
+00001070: 2225 7b73 696f 7965 6b5f 7061 7468 7d22  "%{sioyek_path}"
+00001080: 2022 257b 6c6f 6361 6c5f 6461 7461 6261   "%{local_databa
+00001090: 7365 7d22 2022 257b 7368 6172 6564 5f64  se}" "%{shared_d
+000010a0: 6174 6162 6173 657d 2220 2225 7b66 696c  atabase}" "%{fil
+000010b0: 655f 7061 7468 7d22 2022 257b 7365 6c65  e_path}" "%{sele
+000010c0: 6374 6564 5f72 6563 747d 2220 2225 7b63  cted_rect}" "%{c
+000010d0: 6f6d 6d61 6e64 5f74 6578 747d 220a 6e65  ommand_text}".ne
+000010e0: 775f 636f 6d6d 616e 6420 5f61 6464 5f72  w_command _add_r
+000010f0: 6564 5f74 6578 7420 7079 7468 6f6e 202d  ed_text python -
+00001100: 6d20 7369 6f79 656b 2e61 6464 5f74 6578  m sioyek.add_tex
+00001110: 7420 2225 7b73 696f 7965 6b5f 7061 7468  t "%{sioyek_path
+00001120: 7d22 2022 257b 6c6f 6361 6c5f 6461 7461  }" "%{local_data
+00001130: 6261 7365 7d22 2022 257b 7368 6172 6564  base}" "%{shared
+00001140: 5f64 6174 6162 6173 657d 2220 2225 7b66  _database}" "%{f
+00001150: 696c 655f 7061 7468 7d22 2022 257b 7365  ile_path}" "%{se
+00001160: 6c65 6374 6564 5f72 6563 747d 2220 2225  lected_rect}" "%
+00001170: 7b63 6f6d 6d61 6e64 5f74 6578 747d 2220  {command_text}" 
+00001180: 666f 6e74 7369 7a65 3d35 2074 6578 745f  fontsize=5 text_
+00001190: 636f 6c6f 723d 3235 352c 302c 300a 6060  color=255,0,0.``
+000011a0: 600a 0a0a 2323 2055 7365 7220 5363 7269  `...## User Scri
+000011b0: 7074 730a 4865 7265 2069 7320 6120 6c69  pts.Here is a li
+000011c0: 7374 206f 6620 7363 7269 7074 7320 6372  st of scripts cr
+000011d0: 6561 7465 6420 6279 2073 696f 7965 6b20  eated by sioyek 
+000011e0: 7573 6572 733a 0a2a 2041 2073 6372 6970  users:.* A scrip
+000011f0: 7420 746f 2069 6d70 6f72 7420 616e 6e6f  t to import anno
+00001200: 7461 7469 6f6e 7320 666f 7220 6b6f 7265  tations for kore
+00001210: 6164 6572 3a20 6874 7470 733a 2f2f 6769  ader: https://gi
+00001220: 7468 7562 2e63 6f6d 2f62 6c6f 6234 322f  thub.com/blob42/
+00001230: 6b6f 7265 6164 6572 2d73 696f 7965 6b2d  koreader-sioyek-
+00001240: 696d 706f 7274 0a0a 2323 2044 6f6e 6174  import..## Donat
+00001250: 696f 6e0a 4966 2079 6f75 2065 6e6a 6f79  ion.If you enjoy
+00001260: 2073 696f 7965 6b2c 2070 6c65 6173 6520   sioyek, please 
+00001270: 636f 6e73 6964 6572 2064 6f6e 6174 696e  consider donatin
+00001280: 6720 746f 2073 7570 706f 7274 2069 7473  g to support its
+00001290: 2064 6576 656c 6f70 6d65 6e74 2e0a 0a3c   development...<
+000012a0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000012b0: 7777 772e 6275 796d 6561 636f 6666 6565  www.buymeacoffee
+000012c0: 2e63 6f6d 2f61 6872 6d22 2074 6172 6765  .com/ahrm" targe
+000012d0: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
+000012e0: 7372 633d 2268 7474 7073 3a2f 2f63 646e  src="https://cdn
+000012f0: 2e62 7579 6d65 6163 6f66 6665 652e 636f  .buymeacoffee.co
+00001300: 6d2f 6275 7474 6f6e 732f 6465 6661 756c  m/buttons/defaul
+00001310: 742d 6f72 616e 6765 2e70 6e67 2220 616c  t-orange.png" al
+00001320: 743d 2242 7579 204d 6520 4120 436f 6666  t="Buy Me A Coff
+00001330: 6565 2220 6865 6967 6874 3d22 3431 2220  ee" height="41" 
+00001340: 7769 6474 683d 2231 3734 223e 3c2f 613e  width="174"></a>
+00001350: 0a                                       .
```

