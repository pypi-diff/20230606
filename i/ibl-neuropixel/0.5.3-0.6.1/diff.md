# Comparing `tmp/ibl-neuropixel-0.5.3.tar.gz` & `tmp/ibl-neuropixel-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibl-neuropixel-0.5.3.tar", last modified: Mon Apr 24 09:36:49 2023, max compression
+gzip compressed data, was "ibl-neuropixel-0.6.1.tar", last modified: Tue Jun  6 14:33:25 2023, max compression
```

## Comparing `ibl-neuropixel-0.5.3.tar` & `ibl-neuropixel-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:36:49.742417 ibl-neuropixel-0.5.3/
--rw-rw-rw-   0        0        0     1087 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/LICENSE
--rw-rw-rw-   0        0        0       25 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2015 2023-04-24 09:36:49.741416 ibl-neuropixel-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1369 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 09:36:49.742417 ibl-neuropixel-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-04-24 09:35:44.000000 ibl-neuropixel-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:36:49.708415 ibl-neuropixel-0.5.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:36:49.717416 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/
--rw-rw-rw-   0        0        0     2015 2023-04-24 09:36:49.000000 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-04-24 09:36:49.000000 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:36:49.000000 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-24 09:36:49.000000 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-24 09:36:49.000000 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 09:36:49.739416 ibl-neuropixel-0.5.3/src/neurodsp/
--rw-rw-rw-   0        0        0        0 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/__init__.py
--rw-rw-rw-   0        0        0     6071 2023-04-24 09:18:28.000000 ibl-neuropixel-0.5.3/src/neurodsp/cadzow.py
--rw-rw-rw-   0        0        0     2371 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/cuda_tools.py
--rw-rw-rw-   0        0        0     2763 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/destripe_gpu.py
--rw-rw-rw-   0        0        0     5838 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/filter_gpu.py
--rw-rw-rw-   0        0        0    10529 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/fourier.py
--rw-rw-rw-   0        0        0     7947 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/smooth.py
--rw-rw-rw-   0        0        0     8976 2023-04-19 09:09:00.000000 ibl-neuropixel-0.5.3/src/neurodsp/utils.py
--rw-rw-rw-   0        0        0    33238 2023-04-24 09:18:28.000000 ibl-neuropixel-0.5.3/src/neurodsp/voltage.py
--rw-rw-rw-   0        0        0     4658 2023-04-24 09:18:28.000000 ibl-neuropixel-0.5.3/src/neurodsp/waveforms.py
--rw-rw-rw-   0        0        0    35321 2023-04-24 09:19:36.000000 ibl-neuropixel-0.5.3/src/neuropixel.py
--rw-rw-rw-   0        0        0    33762 2023-04-24 09:35:44.000000 ibl-neuropixel-0.5.3/src/spikeglx.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1087 2022-04-18 09:47:34.000000 ibl-neuropixel-0.6.1/LICENSE
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       25 2022-04-18 12:17:34.000000 ibl-neuropixel-0.6.1/MANIFEST.in
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1910 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1369 2022-06-01 09:21:00.000000 ibl-neuropixel-0.6.1/README.md
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/setup.cfg
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1072 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.1/setup.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:33:25.232391 ibl-neuropixel-0.6.1/src/
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1910 2023-06-06 14:33:25.000000 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      590 2023-06-06 14:33:25.000000 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/SOURCES.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2023-06-06 14:33:25.000000 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/dependency_links.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       57 2023-06-06 14:33:25.000000 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/requires.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       44 2023-06-06 14:33:25.000000 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/top_level.txt
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/src/neurodsp/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        0 2022-04-18 12:01:15.000000 ibl-neuropixel-0.6.1/src/neurodsp/__init__.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     6071 2023-03-07 11:56:59.000000 ibl-neuropixel-0.6.1/src/neurodsp/cadzow.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     2371 2022-04-18 10:38:28.000000 ibl-neuropixel-0.6.1/src/neurodsp/cuda_tools.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     2763 2022-04-20 07:48:28.000000 ibl-neuropixel-0.6.1/src/neurodsp/destripe_gpu.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     5838 2022-04-18 09:54:14.000000 ibl-neuropixel-0.6.1/src/neurodsp/filter_gpu.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    10529 2022-04-18 10:39:58.000000 ibl-neuropixel-0.6.1/src/neurodsp/fourier.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     7947 2022-04-18 14:10:58.000000 ibl-neuropixel-0.6.1/src/neurodsp/smooth.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8976 2022-09-07 17:44:13.000000 ibl-neuropixel-0.6.1/src/neurodsp/utils.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    33322 2023-06-05 17:01:59.000000 ibl-neuropixel-0.6.1/src/neurodsp/voltage.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)    18164 2023-06-06 14:29:50.000000 ibl-neuropixel-0.6.1/src/neurodsp/waveforms.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    35717 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.1/src/neuropixel.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/src/neurowaveforms/
+-rw-r--r--   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.1/src/neurowaveforms/__init__.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     4692 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.1/src/neurowaveforms/model.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    33746 2023-05-15 12:25:43.000000 ibl-neuropixel-0.6.1/src/spikeglx.py
```

### Comparing `ibl-neuropixel-0.5.3/LICENSE` & `ibl-neuropixel-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.3/PKG-INFO` & `ibl-neuropixel-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,64 @@
-Metadata-Version: 2.1
-Name: ibl-neuropixel
-Version: 0.5.3
-Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
-Home-page: https://github.com/int-brain-lab/ibl-neuropixel
-Author: The International Brain Laboratory
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ibl-neuropixel
-Collection of tools to handle Neuropixel 1.0 and 2.0 data
-(documentation coming soon...)
-
-## Installation
-`pip install ibl-neuropixel`
-
-
-## Destriping
-### Getting started
-This relies on a fast fourier transform external library: `pip install pyfftw`.
-
-Minimal working example to destripe a neuropixel binary file. 
-```python
-from pathlib import Path
-from neurodsp.voltage import decompress_destripe_cbin
-sr_file = Path('/datadisk/Data/spike_sorting/pykilosort_tests/imec_385_100s.ap.bin')
-out_file = Path('/datadisk/scratch/imec_385_100s.ap.bin')
-
-decompress_destripe_cbin(sr_file=sr_file, output_file=out_file, nprocesses=8)
-```
-
-### Viewer
-
-The best way to look at the results is to use [viewephys](https://github.com/oliche/viewephys),
-open an ephys viewer on the raw data.
-
-- tick the destipe box.
-- move to a desired location in the file
-- ctr+P will make the gain and axis the same on both windows
-
-![alt text](./docs/raw_bin_viewer_destripe.png "Ephys viewer")
-
-You can then move within the raw data file.
-
-### White Paper
-The following describes the methods implemented in this repository.
-https://doi.org/10.6084/m9.figshare.19705522
-
-## Contribution
-
-Pypi Release checklist:
-```shell
-flake8
-rm -fR dist
-rm -fR build
-python setup.py sdist bdist_wheel
-twine upload dist/*
-#twine upload --repository-url https://test.pypi.org/legacy/ dist/*
-```
-
-
+Metadata-Version: 2.1
+Name: ibl-neuropixel
+Version: 0.6.1
+Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
+Home-page: https://github.com/int-brain-lab/ibl-neuropixel
+Author: The International Brain Laboratory
+Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ibl-neuropixel
+Collection of tools to handle Neuropixel 1.0 and 2.0 data
+(documentation coming soon...)
+
+## Installation
+`pip install ibl-neuropixel`
+
+
+## Destriping
+### Getting started
+This relies on a fast fourier transform external library: `pip install pyfftw`.
+
+Minimal working example to destripe a neuropixel binary file. 
+```python
+from pathlib import Path
+from neurodsp.voltage import decompress_destripe_cbin
+sr_file = Path('/datadisk/Data/spike_sorting/pykilosort_tests/imec_385_100s.ap.bin')
+out_file = Path('/datadisk/scratch/imec_385_100s.ap.bin')
+
+decompress_destripe_cbin(sr_file=sr_file, output_file=out_file, nprocesses=8)
+```
+
+### Viewer
+
+The best way to look at the results is to use [viewephys](https://github.com/oliche/viewephys),
+open an ephys viewer on the raw data.
+
+- tick the destipe box.
+- move to a desired location in the file
+- ctr+P will make the gain and axis the same on both windows
+
+![alt text](./docs/raw_bin_viewer_destripe.png "Ephys viewer")
+
+You can then move within the raw data file.
+
+### White Paper
+The following describes the methods implemented in this repository.
+https://doi.org/10.6084/m9.figshare.19705522
+
+## Contribution
+
+Pypi Release checklist:
+```shell
+flake8
+rm -fR dist
+rm -fR build
+python setup.py sdist bdist_wheel
+twine upload dist/*
+#twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+```
```

### Comparing `ibl-neuropixel-0.5.3/README.md` & `ibl-neuropixel-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.3/setup.py` & `ibl-neuropixel-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     require = [x.strip() for x in f.readlines() if not x.startswith('git+')]
 
 setuptools.setup(
     name="ibl-neuropixel",
-    version="0.5.3",
+    version="0.6.1",
     author="The International Brain Laboratory",
     description="Collection of tools for Neuropixel 1.0 and 2.0 probes data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/int-brain-lab/ibl-neuropixel",
     project_urls={
         "Bug Tracker": "https://github.com/int-brain-lab/ibl-neuropixel/issues",
```

### Comparing `ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/PKG-INFO` & `ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,64 @@
-Metadata-Version: 2.1
-Name: ibl-neuropixel
-Version: 0.5.3
-Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
-Home-page: https://github.com/int-brain-lab/ibl-neuropixel
-Author: The International Brain Laboratory
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ibl-neuropixel
-Collection of tools to handle Neuropixel 1.0 and 2.0 data
-(documentation coming soon...)
-
-## Installation
-`pip install ibl-neuropixel`
-
-
-## Destriping
-### Getting started
-This relies on a fast fourier transform external library: `pip install pyfftw`.
-
-Minimal working example to destripe a neuropixel binary file. 
-```python
-from pathlib import Path
-from neurodsp.voltage import decompress_destripe_cbin
-sr_file = Path('/datadisk/Data/spike_sorting/pykilosort_tests/imec_385_100s.ap.bin')
-out_file = Path('/datadisk/scratch/imec_385_100s.ap.bin')
-
-decompress_destripe_cbin(sr_file=sr_file, output_file=out_file, nprocesses=8)
-```
-
-### Viewer
-
-The best way to look at the results is to use [viewephys](https://github.com/oliche/viewephys),
-open an ephys viewer on the raw data.
-
-- tick the destipe box.
-- move to a desired location in the file
-- ctr+P will make the gain and axis the same on both windows
-
-![alt text](./docs/raw_bin_viewer_destripe.png "Ephys viewer")
-
-You can then move within the raw data file.
-
-### White Paper
-The following describes the methods implemented in this repository.
-https://doi.org/10.6084/m9.figshare.19705522
-
-## Contribution
-
-Pypi Release checklist:
-```shell
-flake8
-rm -fR dist
-rm -fR build
-python setup.py sdist bdist_wheel
-twine upload dist/*
-#twine upload --repository-url https://test.pypi.org/legacy/ dist/*
-```
-
-
+Metadata-Version: 2.1
+Name: ibl-neuropixel
+Version: 0.6.1
+Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
+Home-page: https://github.com/int-brain-lab/ibl-neuropixel
+Author: The International Brain Laboratory
+Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ibl-neuropixel
+Collection of tools to handle Neuropixel 1.0 and 2.0 data
+(documentation coming soon...)
+
+## Installation
+`pip install ibl-neuropixel`
+
+
+## Destriping
+### Getting started
+This relies on a fast fourier transform external library: `pip install pyfftw`.
+
+Minimal working example to destripe a neuropixel binary file. 
+```python
+from pathlib import Path
+from neurodsp.voltage import decompress_destripe_cbin
+sr_file = Path('/datadisk/Data/spike_sorting/pykilosort_tests/imec_385_100s.ap.bin')
+out_file = Path('/datadisk/scratch/imec_385_100s.ap.bin')
+
+decompress_destripe_cbin(sr_file=sr_file, output_file=out_file, nprocesses=8)
+```
+
+### Viewer
+
+The best way to look at the results is to use [viewephys](https://github.com/oliche/viewephys),
+open an ephys viewer on the raw data.
+
+- tick the destipe box.
+- move to a desired location in the file
+- ctr+P will make the gain and axis the same on both windows
+
+![alt text](./docs/raw_bin_viewer_destripe.png "Ephys viewer")
+
+You can then move within the raw data file.
+
+### White Paper
+The following describes the methods implemented in this repository.
+https://doi.org/10.6084/m9.figshare.19705522
+
+## Contribution
+
+Pypi Release checklist:
+```shell
+flake8
+rm -fR dist
+rm -fR build
+python setup.py sdist bdist_wheel
+twine upload dist/*
+#twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+```
```

### Comparing `ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/SOURCES.txt` & `ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 src/neurodsp/cuda_tools.py
 src/neurodsp/destripe_gpu.py
 src/neurodsp/filter_gpu.py
 src/neurodsp/fourier.py
 src/neurodsp/smooth.py
 src/neurodsp/utils.py
 src/neurodsp/voltage.py
-src/neurodsp/waveforms.py
+src/neurodsp/waveforms.py
+src/neurowaveforms/__init__.py
+src/neurowaveforms/model.py
```

### Comparing `ibl-neuropixel-0.5.3/src/neurodsp/cadzow.py` & `ibl-neuropixel-0.6.1/src/neurodsp/cadzow.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.3/src/neurodsp/cuda_tools.py` & `ibl-neuropixel-0.6.1/src/neurodsp/cuda_tools.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.3/src/neurodsp/destripe_gpu.py` & `ibl-neuropixel-0.6.1/src/neurodsp/destripe_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.3/src/neurodsp/filter_gpu.py` & `ibl-neuropixel-0.6.1/src/neurodsp/filter_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.3/src/neurodsp/fourier.py` & `ibl-neuropixel-0.6.1/src/neurodsp/fourier.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.3/src/neurodsp/smooth.py` & `ibl-neuropixel-0.6.1/src/neurodsp/smooth.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.3/src/neurodsp/utils.py` & `ibl-neuropixel-0.6.1/src/neurodsp/utils.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.3/src/neurodsp/voltage.py` & `ibl-neuropixel-0.6.1/src/neurodsp/voltage.py`

 * *Files 1% similar despite different names*

```diff
@@ -747,16 +747,16 @@
             csd[itr[1:-1], :] = np.diff(lfp[itr, :].astype(np.float64), n=2, axis=0) / dx ** 2 * sigma
         elif method == 'kcsd':
             from kcsd import KCSD1D
             # here we could eventually expose the KCSD kwargs
             csd[itr, :] = KCSD1D(
                 h['y'][itr, np.newaxis],
                 lfp[itr, :],
-                h=1.,
-                sigma=1 / 3,
+                h=np.median(np.diff(h['y'][ind])),  # this seems to work well with the current intertrace
+                sigma=sigma,
                 xmin=np.min(h['y'][itr]),
                 xmax=np.max(h['y'][itr]),
                 gdx=np.ceil((np.max(h['y'][itr]) - np.min(h['y'][itr])) / itr.size),
                 lambd=0.,
                 R_init=5.,
                 n_src_init=10000,
                 src_type='gauss').values('CSD')
```

### Comparing `ibl-neuropixel-0.5.3/src/neuropixel.py` & `ibl-neuropixel-0.6.1/src/neuropixel.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,43 +124,52 @@
     # for all, get coordinates
     ch.update(rc2xy(ch['row'], ch['col'], version=version))
     return ch
 
 
 def adc_shifts(version=1, nc=NC):
     """
+    Neuropixel NP1
     The sampling is serial within the same ADC, but it happens at the same time in all ADCs.
     The ADC to channel mapping is done per odd and even channels:
     ADC1: ch1, ch3, ch5, ch7...
     ADC2: ch2, ch4, ch6....
     ADC3: ch33, ch35, ch37...
     ADC4: ch34, ch36, ch38...
     Therefore, channels 1, 2, 33, 34 get sample at the same time. I hope this is more or
     less clear. In 1.0, it is similar, but there we have 32 ADC that sample each 12 channels."
     - Nick on Slack after talking to Carolina - ;-)
 
+    There are 384 channels (each with AP and LFP) divided into 32 groups (each group containing 1 ADC)
+    The ADC cycle is at 30kHz * 13 = 360 kHz (hence the 13 cycles per AP sample).
+    The ADC (from what I understand) goes like this : AP1-AP2-AP3-...-AP11-AP12-LF1-AP1-AP2-...-AP12-LF2-AP1-...
+    A. Wyngaard
+
+    For NP2 there are 16 cycles
+
     The probe always records from all 384 channels; you can disable sites, but they actually still get read back.
     The sample time shifts are always the same for a given channel -- each channel is hardwired to a specific
      ADC and has a specific order in the sampling lineup. So you should always calculate
       the sample shift based on the original channel number. In the SpikeGLX metadata,
       these are listed in the snsSaveChannelSubset field.
 
     :param version: neuropixel major version 1 or 2
     :param nc: number of channels
     """
     if version == 1:
         adc_channels = 12
+        n_cycles = 13
         # version 1 uses 32 ADC that sample 12 channels each
     elif np.floor(version) == 2:
         # version 2 uses 24 ADC that sample 16 channels each
-        adc_channels = 16
+        adc_channels = n_cycles = 16
     adc = np.floor(np.arange(NC) / (adc_channels * 2)) * 2 + np.mod(np.arange(NC), 2)
     sample_shift = np.zeros_like(adc)
     for a in adc:
-        sample_shift[adc == a] = np.arange(adc_channels) / adc_channels
+        sample_shift[adc == a] = np.arange(adc_channels) / n_cycles
     return sample_shift[:nc], adc[:nc]
 
 
 def trace_header(version=1, nshank=1):
     """
     Returns the channel map for the dense layouts used at IBL. The following pairs are commonly used:
     version=1: NP1: returns single shank dense layout with 4 columns in checkerboard pattern
```

### Comparing `ibl-neuropixel-0.5.3/src/spikeglx.py` & `ibl-neuropixel-0.6.1/src/spikeglx.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,15 +581,15 @@
     # for digital nidq types, the key exists but does not contain any information
     if not chmap:
         return {'shank': None, 'col': None, 'row': None, 'flag': None}
     # shank#, col#, row#, drawflag
     # (nb: drawflag is one should be drawn and considered spatial average)
     chmap = np.array([np.float32(cm.split(':')) for cm in chmap])
     return {k: chmap[:, v] for (k, v) in {'shank': 0, 'col': 1, 'row': 2, 'flag': 3}.items()}
-                
+
 
 def _conversion_sample2v_from_meta(meta_data):
     """
     Interpret the meta data to extract an array of conversion factors for each channel
     so the output data is in Volts
     Conversion factor is: int2volt / channelGain
     For Lf/Ap interpret the gain string from metadata
```

