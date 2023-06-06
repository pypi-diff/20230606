# Comparing `tmp/module_qc_tools-2.0.0.tar.gz` & `tmp/module_qc_tools-2.0.1.tar.gz`

## Comparing `module_qc_tools-2.0.0.tar` & `module_qc_tools-2.0.1.tar`

### file list

```diff
@@ -1,55 +1,58 @@
--rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/.gitmodules
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/tbump.toml
--rw-r--r--   0        0        0    40206 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/ADC_CALIBRATION/2023-05-23_144715/20UPGXM1234567.json
--rw-r--r--   0        0        0   311598 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/ANALOG_READBACK/2023-05-23_144719/20UPGXM1234567.json
--rw-r--r--   0        0        0    22334 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/INJECTION_CAPACITANCE/2023-05-23_144710/20UPGXM1234567.json
--rw-r--r--   0        0        0    27182 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/LP_MODE/2023-05-23_144908/20UPGXM1234567.json
--rw-r--r--   0        0        0    23786 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/OVERVOLTAGE_PROTECTION/2023-05-23_144903/20UPGXM1234567.json
--rw-r--r--   0        0        0    75466 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/SLDO/2023-05-23_144651/20UPGXM1234567.json
--rw-r--r--   0        0        0   140154 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/VCAL_CALIBRATION/2023-05-23_144703/20UPGXM1234567.json
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/emulator/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/_version.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    22166 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0    10519 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/LP_MODE.py
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/SLDO.py
--rw-r--r--   0        0        0    12449 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0    18660 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/hardware_emulator.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/main.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/upload_localdb.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/configs/emulator_merged_vmux.json
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/configs/example_merged_vmux.json
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/configs/example_separate_vmux.json
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/module_state_template.json
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
--rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
--rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
--rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
--rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/ANALOG_READBACK.json
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/LP_MODE.json
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/SLDO.json
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
--rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/common.json
--rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/config.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/__init__.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/hardware_control_base.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/misc.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/multimeter.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/ntc.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/power_supply.py
--rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/yarr.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/tests/test_package.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/LICENSE
--rw-r--r--   0        0        0    28528 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/README.md
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    30650 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/.gitmodules
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/tbump.toml
+-rw-r--r--   0        0        0    41758 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/Measurements/ADC_CALIBRATION/2023-06-06_154819/20UPGXM1234567.json
+-rw-r--r--   0        0        0   320866 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/Measurements/ANALOG_READBACK/2023-06-06_154826/20UPGXM1234567.json
+-rw-r--r--   0        0        0    22834 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/Measurements/INJECTION_CAPACITANCE/2023-06-06_154820/20UPGXM1234567.json
+-rw-r--r--   0        0        0    27510 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/Measurements/LP_MODE/2023-06-06_154818/20UPGXM1234567.json
+-rw-r--r--   0        0        0    23926 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/Measurements/OVERVOLTAGE_PROTECTION/2023-06-06_154826/20UPGXM1234567.json
+-rw-r--r--   0        0        0    82032 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/Measurements/SLDO/2023-06-06_154808/20UPGXM1234567.json
+-rw-r--r--   0        0        0   147898 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/Measurements/VCAL_CALIBRATION/2023-06-06_154818/20UPGXM1234567.json
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/emulator/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/_version.py
+-rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    21713 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/__main__.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/globals.py
+-rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/hardware_emulator.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/main.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/cli/upload_localdb.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/configs/emulator_merged_vmux.json
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/configs/example_merged_vmux.json
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/configs/example_separate_vmux.json
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/module_state_template.json
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
+-rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
+-rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
+-rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
+-rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/schema/ANALOG_READBACK.json
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/schema/LP_MODE.json
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/schema/SLDO.json
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
+-rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/schema/common.json
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/data/schema/config.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/utils/__init__.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/utils/hardware_control_base.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/utils/misc.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/utils/multimeter.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/utils/ntc.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/utils/power_supply.py
+-rw-r--r--   0        0        0    15335 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/src/module_qc_tools/utils/yarr.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/tests/test_package.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/LICENSE
+-rw-r--r--   0        0        0    28528 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/README.md
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    30740 2020-02-02 00:00:00.000000 module_qc_tools-2.0.1/PKG-INFO
```

### Comparing `module_qc_tools-2.0.0/.gitlab-ci.yml` & `module_qc_tools-2.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/.pre-commit-config.yaml` & `module_qc_tools-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/tbump.toml` & `module_qc_tools-2.0.1/tbump.toml`

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

### Comparing `module_qc_tools-2.0.0/Measurements/ANALOG_READBACK/2023-05-23_144719/20UPGXM1234567.json` & `module_qc_tools-2.0.1/Measurements/ANALOG_READBACK/2023-06-06_154826/20UPGXM1234567.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9902066710992908%*

 * *Differences: {'0': "{0: {'results': {'property': {'ANALOG_READBACK_MEASUREMENT_VERSION': '2.0.1'}, "*

 * *      "'Measurements': {'Vmux0': {'Values': [6.191648388447707]}, 'Vmux3': {'Values': "*

 * *      "[6.191648388447707]}, 'Vmux4': {'Values': [6.191648388447707]}, 'Vmux5': {'Values': "*

 * *      "[6.191648388447707]}, 'Vmux6': {'Values': [6.191648388447707]}, 'Vmux7': {'Values': "*

 * *      "[6.191648388447707]}, 'Vmux8': {'Values': [6.191648388447707]}, 'Vmux9': {'Values': "*

 * *      "[6.191648388447707]}, 'Vmux10': {'Values': [6.1916 […]*

```diff
@@ -2,393 +2,393 @@
     [
         {
             "results": {
                 "Measurements": {
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            0.04
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux1": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux10": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux11": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux12": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux13": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux14": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux15": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux16": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux17": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux18": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux19": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux2": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux20": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux21": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux22": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux23": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux24": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux25": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            0.35000000000000003
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            0.20576923076923084
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux3": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            0.35000000000000003
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            0.20576923076923084
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux4": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux5": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux6": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux7": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux8": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux0": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux10": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux11": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux12": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux13": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux15": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux17": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux3": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux31": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            0.6006006006006006
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            0.3779976775
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            0.6
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            0.25
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            0.3779976775
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            0.6
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux39": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux4": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux5": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux6": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux7": {
                         "Unit": "V",
                         "Values": [
-                            0.0027395604855596336
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux8": {
                         "Unit": "V",
                         "Values": [
-                            0.0027395604855596336
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux9": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -450,102 +450,102 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853241
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686066509
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
             "results": {
                 "Measurements": {
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux9": {
                         "Unit": "V",
                         "Values": [
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "MonSensAcbDem": {
                         "Unit": "-",
                         "Values": [
                             0,
@@ -810,198 +810,198 @@
                             36.760000000000005
                         ],
                         "X": false
                     },
                     "Vmux14": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux16": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux18": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux2": {
                         "Unit": "V",
                         "Values": [
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -1063,20 +1063,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853331
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686066702
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -2049,74 +2049,74 @@
                             15
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -2178,413 +2178,413 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853728
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686067384
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            0.04
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux1": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux10": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux11": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux12": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux13": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux14": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux15": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux16": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux17": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux18": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux19": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux2": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux20": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux21": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux22": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux23": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux24": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux25": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            0.35000000000000003
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            0.20576923076923084
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux3": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            0.35000000000000003
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            0.20576923076923084
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux4": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux5": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux6": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux7": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux8": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux0": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux10": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux11": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux12": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux13": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux15": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux17": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux3": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux31": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            0.6006006006006006
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            0.3779976775
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            0.6
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            0.25
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            0.3779976775
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            0.6
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux39": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux4": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux5": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux6": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux7": {
                         "Unit": "V",
                         "Values": [
-                            0.0027395604855596336
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux8": {
                         "Unit": "V",
                         "Values": [
-                            0.0027395604855596336
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux9": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -2646,102 +2646,102 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853241
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686066509
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
             "results": {
                 "Measurements": {
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux9": {
                         "Unit": "V",
                         "Values": [
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "MonSensAcbDem": {
                         "Unit": "-",
                         "Values": [
                             0,
@@ -3006,198 +3006,198 @@
                             36.760000000000005
                         ],
                         "X": false
                     },
                     "Vmux14": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux16": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux18": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux2": {
                         "Unit": "V",
                         "Values": [
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -3259,20 +3259,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853331
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686066702
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -4245,74 +4245,74 @@
                             15
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -4374,413 +4374,413 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853728
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686067384
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            0.04
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux1": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux10": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux11": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux12": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux13": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux14": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux15": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux16": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux17": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux18": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux19": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux2": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux20": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux21": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux22": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux23": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux24": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux25": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            0.35000000000000003
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            0.20576923076923084
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux3": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            0.35000000000000003
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            0.20576923076923084
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux4": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux5": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux6": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux7": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux8": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux0": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux10": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux11": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux12": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux13": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux15": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux17": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux3": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux31": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            0.6006006006006006
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            0.3779976775
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            0.6
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            0.25
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            0.3779976775
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            0.6
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux39": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux4": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux5": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux6": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux7": {
                         "Unit": "V",
                         "Values": [
-                            0.0027395604855596336
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux8": {
                         "Unit": "V",
                         "Values": [
-                            0.0027395604855596336
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux9": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -4842,102 +4842,102 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853241
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686066509
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
             "results": {
                 "Measurements": {
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux9": {
                         "Unit": "V",
                         "Values": [
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "MonSensAcbDem": {
                         "Unit": "-",
                         "Values": [
                             0,
@@ -5202,198 +5202,198 @@
                             36.760000000000005
                         ],
                         "X": false
                     },
                     "Vmux14": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux16": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux18": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux2": {
                         "Unit": "V",
                         "Values": [
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -5455,20 +5455,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853331
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686066702
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -6441,74 +6441,74 @@
                             15
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -6570,413 +6570,413 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853728
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686067384
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            0.04
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux1": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux10": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux11": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux12": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux13": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux14": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux15": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux16": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux17": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux18": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux19": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux2": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux20": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux21": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux22": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux23": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux24": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux25": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            0.35000000000000003
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            0.20576923076923084
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux3": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            0.35000000000000003
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            0.20576923076923084
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux4": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux5": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux6": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux7": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux8": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux0": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux10": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux11": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux12": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux13": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux15": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux17": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux3": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux31": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            0.6006006006006006
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            0.3779976775
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            0.6
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            0.25
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            0.3779976775
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            0.6
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux39": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux4": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux5": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux6": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux7": {
                         "Unit": "V",
                         "Values": [
-                            0.0027395604855596336
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux8": {
                         "Unit": "V",
                         "Values": [
-                            0.0027395604855596336
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux9": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -7038,102 +7038,102 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853241
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686066509
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
             "results": {
                 "Measurements": {
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux9": {
                         "Unit": "V",
                         "Values": [
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054,
-                            0.054
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "MonSensAcbDem": {
                         "Unit": "-",
                         "Values": [
                             0,
@@ -7398,198 +7398,198 @@
                             36.760000000000005
                         ],
                         "X": false
                     },
                     "Vmux14": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux16": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux18": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux2": {
                         "Unit": "V",
                         "Values": [
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084,
-                            0.084
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -7651,20 +7651,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853331
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686066702
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -8637,74 +8637,74 @@
                             15
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6,
-                            0.6
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -8766,20 +8766,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853804,
-                    "TimeStart": 1684853728
+                    "TimeEnd": 1686067520,
+                    "TimeStart": 1686067384
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ]
```

### Comparing `module_qc_tools-2.0.0/Measurements/INJECTION_CAPACITANCE/2023-05-23_144710/20UPGXM1234567.json` & `module_qc_tools-2.0.1/Measurements/OVERVOLTAGE_PROTECTION/2023-06-06_154826/20UPGXM1234567.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8435496794871795%*

 * *Differences: {'0': "{0: {'testType': 'OVERVOLTAGE_PROTECTION', 'results': {'property': {replace: "*

 * *      "OrderedDict([('OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION', '2.0.1')])}, 'Measurements': "*

 * *      "{'Vmux30': {'Values': [6.191648388447707]}, 'Imux63': {'Values': [6.191648388447707]}, "*

 * *      "'Temperature': OrderedDict([('X', False), ('Unit', 'C'), ('Values', [39.0])]), "*

 * *      "'SetCurrent': OrderedDict([('X', False), ('Unit', 'A'), ('Values', [2.1])]), 'Current': "*

 * *      "OrderedDict([('X', True), ('Unit', 'A'), […]*

```diff
@@ -1,69 +1,85 @@
 [
     [
         {
             "results": {
                 "Measurements": {
-                    "Imux10": {
+                    "Current": {
+                        "Unit": "A",
+                        "Values": [
+                            6.999999999999999
+                        ],
+                        "X": true
+                    },
+                    "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
-                    "Imux11": {
+                    "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "SetCurrent": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1
+                        ],
+                        "X": false
+                    },
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            39.0
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux32": {
+                        "Unit": "V",
+                        "Values": [
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
+                            6.191648388447707
                         ],
                         "X": false
                     },
-                    "Vmux4": {
+                    "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 39.0,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -120,88 +136,104 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853276,
-                    "TimeStart": 1684853231
+                    "TimeEnd": 1686066540,
+                    "TimeStart": 1686066506
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.0.0"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
-            "testType": "INJECTION_CAPACITANCE"
+            "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
-                    "Imux10": {
+                    "Current": {
+                        "Unit": "A",
+                        "Values": [
+                            6.999999999999999
+                        ],
+                        "X": true
+                    },
+                    "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
-                    "Imux11": {
+                    "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "SetCurrent": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1
+                        ],
+                        "X": false
+                    },
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            39.0
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux32": {
+                        "Unit": "V",
+                        "Values": [
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
+                            6.191648388447707
                         ],
                         "X": false
                     },
-                    "Vmux4": {
+                    "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 39.0,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -258,88 +290,104 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853276,
-                    "TimeStart": 1684853231
+                    "TimeEnd": 1686066540,
+                    "TimeStart": 1686066506
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.0.0"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
-            "testType": "INJECTION_CAPACITANCE"
+            "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
-                    "Imux10": {
+                    "Current": {
+                        "Unit": "A",
+                        "Values": [
+                            6.999999999999999
+                        ],
+                        "X": true
+                    },
+                    "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
-                    "Imux11": {
+                    "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "SetCurrent": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1
+                        ],
+                        "X": false
+                    },
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            39.0
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux32": {
+                        "Unit": "V",
+                        "Values": [
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
+                            6.191648388447707
                         ],
                         "X": false
                     },
-                    "Vmux4": {
+                    "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 39.0,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -396,88 +444,104 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853276,
-                    "TimeStart": 1684853232
+                    "TimeEnd": 1686066540,
+                    "TimeStart": 1686066506
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.0.0"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
-            "testType": "INJECTION_CAPACITANCE"
+            "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
-                    "Imux10": {
+                    "Current": {
+                        "Unit": "A",
+                        "Values": [
+                            6.999999999999999
+                        ],
+                        "X": true
+                    },
+                    "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
-                    "Imux11": {
+                    "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "SetCurrent": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1
+                        ],
+                        "X": false
+                    },
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            39.0
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux32": {
+                        "Unit": "V",
+                        "Values": [
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
+                            6.191648388447707
                         ],
                         "X": false
                     },
-                    "Vmux4": {
+                    "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267,
-                            1.5479120971119267
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 39.0,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -534,21 +598,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853276,
-                    "TimeStart": 1684853232
+                    "TimeEnd": 1686066540,
+                    "TimeStart": 1686066506
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.0.0"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
-            "testType": "INJECTION_CAPACITANCE"
+            "testType": "OVERVOLTAGE_PROTECTION"
         }
     ]
 ]
```

### Comparing `module_qc_tools-2.0.0/Measurements/LP_MODE/2023-05-23_144908/20UPGXM1234567.json` & `module_qc_tools-2.0.1/Measurements/LP_MODE/2023-06-06_154818/20UPGXM1234567.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9900555173992673%*

 * *Differences: {'0': "{0: {'results': {'property': {'LP_MODE_MEASUREMENT_VERSION': '2.0.1'}, 'Measurements': "*

 * *      "{'Vmux30': {'Values': [6.191648388447707]}, 'Vmux33': {'Values': [6.191648388447707]}, "*

 * *      "'Vmux36': {'Values': [6.191648388447707]}, 'Vmux37': {'Values': [6.191648388447707]}, "*

 * *      "'Imux0': {'Values': [6.191648388447707]}, 'Imux28': {'Values': [6.191648388447707]}, "*

 * *      "'Imux29': {'Values': [6.191648388447707]}, 'Imux30': {'Values': [6.191648388447707]}, "*

 * *      "'Imux31': {'Values': [6.19164 […]*

```diff
@@ -16,50 +16,50 @@
                             -1
                         ],
                         "X": false
                     },
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            0.04
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            0.125
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            0.02403846153846154
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            0.125
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            0.02403846153846154
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
                             2.1
@@ -72,36 +72,36 @@
                             29.2
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            0.29571345625
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            0.25
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            0.29571345625
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 29.2,
                     "ChannelConfig": "",
@@ -164,20 +164,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853370,
-                    "TimeStart": 1684853349
+                    "TimeEnd": 1686066536,
+                    "TimeStart": 1686066498
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.0.0"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ],
@@ -198,50 +198,50 @@
                             -1
                         ],
                         "X": false
                     },
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            0.04
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            0.125
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            0.02403846153846154
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            0.125
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            0.02403846153846154
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
                             2.1
@@ -254,36 +254,36 @@
                             29.2
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            0.29571345625
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            0.25
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            0.29571345625
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 29.2,
                     "ChannelConfig": "",
@@ -346,20 +346,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853370,
-                    "TimeStart": 1684853349
+                    "TimeEnd": 1686066536,
+                    "TimeStart": 1686066498
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.0.0"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ],
@@ -380,50 +380,50 @@
                             -1
                         ],
                         "X": false
                     },
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            0.04
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            0.125
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            0.02403846153846154
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            0.125
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            0.02403846153846154
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
                             2.1
@@ -436,36 +436,36 @@
                             29.2
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            0.29571345625
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            0.25
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            0.29571345625
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 29.2,
                     "ChannelConfig": "",
@@ -528,20 +528,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853370,
-                    "TimeStart": 1684853349
+                    "TimeEnd": 1686066536,
+                    "TimeStart": 1686066498
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.0.0"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ],
@@ -562,50 +562,50 @@
                             -1
                         ],
                         "X": false
                     },
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            0.04
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            0.125
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            0.02403846153846154
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            0.125
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            0.02403846153846154
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
                             2.1
@@ -618,36 +618,36 @@
                             29.2
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            0.0
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            0.29571345625
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            0.25
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            0.29571345625
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 29.2,
                     "ChannelConfig": "",
@@ -710,20 +710,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684853370,
-                    "TimeStart": 1684853349
+                    "TimeEnd": 1686066536,
+                    "TimeStart": 1686066499
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.0.0"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.0.1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ]
```

### Comparing `module_qc_tools-2.0.0/emulator/README.md` & `module_qc_tools-2.0.1/emulator/README.md`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/cli/ADC_CALIBRATION.py` & `module_qc_tools-2.0.1/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,208 +1,186 @@
-#!/usr/bin/env python3
-from __future__ import annotations
-
 import json
 import logging
 import sys
-from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
+from typing import Optional
 
-import numpy as np
 import pkg_resources
+import typer
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
-from module_qc_tools import data
+from module_qc_tools.cli.globals import (
+    CONTEXT_SETTINGS,
+    OPTIONS,
+    LogLevel,
+)
 from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger("measurement")
 
-parser = ArgumentParser()
-parser.add_argument(
-    "-c",
-    "--config",
-    action="store",
-    default=data / "configs/example_merged_vmux.json",
-    help="Config file",
-)
-parser.add_argument(
-    "-o",
-    "--output-dir",
-    action="store",
-    default="outputs",
-    help="output directory",
-)
-parser.add_argument(
-    "-m",
-    "--module-connectivity",
-    action="store",
-    help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
-)
-parser.add_argument(
-    "-v",
-    "--verbosity",
-    action="store",
-    default="INFO",
-    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
-)
-parser.add_argument(
-    "--perchip",
-    action="store_true",
-    help="Store results in one file per chip (default: one file per module)",
-)
-args = parser.parse_args()
+app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
 
-def run(data, adc_calib_config, ps, yr, meter, layer):
-    """The function which does the ADC calibration.
+def run(data, inj_cap_config, ps, yr, meter, layer):
+    """The function which does the injection capacitance measurement.
 
     Args:
         data (list): data[chip_id].
-        adc_calib_config (dict): An subdict dumped from json including the task information.
+        inj_cap_config (dict): An subdict dumped from json including the task information.
         ps (Class power_supply): An instance of Class power_supply for power on and power off.
         yr (Class yarr): An instance of Class yarr for chip conifugration and change register.
         meter (Class meter): An instance of Class meter. Used to control the multimeter to measure voltages.
 
     Returns:
         None: The measurements are recorded in `data`.
     """
     if yr.running_emulator():
         ps.on(
-            adc_calib_config["v_max"], adc_calib_config["i_config"][layer]
+            inj_cap_config["v_max"], inj_cap_config["i_config"][layer]
         )  # Only for emulator do the emulation of power on/off
         # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
 
+    # This sends global pulse
     status = yr.configure()
     assert status >= 0
 
-    InjVcalRange = adc_calib_config["InjVcalRange"]
-    MonitorV = adc_calib_config["MonitorV"]
-
-    Range = [
-        adc_calib_config["Range"]["start"],
-        adc_calib_config["Range"]["stop"],
-        adc_calib_config["Range"]["step"],
-    ]
-    DACs = np.arange(start=Range[0], stop=Range[1], step=Range[2])
-
-    for DAC in DACs:
+    for _i in range(inj_cap_config["n_meas"]):
         v_mea = [{} for _ in range(yr._number_of_chips)]
+
         for chip in range(yr._number_of_chips):
             if chip in yr._disabled_chip_positions:
                 continue
 
-            yr.write_register("MonitorEnable", 1, chip)
-            yr.write_register("InjVcalMed", DAC, chip)  # write DAC values
-            v_mea[chip]["DACs_input"] = [float(DAC)]
+            # Disable both capmeasure and parasitic circuits
+            yr.write_register("CapMeasEn", 0, chip)
+            yr.write_register("CapMeasEnPar", 0, chip)
 
-            yr.write_register("InjVcalRange", InjVcalRange, chip)
-            for i, vmux_value in enumerate(MonitorV):
+            for vmux_value in inj_cap_config["v_mux"]:
                 yr.set_mux(
                     chip_position=chip,
-                    v_mux=MonitorV[i],
-                    reset_other_chips=adc_calib_config["share_vmux"],
+                    v_mux=vmux_value,
+                    reset_other_chips=inj_cap_config["share_vmux"],
                 )
                 v_mea[chip][f"Vmux{vmux_value}"] = [meter.measure_dcv()[0]]
-                v_mea[chip][f"ADC_Vmux{vmux_value}"] = [
-                    int(yr.read_adc(MonitorV[i], chip_position=chip, rawCounts=True)[0])
-                ]
+
+            for imux_value in inj_cap_config["i_mux"]:
+                if imux_value == 10:
+                    # Enable capmeasure circuit
+                    yr.write_register("CapMeasEn", 1, chip)
+                    yr.write_register("CapMeasEnPar", 0, chip)
+                elif imux_value == 11:
+                    # Enable capmeasure circuit
+                    yr.write_register("CapMeasEn", 0, chip)
+                    yr.write_register("CapMeasEnPar", 1, chip)
+                else:
+                    # Disable both
+                    yr.write_register("CapMeasEn", 0, chip)
+                    yr.write_register("CapMeasEnPar", 0, chip)
+
+                yr.set_mux(
+                    chip_position=chip,
+                    i_mux=imux_value,
+                    reset_other_chips=inj_cap_config["share_vmux"],
+                )
+
+                v_mea[chip][f"Imux{imux_value}"] = [meter.measure_dcv()[0]]
+
             data[chip].add_data(v_mea[chip])
 
     if yr.running_emulator():
         ps.off()
 
 
-def main():
+@app.command()
+def main(
+    config_path: Path = OPTIONS["config"],
+    base_output_dir: Path = OPTIONS["output_dir"],
+    module_connectivity: Optional[Path] = OPTIONS["module_connectivity"],
+    verbosity: LogLevel = OPTIONS["verbosity"],
+    perchip: bool = OPTIONS["perchip"],
+    use_pixel_config: bool = OPTIONS["use_pixel_config"],
+):
     """main() creates the qcDataFrame and pass it to the run() where the measurements are stored in the qcDataFrame."""
 
-    log.setLevel(args.verbosity)
+    log.setLevel(verbosity.value)
 
-    log.info("[run_ADC_calib] Start ADC calibration!")
+    log.info("[run_inj_capacitance] Start injection capacitance measurement!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-    log.info(f"[run_ADC_calib] TimeStart: {timestart}")
+    log.info(f"[run_inj_capacitance] TimeStart: {timestart}")
 
-    with resources.as_file(Path(args.config)) as path:
+    with resources.as_file(Path(config_path)) as path:
         config = json.loads(path.read_text())
 
-    check_meas_config(config, args.config)
+    check_meas_config(config, config_path)
 
-    if args.module_connectivity:
-        config["yarr"]["connectivity"] = args.module_connectivity
+    if module_connectivity:
+        config["yarr"]["connectivity"] = module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
-    if "emulator" not in args.config and not args.module_connectivity:
-        msg = "must supply path to connectivity file [-m --module-connectivity]"
-        raise RuntimeError(msg)
+    if "emulator" not in str(config_path) and not module_connectivity:
+        typer.echo("must supply path to connectivity file [-m --module-connectivity]")
+        raise typer.Exit(2)
 
-    adc_calib_config = config["tasks"]["GENERAL"]
-    adc_calib_config.update(config["tasks"]["ADC_CALIBRATION"])
+    inj_cap_config = config["tasks"]["GENERAL"]
+    inj_cap_config.update(config["tasks"]["INJECTION_CAPACITANCE"])
 
     ps = power_supply(config["power_supply"])
     yr = yarr(config["yarr"])
     meter = multimeter(config["multimeter"])
 
+    if not use_pixel_config:
+        yr.omit_pixel_config("tmp")
+
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
     test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if institution is None:
         institution = ""
 
-    ps.set(v=adc_calib_config["v_max"], i=adc_calib_config["i_config"][layer])
+    ps.set(v=inj_cap_config["v_max"], i=inj_cap_config["i_config"][layer])
 
     # if -o option used, overwrite the default output directory
-    if args.module_connectivity:
-        output_dir = args.module_connectivity.rsplit("/", 1)[0]
-    else:
-        output_dir = args.output_dir
+    output_dir = module_connectivity.parent if module_connectivity else base_output_dir
 
-    if args.output_dir != "outputs":
-        output_dir = args.output_dir
+    if base_output_dir != Path("outputs"):
+        output_dir = base_output_dir
 
+    output_dir = output_dir.joinpath("Measurements", test_type, timestart)
     # Make output directory and start log file
-    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
-        parents=True, exist_ok=True
-    )
-    log.addHandler(
-        logging.FileHandler(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
-        )
-    )
-
-    InjVcalRange = adc_calib_config["InjVcalRange"]
+    output_dir.mkdir(parents=True, exist_ok=True)
+    log.addHandler(logging.FileHandler(output_dir.joinpath("output.log")))
 
     input_files = [None] * yr._number_of_chips
     data = [
         qcDataFrame(
-            columns=["DACs_input"]
-            + [f"Vmux{v_mux}" for v_mux in adc_calib_config["MonitorV"]]
-            + [f"ADC_Vmux{v_mux}" for v_mux in adc_calib_config["MonitorV"]],
-            units=["Count"]
-            + ["V" for v_mux in adc_calib_config["MonitorV"]]
-            + ["Count" for v_mux in adc_calib_config["MonitorV"]],
+            columns=[f"Vmux{v_mux}" for v_mux in inj_cap_config["v_mux"]]
+            + [f"Imux{i_mux}" for i_mux in inj_cap_config["i_mux"]],
+            units=["V" for v_mux in inj_cap_config["v_mux"]]
+            + ["V" for i_mux in inj_cap_config["i_mux"]],
         )
         for input_file in input_files
     ]
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
@@ -211,29 +189,25 @@
             pkg_resources.get_distribution("module-qc-tools").version,
         )
         data[chip]._meta_data = get_identifiers(yr.get_config(chip))
         data[chip].add_meta_data("Institution", institution)
         data[chip].add_meta_data("ModuleSN", module_serial)
         data[chip].add_meta_data("TimeStart", round(datetime.timestamp(datetime.now())))
         data[chip]._meta_data.update(get_meta_data(yr.get_config(chip)))
-        data[chip]._meta_data["ChipConfigs"]["RD53B"]["GlobalConfig"][
-            "InjVcalRange"
-        ] = InjVcalRange
-        data[chip].set_x("DACs_input", True)
 
     logging.basicConfig(level=logging.DEBUG)
     logger = logging.getLogger(__name__)
 
     try:
-        run(data, adc_calib_config, ps, yr, meter, layer)
+        run(data, inj_cap_config, ps, yr, meter, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         logger.exception(err)
-        sys.exit(1)
+        raise typer.Exit(1) from err
 
     log.info(
         "==================================Summary=================================="
     )
     alloutput = []
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
@@ -241,29 +215,33 @@
         chip_name = data[chip]._meta_data["Name"]
         data[chip].add_meta_data("TimeEnd", round(datetime.timestamp(datetime.now())))
         log.info("data[chip]: ")
         log.info(data[chip])
         outputDF = outputDataFrame()
         outputDF.set_test_type(test_type)
         outputDF.set_results(data[chip])
-        if args.perchip:
+        if perchip:
             save_dict_list(
-                f"{output_dir}/Measurements/{test_type}/{timestart}/{chip_name}.json",
+                output_dir.joinpath(f"{chip_name}.json"),
                 [outputDF.to_dict()],
             )
         else:
             alloutput += [outputDF.to_dict()]
-    if not args.perchip:
+    if not perchip:
         save_dict_list(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/{module_serial}.json",
+            output_dir.joinpath(f"{module_serial}.json"),
             alloutput,
         )
 
+    log.info(f"Writing output measurements in {output_dir}")
+    log.info("[run_inj_capacitance] Done!")
     log.info(
-        f"Writing output measurements in {output_dir}/Measurements/{test_type}/{timestart}/"
+        f"[run_inj_capacitance] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
     )
-    log.info("[run_ADC_calib] Done!")
-    log.info(f"[run_ADC_calib] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}")
+
+    # Delete temporary files
+    if not use_pixel_config:
+        yr.remove_tmp_connectivity()
 
 
 if __name__ == "__main__":
-    main()
+    typer.run(main)
```

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/cli/ANALOG_READBACK.py` & `module_qc_tools-2.0.1/src/module_qc_tools/cli/ANALOG_READBACK.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,46 @@
-#!/usr/bin/env python
-from __future__ import annotations
-
 import json
 import logging
 import sys
-from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
+from typing import Optional
 
 import pkg_resources
+import typer
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 from tabulate import tabulate
 
-from module_qc_tools import data
+from module_qc_tools.cli.globals import (
+    CONTEXT_SETTINGS,
+    OPTIONS,
+    LogLevel,
+)
 from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
 from module_qc_tools.utils.ntc import ntc
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger("measurement")
 
-parser = ArgumentParser()
-parser.add_argument(
-    "-c",
-    "--config",
-    action="store",
-    default=data / "configs/example_merged_vmux.json",
-    help="Config file",
-)
-parser.add_argument(
-    "-o",
-    "--output-dir",
-    action="store",
-    default="outputs",
-    help="output directory",
-)
-parser.add_argument(
-    "-m",
-    "--module-connectivity",
-    action="store",
-    help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
-)
-parser.add_argument(
-    "-v",
-    "--verbosity",
-    action="store",
-    default="INFO",
-    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
-)
-parser.add_argument(
-    "--perchip",
-    action="store_true",
-    help="Store results in one file per chip (default: one file per module)",
-)
-args = parser.parse_args()
+app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
 
 def run_vmeas(data, analog_readback_config, ps, yr, meter, layer):
     """
     This function measures given internal voltages by going through all VMUX and IMUX settings provided in the config.
 
     Args:
@@ -373,46 +342,57 @@
 def add_time_end_identifier(yr, data):
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
         data[chip].add_meta_data("TimeEnd", round(datetime.timestamp(datetime.now())))
 
 
-def main():
+@app.command()
+def main(
+    config_path: Path = OPTIONS["config"],
+    base_output_dir: Path = OPTIONS["output_dir"],
+    module_connectivity: Optional[Path] = OPTIONS["module_connectivity"],
+    verbosity: LogLevel = OPTIONS["verbosity"],
+    perchip: bool = OPTIONS["perchip"],
+    use_pixel_config: bool = OPTIONS["use_pixel_config"],
+):
     """
     main() creates the qcDataFrame and pass it to the run() where the measurements are stored in the qcDataFrame.
     """
 
-    log.setLevel(args.verbosity)
+    log.setLevel(verbosity.value)
 
     log.info("[run_AnalogReadBack] Starting analog readback!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     log.info(f"[run_AnalogReadBack] TimeStart: {timestart}")
 
-    with resources.as_file(Path(args.config)) as path:
+    with resources.as_file(Path(config_path)) as path:
         config = json.loads(path.read_text())
 
-    check_meas_config(config, args.config)
+    check_meas_config(config, config_path)
 
-    if args.module_connectivity:
-        config["yarr"]["connectivity"] = args.module_connectivity
+    if module_connectivity:
+        config["yarr"]["connectivity"] = module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
-    if "emulator" not in args.config and not args.module_connectivity:
-        msg = "must supply path to connectivity file [-m --module-connectivity]"
-        raise RuntimeError(msg)
+    if "emulator" not in str(config_path) and not module_connectivity:
+        typer.echo("must supply path to connectivity file [-m --module-connectivity]")
+        raise typer.Exit(2)
 
     analog_readback_config = config["tasks"]["GENERAL"]
     analog_readback_config.update(config["tasks"]["ANALOG_READBACK"])
 
     ps = power_supply(config["power_supply"])
     yr = yarr(config["yarr"])
     meter = multimeter(config["multimeter"])
     nt = ntc(config["ntc"])
 
+    if not use_pixel_config:
+        yr.omit_pixel_config("tmp")
+
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
     test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
@@ -421,31 +401,23 @@
 
     ps.set(
         v=analog_readback_config["v_max"], i=analog_readback_config["i_config"][layer]
     )
     yr.configure()
 
     # if -o option used, overwrite the default output directory
-    if args.module_connectivity:
-        output_dir = args.module_connectivity.rsplit("/", 1)[0]
-    else:
-        output_dir = args.output_dir
+    output_dir = module_connectivity.parent if module_connectivity else base_output_dir
 
-    if args.output_dir != "outputs":
-        output_dir = args.output_dir
+    if base_output_dir != Path("outputs"):
+        output_dir = base_output_dir
 
+    output_dir = output_dir.joinpath("Measurements", test_type, timestart)
     # Make output directory and start log file
-    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
-        parents=True, exist_ok=True
-    )
-    log.addHandler(
-        logging.FileHandler(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
-        )
-    )
+    output_dir.mkdir(parents=True, exist_ok=True)
+    log.addHandler(logging.FileHandler(output_dir.joinpath("output.log")))
 
     input_files = [None] * yr._number_of_chips
 
     data = [
         qcDataFrame(
             columns=[f"Vmux{v_mux}" for v_mux in analog_readback_config["v_mux"]]
             + [f"Imux{i_mux}" for i_mux in analog_readback_config["i_mux"]],
@@ -499,41 +471,41 @@
     try:
         run_vmeas(data, analog_readback_config, ps, yr, meter, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.info("Error in measuring all vmux values.")
         log.exception(err)
-        sys.exit(1)
+        raise typer.Exit(1) from err
     add_time_end_identifier(yr, data)
 
     # Measure temperature
     add_identifier_metadata(data_tempmeas, yr, module_serial, institution)
     try:
         run_tmeas(data_tempmeas, analog_readback_config, ps, yr, meter, nt, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.info("Error in measuring temperature.")
         log.exception(err)
-        sys.exit(1)
+        raise typer.Exit(1) from err
     add_time_end_identifier(yr, data_tempmeas)
 
     # Measure vdda/vddd vs trim
     add_identifier_metadata(data_vdda_vddd_vs_trim, yr, module_serial, institution)
     try:
         run_vdda_vddd_vs_trim(
             data_vdda_vddd_vs_trim, analog_readback_config, ps, yr, meter, layer
         )
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.info("Error in measuring VDDA/VDDD vs trim.")
         log.exception(err)
-        sys.exit(1)
+        raise typer.Exit(1) from err
     add_time_end_identifier(yr, data_vdda_vddd_vs_trim)
 
     # save results in json
     log.info(
         "==================================Summary=================================="
     )
     alloutput = []
@@ -575,36 +547,38 @@
         outputDF_tempmeas.set_subtest_type("AR_TEMP")
         outputDF_tempmeas.set_results(data_tempmeas[chip])
 
         outputDF_vdda_vddd_vs_trim = outputDataFrame()
         outputDF_vdda_vddd_vs_trim.set_test_type(test_type)
         outputDF_vdda_vddd_vs_trim.set_subtest_type("AR_VDD")
         outputDF_vdda_vddd_vs_trim.set_results(data_vdda_vddd_vs_trim[chip])
-        if args.perchip:
+        if perchip:
             save_dict_list(
-                f"{output_dir}/Measurements/{test_type}/{timestart}/{chip_name}.json",
+                output_dir.joinpath(f"{chip_name}.json"),
                 [
                     outputDF.to_dict(),
                     outputDF_tempmeas.to_dict(),
                     outputDF_vdda_vddd_vs_trim.to_dict(),
                 ],
             )
         else:
             alloutput += [
                 outputDF.to_dict(),
                 outputDF_tempmeas.to_dict(),
                 outputDF_vdda_vddd_vs_trim.to_dict(),
             ]
 
-    if not args.perchip:
+    if not perchip:
         save_dict_list(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/{module_serial}.json",
+            output_dir.joinpath(f"{module_serial}.json"),
             alloutput,
         )
 
-    log.info(
-        f"Writing output measurements in {output_dir}/Measurements/{test_type}/{timestart}/"
-    )
+    log.info(f"Writing output measurements in {output_dir}")
+
+    # Delete temporary files
+    if not use_pixel_config:
+        yr.remove_tmp_connectivity()
 
 
 if __name__ == "__main__":
-    main()
+    typer.run(main)
```

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_tools-2.0.1/src/module_qc_tools/cli/LP_MODE.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,273 +1,280 @@
-#!/usr/bin/env python3
-from __future__ import annotations
-
+import copy
 import json
 import logging
+import re
 import sys
-from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
+from typing import Optional
 
+import numpy as np
 import pkg_resources
+import typer
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
+from tabulate import tabulate
 
-from module_qc_tools import data
-from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
+from module_qc_tools.cli.globals import (
+    CONTEXT_SETTINGS,
+    OPTIONS,
+    LogLevel,
+)
+from module_qc_tools.utils.misc import bcolors, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
+from module_qc_tools.utils.ntc import ntc
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger("measurement")
 
-parser = ArgumentParser()
-parser.add_argument(
-    "-c",
-    "--config",
-    action="store",
-    default=data / "configs/example_merged_vmux.json",
-    help="Config file",
-)
-parser.add_argument(
-    "-o",
-    "--output-dir",
-    action="store",
-    default="outputs",
-    help="output directory",
-)
-parser.add_argument(
-    "-m",
-    "--module-connectivity",
-    action="store",
-    help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
-)
-parser.add_argument(
-    "-v",
-    "--verbosity",
-    action="store",
-    default="INFO",
-    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
-)
-parser.add_argument(
-    "--perchip",
-    action="store_true",
-    help="Store results in one file per chip (default: one file per module)",
-)
-args = parser.parse_args()
-
+app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
-def run(data, inj_cap_config, ps, yr, meter, layer):
-    """The function which does the injection capacitance measurement.
 
-    Args:
-        data (list): data[chip_id].
-        inj_cap_config (dict): An subdict dumped from json including the task information.
-        ps (Class power_supply): An instance of Class power_supply for power on and power off.
-        yr (Class yarr): An instance of Class yarr for chip conifugration and change register.
-        meter (Class meter): An instance of Class meter. Used to control the multimeter to measure voltages.
-
-    Returns:
-        None: The measurements are recorded in `data`.
-    """
+def run(
+    data, LP_config, NOMINAL_config, ps, yr, meter, nt, layer, output_dir, log_file
+):
+    # turn off power supply before switching low power mode on
+    ps.off()
+    # turn on low power mode
+    yr.switchLPM("on")
+    # turn on power supply and configure all chips
     if yr.running_emulator():
-        ps.on(
-            inj_cap_config["v_max"], inj_cap_config["i_config"][layer]
-        )  # Only for emulator do the emulation of power on/off
-        # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
-
-    # This sends global pulse
+        ps.on(v=LP_config["v_max"], i=LP_config["i_config"][layer])
+    else:
+        ps.set(v=LP_config["v_max"], i=LP_config["i_config"][layer])
+        ps.on()
     status = yr.configure()
-    assert status >= 0
-
-    for _i in range(inj_cap_config["n_meas"]):
-        v_mea = [{} for _ in range(yr._number_of_chips)]
 
-        for chip in range(yr._number_of_chips):
-            if chip in yr._disabled_chip_positions:
-                continue
-
-            # Disable both capmeasure and parasitic circuits
-            yr.write_register("CapMeasEn", 0, chip)
-            yr.write_register("CapMeasEnPar", 0, chip)
-
-            for vmux_value in inj_cap_config["v_mux"]:
-                yr.set_mux(
-                    chip_position=chip,
-                    v_mux=vmux_value,
-                    reset_other_chips=inj_cap_config["share_vmux"],
-                )
-                v_mea[chip][f"Vmux{vmux_value}"] = [meter.measure_dcv()[0]]
-
-            for imux_value in inj_cap_config["i_mux"]:
-                if imux_value == 10:
-                    # Enable capmeasure circuit
-                    yr.write_register("CapMeasEn", 1, chip)
-                    yr.write_register("CapMeasEnPar", 0, chip)
-                elif imux_value == 11:
-                    # Enable capmeasure circuit
-                    yr.write_register("CapMeasEn", 0, chip)
-                    yr.write_register("CapMeasEnPar", 1, chip)
-                else:
-                    # Disable both
-                    yr.write_register("CapMeasEn", 0, chip)
-                    yr.write_register("CapMeasEnPar", 0, chip)
-
-                yr.set_mux(
-                    chip_position=chip,
-                    i_mux=imux_value,
-                    reset_other_chips=inj_cap_config["share_vmux"],
-                )
+    # measure current for power supply
+    i = LP_config["i_config"][layer]
+    current, status = ps.getI()
+    i_mea = [{} for _ in range(yr._number_of_chips)]
+
+    # Run digital scan
+    yr.run_scan(yr.lpm_digitalscan, f"{output_dir}/YARRscans/")
+
+    # Search log contents for failing pixels
+    with Path(log_file).open() as f:
+        yarr_output = f.readlines()
+    failing_pixels = {}
+    for line in yarr_output:
+        if "Total number of failing pixels" in line:
+            chip_name = "0x" + re.search(r"\[.*?0x(.*?)\].*", line).group(1)
+            nFail = re.search(r"^\d+", line.split(" ")[-1]).group()
+            log.debug(f"{chip_name} has {nFail} failing pixels")
+            failing_pixels.update({chip_name: int(nFail)})
 
-                v_mea[chip][f"Imux{imux_value}"] = [meter.measure_dcv()[0]]
+    for chip in range(yr._number_of_chips):
+        if chip in yr._disabled_chip_positions:
+            continue
 
-            data[chip].add_data(v_mea[chip])
+        # Store of bad pixels in log file
+        chip_name = data[chip]._meta_data["Name"]
+        if chip_name in failing_pixels:
+            i_mea[chip]["FailingPixels"] = [failing_pixels.get(chip_name)]
+        else:
+            i_mea[chip]["FailingPixels"] = [-1]
 
+        i_mea[chip]["SetCurrent"] = [i]
+        i_mea[chip]["Current"] = [current]
+        # measure temperature from NTC
+        temp, status = nt.read()
+        i_mea[chip]["Temperature"] = [temp]
+        # measure v_mux
+        for v_mux in LP_config["v_mux"]:
+            yr.set_mux(
+                chip_position=chip,
+                v_mux=v_mux,
+                reset_other_chips=LP_config["share_vmux"],
+            )
+            mea, status = meter.measure_dcv(channel=LP_config["v_mux_channels"][chip])
+            i_mea[chip][f"Vmux{v_mux}"] = [mea]
+        # measure i_mux
+        for i_mux in LP_config["i_mux"]:
+            yr.set_mux(
+                chip_position=chip,
+                i_mux=i_mux,
+                reset_other_chips=LP_config["share_vmux"],
+            )
+            mea, status = meter.measure_dcv(channel=LP_config["v_mux_channels"][chip])
+            i_mea[chip][f"Imux{i_mux}"] = [mea]
+        data[chip].add_data(i_mea[chip])
+        log.info(
+            "--------------------------------------------------------------------------"
+        )
+        log.info(f"Chip-{chip+1}")
+        log.info(tabulate(i_mea[chip], headers="keys", floatfmt=".3f"))
+    # turn off power supply before switching low power mode off
+    ps.off()
+    # turn off low power mode
+    yr.switchLPM("off")
     if yr.running_emulator():
-        ps.off()
-
+        ps.on(v=NOMINAL_config["v_max"], i=NOMINAL_config["i_config"][layer])
+    else:
+        ps.set(v=NOMINAL_config["v_max"], i=NOMINAL_config["i_config"][layer])
+        ps.on()
 
-def main():
-    """main() creates the qcDataFrame and pass it to the run() where the measurements are stored in the qcDataFrame."""
 
-    log.setLevel(args.verbosity)
+@app.command()
+def main(
+    config_path: Path = OPTIONS["config"],
+    base_output_dir: Path = OPTIONS["output_dir"],
+    module_connectivity: Optional[Path] = OPTIONS["module_connectivity"],
+    verbosity: LogLevel = OPTIONS["verbosity"],
+    perchip: bool = OPTIONS["perchip"],
+):
+    log.setLevel(verbosity.value)
 
-    log.info("[run_inj_capacitance] Start injection capacitance measurement!")
+    log.info("[run_LP] Start LP Mode scan!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-    log.info(f"[run_inj_capacitance] TimeStart: {timestart}")
+    log.info(f"[run_LP] TimeStart: {timestart}")
 
-    with resources.as_file(Path(args.config)) as path:
+    with resources.as_file(Path(config_path)) as path:
         config = json.loads(path.read_text())
 
-    check_meas_config(config, args.config)
-
-    if args.module_connectivity:
-        config["yarr"]["connectivity"] = args.module_connectivity
+    # Need to pass module connectivity path to yarr class (except in case we are running the emulator)
+    if module_connectivity:
+        config["yarr"]["connectivity"] = module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
-    if "emulator" not in args.config and not args.module_connectivity:
-        msg = "must supply path to connectivity file [-m --module-connectivity]"
-        raise RuntimeError(msg)
-
-    inj_cap_config = config["tasks"]["GENERAL"]
-    inj_cap_config.update(config["tasks"]["INJECTION_CAPACITANCE"])
+    if "emulator" not in str(config_path) and not module_connectivity:
+        typer.echo("must supply path to connectivity file [-m --module-connectivity]")
+        raise typer.Exit(2)
+    if module_connectivity and "LP" not in module_connectivity:
+        log.warning(
+            bcolors.WARNING
+            + f"You supplied a module connectivity ({module_connectivity}) which does not have 'LP' (low-power) in the name. Are you sure this is the connectivity file for low-power configuration? If not, chip will fail to configure."
+            + bcolors.ENDC
+        )
 
+    NOMINAL_config = config["tasks"]["GENERAL"]
+    LP_config = copy.deepcopy(config["tasks"]["GENERAL"])
+    LP_config.update(config["tasks"]["LP_MODE"])
     ps = power_supply(config["power_supply"])
     yr = yarr(config["yarr"])
+
     meter = multimeter(config["multimeter"])
+    nt = ntc(config["ntc"])
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
     test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if institution is None:
         institution = ""
 
-    ps.set(v=inj_cap_config["v_max"], i=inj_cap_config["i_config"][layer])
-
     # if -o option used, overwrite the default output directory
-    if args.module_connectivity:
-        output_dir = args.module_connectivity.rsplit("/", 1)[0]
-    else:
-        output_dir = args.output_dir
+    output_dir = module_connectivity.parent if module_connectivity else base_output_dir
 
-    if args.output_dir != "outputs":
-        output_dir = args.output_dir
+    if base_output_dir != Path("outputs"):
+        output_dir = base_output_dir
 
+    output_dir = output_dir.joinpath("Measurements", test_type, timestart)
     # Make output directory and start log file
-    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
-        parents=True, exist_ok=True
-    )
-    log.addHandler(
-        logging.FileHandler(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
-        )
-    )
+    output_dir.mkdir(parents=True, exist_ok=True)
+    log_file = output_dir.joinpath("output.log")
+    log.addHandler(logging.FileHandler(log_file))
 
     input_files = [None] * yr._number_of_chips
     data = [
         qcDataFrame(
-            columns=[f"Vmux{v_mux}" for v_mux in inj_cap_config["v_mux"]]
-            + [f"Imux{i_mux}" for i_mux in inj_cap_config["i_mux"]],
-            units=["V" for v_mux in inj_cap_config["v_mux"]]
-            + ["V" for i_mux in inj_cap_config["i_mux"]],
+            columns=["Temperature", "SetCurrent", "Current", "FailingPixels"]
+            + [f"Vmux{v_mux}" for v_mux in LP_config["v_mux"]]
+            + [f"Imux{i_mux}" for i_mux in LP_config["i_mux"]],
+            units=["C", "A", "A", "Counts"]
+            + ["V" for v_mux in LP_config["v_mux"]]
+            + ["V" for i_mux in LP_config["i_mux"]],
         )
         for input_file in input_files
     ]
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
-        data[chip].add_property(
-            test_type + "_MEASUREMENT_VERSION",
-            pkg_resources.get_distribution("module-qc-tools").version,
-        )
+        data[chip].set_x("Current", True)
         data[chip]._meta_data = get_identifiers(yr.get_config(chip))
         data[chip].add_meta_data("Institution", institution)
         data[chip].add_meta_data("ModuleSN", module_serial)
         data[chip].add_meta_data("TimeStart", round(datetime.timestamp(datetime.now())))
         data[chip]._meta_data.update(get_meta_data(yr.get_config(chip)))
-
-    logging.basicConfig(level=logging.DEBUG)
-    logger = logging.getLogger(__name__)
+        data[chip].add_property(
+            test_type + "_MEASUREMENT_VERSION",
+            pkg_resources.get_distribution("module-qc-tools").version,
+        )
 
     try:
-        run(data, inj_cap_config, ps, yr, meter, layer)
+        run(
+            data,
+            LP_config,
+            NOMINAL_config,
+            ps,
+            yr,
+            meter,
+            nt,
+            layer,
+            output_dir,
+            log_file,
+        )
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
-        logger.exception(err)
-        sys.exit(1)
+        log.exception(err)
+        raise typer.Exit(1) from err
 
+    for chip in range(yr._number_of_chips):
+        if chip in yr._disabled_chip_positions:
+            continue
+        data[chip].add_meta_data("TimeEnd", round(datetime.timestamp(datetime.now())))
+        data[chip].add_meta_data(
+            "AverageTemperature", np.average(data[chip]["Temperature"])
+        )
+
+    # save results in json
     log.info(
         "==================================Summary=================================="
     )
     alloutput = []
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
-        chip_name = data[chip]._meta_data["Name"]
-        data[chip].add_meta_data("TimeEnd", round(datetime.timestamp(datetime.now())))
-        log.info("data[chip]: ")
+        log.info(f"Chip-{chip+1}")
         log.info(data[chip])
+        chip_name = data[chip]._meta_data["Name"]
         outputDF = outputDataFrame()
         outputDF.set_test_type(test_type)
         outputDF.set_results(data[chip])
-        if args.perchip:
+        if perchip:
             save_dict_list(
-                f"{output_dir}/Measurements/{test_type}/{timestart}/{chip_name}.json",
+                output_dir.joinpath(f"{chip_name}.json"),
                 [outputDF.to_dict()],
             )
         else:
             alloutput += [outputDF.to_dict()]
-    if not args.perchip:
+    if not perchip:
         save_dict_list(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/{module_serial}.json",
+            output_dir.joinpath(f"{module_serial}.json"),
             alloutput,
         )
 
-    log.info(
-        f"Writing output measurements in {output_dir}/Measurements/{test_type}/{timestart}/"
-    )
-    log.info("[run_inj_capacitance] Done!")
-    log.info(
-        f"[run_inj_capacitance] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
-    )
+    log.info(f"Writing output measurements in {output_dir}")
+    log.info("[run_LP] Done!")
+    log.info(f"[run_LP] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}")
 
 
 if __name__ == "__main__":
-    main()
+    typer.run(main)
```

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/cli/LP_MODE.py` & `module_qc_tools-2.0.1/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,236 +1,191 @@
-#!/usr/bin/env python
-from __future__ import annotations
-
 import copy
 import json
 import logging
-import re
 import sys
-from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
+from typing import Optional
 
 import numpy as np
 import pkg_resources
+import typer
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 from tabulate import tabulate
 
-from module_qc_tools import data
+from module_qc_tools.cli.globals import (
+    CONTEXT_SETTINGS,
+    OPTIONS,
+    LogLevel,
+)
 from module_qc_tools.utils.misc import bcolors, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
 from module_qc_tools.utils.ntc import ntc
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger("measurement")
 
-parser = ArgumentParser()
-parser.add_argument(
-    "-c",
-    "--config",
-    action="store",
-    default=data / "configs/example_merged_vmux.json",
-    help="Config file",
-)
-parser.add_argument(
-    "-o",
-    "--output-dir",
-    action="store",
-    default="outputs",
-    help="output directory",
-)
-parser.add_argument(
-    "-m",
-    "--module-connectivity",
-    action="store",
-    help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
-)
-parser.add_argument(
-    "--perchip",
-    action="store_true",
-    help="Store results in one file per chip (default: one file per module)",
-)
-parser.add_argument(
-    "-v",
-    "--verbosity",
-    action="store",
-    default="INFO",
-    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
-)
-args = parser.parse_args()
+app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
 
-def run(
-    data, LP_config, NOMINAL_config, ps, yr, meter, nt, layer, output_dir, log_file
-):
+def run(data, OVP_config, NOMINAL_config, ps, yr, meter, nt, layer):
     # turn off power supply before switching low power mode on
     ps.off()
     # turn on low power mode
     yr.switchLPM("on")
     # turn on power supply and configure all chips
     if yr.running_emulator():
-        ps.on(v=LP_config["v_max"], i=LP_config["i_config"][layer])
+        ps.on(v=OVP_config["v_max"], i=OVP_config["i_config"][layer])
     else:
-        ps.set(v=LP_config["v_max"], i=LP_config["i_config"][layer])
+        ps.set(v=OVP_config["v_max"], i=OVP_config["i_config"][layer])
         ps.on()
     status = yr.configure()
 
+    # Increase current to trigger OVP
+    ps.set(v=OVP_config["v_max"], i=OVP_config["i_ovp"][layer])
+
     # measure current for power supply
-    i = LP_config["i_config"][layer]
+    i = OVP_config["i_config"][layer]
     current, status = ps.getI()
     i_mea = [{} for _ in range(yr._number_of_chips)]
-
-    # Run digital scan
-    yr.run_scan(yr.lpm_digitalscan, f"{output_dir}/YARRscans/")
-
-    # Search log contents for failing pixels
-    with Path(log_file).open() as f:
-        yarr_output = f.readlines()
-    failing_pixels = {}
-    for line in yarr_output:
-        if "Total number of failing pixels" in line:
-            chip_name = "0x" + re.search(r"\[.*?0x(.*?)\].*", line).group(1)
-            nFail = re.search(r"^\d+", line.split(" ")[-1]).group()
-            log.debug(f"{chip_name} has {nFail} failing pixels")
-            failing_pixels.update({chip_name: int(nFail)})
-
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
-
-        # Store of bad pixels in log file
-        chip_name = data[chip]._meta_data["Name"]
-        if chip_name in failing_pixels:
-            i_mea[chip]["FailingPixels"] = [failing_pixels.get(chip_name)]
-        else:
-            i_mea[chip]["FailingPixels"] = [-1]
-
         i_mea[chip]["SetCurrent"] = [i]
         i_mea[chip]["Current"] = [current]
         # measure temperature from NTC
         temp, status = nt.read()
         i_mea[chip]["Temperature"] = [temp]
         # measure v_mux
-        for v_mux in LP_config["v_mux"]:
+        for v_mux in OVP_config["v_mux"]:
             yr.set_mux(
                 chip_position=chip,
                 v_mux=v_mux,
-                reset_other_chips=LP_config["share_vmux"],
+                reset_other_chips=OVP_config["share_vmux"],
             )
-            mea, status = meter.measure_dcv(channel=LP_config["v_mux_channels"][chip])
+            mea, status = meter.measure_dcv(channel=OVP_config["v_mux_channels"][chip])
             i_mea[chip][f"Vmux{v_mux}"] = [mea]
         # measure i_mux
-        for i_mux in LP_config["i_mux"]:
+        for i_mux in OVP_config["i_mux"]:
             yr.set_mux(
                 chip_position=chip,
                 i_mux=i_mux,
-                reset_other_chips=LP_config["share_vmux"],
+                reset_other_chips=OVP_config["share_vmux"],
             )
-            mea, status = meter.measure_dcv(channel=LP_config["v_mux_channels"][chip])
+            mea, status = meter.measure_dcv(channel=OVP_config["v_mux_channels"][chip])
             i_mea[chip][f"Imux{i_mux}"] = [mea]
         data[chip].add_data(i_mea[chip])
         log.info(
             "--------------------------------------------------------------------------"
         )
         log.info(f"Chip-{chip+1}")
         log.info(tabulate(i_mea[chip], headers="keys", floatfmt=".3f"))
+
     # turn off power supply before switching low power mode off
     ps.off()
     # turn off low power mode
     yr.switchLPM("off")
+    # Return to initial state
     if yr.running_emulator():
         ps.on(v=NOMINAL_config["v_max"], i=NOMINAL_config["i_config"][layer])
     else:
         ps.set(v=NOMINAL_config["v_max"], i=NOMINAL_config["i_config"][layer])
         ps.on()
 
 
-def main():
-    log.setLevel(args.verbosity)
+@app.command()
+def main(
+    config_path: Path = OPTIONS["config"],
+    base_output_dir: Path = OPTIONS["output_dir"],
+    module_connectivity: Optional[Path] = OPTIONS["module_connectivity"],
+    verbosity: LogLevel = OPTIONS["verbosity"],
+    perchip: bool = OPTIONS["perchip"],
+    use_pixel_config: bool = OPTIONS["use_pixel_config"],
+):
+    log.setLevel(verbosity.value)
 
-    log.info("[run_LP] Start LP Mode scan!")
+    log.info("[run_OVP] Start OVP test!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-    log.info(f"[run_LP] TimeStart: {timestart}")
+    log.info(f"[run_OVP] TimeStart: {timestart}")
 
-    with resources.as_file(Path(args.config)) as path:
+    with resources.as_file(Path(config_path)) as path:
         config = json.loads(path.read_text())
 
     # Need to pass module connectivity path to yarr class (except in case we are running the emulator)
-    if args.module_connectivity:
-        config["yarr"]["connectivity"] = args.module_connectivity
+    if module_connectivity:
+        config["yarr"]["connectivity"] = module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
-    if "emulator" not in args.config and not args.module_connectivity:
-        msg = "must supply path to connectivity file [-m --module-connectivity]"
-        raise RuntimeError(msg)
-    if args.module_connectivity and "LP" not in args.module_connectivity:
+    if "emulator" not in str(config_path) and not module_connectivity:
+        typer.echo("must supply path to connectivity file [-m --module-connectivity]")
+        raise typer.Exit(2)
+
+    if module_connectivity and "LP" not in module_connectivity:
         log.warning(
             bcolors.WARNING
-            + f"You supplied a module connectivity ({args.module_connectivity}) which does not have 'LP' (low-power) in the name. Are you sure this is the connectivity file for low-power configuration? If not, chip will fail to configure."
+            + f"You supplied a module connectivity ({module_connectivity}) which does not have 'LP' (low-power) in the name. Are you sure this is the connectivity file for low-power configuration? If not, chip will fail to configure."
             + bcolors.ENDC
         )
 
     NOMINAL_config = config["tasks"]["GENERAL"]
-    LP_config = copy.deepcopy(config["tasks"]["GENERAL"])
-    LP_config.update(config["tasks"]["LP_MODE"])
+    OVP_config = copy.deepcopy(config["tasks"]["GENERAL"])
+    OVP_config.update(config["tasks"]["OVERVOLTAGE_PROTECTION"])
     ps = power_supply(config["power_supply"])
     yr = yarr(config["yarr"])
 
     meter = multimeter(config["multimeter"])
     nt = ntc(config["ntc"])
 
+    if not use_pixel_config:
+        yr.omit_pixel_config("tmp")
+
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
     test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if institution is None:
         institution = ""
 
     # if -o option used, overwrite the default output directory
-    if args.module_connectivity:
-        output_dir = args.module_connectivity.rsplit("/", 1)[0]
-    else:
-        output_dir = args.output_dir
+    output_dir = module_connectivity.parent if module_connectivity else base_output_dir
 
-    if args.output_dir != "outputs":
-        output_dir = args.output_dir
+    if base_output_dir != Path("outputs"):
+        output_dir = base_output_dir
 
+    output_dir = output_dir.joinpath("Measurements", test_type, timestart)
     # Make output directory and start log file
-    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
-        parents=True, exist_ok=True
-    )
-    log_file = f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
-    log.addHandler(logging.FileHandler(log_file))
+    output_dir.mkdir(parents=True, exist_ok=True)
+    log.addHandler(logging.FileHandler(output_dir.joinpath("output.log")))
 
     input_files = [None] * yr._number_of_chips
     data = [
         qcDataFrame(
-            columns=["Temperature", "SetCurrent", "Current", "FailingPixels"]
-            + [f"Vmux{v_mux}" for v_mux in LP_config["v_mux"]]
-            + [f"Imux{i_mux}" for i_mux in LP_config["i_mux"]],
-            units=["C", "A", "A", "Counts"]
-            + ["V" for v_mux in LP_config["v_mux"]]
-            + ["V" for i_mux in LP_config["i_mux"]],
+            columns=["Temperature", "SetCurrent", "Current"]
+            + [f"Vmux{v_mux}" for v_mux in OVP_config["v_mux"]]
+            + [f"Imux{i_mux}" for i_mux in OVP_config["i_mux"]],
+            units=["C", "A", "A"]
+            + ["V" for v_mux in OVP_config["v_mux"]]
+            + ["V" for i_mux in OVP_config["i_mux"]],
         )
         for input_file in input_files
     ]
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
@@ -242,31 +197,20 @@
         data[chip]._meta_data.update(get_meta_data(yr.get_config(chip)))
         data[chip].add_property(
             test_type + "_MEASUREMENT_VERSION",
             pkg_resources.get_distribution("module-qc-tools").version,
         )
 
     try:
-        run(
-            data,
-            LP_config,
-            NOMINAL_config,
-            ps,
-            yr,
-            meter,
-            nt,
-            layer,
-            output_dir,
-            log_file,
-        )
+        run(data, OVP_config, NOMINAL_config, ps, yr, meter, nt, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.exception(err)
-        sys.exit(1)
+        raise typer.Exit(1) from err
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
         data[chip].add_meta_data("TimeEnd", round(datetime.timestamp(datetime.now())))
         data[chip].add_meta_data(
             "AverageTemperature", np.average(data[chip]["Temperature"])
@@ -282,29 +226,31 @@
             continue
         log.info(f"Chip-{chip+1}")
         log.info(data[chip])
         chip_name = data[chip]._meta_data["Name"]
         outputDF = outputDataFrame()
         outputDF.set_test_type(test_type)
         outputDF.set_results(data[chip])
-        if args.perchip:
+        if perchip:
             save_dict_list(
-                f"{output_dir}/Measurements/{test_type}/{timestart}/{chip_name}.json",
+                output_dir.joinpath(f"{chip_name}.json"),
                 [outputDF.to_dict()],
             )
         else:
             alloutput += [outputDF.to_dict()]
-    if not args.perchip:
+    if not perchip:
         save_dict_list(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/{module_serial}.json",
+            output_dir.joinpath(f"{module_serial}.json"),
             alloutput,
         )
 
-    log.info(
-        f"Writing output measurements in {output_dir}/Measurements/{test_type}/{timestart}/"
-    )
-    log.info("[run_LP] Done!")
-    log.info(f"[run_LP] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}")
+    log.info(f"Writing output measurements in {output_dir}")
+    log.info("[run_OVP] Done!")
+    log.info(f"[run_OVP] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}")
+
+    # Delete temporary files
+    if not use_pixel_config:
+        yr.remove_tmp_connectivity()
 
 
 if __name__ == "__main__":
-    main()
+    typer.run(main)
```

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py` & `module_qc_tools-2.0.1/src/module_qc_tools/cli/SLDO.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,219 +1,183 @@
-#!/usr/bin/env python
-from __future__ import annotations
-
-import copy
 import json
 import logging
 import sys
-from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
+from typing import Optional
 
 import numpy as np
 import pkg_resources
+import typer
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 from tabulate import tabulate
 
-from module_qc_tools import data
-from module_qc_tools.utils.misc import bcolors, get_identifiers, get_meta_data
+from module_qc_tools.cli.globals import (
+    CONTEXT_SETTINGS,
+    OPTIONS,
+    LogLevel,
+)
+from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
 from module_qc_tools.utils.ntc import ntc
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger("measurement")
 
-parser = ArgumentParser()
-parser.add_argument(
-    "-c",
-    "--config",
-    action="store",
-    default=data / "configs/example_merged_vmux.json",
-    help="Config file",
-)
-parser.add_argument(
-    "-o",
-    "--output-dir",
-    action="store",
-    default="outputs",
-    help="output directory",
-)
-parser.add_argument(
-    "-m",
-    "--module-connectivity",
-    action="store",
-    help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
-)
-parser.add_argument(
-    "--perchip",
-    action="store_true",
-    help="Store results in one file per chip (default: one file per module)",
-)
-parser.add_argument(
-    "-v",
-    "--verbosity",
-    action="store",
-    default="INFO",
-    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
-)
-args = parser.parse_args()
+app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
 
-def run(data, OVP_config, NOMINAL_config, ps, yr, meter, nt, layer):
-    # turn off power supply before switching low power mode on
-    ps.off()
-    # turn on low power mode
-    yr.switchLPM("on")
+def run(data, SLDOVI_config, ps, yr, meter, nt, layer):
     # turn on power supply and configure all chips
-    if yr.running_emulator():
-        ps.on(v=OVP_config["v_max"], i=OVP_config["i_config"][layer])
-    else:
-        ps.set(v=OVP_config["v_max"], i=OVP_config["i_config"][layer])
-        ps.on()
+    ps.set(v=SLDOVI_config["v_max"], i=SLDOVI_config["i_config"][layer])
     status = yr.configure()
 
-    # Increase current to trigger OVP
-    ps.set(v=OVP_config["v_max"], i=OVP_config["i_ovp"][layer])
-
-    # measure current for power supply
-    i = OVP_config["i_config"][layer]
-    current, status = ps.getI()
-    i_mea = [{} for _ in range(yr._number_of_chips)]
-    for chip in range(yr._number_of_chips):
-        if chip in yr._disabled_chip_positions:
-            continue
-        i_mea[chip]["SetCurrent"] = [i]
-        i_mea[chip]["Current"] = [current]
-        # measure temperature from NTC
-        temp, status = nt.read()
-        i_mea[chip]["Temperature"] = [temp]
-        # measure v_mux
-        for v_mux in OVP_config["v_mux"]:
-            yr.set_mux(
-                chip_position=chip,
-                v_mux=v_mux,
-                reset_other_chips=OVP_config["share_vmux"],
-            )
-            mea, status = meter.measure_dcv(channel=OVP_config["v_mux_channels"][chip])
-            i_mea[chip][f"Vmux{v_mux}"] = [mea]
-        # measure i_mux
-        for i_mux in OVP_config["i_mux"]:
-            yr.set_mux(
-                chip_position=chip,
-                i_mux=i_mux,
-                reset_other_chips=OVP_config["share_vmux"],
+    currents = sorted(
+        np.concatenate(
+            [
+                np.linspace(
+                    SLDOVI_config["i_min"][layer],
+                    SLDOVI_config["i_max"][layer],
+                    SLDOVI_config["n_points"][layer],
+                ),
+                np.array(SLDOVI_config["extra_i"]),
+            ]
+        ),
+        reverse=True,
+    )
+    for i in currents:
+        # set and measure current for power supply
+        ps.set(v=SLDOVI_config["v_max"], i=i)
+        current, status = ps.getI()
+        i_mea = [{} for _ in range(yr._number_of_chips)]
+        for chip in range(yr._number_of_chips):
+            if chip in yr._disabled_chip_positions:
+                continue
+            i_mea[chip]["SetCurrent"] = [i]
+            i_mea[chip]["Current"] = [current]
+            # measure temperature from NTC
+            temp, status = nt.read()
+            i_mea[chip]["Temperature"] = [temp]
+            # measure v_mux
+            for v_mux in SLDOVI_config["v_mux"]:
+                yr.set_mux(
+                    chip_position=chip,
+                    v_mux=v_mux,
+                    reset_other_chips=SLDOVI_config["share_vmux"],
+                )
+                mea, status = meter.measure_dcv(
+                    channel=SLDOVI_config["v_mux_channels"][chip]
+                )
+                i_mea[chip][f"Vmux{v_mux}"] = [mea]
+            # measure i_mux
+            for i_mux in SLDOVI_config["i_mux"]:
+                yr.set_mux(
+                    chip_position=chip,
+                    i_mux=i_mux,
+                    reset_other_chips=SLDOVI_config["share_vmux"],
+                )
+                mea, status = meter.measure_dcv(
+                    channel=SLDOVI_config["v_mux_channels"][chip]
+                )
+                i_mea[chip][f"Imux{i_mux}"] = [mea]
+            data[chip].add_data(i_mea[chip])
+            log.info(
+                "--------------------------------------------------------------------------"
             )
-            mea, status = meter.measure_dcv(channel=OVP_config["v_mux_channels"][chip])
-            i_mea[chip][f"Imux{i_mux}"] = [mea]
-        data[chip].add_data(i_mea[chip])
-        log.info(
-            "--------------------------------------------------------------------------"
-        )
-        log.info(f"Chip-{chip+1}")
-        log.info(tabulate(i_mea[chip], headers="keys", floatfmt=".3f"))
+            log.info(f"Chip-{chip+1}")
+            log.info(tabulate(i_mea[chip], headers="keys", floatfmt=".3f"))
 
-    # turn off power supply before switching low power mode off
-    ps.off()
-    # turn off low power mode
-    yr.switchLPM("off")
     # Return to initial state
-    if yr.running_emulator():
-        ps.on(v=NOMINAL_config["v_max"], i=NOMINAL_config["i_config"][layer])
-    else:
-        ps.set(v=NOMINAL_config["v_max"], i=NOMINAL_config["i_config"][layer])
-        ps.on()
+    ps.set(v=SLDOVI_config["v_max"], i=SLDOVI_config["i_config"][layer])
 
 
-def main():
-    log.setLevel(args.verbosity)
+@app.command()
+def main(
+    config_path: Path = OPTIONS["config"],
+    base_output_dir: Path = OPTIONS["output_dir"],
+    module_connectivity: Optional[Path] = OPTIONS["module_connectivity"],
+    verbosity: LogLevel = OPTIONS["verbosity"],
+    perchip: bool = OPTIONS["perchip"],
+    use_pixel_config: bool = OPTIONS["use_pixel_config"],
+):
+    log.setLevel(verbosity.value)
 
-    log.info("[run_OVP] Start OVP test!")
+    log.info("[run_SLDOVI] Start VI scan!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-    log.info(f"[run_OVP] TimeStart: {timestart}")
+    log.info(f"[run_SLDOVI] TimeStart: {timestart}")
 
-    with resources.as_file(Path(args.config)) as path:
+    with resources.as_file(Path(config_path)) as path:
         config = json.loads(path.read_text())
 
+    check_meas_config(config, config_path)
+
     # Need to pass module connectivity path to yarr class (except in case we are running the emulator)
-    if args.module_connectivity:
-        config["yarr"]["connectivity"] = args.module_connectivity
+    if module_connectivity:
+        config["yarr"]["connectivity"] = module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
-    if "emulator" not in args.config and not args.module_connectivity:
-        msg = "must supply path to connectivity file [-m --module-connectivity]"
-        raise RuntimeError(msg)
-
-    if args.module_connectivity and "LP" not in args.module_connectivity:
-        log.warning(
-            bcolors.WARNING
-            + f"You supplied a module connectivity ({args.module_connectivity}) which does not have 'LP' (low-power) in the name. Are you sure this is the connectivity file for low-power configuration? If not, chip will fail to configure."
-            + bcolors.ENDC
-        )
+    if "emulator" not in str(config_path) and not module_connectivity:
+        typer.echo("must supply path to connectivity file [-m --module-connectivity]")
+        raise typer.Exit(2)
 
-    NOMINAL_config = config["tasks"]["GENERAL"]
-    OVP_config = copy.deepcopy(config["tasks"]["GENERAL"])
-    OVP_config.update(config["tasks"]["OVERVOLTAGE_PROTECTION"])
+    SLDOVI_config = config["tasks"]["GENERAL"]
+    SLDOVI_config.update(config["tasks"]["SLDO"])
     ps = power_supply(config["power_supply"])
     yr = yarr(config["yarr"])
 
     meter = multimeter(config["multimeter"])
     nt = ntc(config["ntc"])
 
+    if not use_pixel_config:
+        yr.omit_pixel_config("tmp")
+
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
     test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if institution is None:
         institution = ""
 
     # if -o option used, overwrite the default output directory
-    if args.module_connectivity:
-        output_dir = args.module_connectivity.rsplit("/", 1)[0]
-    else:
-        output_dir = args.output_dir
+    output_dir = module_connectivity.parent if module_connectivity else base_output_dir
 
-    if args.output_dir != "outputs":
-        output_dir = args.output_dir
+    if base_output_dir != Path("outputs"):
+        output_dir = base_output_dir
 
+    output_dir = output_dir.joinpath("Measurements", test_type, timestart)
     # Make output directory and start log file
-    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
-        parents=True, exist_ok=True
-    )
-    log.addHandler(
-        logging.FileHandler(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
-        )
-    )
+    output_dir.mkdir(parents=True, exist_ok=True)
+    log.addHandler(logging.FileHandler(output_dir.joinpath("output.log")))
 
     input_files = [None] * yr._number_of_chips
     data = [
         qcDataFrame(
             columns=["Temperature", "SetCurrent", "Current"]
-            + [f"Vmux{v_mux}" for v_mux in OVP_config["v_mux"]]
-            + [f"Imux{i_mux}" for i_mux in OVP_config["i_mux"]],
+            + [f"Vmux{v_mux}" for v_mux in SLDOVI_config["v_mux"]]
+            + [f"Imux{i_mux}" for i_mux in SLDOVI_config["i_mux"]],
             units=["C", "A", "A"]
-            + ["V" for v_mux in OVP_config["v_mux"]]
-            + ["V" for i_mux in OVP_config["i_mux"]],
+            + ["V" for v_mux in SLDOVI_config["v_mux"]]
+            + ["V" for i_mux in SLDOVI_config["i_mux"]],
         )
         for input_file in input_files
     ]
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
@@ -225,20 +189,20 @@
         data[chip]._meta_data.update(get_meta_data(yr.get_config(chip)))
         data[chip].add_property(
             test_type + "_MEASUREMENT_VERSION",
             pkg_resources.get_distribution("module-qc-tools").version,
         )
 
     try:
-        run(data, OVP_config, NOMINAL_config, ps, yr, meter, nt, layer)
+        run(data, SLDOVI_config, ps, yr, meter, nt, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.exception(err)
-        sys.exit(1)
+        raise typer.Exit(1) from err
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
         data[chip].add_meta_data("TimeEnd", round(datetime.timestamp(datetime.now())))
         data[chip].add_meta_data(
             "AverageTemperature", np.average(data[chip]["Temperature"])
@@ -254,29 +218,31 @@
             continue
         log.info(f"Chip-{chip+1}")
         log.info(data[chip])
         chip_name = data[chip]._meta_data["Name"]
         outputDF = outputDataFrame()
         outputDF.set_test_type(test_type)
         outputDF.set_results(data[chip])
-        if args.perchip:
+        if perchip:
             save_dict_list(
-                f"{output_dir}/Measurements/{test_type}/{timestart}/{chip_name}.json",
+                output_dir.joinpath(f"{chip_name}.json"),
                 [outputDF.to_dict()],
             )
         else:
             alloutput += [outputDF.to_dict()]
-    if not args.perchip:
+    if not perchip:
         save_dict_list(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/{module_serial}.json",
+            output_dir.joinpath(f"{module_serial}.json"),
             alloutput,
         )
 
-    log.info(
-        f"Writing output measurements in {output_dir}/Measurements/{test_type}/{timestart}/"
-    )
-    log.info("[run_OVP] Done!")
-    log.info(f"[run_OVP] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}")
+    log.info(f"Writing output measurements in {output_dir}")
+    log.info("[run_SLDOVI] Done!")
+    log.info(f"[run_SLDOVI] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}")
+
+    # Delete temporary files
+    if not use_pixel_config:
+        yr.remove_tmp_connectivity()
 
 
 if __name__ == "__main__":
-    main()
+    typer.run(main)
```

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/cli/SLDO.py` & `module_qc_tools-2.0.1/src/module_qc_tools/cli/ADC_CALIBRATION.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,274 +1,243 @@
-#!/usr/bin/env python
-from __future__ import annotations
-
 import json
 import logging
 import sys
-from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
+from typing import Optional
 
 import numpy as np
 import pkg_resources
+import typer
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
-from tabulate import tabulate
 
-from module_qc_tools import data
+from module_qc_tools.cli.globals import (
+    CONTEXT_SETTINGS,
+    OPTIONS,
+    LogLevel,
+)
 from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
-from module_qc_tools.utils.ntc import ntc
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger("measurement")
 
-parser = ArgumentParser()
-parser.add_argument(
-    "-c",
-    "--config",
-    action="store",
-    default=data / "configs/example_merged_vmux.json",
-    help="Config file",
-)
-parser.add_argument(
-    "-o",
-    "--output-dir",
-    action="store",
-    default="outputs",
-    help="output directory",
-)
-parser.add_argument(
-    "-m",
-    "--module-connectivity",
-    action="store",
-    help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
-)
-parser.add_argument(
-    "--perchip",
-    action="store_true",
-    help="Store results in one file per chip (default: one file per module)",
-)
-parser.add_argument(
-    "-v",
-    "--verbosity",
-    action="store",
-    default="INFO",
-    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
-)
-args = parser.parse_args()
+app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
 
-def run(data, SLDOVI_config, ps, yr, meter, nt, layer):
-    # turn on power supply and configure all chips
-    ps.set(v=SLDOVI_config["v_max"], i=SLDOVI_config["i_config"][layer])
+def run(data, adc_calib_config, ps, yr, meter, layer):
+    """The function which does the ADC calibration.
+
+    Args:
+        data (list): data[chip_id].
+        adc_calib_config (dict): An subdict dumped from json including the task information.
+        ps (Class power_supply): An instance of Class power_supply for power on and power off.
+        yr (Class yarr): An instance of Class yarr for chip conifugration and change register.
+        meter (Class meter): An instance of Class meter. Used to control the multimeter to measure voltages.
+
+    Returns:
+        None: The measurements are recorded in `data`.
+    """
+    if yr.running_emulator():
+        ps.on(
+            adc_calib_config["v_max"], adc_calib_config["i_config"][layer]
+        )  # Only for emulator do the emulation of power on/off
+        # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
+
     status = yr.configure()
+    assert status >= 0
 
-    currents = sorted(
-        np.concatenate(
-            [
-                np.linspace(
-                    SLDOVI_config["i_min"][layer],
-                    SLDOVI_config["i_max"][layer],
-                    SLDOVI_config["n_points"][layer],
-                ),
-                np.array(SLDOVI_config["extra_i"]),
-            ]
-        ),
-        reverse=True,
-    )
-    for i in currents:
-        # set and measure current for power supply
-        ps.set(v=SLDOVI_config["v_max"], i=i)
-        current, status = ps.getI()
-        i_mea = [{} for _ in range(yr._number_of_chips)]
+    InjVcalRange = adc_calib_config["InjVcalRange"]
+    MonitorV = adc_calib_config["MonitorV"]
+
+    Range = [
+        adc_calib_config["Range"]["start"],
+        adc_calib_config["Range"]["stop"],
+        adc_calib_config["Range"]["step"],
+    ]
+    DACs = np.arange(start=Range[0], stop=Range[1], step=Range[2])
+
+    for DAC in DACs:
+        v_mea = [{} for _ in range(yr._number_of_chips)]
         for chip in range(yr._number_of_chips):
             if chip in yr._disabled_chip_positions:
                 continue
-            i_mea[chip]["SetCurrent"] = [i]
-            i_mea[chip]["Current"] = [current]
-            # measure temperature from NTC
-            temp, status = nt.read()
-            i_mea[chip]["Temperature"] = [temp]
-            # measure v_mux
-            for v_mux in SLDOVI_config["v_mux"]:
-                yr.set_mux(
-                    chip_position=chip,
-                    v_mux=v_mux,
-                    reset_other_chips=SLDOVI_config["share_vmux"],
-                )
-                mea, status = meter.measure_dcv(
-                    channel=SLDOVI_config["v_mux_channels"][chip]
-                )
-                i_mea[chip][f"Vmux{v_mux}"] = [mea]
-            # measure i_mux
-            for i_mux in SLDOVI_config["i_mux"]:
+
+            yr.write_register("MonitorEnable", 1, chip)
+            yr.write_register("InjVcalMed", DAC, chip)  # write DAC values
+            v_mea[chip]["DACs_input"] = [float(DAC)]
+
+            yr.write_register("InjVcalRange", InjVcalRange, chip)
+            for i, vmux_value in enumerate(MonitorV):
                 yr.set_mux(
                     chip_position=chip,
-                    i_mux=i_mux,
-                    reset_other_chips=SLDOVI_config["share_vmux"],
-                )
-                mea, status = meter.measure_dcv(
-                    channel=SLDOVI_config["v_mux_channels"][chip]
+                    v_mux=MonitorV[i],
+                    reset_other_chips=adc_calib_config["share_vmux"],
                 )
-                i_mea[chip][f"Imux{i_mux}"] = [mea]
-            data[chip].add_data(i_mea[chip])
-            log.info(
-                "--------------------------------------------------------------------------"
-            )
-            log.info(f"Chip-{chip+1}")
-            log.info(tabulate(i_mea[chip], headers="keys", floatfmt=".3f"))
-
-    # Return to initial state
-    ps.set(v=SLDOVI_config["v_max"], i=SLDOVI_config["i_config"][layer])
-
+                v_mea[chip][f"Vmux{vmux_value}"] = [meter.measure_dcv()[0]]
+                v_mea[chip][f"ADC_Vmux{vmux_value}"] = [
+                    int(yr.read_adc(MonitorV[i], chip_position=chip, rawCounts=True)[0])
+                ]
+            data[chip].add_data(v_mea[chip])
+
+    if yr.running_emulator():
+        ps.off()
+
+
+@app.command()
+def main(
+    config_path: Path = OPTIONS["config"],
+    base_output_dir: Path = OPTIONS["output_dir"],
+    module_connectivity: Optional[Path] = OPTIONS["module_connectivity"],
+    verbosity: LogLevel = OPTIONS["verbosity"],
+    perchip: bool = OPTIONS["perchip"],
+    use_pixel_config: bool = OPTIONS["use_pixel_config"],
+):
+    """main() creates the qcDataFrame and pass it to the run() where the measurements are stored in the qcDataFrame."""
 
-def main():
-    log.setLevel(args.verbosity)
+    log.setLevel(verbosity.value)
 
-    log.info("[run_SLDOVI] Start VI scan!")
+    log.info("[run_ADC_calib] Start ADC calibration!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-    log.info(f"[run_SLDOVI] TimeStart: {timestart}")
+    log.info(f"[run_ADC_calib] TimeStart: {timestart}")
 
-    with resources.as_file(Path(args.config)) as path:
+    with resources.as_file(config_path) as path:
         config = json.loads(path.read_text())
 
-    check_meas_config(config, args.config)
+    check_meas_config(config, config_path)
 
-    # Need to pass module connectivity path to yarr class (except in case we are running the emulator)
-    if args.module_connectivity:
-        config["yarr"]["connectivity"] = args.module_connectivity
+    if module_connectivity:
+        config["yarr"]["connectivity"] = module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
-    if "emulator" not in args.config and not args.module_connectivity:
-        msg = "must supply path to connectivity file [-m --module-connectivity]"
-        raise RuntimeError(msg)
+    if "emulator" not in str(config_path) and not module_connectivity:
+        typer.echo("must supply path to connectivity file [-m --module-connectivity]")
+        raise typer.Exit(2)
+
+    adc_calib_config = config["tasks"]["GENERAL"]
+    adc_calib_config.update(config["tasks"]["ADC_CALIBRATION"])
 
-    SLDOVI_config = config["tasks"]["GENERAL"]
-    SLDOVI_config.update(config["tasks"]["SLDO"])
     ps = power_supply(config["power_supply"])
     yr = yarr(config["yarr"])
-
     meter = multimeter(config["multimeter"])
-    nt = ntc(config["ntc"])
+
+    if not use_pixel_config:
+        yr.omit_pixel_config("tmp")
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
     test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if institution is None:
         institution = ""
 
+    ps.set(v=adc_calib_config["v_max"], i=adc_calib_config["i_config"][layer])
+
     # if -o option used, overwrite the default output directory
-    if args.module_connectivity:
-        output_dir = args.module_connectivity.rsplit("/", 1)[0]
-    else:
-        output_dir = args.output_dir
+    output_dir = module_connectivity.parent if module_connectivity else base_output_dir
 
-    if args.output_dir != "outputs":
-        output_dir = args.output_dir
+    if base_output_dir != Path("outputs"):
+        output_dir = base_output_dir
 
+    output_dir = output_dir.joinpath("Measurements", test_type, timestart)
     # Make output directory and start log file
-    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
-        parents=True, exist_ok=True
-    )
-    log.addHandler(
-        logging.FileHandler(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
-        )
-    )
+    output_dir.mkdir(parents=True, exist_ok=True)
+    log.addHandler(logging.FileHandler(output_dir.joinpath("output.log")))
+
+    InjVcalRange = adc_calib_config["InjVcalRange"]
 
     input_files = [None] * yr._number_of_chips
     data = [
         qcDataFrame(
-            columns=["Temperature", "SetCurrent", "Current"]
-            + [f"Vmux{v_mux}" for v_mux in SLDOVI_config["v_mux"]]
-            + [f"Imux{i_mux}" for i_mux in SLDOVI_config["i_mux"]],
-            units=["C", "A", "A"]
-            + ["V" for v_mux in SLDOVI_config["v_mux"]]
-            + ["V" for i_mux in SLDOVI_config["i_mux"]],
+            columns=["DACs_input"]
+            + [f"Vmux{v_mux}" for v_mux in adc_calib_config["MonitorV"]]
+            + [f"ADC_Vmux{v_mux}" for v_mux in adc_calib_config["MonitorV"]],
+            units=["Count"]
+            + ["V" for v_mux in adc_calib_config["MonitorV"]]
+            + ["Count" for v_mux in adc_calib_config["MonitorV"]],
         )
         for input_file in input_files
     ]
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
-        data[chip].set_x("Current", True)
+        data[chip].add_property(
+            test_type + "_MEASUREMENT_VERSION",
+            pkg_resources.get_distribution("module-qc-tools").version,
+        )
         data[chip]._meta_data = get_identifiers(yr.get_config(chip))
         data[chip].add_meta_data("Institution", institution)
         data[chip].add_meta_data("ModuleSN", module_serial)
         data[chip].add_meta_data("TimeStart", round(datetime.timestamp(datetime.now())))
         data[chip]._meta_data.update(get_meta_data(yr.get_config(chip)))
-        data[chip].add_property(
-            test_type + "_MEASUREMENT_VERSION",
-            pkg_resources.get_distribution("module-qc-tools").version,
-        )
+        data[chip]._meta_data["ChipConfigs"]["RD53B"]["GlobalConfig"][
+            "InjVcalRange"
+        ] = InjVcalRange
+        data[chip].set_x("DACs_input", True)
+
+    logging.basicConfig(level=logging.DEBUG)
+    logger = logging.getLogger(__name__)
 
     try:
-        run(data, SLDOVI_config, ps, yr, meter, nt, layer)
+        run(data, adc_calib_config, ps, yr, meter, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
-        log.exception(err)
-        sys.exit(1)
-
-    for chip in range(yr._number_of_chips):
-        if chip in yr._disabled_chip_positions:
-            continue
-        data[chip].add_meta_data("TimeEnd", round(datetime.timestamp(datetime.now())))
-        data[chip].add_meta_data(
-            "AverageTemperature", np.average(data[chip]["Temperature"])
-        )
+        logger.exception(err)
+        raise typer.Exit(1) from err
 
-    # save results in json
     log.info(
         "==================================Summary=================================="
     )
     alloutput = []
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
-        log.info(f"Chip-{chip+1}")
-        log.info(data[chip])
         chip_name = data[chip]._meta_data["Name"]
+        data[chip].add_meta_data("TimeEnd", round(datetime.timestamp(datetime.now())))
+        log.info("data[chip]: ")
+        log.info(data[chip])
         outputDF = outputDataFrame()
         outputDF.set_test_type(test_type)
         outputDF.set_results(data[chip])
-        if args.perchip:
+        if perchip:
             save_dict_list(
-                f"{output_dir}/Measurements/{test_type}/{timestart}/{chip_name}.json",
+                output_dir.joinpath(f"{chip_name}.json"),
                 [outputDF.to_dict()],
             )
         else:
             alloutput += [outputDF.to_dict()]
-    if not args.perchip:
+    if not perchip:
         save_dict_list(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/{module_serial}.json",
+            output_dir.joinpath(f"{module_serial}.json"),
             alloutput,
         )
 
-    log.info(
-        f"Writing output measurements in {output_dir}/Measurements/{test_type}/{timestart}/"
-    )
-    log.info("[run_SLDOVI] Done!")
-    log.info(f"[run_SLDOVI] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}")
+    log.info(f"Writing output measurements in {output_dir}")
+    log.info("[run_ADC_calib] Done!")
+    log.info(f"[run_ADC_calib] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}")
+
+    # Delete temporary files
+    if not use_pixel_config:
+        yr.remove_tmp_connectivity()
 
 
 if __name__ == "__main__":
-    main()
+    typer.run(main)
```

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/cli/VCAL_CALIBRATION.py` & `module_qc_tools-2.0.1/src/module_qc_tools/cli/VCAL_CALIBRATION.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,45 @@
-#!/usr/bin/env python3
-from __future__ import annotations
-
 import json
 import logging
 import sys
-from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
+from typing import Optional
 
 import numpy as np
 import pkg_resources
+import typer
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
-from module_qc_tools import data
+from module_qc_tools.cli.globals import (
+    CONTEXT_SETTINGS,
+    OPTIONS,
+    LogLevel,
+)
 from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger("measurement")
 
-
-parser = ArgumentParser()
-parser.add_argument(
-    "-c",
-    "--config",
-    action="store",
-    default=data / "configs/example_merged_vmux.json",
-    help="Config file",
-)
-parser.add_argument(
-    "-o",
-    "--output-dir",
-    action="store",
-    default="outputs",
-    help="output directory",
-)
-parser.add_argument(
-    "-m",
-    "--module-connectivity",
-    action="store",
-    help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
-)
-parser.add_argument(
-    "-v",
-    "--verbosity",
-    action="store",
-    default="INFO",
-    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
-)
-parser.add_argument(
-    "--perchip",
-    action="store_true",
-    help="Store results in one file per chip (default: one file per module)",
-)
-args = parser.parse_args()
+app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
 
 def run(data, vcal_calib_config, ps, yr, meter, layer):
     """The function which does the VCal calibration for VCal_Med and VCal_Hi in both large and small range.
 
     Args:
         data (list): data[chip_id][vcal_type]. 4 vcal_type in total.
@@ -174,43 +142,54 @@
                 )
                 cal_count += 1
 
     if yr.running_emulator():
         ps.off()
 
 
-def main():
+@app.command()
+def main(
+    config_path: Path = OPTIONS["config"],
+    base_output_dir: Path = OPTIONS["output_dir"],
+    module_connectivity: Optional[Path] = OPTIONS["module_connectivity"],
+    verbosity: LogLevel = OPTIONS["verbosity"],
+    perchip: bool = OPTIONS["perchip"],
+    use_pixel_config: bool = OPTIONS["use_pixel_config"],
+):
     """main() creates the qcDataFrame and pass it to the run() where the measurements are stored in the qcDataFrame."""
 
-    log.setLevel(args.verbosity)
+    log.setLevel(verbosity.value)
 
     log.info("[run_VCal_calib] Start VCal calibration!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     log.info(f"[run_VCal_calib] TimeStart: {timestart}")
 
-    with resources.as_file(Path(args.config)) as path:
+    with resources.as_file(Path(config_path)) as path:
         config = json.loads(path.read_text())
 
-    check_meas_config(config, args.config)
+    check_meas_config(config, config_path)
 
-    if args.module_connectivity:
-        config["yarr"]["connectivity"] = args.module_connectivity
+    if module_connectivity:
+        config["yarr"]["connectivity"] = module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
-    if "emulator" not in args.config and not args.module_connectivity:
-        msg = "must supply path to connectivity file [-m --module-connectivity]"
-        raise RuntimeError(msg)
+    if "emulator" not in str(config_path) and not module_connectivity:
+        typer.echo("must supply path to connectivity file [-m --module-connectivity]")
+        raise typer.Exit(2)
 
     vcal_calib_config = config["tasks"]["GENERAL"]
     vcal_calib_config.update(config["tasks"]["VCAL_CALIBRATION"])
 
     ps = power_supply(config["power_supply"])
     yr = yarr(config["yarr"])
     meter = multimeter(config["multimeter"])
 
+    if not use_pixel_config:
+        yr.omit_pixel_config("tmp")
+
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
     test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
@@ -220,31 +199,23 @@
     ps.set(v=vcal_calib_config["v_max"], i=vcal_calib_config["i_config"][layer])
 
     MonitorV = vcal_calib_config["MonitorV"]
     InjVcalRange = vcal_calib_config["InjVcalRange"]
     vmux_value_GNDA = vcal_calib_config["MonitorV_GND"]
 
     # if -o option used, overwrite the default output directory
-    if args.module_connectivity:
-        output_dir = args.module_connectivity.rsplit("/", 1)[0]
-    else:
-        output_dir = args.output_dir
+    output_dir = module_connectivity.parent if module_connectivity else base_output_dir
 
-    if args.output_dir != "outputs":
-        output_dir = args.output_dir
+    if base_output_dir != Path("outputs"):
+        output_dir = base_output_dir
 
+    output_dir = output_dir.joinpath("Measurements", test_type, timestart)
     # Make output directory and start log file
-    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
-        parents=True, exist_ok=True
-    )
-    log.addHandler(
-        logging.FileHandler(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
-        )
-    )
+    output_dir.mkdir(parents=True, exist_ok=True)
+    log.addHandler(logging.FileHandler(output_dir.joinpath("output.log")))
 
     chip_data = []
     for chip in range(yr._number_of_chips):
         # if chip in yr._disabled_chip_positions:
         # continue
         qcdata_list = []
         for i, _vmux_value in enumerate(MonitorV):
@@ -281,15 +252,15 @@
 
     try:
         run(chip_data, vcal_calib_config, ps, yr, meter, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.exception(err)
-        sys.exit(1)
+        raise typer.Exit(1) from err
 
     log.info(
         "==================================Summary=================================="
     )
     alloutput = []
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
@@ -318,29 +289,31 @@
                 sub_test_type = "VCAL_MED"
             elif monitorV == 8 and injVcalRange == 0:
                 sub_test_type = "VCAL_MED_SMALL_RANGE"
             outputDF.set_subtest_type(sub_test_type)
 
             outputDF.set_results(chip_data[chip][i])
             alltests += [outputDF.to_dict()]
-        if not args.perchip:
+        if not perchip:
             alloutput += alltests
         else:
             save_dict_list(
-                f"{output_dir}/Measurements/{test_type}/{timestart}/{chip_name}.json",
+                output_dir.joinpath(f"{chip_name}.json"),
                 alltests,
             )
-    if not args.perchip:
+    if not perchip:
         save_dict_list(
-            f"{output_dir}/Measurements/{test_type}/{timestart}/{module_serial}.json",
+            output_dir.joinpath(f"{module_serial}.json"),
             alloutput,
         )
 
-    log.info(
-        f"Writing output measurements in {output_dir}/Measurements/{test_type}/{timestart}/"
-    )
+    log.info(f"Writing output measurements in {output_dir}")
     log.info("[run_VCal_calib] Done!")
     log.info(f"[run_VCal_calib] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}")
 
+    # Delete temporary files
+    if not use_pixel_config:
+        yr.remove_tmp_connectivity()
+
 
 if __name__ == "__main__":
-    main()
+    typer.run(main)
```

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/cli/hardware_emulator.py` & `module_qc_tools-2.0.1/src/module_qc_tools/cli/hardware_emulator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,49 @@
-#!/usr/bin/env python3
-from __future__ import annotations
-
-import argparse
 import json
 import logging
 import shutil
 import sys
+from enum import Enum
 from pathlib import Path
+from typing import Optional
 
 import numpy as np
+import typer
 
 from module_qc_tools import data
+from module_qc_tools.cli.globals import (
+    CONTEXT_SETTINGS,
+    OPTIONS,
+    LogLevel,
+)
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
 rng = np.random.default_rng(42)
-log = logging.getLogger(__name__)
+log = logging.getLogger("emulator")
+
+app = typer.Typer(context_settings=CONTEXT_SETTINGS)
+
+
+class PSAction(str, Enum):
+    on = "on"
+    off = "off"
+    getV = "getV"
+    getI = "getI"
+
 
 _MODULE_STATE_FILE = data / "emulator" / "module_state.json"
-_MODULE_CONNECTIVITY_FILE = "configs/connectivity/20UPGXM1234567_Lx_dummy.json"
+
+
+@app.callback()
+def main(verbosity: LogLevel = OPTIONS["verbosity"]):
+    log.setLevel(verbosity.value)
 
 
 def initialize_module_state():
     with resources.as_file(data / "emulator/module_state_template.json") as path:
         shutil.copyfile(path, _MODULE_STATE_FILE)
 
 
@@ -132,48 +150,63 @@
             )
         else:
             chip_state["MonitoringDataAdc"] = 0
 
     return chip_state
 
 
-def scanConsole():
+@app.command()
+def scanConsole(
+    _controller: Path = OPTIONS["emulator_controller"],
+    connectivity: Path = OPTIONS["emulator_connectivity"],
+    scan: Optional[Path] = typer.Option(
+        None,
+        "-s",
+        "--scan",
+        help="Scan config",
+        # exists=True,  # NB: enable when fixed for emulator (does not check for valid paths)
+        file_okay=True,
+        readable=True,
+        writable=True,
+        resolve_path=True,
+    ),
+    _num_threads: int = typer.Option(
+        1,
+        "-n",
+        "--nThreads",
+        help="Number of threads",
+    ),
+    _output_dir: Path = typer.Option(
+        "./",
+        "-o",
+        "--output-dir",
+        help="output directory",
+        exists=False,
+        writable=True,
+    ),
+    _skip_reset: bool = typer.Option(
+        False,
+        "--skip-reset",
+        help="skip reset",
+    ),
+):
     """
     This function emulates the effect of running YARR scanConsole to configure chips
     """
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-r",
-        "--controller",
-        default="configs/controller/specCfg-rd53b-16x1.json",
-        help="Controller",
-    )
-    parser.add_argument(
-        "-c",
-        "--connectivity",
-        default=_MODULE_CONNECTIVITY_FILE,
-        help="Connectivity",
-    )
-    parser.add_argument("-s", "--scan", default=None, help="Scan config")
-    parser.add_argument("-n", "--nThreads", type=int, help="Number of threads")
-    parser.add_argument("-o", "--output", default="./", help="Output directory")
-    parser.add_argument("--skip-reset", action="store_true", help="skip reset")
-    args = parser.parse_args()
 
     module_state = get_module_state()
 
-    with Path(args.connectivity).open() as path:
+    with connectivity.open() as path:
         spec_connectivity = json.load(path)
 
     nChips = len(spec_connectivity["chips"])
 
     for chip in range(nChips):
         config_path = spec_connectivity["chips"][chip]["config"]
-        abs_path = args.connectivity.rsplit("/", 1)[0] + "/" + config_path
-        with Path(abs_path).open() as path:
+        with connectivity.parent.joinpath(config_path).open() as path:
             spec = json.load(path)
         GlobalConfig = spec["RD53B"]["GlobalConfig"]
         Parameter = spec["RD53B"]["Parameter"]
         # VDDA/D should be trimmed to 1.2 after chip configuring
         module_state[f"Chip{chip+1}"]["VDDA"] = min(1.2, module_state["Vin"])
         module_state[f"Chip{chip+1}"]["VDDD"] = min(1.2, module_state["Vin"])
         # MonitorI and V set according to chip configs
@@ -196,148 +229,141 @@
 
         # Update Vmux
         module_state[f"Chip{chip+1}"] = update_Vmux(module_state[f"Chip{chip+1}"])
 
     update_module_state(module_state)
 
     # YARR returns 0 when scan is run
-    if args.scan is not None:
-        return 0
-    return 1
+    if scan is not None:
+        raise typer.Exit(0)
+    raise typer.Exit(1)
 
 
-def write_register():
+@app.command()
+def write_register(
+    _controller: Path = OPTIONS["emulator_controller"],
+    connectivity: Path = OPTIONS["emulator_connectivity"],
+    chip_position: int = OPTIONS["emulator_chip_position"],
+    name: str = typer.Argument(),
+    value: str = typer.Argument(),
+):
     """
     This function emulates the effect of running YARR write-register
     Currently only emulates register MonitorI, MonitorV. One needs to add a new if statement for a new register name.
     """
-    parser = argparse.ArgumentParser()
-    parser.add_argument("name", type=str, help="Name")
-    parser.add_argument("value", type=str, help="Value")
-    parser.add_argument(
-        "-r",
-        "--controller",
-        default="configs/controller/specCfg-rd53b-16x1.json",
-        help="Controller",
-    )
-    parser.add_argument(
-        "-c",
-        "--connectivity",
-        default=_MODULE_CONNECTIVITY_FILE,
-        help="Connectivity",
-    )
-    parser.add_argument("-i", "--chipPosition", type=int, help="chip position")
-    args = parser.parse_args()
-
     module_state = get_module_state()
 
-    with Path(args.connectivity).open() as path:
+    with connectivity.open() as path:
         spec_connectivity = json.load(path)
 
     nChips = len(spec_connectivity["chips"])
 
-    log.info(args.name, args.value)
+    log.info("%s, %s", name, value)
 
     for chip in range(nChips):
-        if args.chipPosition is not None and chip is not args.chipPosition:
+        if chip_position is not None and chip is not chip_position:
             continue
-        if args.name == "MonitorI":
-            module_state[f"Chip{chip+1}"]["MonitorI"] = int(args.value)
-        elif args.name == "MonitorV":
-            module_state[f"Chip{chip+1}"]["MonitorV"] = int(args.value)
-        elif args.name == "InjVcalMed":
-            module_state[f"Chip{chip+1}"]["InjVcalMed"] = int(args.value)
-        elif args.name == "InjVcalHigh":
-            module_state[f"Chip{chip+1}"]["InjVcalHigh"] = int(args.value)
-        elif args.name == "InjVcalRange":
-            module_state[f"Chip{chip+1}"]["InjVcalRange"] = int(args.value)
+        if name == "MonitorI":
+            module_state[f"Chip{chip+1}"]["MonitorI"] = value
+        elif name == "MonitorV":
+            module_state[f"Chip{chip+1}"]["MonitorV"] = value
+        elif name == "InjVcalMed":
+            module_state[f"Chip{chip+1}"]["InjVcalMed"] = value
+        elif name == "InjVcalHigh":
+            module_state[f"Chip{chip+1}"]["InjVcalHigh"] = value
+        elif name == "InjVcalRange":
+            module_state[f"Chip{chip+1}"]["InjVcalRange"] = value
         module_state[f"Chip{chip+1}"] = update_Vmux(module_state[f"Chip{chip+1}"])
 
     update_module_state(module_state)
 
 
-def read_register():
+@app.command()
+def read_register(
+    name: str,
+    _controller: Path = OPTIONS["emulator_controller"],
+    connectivity: Path = OPTIONS["emulator_connectivity"],
+    chip_position: int = OPTIONS["emulator_chip_position"],
+):
     """
     This function emulates the effect of running YARR read-register
     Currently only emulates register SldoTrimA and SldoTrimD. One needs to add a new if statement for a new register name.
     """
-    parser = argparse.ArgumentParser()
-    parser.add_argument("name", type=str, help="Name")
-    parser.add_argument(
-        "-r",
-        "--controller",
-        default="configs/controller/specCfg-rd53b-16x1.json",
-        help="Controller",
-    )
-    parser.add_argument(
-        "-c",
-        "--connectivity",
-        default=_MODULE_CONNECTIVITY_FILE,
-        help="Connectivity",
-    )
-    parser.add_argument("-i", "--chipPosition", type=int, help="chip position")
-    args = parser.parse_args()
 
-    with Path(args.connectivity).open() as path:
+    with connectivity.open() as path:
         spec_connectivity = json.load(path)
 
     nChips = len(spec_connectivity["chips"])
 
     for chip in range(nChips):
-        if args.chipPosition is not None and chip is not args.chipPosition:
+        if chip_position is not None and chip is not chip_position:
             continue
-        if args.name == "SldoTimA" or args.name == "SldoTrimD":
+        if name == "SldoTimA" or name == "SldoTrimD":
             sys.stdout.write("8")
-            sys.exit(0)
-        else:
-            sys.stdout.write("0")
-            sys.exit(0)
+            raise typer.Exit(0)
+
+        sys.stdout.write("0")
+        raise typer.Exit(0)
 
 
-def control_PS():
+@app.command()
+def control_PS(
+    action: PSAction = typer.Option(
+        ...,
+        "-a",
+        "--action",
+        help="Action to PS",
+    ),
+    voltage: float = typer.Option(
+        -1.0,
+        "-v",
+        "--voltage",
+        help="Set voltage",
+    ),
+    current: float = typer.Option(
+        -1.0,
+        "-i",
+        "--current",
+        help="Set current",
+    ),
+):
     """
     This function emulates the effect of powering the module
     """
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-a", "--action", choices=["on", "off", "getV", "getI"], help="Action to PS"
-    )
-    parser.add_argument("-v", "--voltage", type=float, help="Set voltage")
-    parser.add_argument("-i", "--current", type=float, help="Set current")
-    args = parser.parse_args()
-
-    if args.action == "off":
+    if action == "off":
         # Turning off the power simply means module states go back to initial states. Thus copy the initial states from the template
         initialize_module_state()
-        sys.exit(0)
+        raise typer.Exit(0)
 
     module_state = get_module_state()
 
-    if args.action == "getV":
+    if action == "getV":
         # measure Vin
         v = module_state["Vin"]
         sys.stdout.write(f"{v}")
-        sys.exit(0)
+        raise typer.Exit(0)
 
-    if args.action == "getI":
+    if action == "getI":
         # measure Iin
         i = module_state["Iin"]
         sys.stdout.write(f"{i}")
-        sys.exit(0)
+        raise typer.Exit(0)
+
+    if action == "on":
+        if current < 0 or voltage < 0:
+            typer.echo("Must set voltage and current.")
+            raise typer.Exit(2)
 
-    if args.action == "on":
         nChips = module_state["nChips"]
 
         # check if the module has already been powered on
         already_power = module_state["Vin"] > 0
 
         # Calculate Vin based on the prediction (slope and offset), as well as the voltage and the current set to the power supply
-        module_state["Vin"] = min(
-            0.348293 / nChips * args.current + 1, args.voltage, 2.0
-        )
+        module_state["Vin"] = min(0.348293 / nChips * current + 1, voltage, 2.0)
         # Calculate Iin from the calculated Vin
         module_state["Iin"] = (module_state["Vin"] - 1) * nChips / 0.348293
         # Assume temperature increases linearly with Iin
         module_state["temperature"] = 25.0 + module_state["Iin"] * 2.0
         for chip in range(nChips):  # loop over all the chips
             # VinA = VinD = Vin
             module_state[f"Chip{chip+1}"]["VinA"] = module_state["Vin"]
@@ -383,132 +409,157 @@
             module_state[f"Chip{chip+1}"] = update_Vmux(
                 module_state[f"Chip{chip+1}"]
             )  # update Vmux voltage
 
         update_module_state(module_state)
 
 
+@app.command()
 def measureV():
     """
     This function emulates the effect of multimeter (measuring the Vmux)
     """
     module_state = get_module_state()
 
     nChips = module_state["nChips"]
 
     v = 0
     for chip in range(nChips):
         v += module_state[f"Chip{chip+1}"]["Vmux"]
     sys.stdout.write(f"{v}")
-    sys.exit(0)
+    raise typer.Exit(0)
 
 
-def read_adc():
+@app.command()
+def read_adc(
+    vmux: int,
+    _controller: Path = OPTIONS["emulator_controller"],
+    _connectivity: Path = OPTIONS["emulator_connectivity"],
+    chip_position: int = OPTIONS["emulator_chip_position"],
+    read_current: bool = typer.Option(
+        False,
+        "-I",
+        "--readCurrent",
+        help="Read current instead of voltage",
+    ),
+    read_raw: bool = typer.Option(
+        False,
+        "-R",
+        "--rawCounts",
+        help="Read raw ADC counts",
+    ),
+):
     """
     This function emulates the effect of ADC reading
     R_Imux is assumed to be 10kohm.
     """
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-r",
-        "--controller",
-        default=data / "emulator/configs/controller/specCfg-rd53b-16x1.json",
-        help="Controller",
-    )
-    parser.add_argument(
-        "-c",
-        "--connectivity",
-        default=data / "emulator" / _MODULE_CONNECTIVITY_FILE,
-        help="Connectivity",
-    )
-    parser.add_argument("-i", "--chip_position", type=int, help="chip position")
-    parser.add_argument(
-        "-I",
-        "--readCurrent",
-        help="Read current instead of voltage",
-        action="store_true",
-    )
-    parser.add_argument(
-        "-R", "--rawCounts", help="Read raw ADC counts", action="store_true"
-    )
-    parser.add_argument("vmux", type=int, help="Vmux")
-    args = parser.parse_args()
-
     module_state = get_module_state()
 
     nChips = module_state["nChips"]
 
     # Update Vmux settings first
     for chip in range(nChips):
-        if args.chip_position is not None and chip is not args.chip_position:
+        if chip_position is not None and chip is not chip_position:
             continue
-        if args.readCurrent:
+        if read_current:
             module_state[f"Chip{chip+1}"]["MonitorV"] = 1
-            module_state[f"Chip{chip+1}"]["MonitorI"] = int(args.vmux)
+            module_state[f"Chip{chip+1}"]["MonitorI"] = vmux
         else:
-            module_state[f"Chip{chip+1}"]["MonitorV"] = int(args.vmux)
+            module_state[f"Chip{chip+1}"]["MonitorV"] = vmux
         module_state[f"Chip{chip+1}"] = update_Vmux(module_state[f"Chip{chip+1}"])
 
     # Then read ADC
     for chip in range(nChips):
-        if args.chip_position is not None and chip is not args.chip_position:
+        if chip_position is not None and chip is not chip_position:
             continue
-        if args.rawCounts:
+        if read_raw:
             v = module_state[f"Chip{chip+1}"]["MonitoringDataAdc"]
             u = ""
-        elif args.readCurrent:
+        elif read_current:
             v = (module_state[f"Chip{chip+1}"]["Vmux"] / 10000.0) / 1e-6
             u = "uA"
         else:
             v = module_state[f"Chip{chip+1}"]["Vmux"]
             u = "V"
         sys.stdout.write(f"{v} {u}")
-    sys.exit(0)
+    raise typer.Exit(0)
 
 
-def read_ringosc():
+@app.command()
+def read_ringosc(
+    _controller: Path = OPTIONS["emulator_controller"],
+    connectivity: Path = OPTIONS["emulator_connectivity"],
+    chip_position: int = OPTIONS["emulator_chip_position"],
+):
     """
     This function emulates the effect of ROSC reading
     """
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-r",
-        "--controller",
-        default=data / "emulator/configs/controller/specCfg-rd53b-16x1.json",
-        help="Controller",
-    )
-    parser.add_argument(
-        "-c",
-        "--connectivity",
-        default=data / "emulator" / _MODULE_CONNECTIVITY_FILE,
-        help="Connectivity",
-    )
-    parser.add_argument("-i", "--chip_position", type=int, help="chip position")
-    args = parser.parse_args()
 
-    with Path(args.connectivity).open() as path:
+    with connectivity.open() as path:
         spec_connectivity = json.load(path)
 
     nChips = len(spec_connectivity["chips"])
 
     for chip in range(nChips):
-        if args.chip_position is not None and chip is not args.chip_position:
+        if chip_position is not None and chip is not chip_position:
             continue
 
         rosc_freq = "500 " * 42
         sys.stdout.write(rosc_freq)
-    sys.exit(0)
+    raise typer.Exit(0)
 
 
+@app.command()
 def measureT():
     """
     This function emulates the effect of NTC (measure module temperature)
     """
     module_state = get_module_state()
 
     T = module_state["temperature"]
     sys.stdout.write(f"{T}")
-    sys.exit(0)
+    raise typer.Exit(0)
+
+
+@app.command()
+def switchLPM(_: PSAction):
+    raise typer.Exit(0)
+
+
+def run_scanConsole():
+    typer.run(scanConsole)
+
+
+def run_write_register():
+    typer.run(write_register)
+
+
+def run_read_register():
+    typer.run(read_register)
+
+
+def run_read_adc():
+    typer.run(read_adc)
+
+
+def run_read_ringosc():
+    typer.run(read_ringosc)
+
+
+def run_switchLPM():
+    typer.run(switchLPM)
+
+
+def run_control_PS():
+    typer.run(control_PS)
+
+
+def run_measureV():
+    typer.run(measureV)
+
+
+def run_measureT():
+    typer.run(measureT)
 
 
-def switchLPM():
-    sys.exit(0)
+if __name__ == "__main__":
+    app()
```

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/cli/upload_localdb.py` & `module_qc_tools-2.0.1/src/module_qc_tools/cli/upload_localdb.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,109 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-import argparse
 import json
 import logging
-import sys
 import time
 from pathlib import Path
 
 import requests
+import typer
 
-logging.basicConfig(level=logging.DEBUG)
-log = logging.getLogger(__name__)
-
-parser = argparse.ArgumentParser(
-    description="Walk through the specified directory (recursively) and attempt to submit all json files to LocalDB as the QC measurement"
-)
-parser.add_argument(
-    "--path",
-    default="Analysis/",
-    help="Path to directory with output measurement files",
-)
-parser.add_argument(
-    "--host",
-    default="localhost",
-    help="localDB server",
-)
-parser.add_argument(
-    "--port",
-    default=5000,
-    help="localDB port",
-)
-parser.add_argument(
-    "-n",
-    "--dry-run",
-    default=False,
-    action="store_true",
-    help="Dry-run, do not submit to localDB.",
-)
-parser.add_argument(
-    "--out",
-    default="tmp.json",
-    help="Analysis output result json file path to save in the local host",
-)
-args = parser.parse_args()
-
-
-def main():
+from module_qc_tools.cli.globals import (
+    CONTEXT_SETTINGS,
+    OPTIONS,
+    LogLevel,
+)
+
+logging.basicConfig(level=logging.INFO)
+log = logging.getLogger("upload")
+app = typer.Typer(context_settings=CONTEXT_SETTINGS)
+
+
+@app.command()
+def main(
+    analysis_path: Path = OPTIONS["analysis_path"],
+    host: str = OPTIONS["host"],
+    port: int = OPTIONS["port"],
+    dry_run: bool = OPTIONS["dry_run"],
+    output_path: Path = OPTIONS["output_path"],
+    verbosity: LogLevel = OPTIONS["verbosity"],
+):
     """
     Walk through the specified directory (recursively) and attempt to submit all json files to LocalDB as the QC measurement
 
     Args:
         path (str or pathlib.Path): root directory to walk through
         host (str): localDB server host
         port (int): localDB server port
         out  (str): analysis output result json file path to save in the local host
 
     Returns:
         None: The files are uploaded to localDB.
     """
 
+    log.setLevel(verbosity.value)
     log.info("Searching candidate RAW json files...")
-    flist = list(Path(args.path).rglob("*.json"))
+    flist = list(analysis_path.rglob("*.json"))
 
     pack = []
     for path in flist:
         log.info(f"  - {path}")
         with path.open(encoding="utf-8") as fpointer:
             pack.extend(json.load(fpointer))
 
     log.info(f"Extracted {len(pack)} tests from {len(flist)} input files.")
     log.info("==> Submitting RAW results pack...")
 
-    protocol = "http" if args.port != "443" else "https"
+    protocol = "http" if port != 443 else "https"
 
-    if not args.dry_run:
+    if not dry_run:
         try:
             response = requests.post(
-                f"{protocol}://{args.host}:{args.port}/localdb/qc_uploader_post",
+                f"{protocol}://{host}:{port}/localdb/qc_uploader_post",
                 json=pack,
             )
             response.raise_for_status()
 
             data = response.json()
 
             log.info(data)
 
-        except Exception as e:
+        except Exception as err:
             log.error("failure in uploading!")
-            log.error(e)
-            sys.exit(1)
+            log.error(err)
+            raise typer.Exit(1) from err
 
         log.info(
             f"\nDone! LocalDB has accepted the following {len(data)} TestRun results"
         )
         for testRun in data:
             if testRun is None:
                 log.info("A test run is already uploaded and will be skipped.")
                 continue
 
             log.info(
                 f'SerialNumber: {testRun["serialNumber"]}, Stage: {testRun["stage"]}, TestType: {testRun["testType"]}, QC-passed: {testRun["passed"]}'
             )
 
         try:
-            with Path(args.out).open("w") as f:
+            with output_path.open("w") as f:
                 json.dump(data, f, indent=4)
-                log.info(f"Saved the output TestRun to {args.out}")
+                log.info(f"Saved the output TestRun to {output_path}")
 
         except Exception:
-            log.warning(f"Failed to saved the output TestRun to {args.out}")
+            log.warning(f"Failed to saved the output TestRun to {output_path}")
             altFilePath = f"/var/tmp/module-qc-tools-record-{int(time.time())}.json"
 
             try:
                 with Path(altFilePath).open("w") as f:
                     json.dump(data, f, indent=4)
                 log.info(f"Saved the output TestRun to {altFilePath}")
 
             except Exception:
                 log.warning(f"Failed to saved the output TestRun to {altFilePath}")
                 pass
 
 
 if __name__ == "__main__":
-    main()
+    typer.run(main)
```

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/configs/emulator_merged_vmux.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/configs/emulator_merged_vmux.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/configs/example_merged_vmux.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/configs/example_merged_vmux.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/configs/example_separate_vmux.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/configs/example_separate_vmux.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/module_state_template.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/module_state_template.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/ADC_CALIBRATION.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/schema/ADC_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/ANALOG_READBACK.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/schema/ANALOG_READBACK.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/LP_MODE.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/schema/LP_MODE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/SLDO.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/schema/SLDO.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/common.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/schema/common.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/config.json` & `module_qc_tools-2.0.1/src/module_qc_tools/data/schema/config.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/utils/hardware_control_base.py` & `module_qc_tools-2.0.1/src/module_qc_tools/utils/hardware_control_base.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/utils/misc.py` & `module_qc_tools-2.0.1/src/module_qc_tools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/utils/multimeter.py` & `module_qc_tools-2.0.1/src/module_qc_tools/utils/multimeter.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/utils/ntc.py` & `module_qc_tools-2.0.1/src/module_qc_tools/utils/ntc.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/utils/power_supply.py` & `module_qc_tools-2.0.1/src/module_qc_tools/utils/power_supply.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/src/module_qc_tools/utils/yarr.py` & `module_qc_tools-2.0.1/src/module_qc_tools/utils/yarr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import contextlib
 import json
 import logging
 import re
+import sys
 from pathlib import Path
 
 from module_qc_tools.utils.hardware_control_base import hardware_control_base
 from module_qc_tools.utils.misc import bcolors
 
 # if sys.version_info >= (3, 9):
 #    from importlib import resources
@@ -27,14 +28,15 @@
         self.read_register_exe = ""
         self.read_adc_exe = ""
         self.switchLPM_exe = ""
         self.lpm_digitalscan = ""
         self.read_ringosc_exe = ""
         self.success_code = 0
         self.emulator = False
+        self.usingTempConfig = False
         super().__init__(config, name, *args, **kwargs)
         if "emulator" in self.scanConsole_exe:
             self.emulator = True
             log.info(f"[{name}] running scanConsole emulator!!")
         if "emulator" in self.write_register_exe:
             self.emulator = True
             log.info(f"[{name}] running write_register emulator!!")
@@ -295,16 +297,82 @@
     def get_connectivity(self):
         with Path(self.connectivity).open() as file:
             return json.load(file)
 
     def get_config(self, chip_position):
         connect_spec = self.get_connectivity()
         config_path = connect_spec["chips"][chip_position]["config"]
-        path = self.connectivity.rsplit("/", 1)[0] + "/" + config_path
+        path = Path(self.connectivity).parent / config_path
 
         with Path(path).open() as file:
             spec = json.load(file)
 
         with contextlib.suppress(KeyError):
             spec["RD53B"].pop("PixelConfig")
 
         return spec
+
+    def omit_pixel_config(self, tmp_dir_name="tmp"):
+        tmp_dir = str(Path(self.connectivity).parent) + "/" + tmp_dir_name
+        log.info(
+            f"Creating temporary connectivity file and chip configs without pixel config in {tmp_dir}"
+        )
+
+        # Create new directory for new temporary files, will not overwrite if it already exists
+        try:
+            Path(tmp_dir).mkdir(parents=True, exist_ok=False)
+        except Exception:
+            log.error(
+                bcolors.BADRED
+                + f"Unable to make temporary directory: {tmp_dir} , please delete this directory or choose a different directory name"
+                + bcolors.ENDC
+            )
+            sys.exit(1)
+
+        # Create new connectivity file pointing to new chip config files
+        new_conn = (
+            str(Path(self.connectivity).with_suffix("").stem) + "_noPixConfig.json"
+        )
+        with Path(self.connectivity).open() as file:
+            orig_config = json.load(file)
+        new_config = orig_config
+        for i, c in enumerate(orig_config["chips"]):
+            new_path = str(Path(c["config"]).with_suffix("").stem) + "_noPixConfig.json"
+            new_config["chips"][i]["config"] = new_path
+
+            # Save temporary chip config (without Pixel Config)
+            new_chip_config = Path(tmp_dir + "/" + new_path)
+            new_chip_config.touch(exist_ok=False)
+            with new_chip_config.open(mode="w") as file:
+                json.dump(self.get_config(i), file, indent=4)
+
+        new_conn_file = Path(tmp_dir + "/" + new_conn)
+        new_conn_file.touch(exist_ok=False)
+        with new_conn_file.open(mode="w") as fp:
+            json.dump(new_config, fp, indent=4)
+
+        # Use temporary connectivity file
+        self.connectivity = tmp_dir + "/" + new_conn
+        self.usingTempConfig = True
+        return 0
+
+    def remove_tmp_connectivity(self):
+        log.info(f"Deleting temporary files: {Path(self.connectivity).parent}")
+        if not self.usingTempConfig:
+            log.warning(
+                bcolors.WARNING
+                + "Requesting to delete temporary config files - but temporary config files are not being used! Will not delete any files."
+                + bcolors.ENDC
+            )
+            return 0
+
+        if Path(self.connectivity).parent.exists():
+            for child in Path(self.connectivity).parent.iterdir():
+                child.unlink()
+            Path(self.connectivity).parent.rmdir()
+        else:
+            log.warning(
+                bcolors.WARNING
+                + "Temporary files ({Path(self.connectivity).parent}) do not exist - something may have gone wrong"
+                + bcolors.ENDC
+            )
+        return 0
```

### Comparing `module_qc_tools-2.0.0/.gitignore` & `module_qc_tools-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/LICENSE` & `module_qc_tools-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.0.0/README.md` & `module_qc_tools-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-tools v2.0.0
+# module-qc-tools v2.0.1
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -66,15 +66,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-tools==2.0.0
+python -m pip install -U pip module-qc-tools==2.0.1
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
```

### Comparing `module_qc_tools-2.0.0/pyproject.toml` & `module_qc_tools-2.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,45 +19,48 @@
     "numpy",
     "tabulate",
     "pre-commit",
     "jsonschema",
     "module-qc-data-tools >= 1.0.5",
     'importlib_resources; python_version < "3.9"',
     "requests",
+    'urllib3>=1.26.11,<2; "el7.x86_64" in platform_release',
+    "typer",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools"
 "Bug Tracker" = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools/-/issues"
 "Source" = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools"
 
 [project.scripts]
-module-qc-tools = "module_qc_tools.cli.main:main"
-emulator-scanConsole = "module_qc_tools.cli.hardware_emulator:scanConsole"
-emulator-write-register = "module_qc_tools.cli.hardware_emulator:write_register"
-emulator-read-register = "module_qc_tools.cli.hardware_emulator:read_register"
-emulator-read-adc = "module_qc_tools.cli.hardware_emulator:read_adc"
-emulator-read-ringosc = "module_qc_tools.cli.hardware_emulator:read_ringosc"
-emulator-switch-lpm = "module_qc_tools.cli.hardware_emulator:switchLPM"
-emulator-control-ps = "module_qc_tools.cli.hardware_emulator:control_PS"
-emulator-measureV = "module_qc_tools.cli.hardware_emulator:measureV"
-emulator-measureT = "module_qc_tools.cli.hardware_emulator:measureT"
-measurement-ADC-CALIBRATION = "module_qc_tools.cli.ADC_CALIBRATION:main"
-measurement-ANALOG-READBACK = "module_qc_tools.cli.ANALOG_READBACK:main"
-measurement-SLDO = "module_qc_tools.cli.SLDO:main"
-measurement-VCAL-CALIBRATION = "module_qc_tools.cli.VCAL_CALIBRATION:main"
-measurement-INJECTION-CAPACITANCE = "module_qc_tools.cli.INJECTION_CAPACITANCE:main"
-measurement-LP-MODE = "module_qc_tools.cli.LP_MODE:main"
-measurement-OVERVOLTAGE-PROTECTION = "module_qc_tools.cli.OVERVOLTAGE_PROTECTION:main"
-module-qc-tools-upload = "module_qc_tools.cli.upload_localdb:main"
+module-qc-tools = "module_qc_tools.cli:app"
+"mqt" = "module_qc_tools.cli:app"
+emulator-scanConsole = "module_qc_tools.cli.hardware_emulator:run_scanConsole"
+emulator-write-register = "module_qc_tools.cli.hardware_emulator:run_write_register"
+emulator-read-register = "module_qc_tools.cli.hardware_emulator:run_read_register"
+emulator-read-adc = "module_qc_tools.cli.hardware_emulator:run_read_adc"
+emulator-read-ringosc = "module_qc_tools.cli.hardware_emulator:run_read_ringosc"
+emulator-switch-lpm = "module_qc_tools.cli.hardware_emulator:run_switchLPM"
+emulator-control-ps = "module_qc_tools.cli.hardware_emulator:run_control_PS"
+emulator-measureV = "module_qc_tools.cli.hardware_emulator:run_measureV"
+emulator-measureT = "module_qc_tools.cli.hardware_emulator:run_measureT"
+measurement-ADC-CALIBRATION = "module_qc_tools.cli.ADC_CALIBRATION:app"
+measurement-ANALOG-READBACK = "module_qc_tools.cli.ANALOG_READBACK:app"
+measurement-SLDO = "module_qc_tools.cli.SLDO:app"
+measurement-VCAL-CALIBRATION = "module_qc_tools.cli.VCAL_CALIBRATION:app"
+measurement-INJECTION-CAPACITANCE = "module_qc_tools.cli.INJECTION_CAPACITANCE:app"
+measurement-LP-MODE = "module_qc_tools.cli.LP_MODE:app"
+measurement-OVERVOLTAGE-PROTECTION = "module_qc_tools.cli.OVERVOLTAGE_PROTECTION:app"
+module-qc-tools-upload = "module_qc_tools.cli.upload_localdb:app"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
@@ -120,15 +123,19 @@
   "YTT",         # flake8-2020
 ]
 extend-ignore = ["PLR", "E501"]
 target-version = "py37"
 src = ["src"]
 unfixable = ["T20", "F841"]
 exclude = []
-isort.required-imports = ["from __future__ import annotations"]
+isort.required-imports = []
+
+[tool.ruff.per-file-ignores]
+"src/module_qc_tools/cli/main.py" = ["B008"]
+"src/module_qc_tools/cli/hardware_emulator.py" = ["B008"]
 
 [tool.pylint]
 master.py-version = "3.7"
 master.ignore-paths= ["src/module_qc_tools/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
```

### Comparing `module_qc_tools-2.0.0/PKG-INFO` & `module_qc_tools-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module_qc_tools
-Version: 2.0.0
+Version: 2.0.1
 Summary: Module qc tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -34,17 +34,19 @@
 Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: jsonschema
 Requires-Dist: module-qc-data-tools>=1.0.5
 Requires-Dist: numpy
 Requires-Dist: pre-commit
 Requires-Dist: requests
 Requires-Dist: tabulate
+Requires-Dist: typer
+Requires-Dist: urllib3<2,>=1.26.11; 'el7.x86_64' in platform_release
 Description-Content-Type: text/markdown
 
-# module-qc-tools v2.0.0
+# module-qc-tools v2.0.1
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -108,15 +110,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-tools==2.0.0
+python -m pip install -U pip module-qc-tools==2.0.1
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
```

