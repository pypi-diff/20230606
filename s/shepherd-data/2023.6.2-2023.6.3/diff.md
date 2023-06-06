# Comparing `tmp/shepherd_data-2023.6.2.tar.gz` & `tmp/shepherd_data-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_data-2023.6.2.tar", last modified: Sun Jun  4 18:49:45 2023, max compression
+gzip compressed data, was "shepherd_data-2023.6.3.tar", last modified: Tue Jun  6 10:59:30 2023, max compression
```

## Comparing `shepherd_data-2023.6.2.tar` & `shepherd_data-2023.6.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:45.099721 shepherd_data-2023.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-04 18:49:45.099721 shepherd_data-2023.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-04 18:49:45.099721 shepherd_data-2023.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:45.095721 shepherd_data-2023.6.2/shepherd_data/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/shepherd_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/shepherd_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/shepherd_data/debug_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/shepherd_data/ivonne.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/shepherd_data/mppt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/shepherd_data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:45.099721 shepherd_data-2023.6.2/shepherd_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-04 18:49:45.000000 shepherd_data-2023.6.2/shepherd_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-04 18:49:45.000000 shepherd_data-2023.6.2/shepherd_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:49:45.000000 shepherd_data-2023.6.2/shepherd_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-04 18:49:45.000000 shepherd_data-2023.6.2/shepherd_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-04 18:49:45.000000 shepherd_data-2023.6.2/shepherd_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-04 18:49:45.000000 shepherd_data-2023.6.2/shepherd_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:49:44.000000 shepherd_data-2023.6.2/shepherd_data.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:45.099721 shepherd_data-2023.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/tests/test_cli_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/tests/test_cli_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/tests/test_cli_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/tests/test_cli_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/tests/test_ivonne.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-04 18:49:14.000000 shepherd_data-2023.6.2/tests/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:30.795808 shepherd_data-2023.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-06 10:59:30.795808 shepherd_data-2023.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-06 10:59:30.795808 shepherd_data-2023.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:30.795808 shepherd_data-2023.6.3/shepherd_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/shepherd_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/shepherd_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/shepherd_data/debug_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/shepherd_data/ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/shepherd_data/mppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/shepherd_data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:30.795808 shepherd_data-2023.6.3/shepherd_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-06 10:59:30.000000 shepherd_data-2023.6.3/shepherd_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-06 10:59:30.000000 shepherd_data-2023.6.3/shepherd_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:59:30.000000 shepherd_data-2023.6.3/shepherd_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 10:59:30.000000 shepherd_data-2023.6.3/shepherd_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-06 10:59:30.000000 shepherd_data-2023.6.3/shepherd_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 10:59:30.000000 shepherd_data-2023.6.3/shepherd_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:59:30.000000 shepherd_data-2023.6.3/shepherd_data.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:30.795808 shepherd_data-2023.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/tests/test_cli_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/tests/test_cli_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/tests/test_cli_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/tests/test_cli_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/tests/test_ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 10:58:57.000000 shepherd_data-2023.6.3/tests/test_reader.py
```

### Comparing `shepherd_data-2023.6.2/PKG-INFO` & `shepherd_data-2023.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_data
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-data/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_data-2023.6.2/README.md` & `shepherd_data-2023.6.3/README.md`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.6.2/setup.cfg` & `shepherd_data-2023.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.6.2/shepherd_data/cli.py` & `shepherd_data-2023.6.3/shepherd_data/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def path_to_flist(data_path: Path) -> List[Path]:
     """every path gets transformed to a list of paths
     - if directory: list of files inside
     - if existing file: list with 1 element
     - or else: empty list
     """
-    data_path = Path(data_path).absolute()
+    data_path = Path(data_path).resolve()
     h5files = []
     if data_path.is_file() and data_path.suffix == ".h5":
         h5files.append(data_path)
     elif data_path.is_dir():
         flist = os.listdir(data_path)
         for file in flist:
             fpath = data_path / str(file)
@@ -110,15 +110,15 @@
         logger.info("DS-Factor was invalid was reset to 1'000")
     for file in files:
         logger.info("Extracting IV-Samples from '%s' ...", file.name)
         with Reader(file, verbose=verbose_level >= 2) as shpr:
             # will create a downsampled h5-file (if not existing) and then saving to csv
             ds_file = file.with_suffix(f".downsampled_x{round(ds_factor)}.h5")
             if not ds_file.exists():
-                logger.info("Downsampling '%s' by factor x%s ...", file.name, ds_factor)
+                logger.info("Downsampling '%s' by factor x%f ...", file.name, ds_factor)
                 with Writer(
                     ds_file,
                     mode=shpr.get_mode(),
                     datatype=shpr.get_datatype(),
                     window_samples=shpr.get_window_samples(),
                     cal_data=shpr.get_calibration_data(),
                     verbose=verbose_level >= 2,
@@ -208,21 +208,22 @@
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     for file in files:
         with Reader(file, verbose=verbose_level >= 2) as shpr:
             for _factor in ds_list:
                 if shpr.ds_time.shape[0] / _factor < 1000:
                     logger.warning(
-                        "will skip downsampling for %s because resulting sample-size is too small"
+                        "will skip downsampling for %s because resulting sample-size is too small",
+                        file.name,
                     )
                     break
                 ds_file = file.with_suffix(f".downsampled_x{round(_factor)}.h5")
                 if ds_file.exists():
                     continue
-                logger.info("Downsampling '%s' by factor x%s ...", file.name, _factor)
+                logger.info("Downsampling '%s' by factor x%f ...", file.name, _factor)
                 with Writer(
                     ds_file,
                     mode=shpr.get_mode(),
                     datatype=shpr.get_datatype(),
                     window_samples=shpr.get_window_samples(),
                     cal_data=shpr.get_calibration_data(),
                     verbose=verbose_level >= 2,
```

### Comparing `shepherd_data-2023.6.2/shepherd_data/debug_resampler.py` & `shepherd_data-2023.6.3/shepherd_data/debug_resampler.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.6.2/shepherd_data/ivonne.py` & `shepherd_data-2023.6.3/shepherd_data/ivonne.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self,
         file_path: Path,
         samplerate_sps: Optional[int] = None,
         verbose: bool = True,
     ):
         self._logger.setLevel(logging.INFO if verbose else logging.WARNING)
 
-        self.file_path = Path(file_path)
+        self.file_path = Path(file_path).resolve()
         self.samplerate_sps: int = 50
         if samplerate_sps is not None:
             self.samplerate_sps = samplerate_sps
 
         self.sample_interval_ns: int = int(10**9 // self.samplerate_sps)
         self.sample_interval_s: float = 1 / self.samplerate_sps
 
@@ -64,21 +64,21 @@
                 errno.ENOENT, os.strerror(errno.ENOENT), self.file_path.name
             )
         with open(self.file_path, "rb") as ifr:
             self._df = pickle.load(ifr)  # noqa: S301
         self._refresh_file_stats()
         self._logger.info(
             "Reading data from '%s'\n"
-            "\t- runtime = %s s\n"
-            "\t- size = %s KiB\n"
-            "\t- rate = %s KiB/s",
+            "\t- runtime = %d s\n"
+            "\t- size = %.3f KiB\n"
+            "\t- rate = %.3f KiB/s",
             self.file_path,
             self.runtime_s,
-            round(self.file_size / 2**10, 3),
-            round(self.data_rate / 2**10, 3),
+            self.file_size / 2**10,
+            self.data_rate / 2**10,
         )
         return self
 
     def __exit__(self, *exc):  # type: ignore
         pass
 
     def _refresh_file_stats(self) -> None:
@@ -102,15 +102,15 @@
         :param v_max: Maximum voltage supported by shepherd
         :param pts_per_curve: Number of sampling points of the prototype curve
         :param duration_s: time to stop in seconds, counted from beginning
         """
         if self._df is None:
             raise RuntimeError("IVonne Context was not entered - file not open!")
         if isinstance(duration_s, (float, int)) and self.runtime_s > duration_s:
-            self._logger.info("  -> gets trimmed to %s s", duration_s)
+            self._logger.info("  -> gets trimmed to %f s", duration_s)
             df_elements_n = min(
                 self._df.shape[0], int(duration_s * self.samplerate_sps)
             )
         else:
             df_elements_n = self._df.shape[0]
 
         if shp_output.exists():
@@ -178,15 +178,15 @@
         :param v_max: Maximum voltage supported by shepherd
         :param duration_s: time to stop in seconds, counted from beginning
         :param tracker: VOC or OPT
         """
         if self._df is None:
             raise RuntimeError("IVonne Context was not entered - file not open!")
         if isinstance(duration_s, (float, int)) and self.runtime_s > duration_s:
-            self._logger.info("  -> gets trimmed to %s s", duration_s)
+            self._logger.info("  -> gets trimmed to %f s", duration_s)
             df_elements_n = min(
                 self._df.shape[0], int(duration_s * self.samplerate_sps)
             )
         else:
             df_elements_n = self._df.shape[0]
 
         if shp_output.exists():
@@ -242,15 +242,15 @@
         :param shp_output: Path where the resulting hdf file shall be stored
         :param v_max: Maximum voltage supported by shepherd
         :param duration_s: time to stop in seconds, counted from beginning
         """
         if self._df is None:
             raise RuntimeError("IVonne Context was not entered - file not open!")
         if isinstance(duration_s, (float, int)) and self.runtime_s > duration_s:
-            self._logger.info("  -> gets trimmed to %s s", duration_s)
+            self._logger.info("  -> gets trimmed to %f s", duration_s)
             df_elements_n = min(
                 self._df.shape[0], int(duration_s * self.samplerate_sps)
             )
         else:
             df_elements_n = self._df.shape[0]
 
         if shp_output.exists():
```

### Comparing `shepherd_data-2023.6.2/shepherd_data/mppt.py` & `shepherd_data-2023.6.3/shepherd_data/mppt.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.6.2/shepherd_data/reader.py` & `shepherd_data-2023.6.3/shepherd_data/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,15 +393,15 @@
         if not isinstance(self.file_path, Path):
             return
 
         data = [self.generate_plot_data(start_s, end_s)]
 
         start_str = f"{data[0]['start_s']:.3f}".replace(".", "s")
         end_str = f"{data[0]['end_s']:.3f}".replace(".", "s")
-        plot_path = self.file_path.absolute().with_suffix(
+        plot_path = self.file_path.resolve().with_suffix(
             f".plot_{start_str}_to_{end_str}.png"
         )
         if plot_path.exists():
             return
         self._logger.info("Plot generated, will be saved to '%s'", plot_path.name)
         fig = self.assemble_plot(data, width, height)
         plt.savefig(plot_path)
@@ -420,15 +420,15 @@
         :param width: plot-width
         :param height: plot-height
         """
         start_str = f"{data[0]['start_s']:.3f}".replace(".", "s")
         end_str = f"{data[0]['end_s']:.3f}".replace(".", "s")
         plot_path = (
             Path(plot_path)
-            .absolute()
+            .resolve()
             .with_suffix(f".multiplot_{start_str}_to_{end_str}.png")
         )
         if plot_path.exists():
             return None
         fig = Reader.assemble_plot(data, width, height)
         plt.savefig(plot_path)
         plt.close(fig)
```

### Comparing `shepherd_data-2023.6.2/shepherd_data.egg-info/PKG-INFO` & `shepherd_data-2023.6.3/shepherd_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd-data
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-data/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_data-2023.6.2/shepherd_data.egg-info/SOURCES.txt` & `shepherd_data-2023.6.3/shepherd_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.6.2/tests/conftest.py` & `shepherd_data-2023.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.6.2/tests/test_cli_downsample.py` & `shepherd_data-2023.6.3/tests/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.6.2/tests/test_cli_extract.py` & `shepherd_data-2023.6.3/tests/test_cli_extract.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.6.2/tests/test_cli_plot.py` & `shepherd_data-2023.6.3/tests/test_cli_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         ".plot_0s000_to_10s000.png"
     ).exists()  # full duration of file
 
 
 def test_cli_plot_dir_min(tmp_path: Path) -> None:
     file1_path = generate_h5_file(tmp_path, "hrv_file1.h5")
     file2_path = generate_h5_file(tmp_path, "hrv_file2.h5")
-    res = CliRunner().invoke(cli, ["-vvv", "plot", str(tmp_path.absolute())])
+    res = CliRunner().invoke(cli, ["-vvv", "plot", str(tmp_path.resolve())])
     assert res.exit_code == 0
     assert file1_path.with_suffix(
         ".plot_0s000_to_10s000.png"
     ).exists()  # full duration of file
     assert file2_path.with_suffix(
         ".plot_0s000_to_10s000.png"
     ).exists()  # full duration of file
```

### Comparing `shepherd_data-2023.6.2/tests/test_examples.py` & `shepherd_data-2023.6.3/tests/test_examples.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import pytest
 
 
 @pytest.fixture
 def example_path() -> Path:
-    path = Path(__file__).absolute().parent.parent / "examples"
+    path = Path(__file__).resolve().parent.parent / "examples"
     os.chdir(path)
     return path
 
 
 examples = [
     "example_convert_ivonne.py",
     "example_extract_logs.py",
@@ -19,8 +19,8 @@
     "example_plot_traces.py",
     "example_repair_recordings.py",
 ]
 
 
 @pytest.mark.parametrize("file", examples)
 def test_example_scripts(example_path: Path, file: str) -> None:
-    subprocess.call(f"python {example_path / file}", shell=True)
+    subprocess.check_call(f"python {example_path / file}", shell=True)
```

### Comparing `shepherd_data-2023.6.2/tests/test_ivonne.py` & `shepherd_data-2023.6.3/tests/test_ivonne.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from shepherd_data import Reader
 from shepherd_data import ivonne
 from shepherd_data import mppt
 
 
 @pytest.fixture
 def example_path() -> Path:
-    here = Path(__file__).absolute().parent
+    here = Path(__file__).resolve().parent
     return here.parent / "examples"
 
 
 def test_convert_ivonne(tmp_path: Path, example_path: Path) -> None:
     input_file = "jogging_10m"
     inp_path = example_path / (input_file + ".iv")
     isc_path = tmp_path / (input_file + "_isc.h5")
```

