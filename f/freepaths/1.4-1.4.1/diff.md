# Comparing `tmp/freepaths-1.4.tar.gz` & `tmp/freepaths-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freepaths-1.4.tar", last modified: Thu May 25 06:42:16 2023, max compression
+gzip compressed data, was "freepaths-1.4.1.tar", last modified: Tue Jun  6 02:30:55 2023, max compression
```

## Comparing `freepaths-1.4.tar` & `freepaths-1.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-25 06:42:16.638523 freepaths-1.4/
--rw-r--r--   0 r         (1000) r         (1000)     5298 2023-05-25 06:42:16.638523 freepaths-1.4/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     4542 2023-02-22 13:18:35.000000 freepaths-1.4/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-25 06:42:16.638523 freepaths-1.4/freepaths/
--rw-r--r--   0 r         (1000) r         (1000)      869 2023-05-25 05:49:31.000000 freepaths-1.4/freepaths/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     3677 2023-05-11 08:30:00.000000 freepaths-1.4/freepaths/animation.py
--rw-r--r--   0 r         (1000) r         (1000)    10197 2023-05-25 05:32:25.000000 freepaths-1.4/freepaths/config.py
--rw-r--r--   0 r         (1000) r         (1000)     8140 2023-05-25 02:30:39.000000 freepaths-1.4/freepaths/data.py
--rw-r--r--   0 r         (1000) r         (1000)     3122 2023-05-25 06:39:51.000000 freepaths-1.4/freepaths/default_config.py
--rw-r--r--   0 r         (1000) r         (1000)     2650 2023-02-01 09:15:48.000000 freepaths-1.4/freepaths/flight.py
--rw-r--r--   0 r         (1000) r         (1000)     4366 2023-02-03 02:30:26.000000 freepaths-1.4/freepaths/main_mfp_sampling.py
--rw-r--r--   0 r         (1000) r         (1000)     3330 2023-05-11 07:20:52.000000 freepaths-1.4/freepaths/main_tracing.py
--rw-r--r--   0 r         (1000) r         (1000)     8647 2023-01-25 08:49:48.000000 freepaths-1.4/freepaths/maps.py
--rw-r--r--   0 r         (1000) r         (1000)     3797 2023-01-25 08:49:48.000000 freepaths-1.4/freepaths/materials.py
--rw-r--r--   0 r         (1000) r         (1000)      733 2023-01-24 09:26:17.000000 freepaths-1.4/freepaths/move.py
--rw-r--r--   0 r         (1000) r         (1000)      479 2023-05-25 02:30:36.000000 freepaths-1.4/freepaths/options.py
--rw-r--r--   0 r         (1000) r         (1000)     4837 2023-01-25 08:49:48.000000 freepaths-1.4/freepaths/output_info.py
--rw-r--r--   0 r         (1000) r         (1000)    15254 2023-05-25 02:30:34.000000 freepaths-1.4/freepaths/output_plots.py
--rw-r--r--   0 r         (1000) r         (1000)     2348 2023-02-03 08:43:58.000000 freepaths-1.4/freepaths/output_structure.py
--rw-r--r--   0 r         (1000) r         (1000)     8034 2023-05-25 02:30:40.000000 freepaths-1.4/freepaths/phonon.py
--rw-r--r--   0 r         (1000) r         (1000)      580 2023-01-24 09:16:58.000000 freepaths-1.4/freepaths/progress.py
--rw-r--r--   0 r         (1000) r         (1000)     2312 2023-05-25 02:30:38.000000 freepaths-1.4/freepaths/run_phonon.py
--rw-r--r--   0 r         (1000) r         (1000)    28765 2023-05-25 05:20:49.000000 freepaths-1.4/freepaths/scattering.py
--rw-r--r--   0 r         (1000) r         (1000)     1550 2023-01-25 08:51:17.000000 freepaths-1.4/freepaths/scattering_types.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-25 06:42:16.638523 freepaths-1.4/freepaths.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     5298 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      702 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       53 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       31 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)       10 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/top_level.txt
--rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 freepaths-1.4/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-25 06:42:16.638523 freepaths-1.4/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1439 2023-02-03 05:40:49.000000 freepaths-1.4/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-06-06 02:30:55.244647 freepaths-1.4.1/
+-rw-r--r--   0 r         (1000) r         (1000)     5300 2023-06-06 02:30:55.244647 freepaths-1.4.1/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     4542 2023-02-22 13:18:35.000000 freepaths-1.4.1/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-06-06 02:30:55.241314 freepaths-1.4.1/freepaths/
+-rw-r--r--   0 r         (1000) r         (1000)      871 2023-06-06 02:30:40.000000 freepaths-1.4.1/freepaths/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     3677 2023-05-11 08:30:00.000000 freepaths-1.4.1/freepaths/animation.py
+-rw-r--r--   0 r         (1000) r         (1000)    10197 2023-05-25 05:32:25.000000 freepaths-1.4.1/freepaths/config.py
+-rw-r--r--   0 r         (1000) r         (1000)     8371 2023-05-25 08:12:01.000000 freepaths-1.4.1/freepaths/data.py
+-rw-r--r--   0 r         (1000) r         (1000)     3122 2023-05-25 06:39:51.000000 freepaths-1.4.1/freepaths/default_config.py
+-rw-r--r--   0 r         (1000) r         (1000)     2721 2023-05-25 08:50:50.000000 freepaths-1.4.1/freepaths/flight.py
+-rw-r--r--   0 r         (1000) r         (1000)     4366 2023-02-03 02:30:26.000000 freepaths-1.4.1/freepaths/main_mfp_sampling.py
+-rw-r--r--   0 r         (1000) r         (1000)     3330 2023-05-11 07:20:52.000000 freepaths-1.4.1/freepaths/main_tracing.py
+-rw-r--r--   0 r         (1000) r         (1000)     8647 2023-01-25 08:49:48.000000 freepaths-1.4.1/freepaths/maps.py
+-rw-r--r--   0 r         (1000) r         (1000)     3797 2023-01-25 08:49:48.000000 freepaths-1.4.1/freepaths/materials.py
+-rw-r--r--   0 r         (1000) r         (1000)      733 2023-01-24 09:26:17.000000 freepaths-1.4.1/freepaths/move.py
+-rw-r--r--   0 r         (1000) r         (1000)      479 2023-05-25 02:30:36.000000 freepaths-1.4.1/freepaths/options.py
+-rw-r--r--   0 r         (1000) r         (1000)     4837 2023-01-25 08:49:48.000000 freepaths-1.4.1/freepaths/output_info.py
+-rw-r--r--   0 r         (1000) r         (1000)    16123 2023-05-25 08:52:51.000000 freepaths-1.4.1/freepaths/output_plots.py
+-rw-r--r--   0 r         (1000) r         (1000)     2348 2023-02-03 08:43:58.000000 freepaths-1.4.1/freepaths/output_structure.py
+-rw-r--r--   0 r         (1000) r         (1000)     8034 2023-05-25 02:30:40.000000 freepaths-1.4.1/freepaths/phonon.py
+-rw-r--r--   0 r         (1000) r         (1000)      580 2023-01-24 09:16:58.000000 freepaths-1.4.1/freepaths/progress.py
+-rw-r--r--   0 r         (1000) r         (1000)     2312 2023-05-25 02:30:38.000000 freepaths-1.4.1/freepaths/run_phonon.py
+-rw-r--r--   0 r         (1000) r         (1000)    28765 2023-05-25 05:20:49.000000 freepaths-1.4.1/freepaths/scattering.py
+-rw-r--r--   0 r         (1000) r         (1000)     1550 2023-01-25 08:51:17.000000 freepaths-1.4.1/freepaths/scattering_types.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-06-06 02:30:55.244647 freepaths-1.4.1/freepaths.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     5300 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      702 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       53 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       31 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)       10 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/top_level.txt
+-rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 freepaths-1.4.1/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-06-06 02:30:55.244647 freepaths-1.4.1/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1439 2023-02-03 05:40:49.000000 freepaths-1.4.1/setup.py
```

### Comparing `freepaths-1.4/PKG-INFO` & `freepaths-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freepaths
-Version: 1.4
+Version: 1.4.1
 Summary: Phonon Monte Carlo simulator
 Home-page: https://github.com/anufrievroman/freepaths
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `freepaths-1.4/README.md` & `freepaths-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/__main__.py` & `freepaths-1.4.1/freepaths/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """FreePATHS - Free Phonon and THermal Simulator"""
 
 import argparse
 
 import freepaths.main_tracing
 import freepaths.main_mfp_sampling
 
-__version__ = "1.4"
+__version__ = "1.4.1"
 
 # Parse user arguments:
 parser = argparse.ArgumentParser(
                 prog = 'FreePATHS',
                 description = 'Monte Carlo simulator',
                 epilog = 'For more information, visit: https://anufrievroman.gitbook.io/freepaths'
                 )
```

### Comparing `freepaths-1.4/freepaths/animation.py` & `freepaths-1.4.1/freepaths/animation.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/config.py` & `freepaths-1.4.1/freepaths/config.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/data.py` & `freepaths-1.4.1/freepaths/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,39 +42,42 @@
         self.exit_angles = []
         self.free_paths = []
         self.free_paths_along_y = []
         self.frequencies = []
         self.detected_frequencies = []
         self.group_velocities = []
         self.travel_times = []
+        self.mean_free_paths = []
 
     def save_phonon_data(self, ph):
         """Add information about the phonon to the dataset"""
         self.frequencies.append(ph.f)
         self.group_velocities.append(ph.speed)
 
     def save_flight_data(self, flight):
         """Add information about the phonon flight to the dataset"""
         self.initial_angles.append(flight.initial_theta)
         self.exit_angles.append(flight.exit_theta)
         self.free_paths.extend(flight.free_paths)
         self.free_paths_along_y.extend(flight.free_paths_along_y)
         self.travel_times.append(flight.travel_time)
         self.detected_frequencies.append(flight.detected_frequency)
+        self.mean_free_paths.append(flight.mean_free_path)
 
     def write_into_files(self):
         """Write all the data into files"""
         np.savetxt("Data/All free paths.csv", self.free_paths, fmt='%2.4e', delimiter=",", header="L [m]", encoding='utf-8')
         np.savetxt("Data/All free paths in plane.csv", self.free_paths_along_y, fmt='%2.4e', delimiter=",", header="Ly [m]", encoding='utf-8')
         np.savetxt("Data/All initial frequencies.csv", self.frequencies, fmt='%2.4e', delimiter=",", header="f [Hz]", encoding='utf-8')
         np.savetxt("Data/All detected frequencies.csv", self.detected_frequencies, fmt='%2.4e', delimiter=",", header="f [Hz]", encoding='utf-8')
         np.savetxt("Data/All exit angles.csv", self.exit_angles, fmt='%2.4e', delimiter=",", header="Angle [rad]", encoding='utf-8')
         np.savetxt("Data/All initial angles.csv", self.initial_angles, fmt='%2.4e', delimiter=",", header="Angle [rad]", encoding='utf-8')
         np.savetxt("Data/All group velocities.csv", self.group_velocities, fmt='%2.4e', delimiter=",", header="Vg [rad]", encoding='utf-8')
         np.savetxt("Data/All travel times.csv", self.travel_times, fmt='%2.4e', delimiter=",", header="Travel time [s]", encoding='utf-8')
+        np.savetxt("Data/All mean free paths.csv", self.mean_free_paths, fmt='%2.4e', delimiter=",", header="MFPs [m]", encoding='utf-8')
 
 
 class ScatteringData:
     """Statistics of phonon scattering events"""
 
     def __init__(self):
         """Initialize arrays according to the number of segments"""
```

### Comparing `freepaths-1.4/freepaths/default_config.py` & `freepaths-1.4.1/freepaths/default_config.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/flight.py` & `freepaths-1.4.1/freepaths/flight.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,19 @@
         self.time_since_previous_scattering = 0.0
         self.free_paths = []
         self.free_paths_along_y = []
 
     @property
     def mean_free_path(self):
         """Mean value of all free flights"""
-        return sum(self.free_paths)/len(self.free_paths)
+        try:
+            mfp = sum(self.free_paths)/len(self.free_paths)
+        except:
+            mfp = 0
+        return mfp
 
     def add_point_to_path(self):
         """Add a scattering point to the path"""
         self.path.add_point(self.phonon.x, self.phonon.y, self.phonon.z)
 
     def save_free_paths(self):
         """Save current free path to the list of free paths"""
```

### Comparing `freepaths-1.4/freepaths/main_mfp_sampling.py` & `freepaths-1.4.1/freepaths/main_mfp_sampling.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/main_tracing.py` & `freepaths-1.4.1/freepaths/main_tracing.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/maps.py` & `freepaths-1.4.1/freepaths/maps.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/materials.py` & `freepaths-1.4.1/freepaths/materials.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/move.py` & `freepaths-1.4.1/freepaths/move.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/output_info.py` & `freepaths-1.4.1/freepaths/output_info.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/output_plots.py` & `freepaths-1.4.1/freepaths/output_plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 plt.rcParams['legend.frameon'] = False
 plt.rcParams['figure.autolayout'] = True
 plt.rcParams['figure.figsize'] = [5, 3.5]
 plt.rcParams['figure.dpi'] = 200
 plt.rcParams['savefig.dpi'] = 200
 plt.rcParams['legend.fontsize'] = 8
 
-
 def distribution_calculation(filename, data_range, number_of_nodes):
     """Calculate distribution of numbers (histogram) in a given file"""
     data = np.loadtxt(filename, encoding='utf-8')
     if data_range is None:
         data_range = np.max(data)
     distribution = np.zeros((number_of_nodes, 2))
     distribution[:, 0] = np.linspace(0, data_range, number_of_nodes)
@@ -37,19 +36,19 @@
     return distribution
 
 
 def angle_distribution_calculation():
     """Analyse measured phonon angles and create their distribution"""
     all_exit_angles = np.loadtxt("Data/All exit angles.csv", dtype='float', encoding='utf-8')
     initial_angles = np.loadtxt("Data/All initial angles.csv", dtype='float', encoding='utf-8')
-    distribution = np.zeros((180, 3))
-    distribution[:, 0] = range(-90, 90)
+    distribution = np.zeros((360, 3))
+    distribution[:, 0] = range(-180, 180)
     exit_angles = all_exit_angles[all_exit_angles != 0]
-    distribution[:, 1], _ = np.histogram(np.degrees(exit_angles), 180, range=(-90, 90))
-    distribution[:, 2], _ = np.histogram(np.degrees(initial_angles), 180, range=(-90, 90))
+    distribution[:, 1], _ = np.histogram(np.degrees(exit_angles), 360, range=(-180, 180))
+    distribution[:, 2], _ = np.histogram(np.degrees(initial_angles), 360, range=(-180, 180))
     return distribution
 
 
 def wavelength_distribution_calculation(number_of_nodes):
     """Calculate phonon wavelength distribution from their frequencies and velocities"""
     frequencies = np.loadtxt("Data/All initial frequencies.csv", encoding='utf-8')
     speeds = np.loadtxt("Data/All group velocities.csv", encoding='utf-8')
@@ -62,115 +61,128 @@
     return distribution
 
 
 def plot_angle_distribution():
     """Plot distribution of angles"""
     angle_distributions = angle_distribution_calculation()
     fig, ax = plt.subplots()
-    ax.plot(angle_distributions[:, 0], angle_distributions[:, 1], 'b')
-    ax.plot(angle_distributions[:, 0], angle_distributions[:, 2], 'r')
+    ax.plot(angle_distributions[:, 0], angle_distributions[:, 1], 'royalblue')
+    ax.plot(angle_distributions[:, 0], angle_distributions[:, 2], 'deeppink')
     ax.set_xlabel('Angle (degree)', fontsize=12)
     ax.set_ylabel('Number of phonons', fontsize=12)
+    ax.set_ylim(bottom=0)
     ax.legend(["At cold side", "At hot side"])
     fig.savefig("Distribution of angles.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
     np.savetxt('Data/Distribution of angles.csv', angle_distributions, fmt='%1.3e', delimiter=",")
 
 
 def plot_free_path_distribution():
     """Plot distribution of free path"""
     filename = "Data/All free paths.csv"
     free_path_distribution = distribution_calculation(filename, None, cf.number_of_nodes)
     fig, ax = plt.subplots()
-    ax.plot(free_path_distribution[:, 0] * 1e6, free_path_distribution[:, 1])
+    ax.plot(free_path_distribution[:, 0] * 1e6, free_path_distribution[:, 1], 'royalblue')
     ax.set_xlabel('Free flights (μm)', fontsize=12)
     ax.set_ylabel('Number of flights', fontsize=12)
     # ax.set_xlim([0, max(free_path_distribution[:,0])*1e6])
     fig.savefig("Distribution of free paths.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
     np.savetxt('Data/Distribution of free paths.csv', free_path_distribution, fmt='%1.3e', delimiter=",")
 
 
 def plot_frequency_distribution():
     """Plot distribution of frequencies"""
     filename = "Data/All initial frequencies.csv"
     frequency_distribution = distribution_calculation(filename, None, cf.number_of_nodes)
     fig, ax = plt.subplots()
-    ax.plot(frequency_distribution[:, 0], frequency_distribution[:, 1])
+    ax.plot(frequency_distribution[:, 0], frequency_distribution[:, 1], 'royalblue')
     ax.set_xlabel('Frequency (Hz)', fontsize=12)
     ax.set_ylabel('Number of phonons', fontsize=12)
     fig.savefig("Distribution of initial frequencies.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
     np.savetxt('Data/Distribution of initial frequencies.csv', frequency_distribution, fmt='%1.3e', delimiter=",")
 
 
 def plot_wavelength_distribution():
     """Plot distribution of wavelength"""
     wavelength_distribution = wavelength_distribution_calculation(cf.number_of_nodes)
     fig, ax = plt.subplots()
-    ax.plot(wavelength_distribution[:, 0] * 1e9, wavelength_distribution[:, 1])
+    ax.plot(wavelength_distribution[:, 0] * 1e9, wavelength_distribution[:, 1], 'royalblue')
     ax.set_xlabel('Wavelength (nm)', fontsize=12)
     ax.set_ylabel('Number of phonons', fontsize=12)
     fig.savefig("Distribution of wavelengths.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
     np.savetxt('Data/Distribution of wavelengths.csv', wavelength_distribution, fmt='%1.3e', delimiter=",")
 
 
 def plot_travel_time_distribution():
     """Plot distribution of wavelength"""
     travel_time_distribution = distribution_calculation("Data/All travel times.csv", None, cf.number_of_nodes)
     fig, ax = plt.subplots()
-    ax.plot(travel_time_distribution[:, 0] * 1e9, travel_time_distribution[:, 1])
+    ax.plot(travel_time_distribution[:, 0] * 1e9, travel_time_distribution[:, 1], 'royalblue')
     ax.set_xlabel('Travel time (ns)', fontsize=12)
     ax.set_ylabel('Number of phonons', fontsize=12)
     fig.savefig("Distribution of travel times.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
     np.savetxt('Data/Distribution of travel times.csv', travel_time_distribution, fmt='%1.3e', delimiter=",")
 
 
+def plot_mean_free_path_distribution():
+    """Plot distribution of MFP per phonon"""
+    mean_free_path_distribution = distribution_calculation("Data/All mean free paths.csv", None, cf.number_of_nodes)
+    fig, ax = plt.subplots()
+    ax.plot(mean_free_path_distribution[:, 0] * 1e9, mean_free_path_distribution[:, 1], 'royalblue')
+    ax.set_xlabel('Mean free path (nm)', fontsize=12)
+    ax.set_ylabel('Number of phonons', fontsize=12)
+    fig.savefig("Distribution of MFPs.pdf", dpi=300, format='pdf', bbox_inches="tight")
+    if cf.plots_in_terminal: plt.show()
+    np.savetxt('Data/Distribution of MFPs.csv', mean_free_path_distribution, fmt='%1.3e', delimiter=",")
+
+
 def plot_detected_frequency_distribution():
     """Plot distribution of detected frequencies"""
     detected_frequency_distribution = distribution_calculation("Data/All detected frequencies.csv", None, cf.number_of_nodes)
     fig, ax = plt.subplots()
-    ax.plot(detected_frequency_distribution[:, 0], detected_frequency_distribution[:, 1])
+    ax.plot(detected_frequency_distribution[:, 0], detected_frequency_distribution[:, 1], 'royalblue')
     ax.set_xlabel('Frequency (Hz)', fontsize=12)
     ax.set_ylabel('Number of phonons', fontsize=12)
     fig.savefig("Distribution of detected frequencies.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
     np.savetxt('Data/Distribution of detected frequencies.csv', detected_frequency_distribution, fmt='%1.3e', delimiter=",")
 
 
 def plot_velocity_distribution():
     """Plot distribution of group velocities"""
     fig, ax = plt.subplots()
     speeds = np.loadtxt("Data/All group velocities.csv")
     frequencies = np.loadtxt("Data/All initial frequencies.csv")
-    ax.plot(frequencies, speeds, '.')
+    ax.plot(frequencies, speeds, '.', c='royalblue')
     ax.set_xlabel('Frequency (Hz)', fontsize=12)
     ax.set_ylabel('Group velocity (m/s)', fontsize=12)
     fig.savefig('Group velocities.pdf', dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
 
 
 def plot_time_in_segments():
     """Plot time spent in segments"""
     fig, ax = plt.subplots()
     segment, time = np.genfromtxt("Data/Time spent in segments.csv", unpack=True, delimiter=',', usecols=(0, 1), skip_header=1)
-    ax.plot(segment, time, '-')
+    ax.plot(segment, time, '-', c='royalblue')
     ax.set_xlabel('Y (μm)', fontsize=12)
     ax.set_ylabel('Time spent (ns)', fontsize=12)
     fig.savefig("Time spent in segments.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
 
 
 def plot_thermal_conductivity():
     """Plot thermal conductivity against time segment"""
     fig, ax = plt.subplots()
     time, thermal_conductivity = np.genfromtxt("Data/Thermal conductivity.csv", unpack=True, delimiter=',', usecols=(0, 1), skip_header=1)
-    ax.plot(time, thermal_conductivity, linewidth=1)
+    ax.plot(time, thermal_conductivity, linewidth=1, c='royalblue')
     ax.set_ylabel('Thermal conductivity (W/mK)', fontsize=12)
     ax.set_xlabel('Time (ns)', fontsize=12)
     fig.savefig("Thermal conductivity.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
 
 
 def plot_temperature_profile():
@@ -312,14 +324,15 @@
     """Create plots of various distributions"""
     plot_trajectories()
     plot_angle_distribution()
     plot_free_path_distribution()
     plot_frequency_distribution()
     plot_wavelength_distribution()
     plot_travel_time_distribution()
+    plot_mean_free_path_distribution()
     plot_detected_frequency_distribution()
     plot_velocity_distribution()
     plot_time_in_segments()
     plot_thermal_conductivity()
     plot_temperature_profile()
     plot_heat_flux_profile()
     plot_thermal_map()
```

### Comparing `freepaths-1.4/freepaths/output_structure.py` & `freepaths-1.4.1/freepaths/output_structure.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/phonon.py` & `freepaths-1.4.1/freepaths/phonon.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/progress.py` & `freepaths-1.4.1/freepaths/progress.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/run_phonon.py` & `freepaths-1.4.1/freepaths/run_phonon.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/scattering.py` & `freepaths-1.4.1/freepaths/scattering.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths/scattering_types.py` & `freepaths-1.4.1/freepaths/scattering_types.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/freepaths.egg-info/PKG-INFO` & `freepaths-1.4.1/freepaths.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freepaths
-Version: 1.4
+Version: 1.4.1
 Summary: Phonon Monte Carlo simulator
 Home-page: https://github.com/anufrievroman/freepaths
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `freepaths-1.4/freepaths.egg-info/SOURCES.txt` & `freepaths-1.4.1/freepaths.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freepaths-1.4/setup.py` & `freepaths-1.4.1/setup.py`

 * *Files identical despite different names*

