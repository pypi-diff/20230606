# Comparing `tmp/lkcom-0.3.2.tar.gz` & `tmp/lkcom-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lkcom-0.3.2.tar", last modified: Fri Jun  2 10:19:44 2023, max compression
+gzip compressed data, was "lkcom-0.3.3.tar", last modified: Tue Jun  6 09:17:40 2023, max compression
```

## Comparing `lkcom-0.3.2.tar` & `lkcom-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 10:19:44.888178 lkcom-0.3.2/
--rw-rw-rw-   0        0        0      759 2023-06-02 10:19:44.887178 lkcom-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      332 2021-11-15 10:30:15.000000 lkcom-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 10:19:44.880177 lkcom-0.3.2/lkcom/
--rw-rw-rw-   0        0        0      188 2023-03-02 15:31:24.000000 lkcom-0.3.2/lkcom/__init__.py
--rw-rw-rw-   0        0        0     3183 2023-03-01 07:58:13.000000 lkcom-0.3.2/lkcom/cfgparse.py
--rw-rw-rw-   0        0        0    30480 2023-06-01 06:51:50.000000 lkcom-0.3.2/lkcom/dataio.py
--rw-rw-rw-   0        0        0    14989 2023-03-01 07:58:23.000000 lkcom-0.3.2/lkcom/image.py
--rw-rw-rw-   0        0        0    48811 2023-05-22 05:36:02.000000 lkcom-0.3.2/lkcom/plot.py
--rw-rw-rw-   0        0        0     1780 2023-03-01 07:58:32.000000 lkcom-0.3.2/lkcom/standard_func.py
--rw-rw-rw-   0        0        0    26131 2023-04-27 13:46:59.000000 lkcom-0.3.2/lkcom/string.py
--rw-rw-rw-   0        0        0    32944 2023-05-26 06:41:38.000000 lkcom-0.3.2/lkcom/util.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:19:44.886179 lkcom-0.3.2/lkcom.egg-info/
--rw-rw-rw-   0        0        0      759 2023-06-02 10:19:44.000000 lkcom-0.3.2/lkcom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-02 10:19:44.000000 lkcom-0.3.2/lkcom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 10:19:44.000000 lkcom-0.3.2/lkcom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-02 10:19:44.000000 lkcom-0.3.2/lkcom.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-02 10:19:44.000000 lkcom-0.3.2/lkcom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 10:19:44.888178 lkcom-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1327 2022-12-15 15:01:50.000000 lkcom-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:17:40.734060 lkcom-0.3.3/
+-rw-rw-rw-   0        0        0      759 2023-06-06 09:17:40.734060 lkcom-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2021-11-15 10:30:15.000000 lkcom-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 09:17:40.710055 lkcom-0.3.3/lkcom/
+-rw-rw-rw-   0        0        0      188 2023-06-06 09:16:46.000000 lkcom-0.3.3/lkcom/__init__.py
+-rw-rw-rw-   0        0        0     3183 2023-03-01 07:58:13.000000 lkcom-0.3.3/lkcom/cfgparse.py
+-rw-rw-rw-   0        0        0    30884 2023-06-06 08:46:42.000000 lkcom-0.3.3/lkcom/dataio.py
+-rw-rw-rw-   0        0        0    14989 2023-03-01 07:58:23.000000 lkcom-0.3.3/lkcom/image.py
+-rw-rw-rw-   0        0        0    48813 2023-06-06 06:49:38.000000 lkcom-0.3.3/lkcom/plot.py
+-rw-rw-rw-   0        0        0     2144 2023-06-06 09:10:31.000000 lkcom-0.3.3/lkcom/standard_func.py
+-rw-rw-rw-   0        0        0    26131 2023-04-27 13:46:59.000000 lkcom-0.3.3/lkcom/string.py
+-rw-rw-rw-   0        0        0    32944 2023-05-26 06:41:38.000000 lkcom-0.3.3/lkcom/util.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:17:40.732058 lkcom-0.3.3/lkcom.egg-info/
+-rw-rw-rw-   0        0        0      759 2023-06-06 09:17:40.000000 lkcom-0.3.3/lkcom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-06 09:17:40.000000 lkcom-0.3.3/lkcom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 09:17:40.000000 lkcom-0.3.3/lkcom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-06 09:17:40.000000 lkcom-0.3.3/lkcom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 09:17:40.000000 lkcom-0.3.3/lkcom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 09:17:40.735055 lkcom-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1327 2022-12-15 15:01:50.000000 lkcom-0.3.3/setup.py
```

### Comparing `lkcom-0.3.2/PKG-INFO` & `lkcom-0.3.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkcom
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python library of useful routines.
 Home-page: https://bitbucket.org/lukaskontenis/lkcom/
 Author: Lukas Kontenis
 Author-email: dse.ssd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lkcom-0.3.2/lkcom/cfgparse.py` & `lkcom-0.3.3/lkcom/cfgparse.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.3.2/lkcom/dataio.py` & `lkcom-0.3.3/lkcom/dataio.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This module contains data input and output utilities.
 
 Copyright 2015-2023 Lukas Kontenis
 Contact: dse.ssd@gmail.com
 """
 import os
-import sys
+import pathlib
 import io
 import zipfile
 import glob
 from pathlib import Path
 import json
 import time
 import datetime
@@ -871,7 +871,18 @@
 def read_d_scan_temporal_envelope(dir_name):
     """Read temporal envelope from a Sphere Photonics d-scan retrieval."""
     file_name = list_files_with_extension(dir_name, ext='txt', name_include_filter='retrieved_pulse')[0]
 
     data = np.loadtxt(file_name, converters={0: float_loc_parser, 1:float_loc_parser, 2:float_loc_parser}, skiprows=1)
 
     return {'tarr': data[:, 0], 'ampl_ds': data[:, 1], 'ampl_tl': data[:, 2]}
+
+
+def parse_data_setup_json(data_file_name):
+    """Read a setup.json file if it exists."""
+    setup_file_path = pathlib.Path(data_file_name).absolute().parent / 'setup.json'
+    if check_file_exists(setup_file_path):
+        print("Parsing " + setup_file_path.name)
+        return json.load(open(setup_file_path))
+    else:
+        print("Data file has no setup.json")
+        return {}
```

### Comparing `lkcom-0.3.2/lkcom/image.py` & `lkcom-0.3.3/lkcom/image.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.3.2/lkcom/plot.py` & `lkcom-0.3.3/lkcom/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -562,15 +562,14 @@
     if show_avg_prof_value:
         add_x_marker(np.nanmean(img[:, xprof_index-5:xprof_index+5]), ls='-')
     if show_section_avg_profile:
         plt.plot(np.nanmean(img[:, xprof_index-5:xprof_index+5], 1), np.arange(0, num_px))
     plt.plot(img[:, xprof_index], np.arange(0, num_px), c=profile_color)
 
 
-
 def add_infobox(
         infobox_str=None, show_infobox=True, infobox_hpos='left', text_va='top',
         infobox_vpos='top', ref_y=None, text_x=None, text_y=None, **kwargs):
     if show_infobox and infobox_str:
         xl = kwargs.get('xlim')
         if xl is None:
             xl = plt.gca().get_xlim()
@@ -987,15 +986,15 @@
             show_avg_trace = False
             if not force_plot_sample_trace:
                 print("Number of points {:d} ".format(len(X)) +
                       "is too small to make an occurrence plot " +
                       "({:d} needed). ".format(MIN_PTS_FOR_OCCURRENCE_PLOT) +
                       "Will plot a sample trace instead.")
 
-    if(isnone(sliced_data)):
+    if sliced_data is None:
         [Xb, Yb, Yb_lvls] = bin_and_slice_data(
             X=X, Y=Y, num_slcs=num_slcs, **kwargs)
         if len(Yb_lvls.shape) > 1:
             num_lvls = int((Yb_lvls.shape[1]-1)/2)
     else:
         Xb = X
         Yb = Y
@@ -1044,15 +1043,15 @@
         if yl_frac:
             # If the display limits fraction is given, set the axis limits to
             # Â±fraction of the mean around the mean
             yl = [mean_y*(1-yl_frac), mean_y*(1+yl_frac)]
         else:
             # Otherwise set the axis limits to span the entire percentile range
             # with an extra 10%
-            if Y:
+            if Y is not None:
                 yl = extend_range([
                     np.nanmin(Y), np.nanmax(Y)], 0.1)
             else:
                 yl = extend_range([
                     np.nanmin(Yb_lvls), np.nanmax(Yb_lvls)], 0.1)
 
     # Histogram bar color
@@ -1114,15 +1113,15 @@
 
     if plot_sample_trace:
         h = plt.plot(X, Y, color=get_color('dr'))
         legend_h.append(h[0])
         legend_str.append('Sample')
         marker_color = get_color('black')
 
-    if isnone(xlim):
+    if xlim is None:
         # Determine X axis limits automatically
         x_min = np.nanmin(X)
         x_max = np.nanmax(X)
 
         if round_auto_xlim:
             x_span = x_max - x_min
 
@@ -1141,15 +1140,15 @@
 
         plt.xlim([x_min, x_max])
     else:
         plt.xlim(xlim)
 
     xl = plt.xlim()
 
-    if not isnone(ymarker):
+    if ymarker is not None:
         for ind, ym in enumerate(ymarker):
             h = plt.plot(xl, [ym, ym], ls='--', c=marker_color)
             if ind == 0:
                 legend_h.append(h[0])
                 if ymarker_label is not None:
                     legend_str.append(ymarker_label)
                 else:
@@ -1159,32 +1158,32 @@
 
     if show_zero_line:
         if yl[0] < 0 and yl[1] > 0:
             add_y_marker(0, ls='-')
 
     plt.xlim(xl)
     plt.ylim(yl)
-    if(not isnone(xlabel)):
+    if xlabel is not None:
         plt.xlabel(xlabel)
 
-    if(show_ylabel and not isnone(ylabel)):
+    if show_ylabel and ylabel is not None:
         plt.ylabel(ylabel)
 
-    if(show_title and not isnone(title)):
+    if show_title and title is not None:
         plt.title(title)
 
-    if(show_tltext and not isnone(tltext)):
+    if show_tltext and tltext is not None:
         ofs_x = (xl[1]-xl[0])*0.05
         ofs_y = (yl[1]-yl[0])*0.05
 
         plt.text(xl[0]+ofs_x, yl[1]-ofs_y, tltext, ha='left', va='top',
                  bbox=dict(facecolor='white', alpha=0.75,
                  edgecolor='white'))
 
-    if(not show_yticklabels):
+    if not show_yticklabels:
         plt.gca().set_yticklabels([])
 
     if normalize_y_tick_labels_only:
         yticks = plt.yticks()[0]
         plt.yticks(yticks, np.round(yticks/mean_y, 2))
         plt.ylim(yl)
 
@@ -1193,15 +1192,15 @@
     if show_legend:
         plt.legend(legend_h, legend_str, numpoints=1, loc=legend_loc,
                    handler_map={tuple: HandlerTuple(ndivide=None)})
 
     plt.gca().tick_params(axis='both', which='both', direction='in')
 
     ax_hist = None
-    if(with_hist):
+    if with_hist:
         ax_hist = plt.subplot(grid[0, 4])
         y_span = yl[1] - yl[0]
         y_gran = get_granularity(Y)
 
         y_units = 's'
         try:
             if ylabel:
@@ -1225,15 +1224,15 @@
             y_grans_per_bin = np.max([
                 np.round(num_hist_bins/target_hist_bins), 1])
             bins = np.arange(yl[0], yl[1],
                              y_gran*y_grans_per_bin*hist_bin_size_fac)
 
         num_bins = len(bins)
 
-        if(abs(len(bins)/target_hist_bins - 1) > 0.1):
+        if abs(len(bins)/target_hist_bins - 1) > 0.1:
             print("Number of histogram bins requested: {:d}, actual number is "
                   "{:d} due to Y data granularity".format(
                     target_hist_bins, num_bins))
 
         if with_histogram_dither:
             # Calculate histogram dithering array. Elements of the array are
             # drawn from a Gaussian distribution centered at 1. The width of
@@ -1249,21 +1248,21 @@
                   "compare the histogram with and without dithering.")
         else:
             dith = 1
 
         plt.hist(Y*dith, bins=bins, orientation="horizontal",
                  color=hist_color, zorder=10)[0]
 
-        if not isnone(hist_ymarkers):
+        if hist_ymarkers is not None:
             # Add histogram y markers
             for hist_ymarker in hist_ymarkers:
                 add_y_marker(hist_ymarker, c=[0.75, 0.75, 0.75], ls='-',
                              zorder=1)
 
-        if not isnone(ymarker):
+        if ymarker is not None:
             # Add y markers that are common for the histogram and the main
             # plot area
             for ym in ymarker:
                 add_y_marker(ym, c=marker_color, zorder=20)
 
         plt.ylim(yl)
         plt.xticks([])
```

### Comparing `lkcom-0.3.2/lkcom/standard_func.py` & `lkcom-0.3.3/lkcom/standard_func.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,7 +67,15 @@
     plt.plot([np.min(X), np.max(X)], [y0, y0], c=c, ls=ls_markers)
 
 
 def plot_gaussian_1D_arglist(args, X=None, **kwargs):
     """Plot a 1D Gaussian."""
     return plot_gaussian_1D(
         X, A=args[0], width=args[1], center=args[2], y0=args[3], **kwargs)
+
+
+def pulse_response(x, a=1, x0=0, tau00=0.1, tau01=0, tau1=0.1, b=0):
+    formula = 'v1'
+    if formula == 'v1':
+        return a / (1 + np.exp(-(x-x0)/tau00)) * 1 / (1 + np.exp(-(x-x0)/tau01)) * np.exp(-(x-x0)/tau1) + b
+    elif formula == 'v2':
+        return a / (1 + np.exp(-(x-x0)/tau00)) * 1 / (1 + np.exp(-(x-x0)/tau01)) * np.exp(-(x-x0)/tau1) + b
```

### Comparing `lkcom-0.3.2/lkcom/string.py` & `lkcom-0.3.3/lkcom/string.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.3.2/lkcom/util.py` & `lkcom-0.3.3/lkcom/util.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.3.2/lkcom.egg-info/PKG-INFO` & `lkcom-0.3.3/lkcom.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkcom
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python library of useful routines.
 Home-page: https://bitbucket.org/lukaskontenis/lkcom/
 Author: Lukas Kontenis
 Author-email: dse.ssd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lkcom-0.3.2/setup.py` & `lkcom-0.3.3/setup.py`

 * *Files identical despite different names*

