# Comparing `tmp/viewephys-0.2.0.tar.gz` & `tmp/viewephys-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viewephys-0.2.0.tar", last modified: Sat May  7 14:11:12 2022, max compression
+gzip compressed data, was "viewephys-0.2.1.tar", last modified: Tue Jun  6 11:49:37 2023, max compression
```

## Comparing `viewephys-0.2.0.tar` & `viewephys-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-05-07 14:11:12.341134 viewephys-0.2.0/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1071 2022-02-13 09:54:19.000000 viewephys-0.2.0/LICENSE
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1751 2022-05-07 14:11:12.341134 viewephys-0.2.0/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1244 2022-05-07 13:46:22.000000 viewephys-0.2.0/README.md
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2022-05-07 14:11:12.341134 viewephys-0.2.0/setup.cfg
--rw-r--r--   0 olivier   (1000) olivier   (1000)     1087 2022-05-07 13:24:40.000000 viewephys-0.2.0/setup.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-05-07 14:11:12.337134 viewephys-0.2.0/src/
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-05-07 14:11:12.337134 viewephys-0.2.0/src/viewephys/
--rw-r--r--   0 olivier   (1000) olivier   (1000)        0 2022-02-14 20:18:41.000000 viewephys-0.2.0/src/viewephys/__init__.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)      398 2022-02-21 21:44:45.000000 viewephys-0.2.0/src/viewephys/command_line.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)    11070 2022-04-20 13:35:54.000000 viewephys-0.2.0/src/viewephys/gui.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     3962 2022-02-18 16:50:19.000000 viewephys-0.2.0/src/viewephys/nav_file.ui
--rw-r--r--   0 olivier   (1000) olivier   (1000)     7393 2022-04-20 13:42:26.000000 viewephys-0.2.0/src/viewephys/raster.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     3557 2022-02-14 20:18:41.000000 viewephys-0.2.0/src/viewephys/raster.ui
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4075 2021-04-10 21:37:23.000000 viewephys-0.2.0/src/viewephys/viewephys.svg
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-05-07 14:11:12.341134 viewephys-0.2.0/src/viewephys.egg-info/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1751 2022-05-07 14:11:12.000000 viewephys-0.2.0/src/viewephys.egg-info/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      429 2022-05-07 14:11:12.000000 viewephys-0.2.0/src/viewephys.egg-info/SOURCES.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2022-05-07 14:11:12.000000 viewephys-0.2.0/src/viewephys.egg-info/dependency_links.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       63 2022-05-07 14:11:12.000000 viewephys-0.2.0/src/viewephys.egg-info/entry_points.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       36 2022-05-07 14:11:12.000000 viewephys-0.2.0/src/viewephys.egg-info/requires.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       10 2022-05-07 14:11:12.000000 viewephys-0.2.0/src/viewephys.egg-info/top_level.txt
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 11:49:37.213270 viewephys-0.2.1/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1071 2022-02-13 09:54:19.000000 viewephys-0.2.1/LICENSE
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1959 2023-06-06 11:49:37.213270 viewephys-0.2.1/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1475 2023-06-06 11:45:53.000000 viewephys-0.2.1/README.md
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2023-06-06 11:49:37.213270 viewephys-0.2.1/setup.cfg
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     1101 2023-06-06 11:45:53.000000 viewephys-0.2.1/setup.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 11:49:37.209270 viewephys-0.2.1/src/
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 11:49:37.213270 viewephys-0.2.1/src/viewephys/
+-rw-r--r--   0 olivier   (1000) olivier   (1000)        0 2022-02-14 20:18:41.000000 viewephys-0.2.1/src/viewephys/__init__.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)      908 2023-06-06 08:19:09.000000 viewephys-0.2.1/src/viewephys/command_line.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)    11714 2023-06-06 09:39:38.000000 viewephys-0.2.1/src/viewephys/gui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3962 2022-02-18 16:50:19.000000 viewephys-0.2.1/src/viewephys/nav_file.ui
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     8785 2023-01-18 12:23:09.000000 viewephys-0.2.1/src/viewephys/raster.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     3557 2022-02-14 20:18:41.000000 viewephys-0.2.1/src/viewephys/raster.ui
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     4075 2021-04-10 21:37:23.000000 viewephys-0.2.1/src/viewephys/viewephys.svg
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 11:49:37.213270 viewephys-0.2.1/src/viewephys.egg-info/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1959 2023-06-06 11:49:37.000000 viewephys-0.2.1/src/viewephys.egg-info/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      429 2023-06-06 11:49:37.000000 viewephys-0.2.1/src/viewephys.egg-info/SOURCES.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2023-06-06 11:49:37.000000 viewephys-0.2.1/src/viewephys.egg-info/dependency_links.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       63 2023-06-06 11:49:37.000000 viewephys-0.2.1/src/viewephys.egg-info/entry_points.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       51 2023-06-06 11:49:37.000000 viewephys-0.2.1/src/viewephys.egg-info/requires.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       10 2023-06-06 11:49:37.000000 viewephys-0.2.1/src/viewephys.egg-info/top_level.txt
```

### Comparing `viewephys-0.2.0/LICENSE` & `viewephys-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `viewephys-0.2.0/PKG-INFO` & `viewephys-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: viewephys
-Version: 0.2.0
+Version: 0.2.1
 Summary: Raw Neuropixel data viewer for numpy
-Home-page: https://github.com/oliche/viewephys
+Home-page: https://github.com/int-brain-lab/viewephys
 Author: Olivier Winter
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/oliche/viewephys/issues
-Platform: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/int-brain-lab/viewephys/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,15 +16,15 @@
 Neuropixel raw data viewer
 
 ## Installation
 `pip install viewephys`
 
 Alternatively, in development mode:
 ```shell
-git clone https://github.com/oliche/viewephys.git
+git clone https://github.com/int-brain-lab/viewephys.git
 cd viewephys
 pip install -e .
 ```
 
 ### Supported environments
 This is compatible with the [IBL environment](https://github.com/int-brain-lab/iblenv)
 
@@ -38,34 +36,38 @@
 And then follow the install instructions above.
 
 ## Examples
 
 ### Visualize raw binary file
 Activate your environment and type `viewephys`, you can then load a neuropixel binary file using the file menu.
 
+![alt text](./docs/raw_bin_viewer_destripe.png "Ephys viewer ")
+
+Alternatively you can point the viewer to a specific file using the command line:
+```shell
+viewphys -f /path/to/raw.bin
+```
+
 ### Load in a numpy array or slice
 ```python
 # if running ipython, you may have to use the `%gui qt` magic command
 import numpy as np
 from viewephys.gui import viewephys
 nc, ns, fs = (384, 50000, 30000)  # this mimics one second of neuropixel data
 data = np.random.randn(nc, ns) / 1e6  # volts by default
 ve = viewephys(data, fs=fs)
 ```
-
-### stream IBL data
+![alt text](./docs/view_rand_array.png "Ephys viewer")
     
 
 ## Contribution
 Fork and PR.
 
 Pypi Release checklist:
 ```shell
 flake8
 rm -fR dist
 rm -fR build
 python setup.py sdist bdist_wheel
 twine upload dist/*
 #twine upload --repository-url https://test.pypi.org/legacy/ dist/*
 ```
-
-
```

### Comparing `viewephys-0.2.0/README.md` & `viewephys-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Neuropixel raw data viewer
 
 ## Installation
 `pip install viewephys`
 
 Alternatively, in development mode:
 ```shell
-git clone https://github.com/oliche/viewephys.git
+git clone https://github.com/int-brain-lab/viewephys.git
 cd viewephys
 pip install -e .
 ```
 
 ### Supported environments
 This is compatible with the [IBL environment](https://github.com/int-brain-lab/iblenv)
 
@@ -22,25 +22,31 @@
 And then follow the install instructions above.
 
 ## Examples
 
 ### Visualize raw binary file
 Activate your environment and type `viewephys`, you can then load a neuropixel binary file using the file menu.
 
+![alt text](./docs/raw_bin_viewer_destripe.png "Ephys viewer ")
+
+Alternatively you can point the viewer to a specific file using the command line:
+```shell
+viewphys -f /path/to/raw.bin
+```
+
 ### Load in a numpy array or slice
 ```python
 # if running ipython, you may have to use the `%gui qt` magic command
 import numpy as np
 from viewephys.gui import viewephys
 nc, ns, fs = (384, 50000, 30000)  # this mimics one second of neuropixel data
 data = np.random.randn(nc, ns) / 1e6  # volts by default
 ve = viewephys(data, fs=fs)
 ```
-
-### stream IBL data
+![alt text](./docs/view_rand_array.png "Ephys viewer")
     
 
 ## Contribution
 Fork and PR.
 
 Pypi Release checklist:
 ```shell
```

### Comparing `viewephys-0.2.0/setup.py` & `viewephys-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     require = [x.strip() for x in f.readlines() if not x.startswith('git+')]
 
 setuptools.setup(
     name="viewephys",
-    version="0.2.0",
+    version="0.2.1",
     author="Olivier Winter",
     description="Raw Neuropixel data viewer for numpy",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/oliche/viewephys",
+    url="https://github.com/int-brain-lab/viewephys",
     project_urls={
-        "Bug Tracker": "https://github.com/oliche/viewephys/issues",
+        "Bug Tracker": "https://github.com/int-brain-lab/viewephys/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=require,
```

### Comparing `viewephys-0.2.0/src/viewephys/gui.py` & `viewephys-0.2.1/src/viewephys/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,18 +56,21 @@
         if file is None:
             file, _ = QtWidgets.QFileDialog.getOpenFileName(
                 parent=self, caption='Select Raw electrophysiology recording',
                 directory=self.settings.value('bin_file_path'), filter='*.*bin')
         if file == '':
             return
         file = Path(file)
-        self.settings.setValue("path", str(file.parent))
-        self.sr = spikeglx.Reader(file)
+        self.settings.setValue("bin_file_path", str(file.parent))
+        try:
+            self.sr = spikeglx.Reader(file)
+        except AssertionError:
+            self.sr = spikeglx.Reader(file, dtype='int16', nc=384, fs=30000, ns=file.stat().st_size / 384 / 2)
         # enable and set slider
-        self.horizontalSlider.setMaximum(np.floor(self.sr.ns / NSAMP_CHUNK))
+        self.horizontalSlider.setMaximum(int(np.floor(self.sr.ns / NSAMP_CHUNK)))
         tmax = np.floor(self.sr.ns / NSAMP_CHUNK) * NSAMP_CHUNK / self.sr.fs
         self.label_smax.setText(f"{tmax:0.2f}s")
         tlabel = f'{self.sr.file_bin.name} \n \n' \
                  f'NEUROPIXEL {self.sr.major_version} \n' \
                  f'{self.sr.rl} seconds long \n' \
                  f'{self.sr.fs} Hz Sampling Frequency \n' \
                  f'{self.sr.nc} Channels'
@@ -95,30 +98,30 @@
         sos = scipy.signal.butter(**butter_kwargs, output='sos')
         data = scipy.signal.sosfiltfilt(sos, data)
         t0 = first / self.sr.fs * 0
         for k in self.viewers:
             if not self.cbs[k].isChecked():
                 continue
             if k == 'destripe':
-                data = fcn_destripe(x=data, fs=self.sr.fs, channel_labels=True, neuropixel_version=self.sr.major_version)
-            self.viewers[k] = viewephys(data, self.sr.fs, title=k, t0=t0 * T_SCALAR, t_scalar=T_SCALAR, a_scalar=A_SCALAR)
+                data = fcn_destripe(x=data, fs=self.sr.fs, channel_labels=True, h=self.sr.geometry, neuropixel_version=self.sr.major_version)
+            self.viewers[k] = viewephys(data, self.sr.fs, channels=self.sr.geometry, title=k, t0=t0 * T_SCALAR, t_scalar=T_SCALAR, a_scalar=A_SCALAR)
 
     def closeEvent(self, event):
         for k in self.viewers:
             ev = self.viewers[k]
             if ev is not None:
                 ev.close()
         self.close()
 
 
 class EphysViewer(EasyQC):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.ctrl.model.picks = {'sample': np.array([]), 'trace': np.array([]), 'amp': np.array([])}
+        self.ctrl.model.picks = {'sample': np.array([]), 'trace': np.array([]), 'amp': np.array([])}  # TODO ADD CLUSTERS
         self.menufile.setEnabled(True)
         self.settings = QtCore.QSettings('int-brain-lab', 'EphysViewer')
         self.header_curves = {}
         # menus handling
         # menu pick
         self.menupick = self.menuBar().addMenu('&Pick')
         self.action_pick = QtWidgets.QAction('Pick', self)
@@ -181,78 +184,84 @@
         else:
             self.viewBox_seismic.scene().sigMouseClicked.disconnect(self.mouseClickPickingEvent)
 
     def mouseClickPickingEvent(self, event):
         """
         When the pick action is enabled this is triggered on mouse click
         - left button click sets a point
-        - middle button removes a point
+        - shift + left button removes a point
         - control + left does not wrap on maximum around pick
         """
         TR_RANGE = 3
         S_RANGE = int(0.5 / self.ctrl.model.si)
         qxy = self.imageItem_seismic.mapFromScene(event.scenePos())
         s, tr = (qxy.x(), qxy.y())
-        if event.buttons() == QtCore.Qt.MiddleButton:
-            iclose = np.where(np.logical_and(
-                np.abs(self.ctrl.model.picks['sample'] - s) <= (S_RANGE + 1),
-                np.abs(self.ctrl.model.picks['trace'] - tr) <= (TR_RANGE + 1)
-            ))[0]
-            self.ctrl.model.picks = {k: np.delete(self.ctrl.model.picks[k], iclose) for k in self.ctrl.model.picks}
-
-        elif event.buttons() == QtCore.Qt.LeftButton:
-            if event.modifiers() == QtCore.Qt.ControlModifier:
-                tmax, xmax = (int(round(s)), int(round(tr)))
+        # if event.buttons() == QtCore.Qt.MiddleButton:
+        if event.buttons() == QtCore.Qt.LeftButton:
+            if event.modifiers() == QtCore.Qt.ShiftModifier:
+                iclose = np.where(np.logical_and(
+                    np.abs(self.ctrl.model.picks['sample'] - s) <= (S_RANGE + 1),
+                    np.abs(self.ctrl.model.picks['trace'] - tr) <= (TR_RANGE + 1)
+                ))[0]
+                self.ctrl.model.picks = {k: np.delete(self.ctrl.model.picks[k], iclose) for k in self.ctrl.model.picks}
             else:
-                xscale = np.arange(-TR_RANGE, TR_RANGE + 1) + np.round(tr).astype(np.int32)
-                tscale = np.arange(-S_RANGE, S_RANGE + 1) + np.round(s).astype(np.int32)
-                ix = slice(xscale[0], xscale[-1] + 1)
-                it = slice(tscale[0], tscale[-1] + 1)
-
-                out_of_tr_range = xscale[0] < 0 or xscale[-1] > (self.ctrl.model.ntr - 1)
-                out_of_time_range = tscale[0] < 0 or tscale[-1] > (self.ctrl.model.ns - 1)
-
-                if out_of_time_range or out_of_tr_range:
-                    print(xscale, tscale)
-                    return
-                tmax, xmax = np.unravel_index(np.argmax(np.abs(self.ctrl.model.data[it, ix])),
-                                              (S_RANGE * 2 + 1, TR_RANGE * 2 + 1))
-                tmax, xmax = (tscale[tmax], xscale[xmax])
-
-            self.ctrl.model.picks['sample'] = np.r_[self.ctrl.model.picks['sample'], tmax]
-            self.ctrl.model.picks['trace'] = np.r_[self.ctrl.model.picks['trace'], xmax]
-            self.ctrl.model.picks['amp'] = np.r_[self.ctrl.model.picks['amp'], self.ctrl.model.data[tmax, xmax]]
+                if event.modifiers() == QtCore.Qt.ControlModifier:
+                    tmax, xmax = (int(round(s)), int(round(tr)))
+
+                else:
+                    xscale = np.arange(-TR_RANGE, TR_RANGE + 1) + np.round(tr).astype(np.int32)
+                    tscale = np.arange(-S_RANGE, S_RANGE + 1) + np.round(s).astype(np.int32)
+                    ix = slice(xscale[0], xscale[-1] + 1)
+                    it = slice(tscale[0], tscale[-1] + 1)
+
+                    out_of_tr_range = xscale[0] < 0 or xscale[-1] > (self.ctrl.model.ntr - 1)
+                    out_of_time_range = tscale[0] < 0 or tscale[-1] > (self.ctrl.model.ns - 1)
+
+                    if out_of_time_range or out_of_tr_range:
+                        print(xscale, tscale)
+                        return
+                    tmax, xmax = np.unravel_index(np.argmax(np.abs(self.ctrl.model.data[it, ix])),
+                                                  (S_RANGE * 2 + 1, TR_RANGE * 2 + 1))
+                    tmax, xmax = (tscale[tmax], xscale[xmax])
+
+                self.ctrl.model.picks['sample'] = np.r_[self.ctrl.model.picks['sample'], tmax]
+                self.ctrl.model.picks['trace'] = np.r_[self.ctrl.model.picks['trace'], xmax]
+                self.ctrl.model.picks['amp'] = np.r_[self.ctrl.model.picks['amp'], self.ctrl.model.data[tmax, xmax]]
         # updates scatter plot
         self.ctrl.add_scatter(self.ctrl.model.picks['sample'] * self.ctrl.model.si,
                               self.ctrl.model.picks['trace'],
                               label='_picks', rgb=(0, 255, 255))
 
 
-def viewephys(data, fs, channels=None, br=None, title='ephys', t0=0, t_scalar=T_SCALAR, a_scalar=A_SCALAR):
+def viewephys(data, fs, channels=None, br=None, title='ephys', t0=0, t_scalar=T_SCALAR, a_scalar=A_SCALAR,
+              colormap=None):
     """
     :param data: [nc, ns]
     :param fs:
-    :param channels:
+    :param channels: dictionary of trace headers (nc, ) or dataframe (nc, ncolumns)
     :param br:
     :param title:
+    :param colormap: non-standard colormap from colorcet or matplotlib such as "PuOr"
     :return:
     """
 
     easyqc.qt.create_app()
     ev = EphysViewer._get_or_create(title=title)
 
-    if channels is None or br is None:
+    if channels is None:
         channels = trace_header(version=1)
     if data is not None:
         ev.ctrl.update_data(data.T * a_scalar, si=1 / fs * t_scalar, h=channels, taxis=0, t0=t0)
     if br is not None and 'atlas_id' in channels:
         _, ir = ismember(channels['atlas_id'], br.id)
         image = br.rgb[ir].astype(np.uint8)
         image = image[np.newaxis, :, :]
         imitem = pg.ImageItem(image)
         ev.plotItem_header_v.addItem(imitem)
         transform = [1, 0, 0, 0, 1, 0, -0.5, 0, 1.]
         imitem.setTransform(QtGui.QTransform(*transform))
         ev.plotItem_header_v.setLimits(xMin=-.5, xMax=.5)
 
     ev.show()
+    if colormap is not None:
+        ev.setColorMap(colormap)
     return ev
```

### Comparing `viewephys-0.2.0/src/viewephys/nav_file.ui` & `viewephys-0.2.1/src/viewephys/nav_file.ui`

 * *Files identical despite different names*

### Comparing `viewephys-0.2.0/src/viewephys/raster.py` & `viewephys-0.2.1/src/viewephys/raster.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,51 +6,82 @@
 import numpy as np
 import scipy.signal
 
 from PyQt5 import QtWidgets, QtCore, QtGui, uic
 import pyqtgraph as pg
 
 from brainbox.processing import bincount2D
-from brainbox.io.one import SpikeSortingLoader
+from brainbox.io.one import EphysSessionLoader
+from brainbox.io.spikeglx import Streamer
 import one.alf.io as alfio
 from one.alf.files import get_session_path
 import spikeglx
-from neurodsp import voltage
+from neurodsp import voltage, utils
+from ibllib.atlas import BrainRegions
 
 from viewephys.gui import viewephys, SNS_PALETTE
 
 T_BIN = .007  # time bin size in secs
 D_BIN = 10  # depth bin size in um
 YMAX = 4000
 
 
+def view_pid(pid, one):
+    """
+    Display an interactive raster plot for a given probe insertion
+    :param pid:
+    :param one:
+    :return:
+    """
+    eid, pname = one.pid2eid(pid)
+    sl = EphysSessionLoader(eid=eid, one=one)
+    sl.load_trials()
+    sl.load_spike_sorting(pnames=[pname])
+    sr = Streamer(pid=pid, one=one)
+    rv = RasterView()
+    rv.set_model(sr, *sl.load_spike_sorting(dataset_types=['spikes.samples']), trials=sl.trials)
+    return rv
+
+
 def view_raster(bin_file):
+    """
+    Display an interactive raster plot for a given ap binary file on a local server
+    Mostly deprecated as it requires a full session to be downloaded
+    :param bin_file:
+    :return:
+    """
     bin_file = Path(bin_file)
     pname = bin_file.parent.name
     session_path = get_session_path(bin_file)
-    ssl = SpikeSortingLoader(session_path=session_path, pname=pname)
+    ssl = EphysSessionLoader(session_path=session_path, pname=pname)
     spikes, clusters, channels = ssl.load_spike_sorting(dataset_types=['spikes.samples'])
     trials = alfio.load_object(ssl.session_path.joinpath('alf'), 'trials')
     return RasterView(bin_file, spikes, clusters, trials=trials)
 
 
 @dataclass
 class ProbeData:
-    ap_file: Union[str, Path]
     spikes: Union[dict, pd.DataFrame]
     clusters: Union[dict, pd.DataFrame]
     channels: Union[dict, pd.DataFrame] = field(default_factory=dict)
     trials: Union[dict, pd.DataFrame] = field(default_factory=dict)
-
+    sr: Union[spikeglx.Reader, Streamer, str, Path] = None
     def __post_init__(self):
-        self.sr = spikeglx.Reader(self.ap_file)
+        if isinstance(self.sr, str) or isinstance(self.sr, Path):
+            self.sr = spikeglx.Reader(self.ap_file)
+        # TODO set the good units only ?
+        # set the raster data
+        iok = ~np.isnan(self.spikes.depths)
+        self.raster, self.raster_times, self.raster_depths = bincount2D(
+            self.spikes.times[iok], self.spikes.depths[iok], T_BIN, D_BIN)
+        self.br = BrainRegions()
 
 
 class RasterView(QtWidgets.QMainWindow):
-    def __init__(self, bin_file, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
         self.eqcs = []
         super(RasterView, self).__init__(*args, **kwargs)
         # wave by Diana Militano from the Noun Projectp
         uic.loadUi(Path(__file__).parent.joinpath('raster.ui'), self)
         background_color = self.palette().color(self.backgroundRole())
         self.plotItem_raster.setAspectLocked(False)
         self.imageItem_raster = pg.ImageItem()
@@ -60,25 +91,22 @@
         s = self.viewBox_raster.scene()
         # vb.scene().sigMouseMoved.connect(self.mouseMoveEvent)
         s.sigMouseClicked.connect(self.mouseClick)
         self.show()
         self.actionopen.triggered.connect(self.open_file)
         self.settings = QtCore.QSettings('int-brain-lab', 'Raster')
 
-    def set_model(self, ap_file, spikes, clusters, channels=None, trials=None):
-        self.data = ProbeData(ap_file, spikes, clusters, channels=channels, trials=trials)
+    def set_model(self, sr, spikes, clusters, channels=None, trials=None):
+        self.model = ProbeData(spikes, clusters, channels=channels, trials=trials, sr=sr)
         # set image
-        iok = ~np.isnan(spikes.depths)
-        raster, rtimes, depths = bincount2D(
-            spikes.times[iok], spikes.depths[iok], T_BIN, D_BIN)
-        self.imageItem_raster.setImage(np.flip(raster.T))
+        self.imageItem_raster.setImage(self.data.raster.T)
         transform = [T_BIN, 0., 0., 0., D_BIN, 0., -.5, -.5, 1.]
         self.transform = np.array(transform).reshape((3, 3)).T
         self.imageItem_raster.setTransform(QtGui.QTransform(*transform))
-        self.plotItem_raster.setLimits(xMin=0, xMax=rtimes[-1], yMin=0, yMax=depths[-1])
+        self.plotItem_raster.setLimits(xMin=0, xMax=self.data.raster_times[-1], yMin=0, yMax=self.data.raster_depths[-1])
         # set colormap
         cm = pg.colormap.get('Greys', source='matplotlib')  # prepare a linear color map
         bar = pg.ColorBarItem(values=(0, .5), colorMap=cm)  # prepare interactive color bar
         # Have ColorBarItem control colors of img and appear in 'plot':
         bar.setImageItem(self.imageItem_raster)
         ################################################## plot location
         # self.view.layers[label] = {'layer': new_scatter, 'type': 'scatter'}
@@ -93,15 +121,18 @@
                 reward_times=trials['feedback_times'][trials['feedbackType'] == 1])
             self.trial_lines = {}
             for i, k in enumerate(trial_times):
                 self.trial_lines[k] = pg.PlotCurveItem()
                 self.plotItem_raster.addItem(self.trial_lines[k])
                 x = np.tile(trial_times[k][:, np.newaxis], (1, 2)).flatten()
                 y = np.tile(np.array([0, 1, 1, 0]), int(trial_times[k].shape[0] / 2 + 1))[:trial_times[k].shape[0] * 2] * YMAX
-                self.trial_lines[k].setData(x=x.flatten(), y=y.flatten(), pen=pg.mkPen(np.array(SNS_PALETTE[i]) * 256))
+                couleur = np.r_[np.array(SNS_PALETTE[i]) * 255, 22].astype(np.uint8)
+                print(couleur)
+                self.trial_lines[k].setData(x=x.flatten(), y=y.flatten(), pen=pg.mkPen(couleur))
+                # self.trial_lines[k].setVisible(False)
 
     def open_file(self):
         file, _ = QtWidgets.QFileDialog.getOpenFileName(
             parent=self,
             caption='Select Raw electrophysiology recording',
             directory=self.settings.value('bin_file_path'),
             filter='*.*bin')
@@ -112,16 +143,16 @@
 
     def mouseClick(self, event):
         """Draws a line on the raster and display in EasyQC"""
         if not event.double():
             return
         qxy = self.imageItem_raster.mapFromScene(event.scenePos())
         x = qxy.x()
-        self.show_ephys(t0=self.rtimes[int(x - .5)])
-        ymax = np.max(self.depths) + 50
+        self.show_ephys(t0=self.data.raster_times[int(x - .5)])
+        ymax = np.max(self.data.raster_depths) + 50
         self.line_eqc.setData(x=x + np.array([-.5, -.5, .5, .5]),
                               y=np.array([0, ymax, ymax, 0]),
                               pen=pg.mkPen((0, 255, 0)))
 
     def keyPressEvent(self, e):
         """
         page-up / ctrl + a :  gain up
@@ -134,34 +165,33 @@
                 m == QtCore.Qt.ControlModifier and k == QtCore.Qt.Key_A):
             self.imageItem_raster.setLevels([0, self.imageItem_raster.levels[1] / 1.4])
         # page down / ctrl + z
         elif k == QtCore.Qt.Key_PageDown or (
                 m == QtCore.Qt.ControlModifier and k == QtCore.Qt.Key_Z):
             self.imageItem_raster.setLevels([0, self.imageItem_raster.levels[1] * 1.4])
 
-    def show_ephys(self, t0, tlen=1):
+    def show_ephys(self, t0, tlen=.4):
 
-        first = int(t0 * self.sr.fs)
-        last = first + int(self.sr.fs * tlen)
+        first = int(t0 * self.data.sr.fs)
+        last = first + int(self.data.sr.fs * tlen)
 
-        raw = self.sr[first:last, : - self.sr.nsync].T
+        raw = self.data.sr[first:last, : - self.data.sr.nsync].T
 
-        butter_kwargs = {'N': 3, 'Wn': 300 / self.sr.fs * 2, 'btype': 'highpass'}
+        butter_kwargs = {'N': 3, 'Wn': 300 / self.data.sr.fs * 2, 'btype': 'highpass'}
         sos = scipy.signal.butter(**butter_kwargs, output='sos')
         butt = scipy.signal.sosfiltfilt(sos, raw)
-        destripe = voltage.destripe(raw, fs=self.sr.fs)
-
-        self.eqc_raw = viewephys(butt, self.sr.fs, channels=None, br=None, title='butt', t0=t0, t_scalar=1)
-        self.eqc_des = viewephys(destripe, self.sr.fs, channels=None, br=None, title='destripe', t0=t0, t_scalar=1)
-
+        destripe = voltage.destripe(raw, fs=self.data.sr.fs, channel_labels=True)
+        self.eqc_raw = viewephys(butt, self.data.sr.fs, channels=self.data.channels, br=self.data.br, title='butt', t0=t0, t_scalar=1)
+        self.eqc_des = viewephys(destripe, self.data.sr.fs, channels=self.data.channels, br=self.data.br, title='destripe', t0=t0, t_scalar=1)
+        stripes_noise = 20 * np.log10(np.median(utils.rms(butt - destripe)))
         eqc_xrange = [t0 + tlen / 2 - 0.01, t0 + tlen / 2 + 0.01]
         self.eqc_des.viewBox_seismic.setXRange(*eqc_xrange)
         self.eqc_raw.viewBox_seismic.setXRange(*eqc_xrange)
 
         # eqc2 = viewephys(butt - destripe, self.sr.fs, channels=None, br=None, title='diff')
         # overlay spikes
-        tprobe = self.spikes.samples / self.sr.fs
+        tprobe = self.data.spikes.samples / self.data.sr.fs
         slice_spikes = slice(np.searchsorted(tprobe, t0), np.searchsorted(tprobe, t0 + tlen))
         t = tprobe[slice_spikes]
-        c = self.clusters.channels[self.spikes.clusters[slice_spikes]]
+        c = self.data.clusters.channels[self.data.spikes.clusters[slice_spikes]]
         self.eqc_raw.ctrl.add_scatter(t, c)
         self.eqc_des.ctrl.add_scatter(t, c)
```

### Comparing `viewephys-0.2.0/src/viewephys/raster.ui` & `viewephys-0.2.1/src/viewephys/raster.ui`

 * *Files identical despite different names*

### Comparing `viewephys-0.2.0/src/viewephys/viewephys.svg` & `viewephys-0.2.1/src/viewephys/viewephys.svg`

 * *Files identical despite different names*

### Comparing `viewephys-0.2.0/src/viewephys.egg-info/PKG-INFO` & `viewephys-0.2.1/src/viewephys.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: viewephys
-Version: 0.2.0
+Version: 0.2.1
 Summary: Raw Neuropixel data viewer for numpy
-Home-page: https://github.com/oliche/viewephys
+Home-page: https://github.com/int-brain-lab/viewephys
 Author: Olivier Winter
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/oliche/viewephys/issues
-Platform: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/int-brain-lab/viewephys/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,15 +16,15 @@
 Neuropixel raw data viewer
 
 ## Installation
 `pip install viewephys`
 
 Alternatively, in development mode:
 ```shell
-git clone https://github.com/oliche/viewephys.git
+git clone https://github.com/int-brain-lab/viewephys.git
 cd viewephys
 pip install -e .
 ```
 
 ### Supported environments
 This is compatible with the [IBL environment](https://github.com/int-brain-lab/iblenv)
 
@@ -38,34 +36,38 @@
 And then follow the install instructions above.
 
 ## Examples
 
 ### Visualize raw binary file
 Activate your environment and type `viewephys`, you can then load a neuropixel binary file using the file menu.
 
+![alt text](./docs/raw_bin_viewer_destripe.png "Ephys viewer ")
+
+Alternatively you can point the viewer to a specific file using the command line:
+```shell
+viewphys -f /path/to/raw.bin
+```
+
 ### Load in a numpy array or slice
 ```python
 # if running ipython, you may have to use the `%gui qt` magic command
 import numpy as np
 from viewephys.gui import viewephys
 nc, ns, fs = (384, 50000, 30000)  # this mimics one second of neuropixel data
 data = np.random.randn(nc, ns) / 1e6  # volts by default
 ve = viewephys(data, fs=fs)
 ```
-
-### stream IBL data
+![alt text](./docs/view_rand_array.png "Ephys viewer")
     
 
 ## Contribution
 Fork and PR.
 
 Pypi Release checklist:
 ```shell
 flake8
 rm -fR dist
 rm -fR build
 python setup.py sdist bdist_wheel
 twine upload dist/*
 #twine upload --repository-url https://test.pypi.org/legacy/ dist/*
 ```
-
-
```

