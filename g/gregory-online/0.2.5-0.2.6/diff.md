# Comparing `tmp/gregory_online-0.2.5.tar.gz` & `tmp/gregory_online-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gregory_online-0.2.5.tar", last modified: Mon Jun  5 09:03:56 2023, max compression
+gzip compressed data, was "gregory_online-0.2.6.tar", last modified: Tue Jun  6 11:51:21 2023, max compression
```

## Comparing `gregory_online-0.2.5.tar` & `gregory_online-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:03:56.009804 gregory_online-0.2.5/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-05 09:03:56.009804 gregory_online-0.2.5/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-02 15:20:26.000000 gregory_online-0.2.5/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:03:56.005804 gregory_online-0.2.5/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50146 2023-06-05 09:03:53.000000 gregory_online-0.2.5/bin/gregory_online
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:03:56.009804 gregory_online-0.2.5/gregory_online/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2023-03-15 09:15:19.000000 gregory_online-0.2.5/gregory_online/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-15 09:15:19.000000 gregory_online-0.2.5/gregory_online/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12513 2023-06-05 08:52:20.000000 gregory_online-0.2.5/gregory_online/fetchnp.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 08:56:38.000000 gregory_online-0.2.5/gregory_online/histo_analyze.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3957 2023-06-02 15:34:38.000000 gregory_online-0.2.5/gregory_online/histo_displ.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      779 2023-03-16 17:25:56.000000 gregory_online-0.2.5/gregory_online/histo_global_cont.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13381 2023-06-02 15:20:26.000000 gregory_online-0.2.5/gregory_online/histo_io.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-03-17 14:35:05.000000 gregory_online-0.2.5/gregory_online/histo_np_ops.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-19 12:31:34.000000 gregory_online-0.2.5/gregory_online/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-19 12:17:44.000000 gregory_online-0.2.5/gregory_online/topbar.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2023-03-15 09:15:19.000000 gregory_online-0.2.5/gregory_online/utilone.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2853 2023-06-02 15:20:26.000000 gregory_online-0.2.5/gregory_online/utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:03:56.009804 gregory_online-0.2.5/gregory_online.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      589 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       65 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-05 09:03:56.009804 gregory_online-0.2.5/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1200 2023-06-02 15:20:26.000000 gregory_online-0.2.5/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:51:21.696676 gregory_online-0.2.6/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-06 11:51:21.696676 gregory_online-0.2.6/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-06 11:51:15.000000 gregory_online-0.2.6/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:51:21.692676 gregory_online-0.2.6/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50588 2023-06-06 11:51:18.000000 gregory_online-0.2.6/bin/gregory_online
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:51:21.692676 gregory_online-0.2.6/gregory_online/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2022-09-16 15:11:00.000000 gregory_online-0.2.6/gregory_online/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-17 17:33:40.000000 gregory_online-0.2.6/gregory_online/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12513 2023-06-05 13:30:27.000000 gregory_online-0.2.6/gregory_online/fetchnp.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 14:10:17.000000 gregory_online-0.2.6/gregory_online/histo_analyze.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3957 2023-06-02 15:39:44.000000 gregory_online-0.2.6/gregory_online/histo_displ.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-06 11:16:18.000000 gregory_online-0.2.6/gregory_online/histo_global_cont.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13381 2023-05-31 13:39:18.000000 gregory_online-0.2.6/gregory_online/histo_io.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:29:49.000000 gregory_online-0.2.6/gregory_online/histo_np_ops.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-20 14:10:17.000000 gregory_online-0.2.6/gregory_online/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-20 14:10:17.000000 gregory_online-0.2.6/gregory_online/topbar.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2022-09-16 15:11:00.000000 gregory_online-0.2.6/gregory_online/utilone.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3279 2023-06-06 11:50:54.000000 gregory_online-0.2.6/gregory_online/utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:51:21.692676 gregory_online-0.2.6/gregory_online.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      589 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       65 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-06 11:51:21.696676 gregory_online-0.2.6/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1200 2023-06-01 12:16:03.000000 gregory_online-0.2.6/setup.py
```

### Comparing `gregory_online-0.2.5/PKG-INFO` & `gregory_online-0.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: gregory_online
-Version: 0.2.5
+Version: 0.2.6
 Summary: Online watching HTTP server of ROOT on port 9009
+Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project gregory~online~
 =======================
 
 *experimental code to online survey root spectra from THTTPServer*
 
@@ -77,7 +79,9 @@
   mock~server~.py         
   rebin.py                
   setup.py                
   topbar.py               
   utilone.py              
   version.py              
   ----------------------- ------------------------------
+
+
```

### Comparing `gregory_online-0.2.5/README.md` & `gregory_online-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.5/bin/gregory_online` & `gregory_online-0.2.6/bin/gregory_online`

 * *Files 1% similar despite different names*

```diff
@@ -701,29 +701,37 @@
                     ok = True
                     eline, bline = None,None
                     if is_float(arg.split()[0]):   # ** energy **
                         eline = float(arg.split()[0])
                     elif arg.split()[0].upper() in ECALIBdb.keys():
                         eline = ECALIBdb[arg.split()[0].upper()]
                     else:
+                        print("X... problem if not float nor in DB",arg.split() )
                         ok = False
-                    if is_float(arg.split()[1]):   # ** bin **
+                    print(f"D... ... eline {eline}")
+
+                    print(arg.split(), arg.split()[1], is_float(arg.split()[1]))
+                    if len(arg.split())>1 and is_float(arg.split()[1]):   # ** bin **
                         bline = float(arg.split()[1])
-                    elif arg.split()[1]=="f":      # ** f=fitted bin **
+                        print(f"D... bline={bline}")
+                    # taking from fit....
+                    elif len(arg.split())>1 and arg.split()[1]=="f":      # ** f=fitted bin **
                         if "channel" in last_fit_res:
                             bline = last_fit_res["channel"]
                             dbline = last_fit_res["dchannel"]
                             print("i... GETTING LAST FITTED PEAK for calibration bin", bline)
                         else:
                             ok = False
                             print("X... no fit result stored to get bin from there...")
                     else:
+                        print("X... problem")
                         ok = False
                     if ok:
                         ECALIB.append( [ eline, bline, dbline ] ) # energy, channel, dchannel
+                        print(ECALIB)
             ECALIBa, ECALIBb = ecalibration(ECALIB)
             print(f"i...  calculated energy calibration is {fg.green} E = {ECALIBa:.6f}*k + {ECALIBb:.3f} {fg.default}")
             print(f"i... {fg.blue} REMEMBER!: spectra energy calibration comes from detector (for now)...  {fg.default}")
             print(ECALIB)
 
 
         elif cmd == "i":   # ***CMD***  INFO =======
```

### Comparing `gregory_online-0.2.5/gregory_online/config.py` & `gregory_online-0.2.6/gregory_online/config.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.5/gregory_online/fetchnp.py` & `gregory_online-0.2.6/gregory_online/fetchnp.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.5/gregory_online/histo_analyze.py` & `gregory_online-0.2.6/gregory_online/histo_analyze.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.5/gregory_online/histo_displ.py` & `gregory_online-0.2.6/gregory_online/histo_displ.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.5/gregory_online/histo_global_cont.py` & `gregory_online-0.2.6/gregory_online/histo_global_cont.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 ECALIBb = 0
 
 ECALIBdb = {}
 ECALIBdb['40K'] = 1460.82
 ECALIBdb['214BIB'] = 609.31
 ECALIBdb['214BIA'] = 1764.49
 ECALIBdb['208TL'] = 2614.51
+ECALIBdb['60COA'] = 1173.2
+ECALIBdb['60COB'] = 1332.5
 # ECALIBdb[''] =
 
 # last fit result - useful bin for calib....
 last_fit_res = {}
 
 is_zoomed = [ False, 0.0 ] # yes or no; middle_energy
```

### Comparing `gregory_online-0.2.5/gregory_online/histo_io.py` & `gregory_online-0.2.6/gregory_online/histo_io.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.5/gregory_online/histo_np_ops.py` & `gregory_online-0.2.6/gregory_online/histo_np_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     if ROOT.gDirectory.FindObject(hname):
         #print(f"i... {hname} is there")
         histograms[hname] = ROOT.gDirectory.FindObject(hname)
     else:
         if mytitle is None: mytitle = hname
         print(f"{fg.cyan}X... histo={hname} is NOT there, we create now{fg.default}")
-        histograms[hname] = ROOT.TH1F(hname,f"{hname}:{mytitle}", len(h1np)-2, 0, len(h1np)-2 )
+        histograms[hname] = ROOT.TH1D(hname,f"{hname}:{mytitle}", len(h1np)-2, 0, len(h1np)-2 )
         # print(f"i... {hname} is created now")
 
     suma = 0
     for i in range( len(h1np) ):
         suma+=h1np[i]
         histograms[hname].SetBinContent(i,h1np[i])
         if not errors is None:
```

### Comparing `gregory_online-0.2.5/gregory_online/key_enter.py` & `gregory_online-0.2.6/gregory_online/key_enter.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.5/gregory_online/topbar.py` & `gregory_online-0.2.6/gregory_online/topbar.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.5/gregory_online/utils.py` & `gregory_online-0.2.6/gregory_online/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,52 @@
 import os
 
 #
 #  taken from flashcam and stackoveerflow
 import math
 
 def is_int(n):
-    if n is None or math.isnan(n):
-        return False
+    # try:
+    #     if math.isnan(n):
+    #         return False
+    # except:
+    #     return False
+
     try:
         float_n = float(n)
         int_n = int(float_n)
     except ValueError:
         return False
     else:
         return float_n == int_n
 
+
 def is_float(n):
     try:
         float_n = float(n)
         #print(n, float_n)
     except ValueError:
+        print(f"X... not float /{n}/")
         return False
     else:
         #print("true block", n)
-        if n is None or math.isnan(n):
-            #print("NONE")
+        if n is None:
+            print("X... isfloat ... NONE")
             return False
-        return True
+
+        retval = True
+        try:
+            if type(n) is not str and math.isnan(n): # if Nan comes, it can sort it out, else it crashes with string.
+                print("X... math ... NAN float")
+                retval = False
+        except:
+            print("X... crashed math NaN")
+            retval = False
+        return retval # normally true
+
 
 def is_bool(n):
     if type(n) is str and n=="False": return True
     if type(n) is str and n=="True": return True
     return False
```

### Comparing `gregory_online-0.2.5/gregory_online.egg-info/PKG-INFO` & `gregory_online-0.2.6/gregory_online.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: gregory-online
-Version: 0.2.5
+Version: 0.2.6
 Summary: Online watching HTTP server of ROOT on port 9009
+Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project gregory~online~
 =======================
 
 *experimental code to online survey root spectra from THTTPServer*
 
@@ -77,7 +79,9 @@
   mock~server~.py         
   rebin.py                
   setup.py                
   topbar.py               
   utilone.py              
   version.py              
   ----------------------- ------------------------------
+
+
```

### Comparing `gregory_online-0.2.5/gregory_online.egg-info/SOURCES.txt` & `gregory_online-0.2.6/gregory_online.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.5/setup.py` & `gregory_online-0.2.6/setup.py`

 * *Files identical despite different names*

