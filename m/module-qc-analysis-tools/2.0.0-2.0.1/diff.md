# Comparing `tmp/module_qc_analysis_tools-2.0.0.tar.gz` & `tmp/module_qc_analysis_tools-2.0.1.tar.gz`

## Comparing `module_qc_analysis_tools-2.0.0.tar` & `module_qc_analysis_tools-2.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/.flake8
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/.gitmodules
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/_version.py
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/LP_MODE.py
--rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
--rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/TUNING.py
--rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/__main__.py
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/globals.py
--rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/load_yarr_scans.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/main.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/overwrite_config.py
--rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/update_chip_config.py
--rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/analysis_cuts.json
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/pixel_classification.json
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/schema/info_schema.json
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
--rw-r--r--   0        0        0    33358 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/analysis.py
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/classification.py
--rw-r--r--   0        0        0    36639 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/misc.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/LICENSE
--rw-r--r--   0        0        0    25300 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/README.md
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    27421 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/.flake8
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/.gitmodules
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/tbump.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/_version.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
+-rw-r--r--   0        0        0    24871 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/TUNING.py
+-rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/globals.py
+-rwxr-xr-x   0        0        0     8442 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/load_yarr_scans.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/main.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/overwrite_config.py
+-rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/update_chip_config.py
+-rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/data/analysis_cuts.json
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/data/pixel_classification.json
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/data/schema/info_schema.json
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
+-rw-r--r--   0        0        0    33519 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/utils/analysis.py
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/utils/classification.py
+-rw-r--r--   0        0        0    36639 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/utils/misc.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/tests/test_package.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/LICENSE
+-rw-r--r--   0        0        0    25300 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/README.md
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    27421 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.1/PKG-INFO
```

### Comparing `module_qc_analysis_tools-2.0.0/.gitlab-ci.yml` & `module_qc_analysis_tools-2.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/.pre-commit-config.yaml` & `module_qc_analysis_tools-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/tbump.toml` & `module_qc_analysis_tools-2.0.1/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2232 2e30 2e30 220a 0a23 2045  t = "2.0.0"..# E
+00000010: 7420 3d20 2232 2e30 2e31 220a 0a23 2045  t = "2.0.1"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 322e 302e  mp version: 2.0.
-00000150: 3020 e286 9220 7b6e 6577 5f76 6572 7369  0 ... {new_versi
+00000150: 3120 e286 9220 7b6e 6577 5f76 6572 7369  1 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/IV_MEASURE.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/IV_MEASURE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/LP_MODE.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/LP_MODE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/SLDO.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/SLDO.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,14 +460,17 @@
             residual_VinD = (
                 p1(calculated_data["Current"]["Values"])
                 - (
                     calculated_data["VinD"]["Values"]
                     - calculated_data["Vofs"]["Values"]
                 )
             ) * 1000
+            residual_VinA_VinD = (
+                calculated_data["VinA"]["Values"] - calculated_data["VinD"]["Values"]
+            )
             residual_VinA_nomVofs = (
                 p(calculated_data["Current"]["Values"])
                 - calculated_data["VinA"]["Values"]
             ) * 1000
             residual_VinD_nomVofs = (
                 p(calculated_data["Current"]["Values"])
                 - calculated_data["VinD"]["Values"]
@@ -560,20 +563,15 @@
             ).argmin()
             log.debug(
                 f' Closest current measured to nominal is: {calculated_data["Current"]["Values"][idx]}'
             )
 
             # Calculate values for QC analysis and output file
             SLDO_LINEARITY = max(residual_Vin, key=lambda x: abs(x))
-            SLDO_VINA_VIND = max(
-                abs(
-                    calculated_data["VinA"]["Values"]
-                    - calculated_data["VinD"]["Values"]
-                )
-            )
+            SLDO_VINA_VIND = max(residual_VinA_VinD, key=lambda x: abs(x))
             SLDO_VDDA = calculated_data["VDDA"]["Values"][idx]
             SLDO_VDDD = calculated_data["VDDD"]["Values"][idx]
             SLDO_VINA = calculated_data["VinA"]["Values"][idx]
             SLDO_VIND = calculated_data["VinD"]["Values"][idx]
             SLDO_VOFFS = calculated_data["Vofs"]["Values"][idx]
             SLDO_IINA = calculated_data["IinA"]["Values"][idx]
             SLDO_IIND = calculated_data["IinD"]["Values"][idx]
```

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/TUNING.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/TUNING.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,21 +245,27 @@
             {
                 "UNTUNED_THRESHOLD_FAILED_FITS": failure_summary_untuned.get(
                     "THRESHOLD_FAILED_FITS"
                 ).get("independent")
             }
         )
 
-        passes_qc, summary = perform_qc_analysis(
+        passes_qc_untuned, summary_untuned = perform_qc_analysis(
             test_type, qc_config_untuned, layer, results_untuned
         )
-        passes_qc, summary = perform_qc_analysis(
+        passes_qc_tuned, summary_tuned = perform_qc_analysis(
             test_type, qc_config_tuned, layer, results_tuned
         )
-        print_result_summary(summary, test_type, output_dir, chipName)
+        print_result_summary(
+            summary_untuned, test_type, output_dir, chipName, "untuned"
+        )
+        print_result_summary(summary_tuned, test_type, output_dir, chipName, "tuned")
+
+        passes_qc = passes_qc_untuned and passes_qc_tuned
+
         if passes_qc == -1:
             log.error(
                 bcolors.ERROR
                 + f" QC analysis for {chipName} was NOT successful. Please fix and re-run. Continuing to next chip.."
                 + bcolors.ENDC
             )
             continue
```

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/globals.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,7 +227,15 @@
     None,
     "-ns",
     "--noise-scan",
     help="path to the noise scan output directory to use in YARR analysis",
     exists=True,
     readable=True,
 )
+OPTIONS["totscan"]: Path = typer.Option(
+    None,
+    "-ts",
+    "--tot-scan",
+    help="path to the tot scan output directory to use in YARR analysis",
+    exists=True,
+    readable=True,
+)
```

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/load_yarr_scans.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/load_yarr_scans.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     return latest_results
 
 
 def getDataFile(mname, latest_results, output, test_name, n_chips):
     log.debug(f"Setting module SN to {mname}")
     # Setup structure of output
     config_file = {
-        "datadir": str(output),  # Could be ""
+        "datadir": "",  # Full paths are stored for each file now
         "module": {"serialNumber": mname, "chipType": "RD53B"},
         "chip": [],
     }
 
     # Collect necessary data from each scan
     chip_data = {}
     for scan in latest_results:
@@ -148,14 +148,15 @@
     verbosity: LogLevel = OPTIONS["verbosity"],
     test_name: str = OPTIONS["test_name"],
     digitalscan: Path = OPTIONS["digitalscan"],
     analogscan: Path = OPTIONS["analogscan"],
     thresholdscan_hr: Path = OPTIONS["thresholdscan_hr"],
     thresholdscan_hd: Path = OPTIONS["thresholdscan_hd"],
     noisescan: Path = OPTIONS["noisescan"],
+    totscan: Path = OPTIONS["totscan"],
 ):
     log.setLevel(verbosity.value)
 
     log.info("")
     log.info(" ==============================================================")
     log.info(f" \tCollecting YARR scan output for module {module_sn}")
     log.info(" ==============================================================")
@@ -201,14 +202,18 @@
                 "Overriding latest thresholdscan_hd results with user-supplied scan"
             )
         latest_results.update({"std_thresholdscan_hd": str(thresholdscan_hd.resolve())})
     if noisescan is not None:
         if input_yarr is not None:
             log.info("Overriding latest noisescan results with user-supplied scan")
         latest_results.update({"std_noisescan": str(noisescan.resolve())})
+    if totscan is not None:
+        if input_yarr is not None:
+            log.info("Overriding latest totscan results with user-supplied scan")
+        latest_results.update({"std_totscan": str(totscan.resolve())})
 
     if len(latest_results.keys()) == 0:
         log.error(
             "No YARR results found. Please specify directory to latest YARR scan results, or supply each YARR scan output with appropriate flags. Type `analysis-load-yarr-scans -h` for help"
         )
         raise RuntimeError()
```

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/main.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/overwrite_config.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/overwrite_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/update_chip_config.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/cli/update_chip_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/analysis_cuts.json` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/data/analysis_cuts.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/pixel_classification.json` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/data/pixel_classification.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/schema/info_schema.json` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/data/schema/info_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/analysis.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/utils/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,15 +410,15 @@
     log.info(
         "--------------------------------------------------------------------------------------"
     )
 
     return passes_qc_overall, cell_text
 
 
-def print_result_summary(cell_text, test_type, outputdir, chipname):
+def print_result_summary(cell_text, test_type, outputdir, chipname, label=""):
     # Turn off matplotlib DEBUG messages
     plt.set_loglevel(level="warning")
 
     cell_text = cell_text.reshape(-1, 4)
     nrows, ncols = cell_text.shape
     cellColours = np.empty(0)
     for r in range(0, nrows):
@@ -439,59 +439,67 @@
             cellText=cell_text1,
             colLabels=colLabels,
             loc="upper center",
             cellLoc="center",
             colWidths=colWidths,
             cellColours=cellColours1,
         )
-        format_result_summary(fig, ax, table, chipname, test_type, outputdir, "1")
+        format_result_summary(
+            fig, ax, table, chipname, test_type, outputdir, f"{label}1"
+        )
 
         cell_text2 = cell_text[33:49, :]
         cellColours2 = cellColours[33:49, :]
         nrows, ncols = cell_text2.shape
         fig, ax = plt.subplots(figsize=(6.4, 1.5 + nrows * 0.5))
         table = ax.table(
             cellText=cell_text2,
             colLabels=colLabels,
             loc="upper center",
             cellLoc="center",
             colWidths=colWidths,
             cellColours=cellColours2,
         )
-        format_result_summary(fig, ax, table, chipname, test_type, outputdir, "2")
+        format_result_summary(
+            fig, ax, table, chipname, test_type, outputdir, f"{label}2"
+        )
 
         cell_text3 = cell_text[49:, :]
         cellColours3 = cellColours[49:, :]
         nrows, ncols = cell_text3.shape
         fig, ax = plt.subplots(figsize=(6.4, 1.5 + nrows * 0.5))
         table = ax.table(
             cellText=cell_text3,
             colLabels=colLabels,
             loc="upper center",
             cellLoc="center",
             colWidths=colWidths,
             cellColours=cellColours3,
         )
-        format_result_summary(fig, ax, table, chipname, test_type, outputdir, "3")
+        format_result_summary(
+            fig, ax, table, chipname, test_type, outputdir, f"{label}3"
+        )
 
     else:
         fig, ax = plt.subplots(figsize=(6.4, 1.5 + nrows * 0.5))
         table = ax.table(
             cellText=cell_text,
             colLabels=colLabels,
             loc="upper center",
             cellLoc="center",
             colWidths=colWidths,
             cellColours=cellColours,
         )
-        format_result_summary(fig, ax, table, chipname, test_type, outputdir)
+        format_result_summary(fig, ax, table, chipname, test_type, outputdir, label)
 
 
 def format_result_summary(fig, ax, table, chipname, test_type, outputdir, label=""):
     fig.patch.set_visible(False)
+    if label is not None:
+        label = f"_{label}"
     ax.axis("off")
     ax.axis("tight")
     table.scale(1, 3)
     ax.set_title(f"{test_type} for {chipname}", fontsize=15)
     table.auto_set_font_size(False)
     table.set_fontsize(15)
     plt.savefig(
```

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/classification.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/utils/classification.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/misc.py` & `module_qc_analysis_tools-2.0.1/src/module_qc_analysis_tools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/tests/test_cli.py` & `module_qc_analysis_tools-2.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/.gitignore` & `module_qc_analysis_tools-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/LICENSE` & `module_qc_analysis_tools-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/README.md` & `module_qc_analysis_tools-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-analysis-tools v2.0.0
+# module-qc-analysis-tools v2.0.1
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -71,15 +71,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==2.0.0
+python -m pip install -U pip module-qc-analysis-tools==2.0.1
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

### Comparing `module_qc_analysis_tools-2.0.0/pyproject.toml` & `module_qc_analysis_tools-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-2.0.0/PKG-INFO` & `module_qc_analysis_tools-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-analysis-tools
-Version: 2.0.0
+Version: 2.0.1
 Summary: Module qc analysis tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -34,15 +34,15 @@
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: matplotlib
 Requires-Dist: module-qc-data-tools>=1.0.6
 Requires-Dist: numpy
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# module-qc-analysis-tools v2.0.0
+# module-qc-analysis-tools v2.0.1
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -111,15 +111,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==2.0.0
+python -m pip install -U pip module-qc-analysis-tools==2.0.1
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

