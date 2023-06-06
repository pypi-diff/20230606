# Comparing `tmp/orplib-1.0.5.tar.gz` & `tmp/orplib-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orplib-1.0.5.tar", last modified: Mon Jun  5 21:27:00 2023, max compression
+gzip compressed data, was "orplib-1.0.6.tar", last modified: Tue Jun  6 16:13:54 2023, max compression
```

## Comparing `orplib-1.0.5.tar` & `orplib-1.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.443391 orplib-1.0.5/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       23 2023-05-11 21:09:19.000000 orplib-1.0.5/MANIFEST.in
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7207 2023-06-05 21:27:00.443391 orplib-1.0.5/PKG-INFO
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6777 2023-05-11 21:32:45.000000 orplib-1.0.5/README.md
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      101 2023-04-14 19:45:52.000000 orplib-1.0.5/pyproject.toml
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      821 2023-06-05 21:27:00.443391 orplib-1.0.5/setup.cfg
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.440392 orplib-1.0.5/src/
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.442391 orplib-1.0.5/src/orpl/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      317 2023-05-12 18:34:44.000000 orplib-1.0.5/src/orpl/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       89 2023-06-05 21:20:32.000000 orplib-1.0.5/src/orpl/__main__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    15209 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/baseline_removal.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    16694 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/bubblegif.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     8250 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/calibration.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     3772 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/cosmic_ray.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.442391 orplib-1.0.5/src/orpl/data/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/data/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    63150 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/data/synthetic_presets.json
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1179 2023-06-05 21:21:11.000000 orplib-1.0.5/src/orpl/datatypes.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    10430 2023-06-05 21:21:53.000000 orplib-1.0.5/src/orpl/file_io.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.442391 orplib-1.0.5/src/orpl/gui/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/gui/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1100 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/gui/mplcanvas.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    28290 2023-05-17 15:11:57.000000 orplib-1.0.5/src/orpl/gui/orplGUI.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.442391 orplib-1.0.5/src/orpl/gui/uis/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/gui/uis/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    30696 2023-05-11 19:59:11.000000 orplib-1.0.5/src/orpl/gui/uis/ui_mainWindow.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1846 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/metrics.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     2135 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/normalization.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       92 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/pipelines.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     4566 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/plot.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7014 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/synthetic.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.443391 orplib-1.0.5/src/orplib.egg-info/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7207 2023-06-05 21:27:00.000000 orplib-1.0.5/src/orplib.egg-info/PKG-INFO
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      705 2023-06-05 21:27:00.000000 orplib-1.0.5/src/orplib.egg-info/SOURCES.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        1 2023-06-05 21:27:00.000000 orplib-1.0.5/src/orplib.egg-info/dependency_links.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      161 2023-06-05 21:27:00.000000 orplib-1.0.5/src/orplib.egg-info/requires.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        5 2023-06-05 21:27:00.000000 orplib-1.0.5/src/orplib.egg-info/top_level.txt
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.625627 orplib-1.0.6/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       23 2023-05-11 21:09:19.000000 orplib-1.0.6/MANIFEST.in
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7207 2023-06-06 16:13:54.625627 orplib-1.0.6/PKG-INFO
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6777 2023-05-11 21:32:45.000000 orplib-1.0.6/README.md
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      101 2023-04-14 19:45:52.000000 orplib-1.0.6/pyproject.toml
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      821 2023-06-06 16:13:54.625627 orplib-1.0.6/setup.cfg
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.622627 orplib-1.0.6/src/
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.624627 orplib-1.0.6/src/orpl/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      317 2023-05-12 18:34:44.000000 orplib-1.0.6/src/orpl/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       89 2023-06-06 16:02:21.000000 orplib-1.0.6/src/orpl/__main__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    15209 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/baseline_removal.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    16694 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/bubblegif.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     8250 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/calibration.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     3772 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/cosmic_ray.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.624627 orplib-1.0.6/src/orpl/data/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/data/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    63150 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/data/synthetic_presets.json
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1163 2023-06-06 16:05:52.000000 orplib-1.0.6/src/orpl/datatypes.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    10430 2023-06-06 16:05:49.000000 orplib-1.0.6/src/orpl/file_io.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.624627 orplib-1.0.6/src/orpl/gui/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/gui/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1100 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/gui/mplcanvas.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    28411 2023-06-06 16:05:46.000000 orplib-1.0.6/src/orpl/gui/orplGUI.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.624627 orplib-1.0.6/src/orpl/gui/uis/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/gui/uis/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    30648 2023-06-06 15:27:30.000000 orplib-1.0.6/src/orpl/gui/uis/ui_mainWindow.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1846 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/metrics.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     2135 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/normalization.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       92 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/pipelines.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     4566 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/plot.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7014 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/synthetic.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.625627 orplib-1.0.6/src/orplib.egg-info/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7207 2023-06-06 16:13:54.000000 orplib-1.0.6/src/orplib.egg-info/PKG-INFO
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      705 2023-06-06 16:13:54.000000 orplib-1.0.6/src/orplib.egg-info/SOURCES.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        1 2023-06-06 16:13:54.000000 orplib-1.0.6/src/orplib.egg-info/dependency_links.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      161 2023-06-06 16:13:54.000000 orplib-1.0.6/src/orplib.egg-info/requires.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        5 2023-06-06 16:13:54.000000 orplib-1.0.6/src/orplib.egg-info/top_level.txt
```

### Comparing `orplib-1.0.5/PKG-INFO` & `orplib-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orplib
-Version: 1.0.5
+Version: 1.0.6
 Summary: Open Raman Processing Library
 Home-page: https://github.com/mr-sheg/orpl
 Author: Guillaume Sheehy
 Author-email: guillaume.sheehy@polymtl.ca
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `orplib-1.0.5/README.md` & `orplib-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/setup.cfg` & `orplib-1.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = orplib
-version = 1.0.5
+version = 1.0.6
 author = Guillaume Sheehy
 author_email = guillaume.sheehy@polymtl.ca
 description = Open Raman Processing Library
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 url = https://github.com/mr-sheg/orpl
```

### Comparing `orplib-1.0.5/src/orpl/baseline_removal.py` & `orplib-1.0.6/src/orpl/baseline_removal.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orpl/bubblegif.py` & `orplib-1.0.6/src/orpl/bubblegif.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orpl/calibration.py` & `orplib-1.0.6/src/orpl/calibration.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orpl/cosmic_ray.py` & `orplib-1.0.6/src/orpl/cosmic_ray.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orpl/data/synthetic_presets.json` & `orplib-1.0.6/src/orpl/data/synthetic_presets.json`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orpl/datatypes.py` & `orplib-1.0.6/src/orpl/datatypes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Type
 
-from numpy import ndarray
+from numpy import expand_dims, ndarray
 
 
 @dataclass(frozen=True)
 class Acquisition_info:
     exposure_time: float  # [ms]
     n_accumulations: int
     laser_power: float
@@ -29,15 +29,15 @@
     accumulations: ndarray
     background: ndarray
     nbins: int = field(init=False)
     naccumulations: int = field(init=False)
     mean_spectrum: ndarray = field(init=False)
 
     def __post_init__(self):
-        if self.accumulations.ndim > 1:
-            object.__setattr__(self, "naccumulations", self.accumulations.shape[1])
-            object.__setattr__(self, "mean_spectrum", self.accumulations.mean(axis=1))
-        else:
-            object.__setattr__(self, "naccumulations", 1)
-            object.__setattr__(self, "mean_spectrum", self.accumulations)
+        if self.accumulations.ndim < 2:
+            object.__setattr__(
+                self, "accumulations", expand_dims(self.accumulations, axis=1)
+            )
 
+        object.__setattr__(self, "naccumulations", self.accumulations.shape[1])
+        object.__setattr__(self, "mean_spectrum", self.accumulations.mean(axis=1))
         object.__setattr__(self, "nbins", self.accumulations.shape[0])
```

### Comparing `orplib-1.0.5/src/orpl/file_io.py` & `orplib-1.0.6/src/orpl/file_io.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orpl/gui/mplcanvas.py` & `orplib-1.0.6/src/orpl/gui/mplcanvas.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orpl/gui/orplGUI.py` & `orplib-1.0.6/src/orpl/gui/orplGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,20 +173,20 @@
         self.boxProcessedSignal.setLayout(self.processedDataPlot.createLayout())
         self.boxBaselineFit.setLayout(self.baselineFitPlot.createLayout())
         self.boxIRFCorrection.setLayout(self.irfCorrectionPlot.createLayout())
 
     def connectSlots(self):
         # File IO tab
         self.buttonSelectDirectory.clicked.connect(self.select_working_directory)
-        self.buttonSelectSpectra.clicked.connect(self.select_data)
+        self.buttonLoadSpectra.clicked.connect(self.load_spectra)
         self.treeViewFiles.selectionModel().selectionChanged.connect(
             self.selected_file_changed
         )
-        self.buttonSelectXref.clicked.connect(self.select_xref)
-        self.buttonSelectYref.clicked.connect(self.select_yref)
+        self.buttonLoadXref.clicked.connect(self.load_xref)
+        self.buttonLoadYref.clicked.connect(self.load_yref)
         self.buttonDropSpectra.clicked.connect(self.drop_data)
         self.buttonDropXref.clicked.connect(self.drop_xref)
         self.buttonDropYref.clicked.connect(self.drop_yref)
 
         # Processing tab
         self.spinBoxLeftCrop.valueChanged.connect(self.left_crop_changed)
         self.spinBoxRightCrop.valueChanged.connect(self.right_crop_changed)
@@ -260,27 +260,29 @@
         if new_dir:
             self.treeViewFiles.setRootIndex(self.file_system_model.index(new_dir))
             self.textEditDataDir.setText(new_dir)
             self.textEditExportDir.setText(new_dir)
 
         logger.info("Changed data directory - %s", new_dir)
 
-    def select_data(self):
+    def load_spectra(self):
         # Load selected data
         self.raw_spectra = []
         for file in self.get_selected_files():
             try:
                 spectrum = file_io.load_file(file)
                 self.raw_spectra.append(spectrum)
                 logger.info("Loaded data file - %s", file)
             except Exception:
                 logger.error(traceback.format_exc())
 
         if not self.raw_spectra:
             return
+        else:
+            print(self.raw_spectra[0].accumulations.shape)
 
         # Update processing controls
         spectrum_length = self.raw_spectra[0].nbins
         self.spinBoxLeftCrop.setMaximum(spectrum_length)
         self.spinBoxLeftCrop.setValue(0)
         self.spinBoxRightCrop.setMaximum(spectrum_length)
         self.spinBoxRightCrop.setValue(spectrum_length)
@@ -288,15 +290,15 @@
         self.spinBoxHWS.setMaximum(spectrum_length)
         self.spinBoxNormBand.setMaximum(spectrum_length)
 
         # Update plots
         self.plot_loaded_data()
         self.plot_raw_spectra()
 
-    def select_xref(self):
+    def load_xref(self):
         selected_file = self.get_selected_files()
 
         if len(selected_file) == 0:
             return
         elif len(selected_file) > 1:
             error_dialog = QErrorMessage()
             error_dialog.showMessage(
@@ -316,15 +318,15 @@
         self.xaxis = xaxis
 
         # Update xaxis dependant control
         self.spinBoxNormBand.setMaximum(max(xaxis))
 
         self.plot_xref(xref)
 
-    def select_yref(self):
+    def load_yref(self):
         selected_file = self.get_selected_files()
 
         if len(selected_file) == 0:
             return
         elif len(selected_file) > 1:
             error_dialog = QErrorMessage()
             error_dialog.showMessage(
@@ -400,17 +402,19 @@
         logger.info("Plotting Instrument Response Function")
         # Update Y-ref plot
         ax = self.yrefPlot.canvas.axes
         ax.clear()
         if self.irf is not None:
             if self.xaxis is None:
                 ax.plot(self.irf)
+                ax.set_xlabel(r"Camera pixel [au]")
             else:
                 ax.plot(self.xaxis, self.irf)
-        ax.set_xlabel("Camera pixel [au]")
+                ax.set_xlabel(r"Raman Shift [cm$^{-1}$]")
+
         ax.set_ylabel("Intensity [counts]")
         ax.figure.tight_layout()
         ax.figure.canvas.draw()
         self.yrefPlot.toolbar.update()
 
     # Tab Processing
 
@@ -518,15 +522,15 @@
             background_ = crfilter_single(background_)
             if background_.ndim != spectrum_.ndim:
                 spectrum_ = spectrum_ - np.expand_dims(background_, axis=1)
             else:
                 spectrum_ = spectrum_ - background_
 
         # Combining accumulations
-        if spectrum.naccumulations > 1:
+        if spectrum_.ndim > 1:
             spectrum_ = spectrum_.mean(axis=1)
 
         # IRF correction
         if self.irf is not None:
             spectrum_ = spectrum_ / self.irf[lbound:rbound]
         irf_correction = spectrum_
 
@@ -592,15 +596,15 @@
                 lbound = self.spinBoxLeftCrop.value()
                 rbound = self.spinBoxRightCrop.value()
                 xaxis = self.xaxis[lbound:rbound]
                 ax.plot(xaxis, raman)
                 ax.set_xlabel(r"Raman shift [cm$^{-1}$]")
             else:
                 ax.plot(raman)
-                ax.set_xlabel("Camera pixel")
+                ax.set_xlabel(r"Camera pixel")
 
         if self.radioButtonNoNorm.isChecked():
             ax.set_ylabel("Intensity [counts]")
         else:
             ax.set_ylabel("Normalized Intensity [au]")
 
         ax.figure.tight_layout()
```

### Comparing `orplib-1.0.5/src/orpl/gui/uis/ui_mainWindow.py` & `orplib-1.0.6/src/orpl/gui/uis/ui_mainWindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_mainWindow(object):
     def setupUi(self, mainWindow):
         mainWindow.setObjectName("mainWindow")
-        mainWindow.resize(921, 715)
+        mainWindow.resize(881, 663)
         self.centralwidget = QtWidgets.QWidget(mainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.horizontalLayout = QtWidgets.QHBoxLayout(self.centralwidget)
         self.horizontalLayout.setObjectName("horizontalLayout")
         self.tabWidget = QtWidgets.QTabWidget(self.centralwidget)
         self.tabWidget.setObjectName("tabWidget")
         self.tabFileIO = QtWidgets.QWidget()
@@ -79,22 +79,22 @@
         self.groupBox.setObjectName("groupBox")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.groupBox)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.groupBox_4 = QtWidgets.QGroupBox(self.groupBox)
         self.groupBox_4.setObjectName("groupBox_4")
         self.horizontalLayout_14 = QtWidgets.QHBoxLayout(self.groupBox_4)
         self.horizontalLayout_14.setObjectName("horizontalLayout_14")
-        self.buttonSelectSpectra = QtWidgets.QPushButton(self.groupBox_4)
+        self.buttonLoadSpectra = QtWidgets.QPushButton(self.groupBox_4)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.buttonSelectSpectra.sizePolicy().hasHeightForWidth())
-        self.buttonSelectSpectra.setSizePolicy(sizePolicy)
-        self.buttonSelectSpectra.setObjectName("buttonSelectSpectra")
-        self.horizontalLayout_14.addWidget(self.buttonSelectSpectra)
+        sizePolicy.setHeightForWidth(self.buttonLoadSpectra.sizePolicy().hasHeightForWidth())
+        self.buttonLoadSpectra.setSizePolicy(sizePolicy)
+        self.buttonLoadSpectra.setObjectName("buttonLoadSpectra")
+        self.horizontalLayout_14.addWidget(self.buttonLoadSpectra)
         self.buttonDropSpectra = QtWidgets.QPushButton(self.groupBox_4)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.buttonDropSpectra.sizePolicy().hasHeightForWidth())
         self.buttonDropSpectra.setSizePolicy(sizePolicy)
         self.buttonDropSpectra.setText("")
@@ -106,22 +106,22 @@
         self.verticalLayout_2.addLayout(self.horizontalLayout_11)
         self.groupBox_2 = QtWidgets.QGroupBox(self.groupBox)
         self.groupBox_2.setObjectName("groupBox_2")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.groupBox_2)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.horizontalLayout_10 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_10.setObjectName("horizontalLayout_10")
-        self.buttonSelectXref = QtWidgets.QPushButton(self.groupBox_2)
+        self.buttonLoadXref = QtWidgets.QPushButton(self.groupBox_2)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.buttonSelectXref.sizePolicy().hasHeightForWidth())
-        self.buttonSelectXref.setSizePolicy(sizePolicy)
-        self.buttonSelectXref.setObjectName("buttonSelectXref")
-        self.horizontalLayout_10.addWidget(self.buttonSelectXref)
+        sizePolicy.setHeightForWidth(self.buttonLoadXref.sizePolicy().hasHeightForWidth())
+        self.buttonLoadXref.setSizePolicy(sizePolicy)
+        self.buttonLoadXref.setObjectName("buttonLoadXref")
+        self.horizontalLayout_10.addWidget(self.buttonLoadXref)
         self.buttonDropXref = QtWidgets.QPushButton(self.groupBox_2)
         self.buttonDropXref.setText("")
         self.buttonDropXref.setObjectName("buttonDropXref")
         self.horizontalLayout_10.addWidget(self.buttonDropXref)
         self.verticalLayout_3.addLayout(self.horizontalLayout_10)
         self.radioButtonTylenol = QtWidgets.QRadioButton(self.groupBox_2)
         self.radioButtonTylenol.setChecked(True)
@@ -134,22 +134,22 @@
         self.verticalLayout_2.addWidget(self.groupBox_2)
         self.groupBox_3 = QtWidgets.QGroupBox(self.groupBox)
         self.groupBox_3.setObjectName("groupBox_3")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.groupBox_3)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
         self.horizontalLayout_9 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_9.setObjectName("horizontalLayout_9")
-        self.buttonSelectYref = QtWidgets.QPushButton(self.groupBox_3)
+        self.buttonLoadYref = QtWidgets.QPushButton(self.groupBox_3)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.buttonSelectYref.sizePolicy().hasHeightForWidth())
-        self.buttonSelectYref.setSizePolicy(sizePolicy)
-        self.buttonSelectYref.setObjectName("buttonSelectYref")
-        self.horizontalLayout_9.addWidget(self.buttonSelectYref)
+        sizePolicy.setHeightForWidth(self.buttonLoadYref.sizePolicy().hasHeightForWidth())
+        self.buttonLoadYref.setSizePolicy(sizePolicy)
+        self.buttonLoadYref.setObjectName("buttonLoadYref")
+        self.horizontalLayout_9.addWidget(self.buttonLoadYref)
         self.buttonDropYref = QtWidgets.QPushButton(self.groupBox_3)
         self.buttonDropYref.setText("")
         self.buttonDropYref.setObjectName("buttonDropYref")
         self.horizontalLayout_9.addWidget(self.buttonDropYref)
         self.verticalLayout_4.addLayout(self.horizontalLayout_9)
         self.radioButtonNIST = QtWidgets.QRadioButton(self.groupBox_3)
         self.radioButtonNIST.setEnabled(False)
@@ -169,15 +169,15 @@
         self.horizontalLayout_16 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_16.setObjectName("horizontalLayout_16")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout()
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.processingToolBox = QtWidgets.QToolBox(self.tabProcessing)
         self.processingToolBox.setObjectName("processingToolBox")
         self.pageCRR = QtWidgets.QWidget()
-        self.pageCRR.setGeometry(QtCore.QRect(0, 0, 122, 342))
+        self.pageCRR.setGeometry(QtCore.QRect(0, 0, 116, 290))
         self.pageCRR.setObjectName("pageCRR")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.pageCRR)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.label_4 = QtWidgets.QLabel(self.pageCRR)
         self.label_4.setObjectName("label_4")
         self.verticalLayout_6.addWidget(self.label_4)
         self.spinBoxLeftCrop = QtWidgets.QSpinBox(self.pageCRR)
@@ -234,15 +234,15 @@
         self.spinBoxSCRRstd.setSingleStep(0.01)
         self.spinBoxSCRRstd.setObjectName("spinBoxSCRRstd")
         self.verticalLayout_10.addWidget(self.spinBoxSCRRstd)
         spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_10.addItem(spacerItem2)
         self.processingToolBox.addItem(self.page_3, "")
         self.page_2 = QtWidgets.QWidget()
-        self.page_2.setGeometry(QtCore.QRect(0, 0, 226, 335))
+        self.page_2.setGeometry(QtCore.QRect(0, 0, 226, 258))
         self.page_2.setObjectName("page_2")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.page_2)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.comboBoxBRAlgorithm = QtWidgets.QComboBox(self.page_2)
         self.comboBoxBRAlgorithm.setObjectName("comboBoxBRAlgorithm")
         self.comboBoxBRAlgorithm.addItem("")
         self.comboBoxBRAlgorithm.addItem("")
@@ -434,21 +434,21 @@
         self.buttonSelectDirectory.setText(_translate("mainWindow", "Select Directory"))
         self.boxDataSelection.setTitle(_translate("mainWindow", "Selected Spectrum"))
         self.boxDataPlot.setTitle(_translate("mainWindow", "Loaded Data"))
         self.boxXrefPlot.setTitle(_translate("mainWindow", "X Reference"))
         self.boxYrefPlot.setTitle(_translate("mainWindow", "Y Reference"))
         self.groupBox.setTitle(_translate("mainWindow", "File selection"))
         self.groupBox_4.setTitle(_translate("mainWindow", "Spectra"))
-        self.buttonSelectSpectra.setText(_translate("mainWindow", "Select Spectra"))
+        self.buttonLoadSpectra.setText(_translate("mainWindow", "Load Spectra"))
         self.groupBox_2.setTitle(_translate("mainWindow", "X-axis Calibration"))
-        self.buttonSelectXref.setText(_translate("mainWindow", "Select X-reference"))
+        self.buttonLoadXref.setText(_translate("mainWindow", "Load X-reference"))
         self.radioButtonTylenol.setText(_translate("mainWindow", "Tylenol"))
         self.radioButtonNylon.setText(_translate("mainWindow", "Nylon"))
         self.groupBox_3.setTitle(_translate("mainWindow", "Y-axis Calibration"))
-        self.buttonSelectYref.setText(_translate("mainWindow", "Select Y-reference"))
+        self.buttonLoadYref.setText(_translate("mainWindow", "Load Y-reference"))
         self.radioButtonNIST.setText(_translate("mainWindow", "NIST SRM-2241"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tabFileIO), _translate("mainWindow", "File IO"))
         self.label_4.setText(_translate("mainWindow", "Crop from left"))
         self.label_5.setText(_translate("mainWindow", "Crop from right"))
         self.processingToolBox.setItemText(self.processingToolBox.indexOf(self.pageCRR), _translate("mainWindow", "Xaxis range"))
         self.checkBoxMultiCRR.setText(_translate("mainWindow", "Multi-accumulation Filter"))
         self.label_10.setText(_translate("mainWindow", "Width"))
```

### Comparing `orplib-1.0.5/src/orpl/metrics.py` & `orplib-1.0.6/src/orpl/metrics.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orpl/normalization.py` & `orplib-1.0.6/src/orpl/normalization.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orpl/plot.py` & `orplib-1.0.6/src/orpl/plot.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orpl/synthetic.py` & `orplib-1.0.6/src/orpl/synthetic.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.5/src/orplib.egg-info/PKG-INFO` & `orplib-1.0.6/src/orplib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orplib
-Version: 1.0.5
+Version: 1.0.6
 Summary: Open Raman Processing Library
 Home-page: https://github.com/mr-sheg/orpl
 Author: Guillaume Sheehy
 Author-email: guillaume.sheehy@polymtl.ca
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `orplib-1.0.5/src/orplib.egg-info/SOURCES.txt` & `orplib-1.0.6/src/orplib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

