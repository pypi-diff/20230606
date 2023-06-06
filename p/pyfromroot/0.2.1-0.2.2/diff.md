# Comparing `tmp/pyfromroot-0.2.1.tar.gz` & `tmp/pyfromroot-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfromroot-0.2.1.tar", last modified: Mon Jun  5 09:04:28 2023, max compression
+gzip compressed data, was "pyfromroot-0.2.2.tar", last modified: Tue Jun  6 11:22:21 2023, max compression
```

## Comparing `pyfromroot-0.2.1.tar` & `pyfromroot-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:04:28.873340 pyfromroot-0.2.1/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    10569 2023-06-05 09:04:28.873340 pyfromroot-0.2.1/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    10303 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:04:28.869340 pyfromroot-0.2.1/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11413 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/bin/pyfromroot
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:04:28.873340 pyfromroot-0.2.1/pyfromroot/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      253 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/__init__.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     3880 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_draw.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    17383 2023-03-16 17:23:03.000000 pyfromroot-0.2.1/pyfromroot/pr_fit.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9850 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_load.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     3678 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_model_decay.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     9945 2023-03-16 17:21:17.000000 pyfromroot-0.2.1/pyfromroot/pr_model_gpol1.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5984 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_model_logxy.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     6835 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_model_pocall.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5516 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_model_polall.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5407 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_zoom.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2301 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/prj_utils.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     8691 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/prun.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      565 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/unitname.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:04:28.873340 pyfromroot-0.2.1/pyfromroot.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    10569 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      547 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       54 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       11 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-05 09:04:28.873340 pyfromroot-0.2.1/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1367 2023-04-03 13:37:30.000000 pyfromroot-0.2.1/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:22:21.622006 pyfromroot-0.2.2/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    11504 2023-06-06 11:22:21.622006 pyfromroot-0.2.2/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    11218 2023-06-06 11:22:18.000000 pyfromroot-0.2.2/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:22:21.618006 pyfromroot-0.2.2/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11413 2022-09-01 09:03:00.000000 pyfromroot-0.2.2/bin/pyfromroot
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:22:21.618006 pyfromroot-0.2.2/pyfromroot/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      253 2022-04-20 07:42:46.000000 pyfromroot-0.2.2/pyfromroot/__init__.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     3880 2023-06-06 11:21:18.000000 pyfromroot-0.2.2/pyfromroot/pr_draw.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    17383 2023-06-06 11:21:24.000000 pyfromroot-0.2.2/pyfromroot/pr_fit.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9850 2023-06-06 11:21:31.000000 pyfromroot-0.2.2/pyfromroot/pr_load.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     3678 2022-04-20 07:42:46.000000 pyfromroot-0.2.2/pyfromroot/pr_model_decay.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     9945 2023-03-17 17:41:27.000000 pyfromroot-0.2.2/pyfromroot/pr_model_gpol1.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5984 2022-09-01 09:03:00.000000 pyfromroot-0.2.2/pyfromroot/pr_model_logxy.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     6835 2022-09-01 09:03:00.000000 pyfromroot-0.2.2/pyfromroot/pr_model_pocall.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5516 2022-09-01 09:03:00.000000 pyfromroot-0.2.2/pyfromroot/pr_model_polall.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5407 2023-06-06 11:20:39.000000 pyfromroot-0.2.2/pyfromroot/pr_zoom.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2301 2022-04-20 07:42:46.000000 pyfromroot-0.2.2/pyfromroot/prj_utils.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     8691 2023-03-17 17:41:27.000000 pyfromroot-0.2.2/pyfromroot/prun.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      565 2022-04-20 07:42:46.000000 pyfromroot-0.2.2/pyfromroot/unitname.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-06 11:22:21.000000 pyfromroot-0.2.2/pyfromroot/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:22:21.622006 pyfromroot-0.2.2/pyfromroot.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    11504 2023-06-06 11:22:21.000000 pyfromroot-0.2.2/pyfromroot.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      547 2023-06-06 11:22:21.000000 pyfromroot-0.2.2/pyfromroot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-06 11:22:21.000000 pyfromroot-0.2.2/pyfromroot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       54 2023-06-06 11:22:21.000000 pyfromroot-0.2.2/pyfromroot.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       11 2023-06-06 11:22:21.000000 pyfromroot-0.2.2/pyfromroot.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-06 11:22:21.622006 pyfromroot-0.2.2/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1367 2023-04-13 15:06:35.000000 pyfromroot-0.2.2/setup.py
```

### Comparing `pyfromroot-0.2.1/PKG-INFO` & `pyfromroot-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,28 @@
-Metadata-Version: 2.1
-Name: pyfromroot
-Version: 0.2.1
-Summary: Python should be callable from root environment
-Home-page: https://gitlab.com/jaromrax/pyfromroot
-Author: jaromrax
-Author-email: jaromrax@gmail.com
-License: GPL2
-Description-Content-Type: text/markdown
-
 PyFromRoot - fitting with iminuit in root
 =========================================
 
-The goal is to have a framework to run Python scripts from root\'s
-CLINT.
+The goal is to have a framework to combine Python and iminuit with root
+to get the best of both.
 
-What?
+Basic commands for the moment
 
--   `load` - load csv liike data or histogram
+-   `load` - load csv like data or histogram
 -   `zoom` - zoom to the desired range
 -   `fit` - fit with a desired model
 
-Why?
+Fit models - filename is like `pr_model_*.py` and it will be recognized
+by the loader
 
--   TH1F and TGraph on TCanvas are superior and interactive
--   staying in `root` CLINT allows to have a access to histograms and
-    all other stuff
-    -   BUT it is possible to call everything from python script too (no
-        CLINT though)
--   `MODELS` - user can build simply any model separate of the rest of
-    the code `pr_model_*.py`
-    -   `polall` - model for 0-5th degree polynomials
-    -   `pocall` - model for 0-5th degree chebyshev polymonials
-    -   `logxy` - model for pol in log space
-    -   `gpol1` - model for gauss plus pol1
-    -   `decay` - model for exponential
-    -   `circle` - model for circle - image 640x480, center at top
+-   `polall` - model for 0-5th degree polynomials
+-   `pocall` - model for 0-5th degree chebyshev polymonials
+-   `logxy` - model for pol in log space
+-   `gpol1` - model for gauss plus pol1
+-   `decay` - model for exponential
+-   `circle` - model for circle - image 640x480, center at top
 
 Features and issues
 ===================
 
 Issues
 ------
 
@@ -183,30 +167,71 @@
 #  510   1659.27    0.36    2.91    0.86     1123.24    0.25    1.97    0.58          1.00         0.28     0.87
 #  570   1661.82    1.72    6.83    2.66     1124.97    1.17    4.62    1.80          1.05         0.50     1.37
 ```
 
 Usage
 =====
 
-From root
----------
+From root (problems now)
+------------------------
+
+For text file with columns
 
-    .L prun.L
+    .L prun.C
     prun("load filename _,x,y")
 
+For text file with one column and histogram
+
+    .L prun.C
+    prun("load nn.asc1 h")
+    prun("zoom nn 3827,30")
+
 TGraph of name `filename_x_y` is created, kept in
 `gROOT->GetSpecials()`, visible with `shspe()`
 
-From python
------------
+From python (changes in time now)
+---------------------------------
 
-Full example:
+Canvas control 2022/11 . If there is no canvas name in FIT, no display
+is done....
 
 ``` {.python results="replace output" session="test" exports="both"}
+#!/usr/bin/env python3
+
+from fire import Fire
+from pyfromroot import prun
+import ROOT
+import time
 
+def main():
+
+    prun.do("load","n2.asc1 h")
+    prun.do("zoom","n2 13825,60") # 14042.88   154
+    prun.do("draw","n2", canvas = "cn2")
+    res2 = prun.do("fit","n2 gpol1", canvas="xoxo2")
+    #return
+
+    prun.do("load","nn.asc1 h")
+    prun.do("zoom","nn 6582,29") # 14059.07
+    prun.do("draw","nn", canvas = "cnn")
+    res1 = prun.do("fit","nn gpol1", canvas="xoxo")
+    print("X"*60)
+
+    print( res1.keys() )
+    for i in  ['area','darea','channel','chi2dof']: print(f"{i:12s} nn: {res1[i]:10.2f}   n2:{res2[i]:10.2f}")
+
+if __name__=="__main__":
+    Fire(main)
+    while ROOT.addressof(ROOT.gPad)!=0: time.sleep(0.2)
+
+```
+
+Full example earlier 2022:
+
+``` {.python results="replace output" session="test" exports="both"}
 #!/usr/bin/env python3
 
 from  pyfromroot import  prun
 import ROOT
 import time
 import sys
 from fire import Fire
@@ -254,7 +279,8 @@
 
 ```
 
 Versions
 ========
 
 -   0.1.
+-   0.2. works on ubuntu 22 with numpy 1.23.5
```

### Comparing `pyfromroot-0.2.1/README.md` & `pyfromroot-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,39 @@
+Metadata-Version: 2.1
+Name: pyfromroot
+Version: 0.2.2
+Summary: Python should be callable from root environment
+Home-page: https://gitlab.com/jaromrax/pyfromroot
+Author: jaromrax
+Author-email: jaromrax@gmail.com
+License: GPL2
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 PyFromRoot - fitting with iminuit in root
 =========================================
 
-The goal is to have a framework to run Python scripts from root\'s
-CLINT.
+The goal is to have a framework to combine Python and iminuit with root
+to get the best of both.
 
-What?
+Basic commands for the moment
 
--   `load` - load csv liike data or histogram
+-   `load` - load csv like data or histogram
 -   `zoom` - zoom to the desired range
 -   `fit` - fit with a desired model
 
-Why?
+Fit models - filename is like `pr_model_*.py` and it will be recognized
+by the loader
 
--   TH1F and TGraph on TCanvas are superior and interactive
--   staying in `root` CLINT allows to have a access to histograms and
-    all other stuff
-    -   BUT it is possible to call everything from python script too (no
-        CLINT though)
--   `MODELS` - user can build simply any model separate of the rest of
-    the code `pr_model_*.py`
-    -   `polall` - model for 0-5th degree polynomials
-    -   `pocall` - model for 0-5th degree chebyshev polymonials
-    -   `logxy` - model for pol in log space
-    -   `gpol1` - model for gauss plus pol1
-    -   `decay` - model for exponential
-    -   `circle` - model for circle - image 640x480, center at top
+-   `polall` - model for 0-5th degree polynomials
+-   `pocall` - model for 0-5th degree chebyshev polymonials
+-   `logxy` - model for pol in log space
+-   `gpol1` - model for gauss plus pol1
+-   `decay` - model for exponential
+-   `circle` - model for circle - image 640x480, center at top
 
 Features and issues
 ===================
 
 Issues
 ------
 
@@ -173,30 +178,71 @@
 #  510   1659.27    0.36    2.91    0.86     1123.24    0.25    1.97    0.58          1.00         0.28     0.87
 #  570   1661.82    1.72    6.83    2.66     1124.97    1.17    4.62    1.80          1.05         0.50     1.37
 ```
 
 Usage
 =====
 
-From root
----------
+From root (problems now)
+------------------------
+
+For text file with columns
 
-    .L prun.L
+    .L prun.C
     prun("load filename _,x,y")
 
+For text file with one column and histogram
+
+    .L prun.C
+    prun("load nn.asc1 h")
+    prun("zoom nn 3827,30")
+
 TGraph of name `filename_x_y` is created, kept in
 `gROOT->GetSpecials()`, visible with `shspe()`
 
-From python
------------
+From python (changes in time now)
+---------------------------------
 
-Full example:
+Canvas control 2022/11 . If there is no canvas name in FIT, no display
+is done....
 
 ``` {.python results="replace output" session="test" exports="both"}
+#!/usr/bin/env python3
+
+from fire import Fire
+from pyfromroot import prun
+import ROOT
+import time
+
+def main():
 
+    prun.do("load","n2.asc1 h")
+    prun.do("zoom","n2 13825,60") # 14042.88   154
+    prun.do("draw","n2", canvas = "cn2")
+    res2 = prun.do("fit","n2 gpol1", canvas="xoxo2")
+    #return
+
+    prun.do("load","nn.asc1 h")
+    prun.do("zoom","nn 6582,29") # 14059.07
+    prun.do("draw","nn", canvas = "cnn")
+    res1 = prun.do("fit","nn gpol1", canvas="xoxo")
+    print("X"*60)
+
+    print( res1.keys() )
+    for i in  ['area','darea','channel','chi2dof']: print(f"{i:12s} nn: {res1[i]:10.2f}   n2:{res2[i]:10.2f}")
+
+if __name__=="__main__":
+    Fire(main)
+    while ROOT.addressof(ROOT.gPad)!=0: time.sleep(0.2)
+
+```
+
+Full example earlier 2022:
+
+``` {.python results="replace output" session="test" exports="both"}
 #!/usr/bin/env python3
 
 from  pyfromroot import  prun
 import ROOT
 import time
 import sys
 from fire import Fire
@@ -244,7 +290,10 @@
 
 ```
 
 Versions
 ========
 
 -   0.1.
+-   0.2. works on ubuntu 22 with numpy 1.23.5
+
+
```

### Comparing `pyfromroot-0.2.1/bin/pyfromroot` & `pyfromroot-0.2.2/bin/pyfromroot`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.2.1/pyfromroot/pr_draw.py` & `pyfromroot-0.2.2/pyfromroot/pr_draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     gontainer = ROOT.gDirectory.FindObject( fname )
 
     print( gontainer )
     print( type(gontainer) )
     import cppyy
 
-    if type(gontainer)==cppyy.gbl.TH1F :
+    if type(gontainer)==cppyy.gbl.TH1D :
         histo = True
     else:
         histo = False
 
 
 
 
@@ -104,15 +104,15 @@
     else:
         print("--------------existin canvas ------ I cd INTO it",cmain)
         cmain.cd()
 
 
 
     if histo:
-        # it will be TH1F
+        # it will be TH1D
         print("i... ============= OPT=", drawopt)
         gontainer.SetLineColor( coloropt )
         gontainer.SetMarkerColor( coloropt )
         #gontainer.SetLineColor( coloropt )
 
         print(f"i... DRAWING {gontainer} WITH OPTION ", drawopt )
         gontainer.Draw( drawopt)  # this can be also: same ex0
```

### Comparing `pyfromroot-0.2.1/pyfromroot/pr_fit.py` & `pyfromroot-0.2.2/pyfromroot/pr_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         x=np.asarray( g_orig.GetX() )
         y=np.asarray( g_orig.GetY() )
         dx=np.asarray( g_orig.GetEX() )
         dy=np.asarray( g_orig.GetEY() )
 
     cala = 1
     calb = 0
-    if g_orig.ClassName()=="TH1F":
+    if g_orig.ClassName()=="TH1D":
         ishisto = True
         #
         # i need to convert to np; be sure it is np.float64!
         # maybe - kill all zero points??? or set error 1??
         # ZOOM with GetFirst GetLast
         #
         #   x chan -0.5 to compensate midbin!
```

### Comparing `pyfromroot-0.2.1/pyfromroot/pr_load.py` & `pyfromroot-0.2.2/pyfromroot/pr_load.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 #
 
 
 
 
 def create_histo(df, hpos, cala, calb ):
     """
-    TH1F * created
+    TH1D * created
     """
     x = np.array(  df[ df.columns[hpos] ]  ,  np.float64)
-    h = ROOT.TH1F( "h", "h", len(df), 0, len(df) )
+    h = ROOT.TH1D( "h", "h", len(df), 0, len(df) )
     bn = 0
     for bc in x:
         bn+=1
         h.SetBinContent(  bn, bc )
     h.GetXaxis().SetLimits( calb, cala*len(df)+calb )
     return h
 
@@ -247,15 +247,15 @@
 
 
     NAMEO = os.path.splitext(fname)[0]
     print(f"D... graph name = {NAMEO}; for multiloads=>{NAME1} ")
 
 
     if histo:
-        # it will be TH1F
+        # it will be TH1D
 
         gontainer = create_histo(df, hpos, cala, calb)
         #gontainer.Draw()
         gontainer.SetTitle(f"{NAME1};channel;{names[hpos]}")
         #ROOT.gPad.SetLogy()
         gontainer.Print()
```

### Comparing `pyfromroot-0.2.1/pyfromroot/pr_model_decay.py` & `pyfromroot-0.2.2/pyfromroot/pr_model_decay.py`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.2.1/pyfromroot/pr_model_gpol1.py` & `pyfromroot-0.2.2/pyfromroot/pr_model_gpol1.py`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.2.1/pyfromroot/pr_model_logxy.py` & `pyfromroot-0.2.2/pyfromroot/pr_model_logxy.py`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.2.1/pyfromroot/pr_model_pocall.py` & `pyfromroot-0.2.2/pyfromroot/pr_model_pocall.py`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.2.1/pyfromroot/pr_model_polall.py` & `pyfromroot-0.2.2/pyfromroot/pr_model_polall.py`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.2.1/pyfromroot/pr_zoom.py` & `pyfromroot-0.2.2/pyfromroot/pr_zoom.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         x=np.asarray( g_orig.GetX() )
         y=np.asarray( g_orig.GetY() )
         dx=np.asarray( g_orig.GetEX() )
         dy=np.asarray( g_orig.GetEY() )
 
 
     cala,calb=1,0
-    if g_orig.ClassName()=="TH1F":
+    if g_orig.ClassName()=="TH1D":
         #
         # i need to convert to np; be sure it is np.float64!
         # maybe - kill all zero points??? or set error 1??
         # ZOOM with GetFirst GetLast
         #
         #   x chan -0.5 to compensate midbin!
         #
```

### Comparing `pyfromroot-0.2.1/pyfromroot/prj_utils.py` & `pyfromroot-0.2.2/pyfromroot/prj_utils.py`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.2.1/pyfromroot/prun.py` & `pyfromroot-0.2.2/pyfromroot/prun.py`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.2.1/pyfromroot/unitname.py` & `pyfromroot-0.2.2/pyfromroot/unitname.py`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.2.1/pyfromroot.egg-info/PKG-INFO` & `pyfromroot-0.2.2/pyfromroot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 Metadata-Version: 2.1
 Name: pyfromroot
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python should be callable from root environment
 Home-page: https://gitlab.com/jaromrax/pyfromroot
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 PyFromRoot - fitting with iminuit in root
 =========================================
 
-The goal is to have a framework to run Python scripts from root\'s
-CLINT.
+The goal is to have a framework to combine Python and iminuit with root
+to get the best of both.
 
-What?
+Basic commands for the moment
 
--   `load` - load csv liike data or histogram
+-   `load` - load csv like data or histogram
 -   `zoom` - zoom to the desired range
 -   `fit` - fit with a desired model
 
-Why?
+Fit models - filename is like `pr_model_*.py` and it will be recognized
+by the loader
 
--   TH1F and TGraph on TCanvas are superior and interactive
--   staying in `root` CLINT allows to have a access to histograms and
-    all other stuff
-    -   BUT it is possible to call everything from python script too (no
-        CLINT though)
--   `MODELS` - user can build simply any model separate of the rest of
-    the code `pr_model_*.py`
-    -   `polall` - model for 0-5th degree polynomials
-    -   `pocall` - model for 0-5th degree chebyshev polymonials
-    -   `logxy` - model for pol in log space
-    -   `gpol1` - model for gauss plus pol1
-    -   `decay` - model for exponential
-    -   `circle` - model for circle - image 640x480, center at top
+-   `polall` - model for 0-5th degree polynomials
+-   `pocall` - model for 0-5th degree chebyshev polymonials
+-   `logxy` - model for pol in log space
+-   `gpol1` - model for gauss plus pol1
+-   `decay` - model for exponential
+-   `circle` - model for circle - image 640x480, center at top
 
 Features and issues
 ===================
 
 Issues
 ------
 
@@ -183,30 +178,71 @@
 #  510   1659.27    0.36    2.91    0.86     1123.24    0.25    1.97    0.58          1.00         0.28     0.87
 #  570   1661.82    1.72    6.83    2.66     1124.97    1.17    4.62    1.80          1.05         0.50     1.37
 ```
 
 Usage
 =====
 
-From root
----------
+From root (problems now)
+------------------------
 
-    .L prun.L
+For text file with columns
+
+    .L prun.C
     prun("load filename _,x,y")
 
+For text file with one column and histogram
+
+    .L prun.C
+    prun("load nn.asc1 h")
+    prun("zoom nn 3827,30")
+
 TGraph of name `filename_x_y` is created, kept in
 `gROOT->GetSpecials()`, visible with `shspe()`
 
-From python
------------
+From python (changes in time now)
+---------------------------------
 
-Full example:
+Canvas control 2022/11 . If there is no canvas name in FIT, no display
+is done....
 
 ``` {.python results="replace output" session="test" exports="both"}
+#!/usr/bin/env python3
+
+from fire import Fire
+from pyfromroot import prun
+import ROOT
+import time
+
+def main():
+
+    prun.do("load","n2.asc1 h")
+    prun.do("zoom","n2 13825,60") # 14042.88   154
+    prun.do("draw","n2", canvas = "cn2")
+    res2 = prun.do("fit","n2 gpol1", canvas="xoxo2")
+    #return
+
+    prun.do("load","nn.asc1 h")
+    prun.do("zoom","nn 6582,29") # 14059.07
+    prun.do("draw","nn", canvas = "cnn")
+    res1 = prun.do("fit","nn gpol1", canvas="xoxo")
+    print("X"*60)
 
+    print( res1.keys() )
+    for i in  ['area','darea','channel','chi2dof']: print(f"{i:12s} nn: {res1[i]:10.2f}   n2:{res2[i]:10.2f}")
+
+if __name__=="__main__":
+    Fire(main)
+    while ROOT.addressof(ROOT.gPad)!=0: time.sleep(0.2)
+
+```
+
+Full example earlier 2022:
+
+``` {.python results="replace output" session="test" exports="both"}
 #!/usr/bin/env python3
 
 from  pyfromroot import  prun
 import ROOT
 import time
 import sys
 from fire import Fire
@@ -254,7 +290,10 @@
 
 ```
 
 Versions
 ========
 
 -   0.1.
+-   0.2. works on ubuntu 22 with numpy 1.23.5
+
+
```

### Comparing `pyfromroot-0.2.1/pyfromroot.egg-info/SOURCES.txt` & `pyfromroot-0.2.2/pyfromroot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.2.1/setup.py` & `pyfromroot-0.2.2/setup.py`

 * *Files identical despite different names*

