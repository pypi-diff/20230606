# Comparing `tmp/iLCDirac-34.0.0a4.tar.gz` & `tmp/iLCDirac-34.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iLCDirac-34.0.0a4.tar", last modified: Mon May 29 13:18:57 2023, max compression
+gzip compressed data, was "iLCDirac-34.0.0a5.tar", last modified: Tue Jun  6 10:56:24 2023, max compression
```

## Comparing `iLCDirac-34.0.0a4.tar` & `iLCDirac-34.0.0a5.tar`

### file list

```diff
@@ -1,472 +1,472 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.331254 iLCDirac-34.0.0a4/
--rw-rw-rw-   0 root         (0) root         (0)    32452 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-29 13:18:57.332254 iLCDirac-34.0.0a4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)    82539 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/release.notes
--rw-rw-rw-   0 root         (0) root         (0)    27753 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/releases.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4370 2023-05-29 13:18:57.333254 iLCDirac-34.0.0a4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      276 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.223255 iLCDirac-34.0.0a4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.226255 iLCDirac-34.0.0a4/src/ILCDIRAC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.227254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.227254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    10978 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.228254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     6343 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.229254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)    36181 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    44494 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py
--rw-rw-rw-   0 root         (0) root         (0)     5951 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3971 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/TODO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.230255 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/
--rw-rw-rw-   0 root         (0) root         (0)    14462 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     2255 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py
--rw-rw-rw-   0 root         (0) root         (0)    51085 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py
--rw-rw-rw-   0 root         (0) root         (0)     2037 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py
--rw-rw-rw-   0 root         (0) root         (0)     9201 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.232254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.235254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/
--rw-rw-rw-   0 root         (0) root         (0)     3152 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     2682 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     3967 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py
--rw-rw-rw-   0 root         (0) root         (0)     4968 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Helper_Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3579 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.235254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/
--rw-rw-rw-   0 root         (0) root         (0)     1765 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt
--rw-rw-rw-   0 root         (0) root         (0)     3928 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml
--rw-rw-rw-   0 root         (0) root         (0)     1484 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py
--rw-rw-rw-   0 root         (0) root         (0)    12301 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/dev_create_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.236254 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.243254 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     3755 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py
--rw-rw-rw-   0 root         (0) root         (0)    15006 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    18781 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/DetectOS.py
--rw-rw-rw-   0 root         (0) root         (0)     4861 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FileUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     9749 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py
--rw-rw-rw-   0 root         (0) root         (0)     2767 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py
--rw-rw-rw-   0 root         (0) root         (0)     4110 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/GeneratorModels.py
--rw-rw-rw-   0 root         (0) root         (0)    17917 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/HTML.py
--rw-rw-rw-   0 root         (0) root         (0)     6866 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InputDataResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     4246 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5506 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InstalledFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/JobPathResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     7040 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/MarlinXML.py
--rw-rw-rw-   0 root         (0) root         (0)     3285 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/OverlayFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2856 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/PrepareLibs.py
--rw-rw-rw-   0 root         (0) root         (0)    34638 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     7483 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ProcessList.py
--rw-rw-rw-   0 root         (0) root         (0)    11004 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ProductionData.py
--rw-rw-rw-   0 root         (0) root         (0)     3993 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/RemoveSoft.py
--rw-rw-rw-   0 root         (0) root         (0)     2690 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ResolveSE.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Splitting.py
--rw-rw-rw-   0 root         (0) root         (0)    21977 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/TARsoft.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/WasteCPU.py
--rw-rw-rw-   0 root         (0) root         (0)    41912 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/WhizardOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1100 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6604 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.250254 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6226 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py
--rw-rw-rw-   0 root         (0) root         (0)    31722 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    23878 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py
--rw-rw-rw-   0 root         (0) root         (0)    17273 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py
--rw-rw-rw-   0 root         (0) root         (0)    16707 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py
--rw-rw-rw-   0 root         (0) root         (0)     4872 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py
--rw-rw-rw-   0 root         (0) root         (0)    10164 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     7506 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)    18959 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)     2654 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     6803 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py
--rw-rw-rw-   0 root         (0) root         (0)    26585 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py
--rw-rw-rw-   0 root         (0) root         (0)    84519 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py
--rw-rw-rw-   0 root         (0) root         (0)    14816 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py
--rw-rw-rw-   0 root         (0) root         (0)     6220 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    11294 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py
--rw-rw-rw-   0 root         (0) root         (0)     9475 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py
--rw-rw-rw-   0 root         (0) root         (0)     2278 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py
--rw-rw-rw-   0 root         (0) root         (0)    72966 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py
--rw-rw-rw-   0 root         (0) root         (0)     3214 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py
--rw-rw-rw-   0 root         (0) root         (0)    26730 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.254254 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     3224 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     6151 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     6706 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     3200 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     2307 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh
--rwxrwxrwx   0 root         (0) root         (0)     9197 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac-architecture
--rw-rw-rw-   0 root         (0) root         (0)    15857 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py
--rw-rw-rw-   0 root         (0) root         (0)    10543 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py
--rw-rw-rw-   0 root         (0) root         (0)     9819 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py
--rw-rw-rw-   0 root         (0) root         (0)    16436 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py
--rw-rw-rw-   0 root         (0) root         (0)     1573 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.254254 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.254254 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.255254 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/
--rw-rw-rw-   0 root         (0) root         (0)     5544 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.255254 iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.255254 iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/ConfigTemplate.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.256254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.257254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    25777 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     9996 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     5395 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.257254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.259254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/
--rw-rw-rw-   0 root         (0) root         (0)    35437 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    14308 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py
--rw-rw-rw-   0 root         (0) root         (0)    19604 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py
--rw-rw-rw-   0 root         (0) root         (0)    13782 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py
--rw-rw-rw-   0 root         (0) root         (0)    30921 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py
--rw-rw-rw-   0 root         (0) root         (0)     7554 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2889 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.260254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     5456 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py
--rw-rw-rw-   0 root         (0) root         (0)     6462 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py
--rw-rw-rw-   0 root         (0) root         (0)     3204 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.264254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49360 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py
--rw-rw-rw-   0 root         (0) root         (0)    48013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py
--rw-rw-rw-   0 root         (0) root         (0)     6228 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py
--rw-rw-rw-   0 root         (0) root         (0)     3366 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    12482 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py
--rw-rw-rw-   0 root         (0) root         (0)     7314 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py
--rwxrwxrwx   0 root         (0) root         (0)     9954 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py
--rw-rw-rw-   0 root         (0) root         (0)     4673 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    16641 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     3536 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    12116 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.264254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.264254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/
--rw-rw-rw-   0 root         (0) root         (0)    13833 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/DiracILC.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.219255 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.265254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/alias.properties
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py
--rw-rw-rw-   0 root         (0) root         (0)     9474 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml
--rw-rw-rw-   0 root         (0) root         (0)    10942 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.266254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.277254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/default.mac
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/defaultClicCrossingAngle.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_10gev_theta5-175.mac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.278254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/
--rw-rw-rw-   0 root         (0) root         (0)     8759 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.280254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/
--rw-rw-rw-   0 root         (0) root         (0)    27099 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.288254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     3757 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2335 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py
--rw-rw-rw-   0 root         (0) root         (0)    10462 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py
--rw-rw-rw-   0 root         (0) root         (0)     9579 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py
--rw-rw-rw-   0 root         (0) root         (0)    35946 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py
--rw-rw-rw-   0 root         (0) root         (0)    12520 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py
--rw-rw-rw-   0 root         (0) root         (0)     6521 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     3885 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)     6140 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py
--rw-rw-rw-   0 root         (0) root         (0)     9573 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py
--rw-rw-rw-   0 root         (0) root         (0)    10161 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py
--rw-rw-rw-   0 root         (0) root         (0)     8281 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py
--rw-rw-rw-   0 root         (0) root         (0)    16303 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     3918 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)     3312 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py
--rw-rw-rw-   0 root         (0) root         (0)     2090 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py
--rw-rw-rw-   0 root         (0) root         (0)     3752 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     4434 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6174 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py
--rw-rw-rw-   0 root         (0) root         (0)     6089 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py
--rw-rw-rw-   0 root         (0) root         (0)     5479 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6957 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py
--rw-rw-rw-   0 root         (0) root         (0)    17277 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py
--rw-rw-rw-   0 root         (0) root         (0)    12788 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py
--rw-rw-rw-   0 root         (0) root         (0)     4441 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py
--rw-rw-rw-   0 root         (0) root         (0)     4984 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.290254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/
--rw-rw-rw-   0 root         (0) root         (0)     2831 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py
--rw-rw-rw-   0 root         (0) root         (0)     2665 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py
--rw-rw-rw-   0 root         (0) root         (0)    19613 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py
--rw-rw-rw-   0 root         (0) root         (0)    22228 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py
--rw-rw-rw-   0 root         (0) root         (0)     2834 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py
--rw-rw-rw-   0 root         (0) root         (0)     4247 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py
--rw-rw-rw-   0 root         (0) root         (0)     9857 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    24484 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py
--rw-rw-rw-   0 root         (0) root         (0)    26292 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py
--rw-rw-rw-   0 root         (0) root         (0)    15111 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py
--rw-rw-rw-   0 root         (0) root         (0)     3097 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     2402 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py
--rw-rw-rw-   0 root         (0) root         (0)    40172 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.291254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/
--rw-rw-rw-   0 root         (0) root         (0)    27996 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    29727 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py
--rwxrwxrwx   0 root         (0) root         (0)    35679 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py
--rw-rw-rw-   0 root         (0) root         (0)    13124 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    12330 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.300254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/
--rw-rw-rw-   0 root         (0) root         (0)     7876 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     4672 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2878 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py
--rw-rw-rw-   0 root         (0) root         (0)    18299 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py
--rw-rw-rw-   0 root         (0) root         (0)    15439 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py
--rw-rw-rw-   0 root         (0) root         (0)    41414 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py
--rw-rw-rw-   0 root         (0) root         (0)    15264 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py
--rw-rw-rw-   0 root         (0) root         (0)     5930 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     4218 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)    13745 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py
--rw-rw-rw-   0 root         (0) root         (0)     7579 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py
--rw-rw-rw-   0 root         (0) root         (0)    12305 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py
--rw-rw-rw-   0 root         (0) root         (0)     8309 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py
--rw-rw-rw-   0 root         (0) root         (0)     6492 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py
--rw-rw-rw-   0 root         (0) root         (0)    14537 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     4767 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)    71676 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py
--rw-rw-rw-   0 root         (0) root         (0)     4830 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     4798 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6232 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py
--rw-rw-rw-   0 root         (0) root         (0)     7551 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py
--rw-rw-rw-   0 root         (0) root         (0)     5077 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6829 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     4763 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py
--rw-rw-rw-   0 root         (0) root         (0)    22726 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py
--rw-rw-rw-   0 root         (0) root         (0)    20865 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py
--rw-rw-rw-   0 root         (0) root         (0)    13044 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py
--rw-rw-rw-   0 root         (0) root         (0)     4169 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9860 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.300254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Test/
--rw-rw-rw-   0 root         (0) root         (0)    20190 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py
--rw-rw-rw-   0 root         (0) root         (0)     1132 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.300254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Tests/
--rw-rw-rw-   0 root         (0) root         (0)     2622 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.301254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     4727 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py
--rw-rw-rw-   0 root         (0) root         (0)    15312 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.303254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2968 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7808 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py
--rw-rw-rw-   0 root         (0) root         (0)     3538 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py
--rw-rw-rw-   0 root         (0) root         (0)     2636 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3088 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py
--rw-rw-rw-   0 root         (0) root         (0)     2396 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py
--rwxrwxrwx   0 root         (0) root         (0)     3724 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.304254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.304254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)     2638 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.305254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.305254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/
--rw-rw-rw-   0 root         (0) root         (0)     6376 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.306254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/Test/
--rw-rw-rw-   0 root         (0) root         (0)     9281 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.306254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)     2462 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.306254 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.318254 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/
--rw-rw-rw-   0 root         (0) root         (0)     4515 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py
--rw-rw-rw-   0 root         (0) root         (0)     5524 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py
--rw-rw-rw-   0 root         (0) root         (0)    23026 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     5789 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py
--rw-rw-rw-   0 root         (0) root         (0)     3146 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    16673 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     8009 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DummyModule.py
--rw-rw-rw-   0 root         (0) root         (0)     6809 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py
--rw-rw-rw-   0 root         (0) root         (0)    19926 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     8774 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)     4454 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)     6156 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     6801 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5057 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     8078 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)    13096 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18950 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    31351 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ModuleBase.py
--rw-rw-rw-   0 root         (0) root         (0)    26082 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5266 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MoveInFC.py
--rw-rw-rw-   0 root         (0) root         (0)    33871 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     7960 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)     8182 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5743 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ReportErrors.py
--rw-rw-rw-   0 root         (0) root         (0)     5915 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5740 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    11639 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    11192 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4044 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py
--rw-rw-rw-   0 root         (0) root         (0)     9340 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     3020 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.325254 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py
--rw-rw-rw-   0 root         (0) root         (0)    14814 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)    44092 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py
--rw-rw-rw-   0 root         (0) root         (0)    18662 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)    28578 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    20599 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)    10005 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    45397 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    43848 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py
--rw-rw-rw-   0 root         (0) root         (0)    41500 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)    10867 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py
--rw-rw-rw-   0 root         (0) root         (0)     8844 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    28021 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py
--rw-rw-rw-   0 root         (0) root         (0)    19461 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py
--rw-rw-rw-   0 root         (0) root         (0)    14457 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)    12973 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py
--rw-rw-rw-   0 root         (0) root         (0)    10007 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    32143 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py
--rw-rw-rw-   0 root         (0) root         (0)    14235 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    67243 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    86847 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py
--rw-rw-rw-   0 root         (0) root         (0)     6505 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    17704 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py
--rw-rw-rw-   0 root         (0) root         (0)    15076 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    17792 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py
--rw-rw-rw-   0 root         (0) root         (0)     9795 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    22938 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.326254 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     3265 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     4526 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/RootMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.327254 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.327254 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    24455 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.328254 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)    15894 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.329254 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Executor/
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.329254 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/
--rw-rw-rw-   0 root         (0) root         (0)    13587 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py
--rw-rw-rw-   0 root         (0) root         (0)    31624 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     3345 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2395 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.331254 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24527 2023-05-29 13:18:57.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2121 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      279 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.654826 iLCDirac-34.0.0a5/
+-rw-rw-rw-   0 root         (0) root         (0)    32452 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-06 10:56:24.654826 iLCDirac-34.0.0a5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)    83183 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/release.notes
+-rw-rw-rw-   0 root         (0) root         (0)    27753 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/releases.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2023-06-06 10:56:24.655826 iLCDirac-34.0.0a5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.550825 iLCDirac-34.0.0a5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.552825 iLCDirac-34.0.0a5/src/ILCDIRAC/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.552825 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.553825 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    10978 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.553825 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.554825 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)    36181 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    44494 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py
+-rw-rw-rw-   0 root         (0) root         (0)     5951 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3971 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/TODO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.556825 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/
+-rw-rw-rw-   0 root         (0) root         (0)    14462 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    51085 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9201 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.557825 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.560825 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     3152 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     3967 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py
+-rw-rw-rw-   0 root         (0) root         (0)     4968 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Helper_Functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3579 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.560825 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3928 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12301 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/dev_create_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.560825 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.568825 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     3755 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py
+-rw-rw-rw-   0 root         (0) root         (0)    15006 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/Configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    18781 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/DetectOS.py
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/FileUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9749 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2767 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py
+-rw-rw-rw-   0 root         (0) root         (0)     4110 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/GeneratorModels.py
+-rw-rw-rw-   0 root         (0) root         (0)    17917 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/HTML.py
+-rw-rw-rw-   0 root         (0) root         (0)     6866 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/InputDataResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5489 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/InstalledFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/JobPathResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     7040 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/MarlinXML.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/OverlayFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2856 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/PrepareLibs.py
+-rw-rw-rw-   0 root         (0) root         (0)    36224 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     7483 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/ProcessList.py
+-rw-rw-rw-   0 root         (0) root         (0)    11004 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/ProductionData.py
+-rw-rw-rw-   0 root         (0) root         (0)     3993 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/RemoveSoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/ResolveSE.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/Splitting.py
+-rw-rw-rw-   0 root         (0) root         (0)    21977 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/TARsoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/WasteCPU.py
+-rw-rw-rw-   0 root         (0) root         (0)    41912 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/WhizardOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6604 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.573825 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py
+-rw-rw-rw-   0 root         (0) root         (0)    31722 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    23878 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py
+-rw-rw-rw-   0 root         (0) root         (0)    17273 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16707 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     4872 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py
+-rw-rw-rw-   0 root         (0) root         (0)    10164 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     7506 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18959 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py
+-rw-rw-rw-   0 root         (0) root         (0)    26585 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py
+-rw-rw-rw-   0 root         (0) root         (0)    85249 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)    14816 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py
+-rw-rw-rw-   0 root         (0) root         (0)     6220 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    11294 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py
+-rw-rw-rw-   0 root         (0) root         (0)     9475 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py
+-rw-rw-rw-   0 root         (0) root         (0)    72966 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py
+-rw-rw-rw-   0 root         (0) root         (0)    26730 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.577825 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     3224 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     6151 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     6706 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     3200 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2307 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh
+-rwxrwxrwx   0 root         (0) root         (0)     9197 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac-architecture
+-rw-rw-rw-   0 root         (0) root         (0)    15857 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py
+-rw-rw-rw-   0 root         (0) root         (0)    10543 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     9819 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    16436 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.577825 iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.577825 iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/Agent/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.578825 iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/
+-rw-rw-rw-   0 root         (0) root         (0)     5544 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.578825 iLCDirac-34.0.0a5/src/ILCDIRAC/FrameworkSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.579825 iLCDirac-34.0.0a5/src/ILCDIRAC/FrameworkSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/FrameworkSystem/ConfigTemplate.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/FrameworkSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.579825 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.580825 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    25777 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     9996 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     5395 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.581825 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.582825 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)    35437 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    14308 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)    19604 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13782 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    30921 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7554 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.583825 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     5456 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.587825 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49360 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py
+-rw-rw-rw-   0 root         (0) root         (0)    46600 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6228 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py
+-rw-rw-rw-   0 root         (0) root         (0)     3366 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12482 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     7314 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py
+-rwxrwxrwx   0 root         (0) root         (0)     9954 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py
+-rw-rw-rw-   0 root         (0) root         (0)     4673 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    16641 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12116 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.587825 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.588825 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/
+-rw-rw-rw-   0 root         (0) root         (0)    13833 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/DiracILC.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.546825 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.589825 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/alias.properties
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py
+-rw-rw-rw-   0 root         (0) root         (0)     9474 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml
+-rw-rw-rw-   0 root         (0) root         (0)    10942 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.589825 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.601826 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/default.mac
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/defaultClicCrossingAngle.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_10gev_theta5-175.mac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.602825 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/
+-rw-rw-rw-   0 root         (0) root         (0)     8759 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.604826 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/
+-rw-rw-rw-   0 root         (0) root         (0)    27099 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.612826 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py
+-rw-rw-rw-   0 root         (0) root         (0)    10462 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py
+-rw-rw-rw-   0 root         (0) root         (0)    10003 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py
+-rw-rw-rw-   0 root         (0) root         (0)    35946 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py
+-rw-rw-rw-   0 root         (0) root         (0)    12944 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py
+-rw-rw-rw-   0 root         (0) root         (0)     6521 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6140 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py
+-rw-rw-rw-   0 root         (0) root         (0)     9573 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py
+-rw-rw-rw-   0 root         (0) root         (0)    10161 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8281 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py
+-rw-rw-rw-   0 root         (0) root         (0)    16303 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     3918 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py
+-rw-rw-rw-   0 root         (0) root         (0)     2090 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py
+-rw-rw-rw-   0 root         (0) root         (0)     3752 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6174 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)     5479 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6957 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py
+-rw-rw-rw-   0 root         (0) root         (0)    17277 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12788 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4441 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py
+-rw-rw-rw-   0 root         (0) root         (0)     4984 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.614826 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py
+-rw-rw-rw-   0 root         (0) root         (0)     2665 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    19613 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py
+-rw-rw-rw-   0 root         (0) root         (0)    22228 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4247 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py
+-rw-rw-rw-   0 root         (0) root         (0)     9857 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    24484 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py
+-rw-rw-rw-   0 root         (0) root         (0)    26292 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py
+-rw-rw-rw-   0 root         (0) root         (0)    15111 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3097 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)    40172 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.615826 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/
+-rw-rw-rw-   0 root         (0) root         (0)    27996 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    29727 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py
+-rwxrwxrwx   0 root         (0) root         (0)    35679 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py
+-rw-rw-rw-   0 root         (0) root         (0)    13124 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    12330 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.623826 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7876 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4672 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18299 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py
+-rw-rw-rw-   0 root         (0) root         (0)    15725 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py
+-rw-rw-rw-   0 root         (0) root         (0)    41414 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15653 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     4218 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    13745 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py
+-rw-rw-rw-   0 root         (0) root         (0)     7579 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py
+-rw-rw-rw-   0 root         (0) root         (0)    12305 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py
+-rw-rw-rw-   0 root         (0) root         (0)     8309 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6492 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py
+-rw-rw-rw-   0 root         (0) root         (0)    14537 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     4767 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)    71676 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4798 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py
+-rw-rw-rw-   0 root         (0) root         (0)     7551 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6829 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     4763 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py
+-rw-rw-rw-   0 root         (0) root         (0)    22726 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py
+-rw-rw-rw-   0 root         (0) root         (0)    20865 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13044 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4169 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9860 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.624826 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Test/
+-rw-rw-rw-   0 root         (0) root         (0)    20190 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.624826 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.625826 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15312 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.627826 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2968 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7808 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py
+-rw-rw-rw-   0 root         (0) root         (0)     3538 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     2636 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2396 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     3724 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.627826 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.628826 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)     2638 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.628826 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.629826 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/DB/
+-rw-rw-rw-   0 root         (0) root         (0)     6376 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.629826 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/DB/Test/
+-rw-rw-rw-   0 root         (0) root         (0)     9281 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/DB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.630826 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.630826 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.641826 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/
+-rw-rw-rw-   0 root         (0) root         (0)     4515 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py
+-rw-rw-rw-   0 root         (0) root         (0)     5524 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py
+-rw-rw-rw-   0 root         (0) root         (0)    23026 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5789 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py
+-rw-rw-rw-   0 root         (0) root         (0)     3146 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    16673 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8022 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/DummyModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     6809 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)    19926 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8787 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     4454 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6156 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     6801 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5057 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8078 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)    13096 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18950 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    31351 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/ModuleBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    26082 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5266 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/MoveInFC.py
+-rw-rw-rw-   0 root         (0) root         (0)    33871 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     7960 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8182 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5743 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/ReportErrors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5915 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5740 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    11639 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4044 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9340 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/StdHepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     3020 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.647826 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)    14814 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)    44092 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    18662 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)    28578 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    20599 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)    10005 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    45397 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    43848 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    41500 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)    10867 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8844 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    28021 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)    19461 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)    14457 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)    12973 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    10007 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    32143 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py
+-rw-rw-rw-   0 root         (0) root         (0)    14235 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    67243 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    86847 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py
+-rw-rw-rw-   0 root         (0) root         (0)     6505 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    17704 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    15076 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    17792 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py
+-rw-rw-rw-   0 root         (0) root         (0)     9795 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    22938 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.649826 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     3265 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Utilities/RootMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.649826 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.650826 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    24455 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.650826 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)    15894 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.651826 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Executor/
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.652826 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13587 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    31624 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3345 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2023-06-06 10:56:02.000000 iLCDirac-34.0.0a5/src/ILCDIRAC/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:56:24.653826 iLCDirac-34.0.0a5/src/iLCDirac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-06 10:56:24.000000 iLCDirac-34.0.0a5/src/iLCDirac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24527 2023-06-06 10:56:24.000000 iLCDirac-34.0.0a5/src/iLCDirac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 10:56:24.000000 iLCDirac-34.0.0a5/src/iLCDirac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-06-06 10:56:24.000000 iLCDirac-34.0.0a5/src/iLCDirac.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 10:56:23.000000 iLCDirac-34.0.0a5/src/iLCDirac.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-06 10:56:24.000000 iLCDirac-34.0.0a5/src/iLCDirac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-06 10:56:24.000000 iLCDirac-34.0.0a5/src/iLCDirac.egg-info/top_level.txt
```

### Comparing `iLCDirac-34.0.0a4/LICENSE` & `iLCDirac-34.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/PKG-INFO` & `iLCDirac-34.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iLCDirac
-Version: 34.0.0a4
+Version: 34.0.0a5
 Summary: iLCDirac is the iLC/CLIC/FCC extension of DIRAC
 Home-page: https://gitlab.cern.ch/clicdp/ilcdirac/ilcdirac.git
 Maintainer: Andre Sailer
 Maintainer-email: ilcdirac-support@cern.ch
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://its.cern.ch/jira/browse/ILCDIRAC
 Project-URL: Documentation, https://ilcdirac-doc.web.cern.ch/
```

### Comparing `iLCDirac-34.0.0a4/release.notes` & `iLCDirac-34.0.0a5/release.notes`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-[v34r0]
-Release date: 2023-05-26
+[v34.0]
+Release date: 2023-06-06
 
 *Core
 
+CHANGE: (!440) Delphes Application: After looking in the local folder, look up the pythia cards in outside folder defined by OperationsOption "/ProcessList/PythiaCardsLocation". Reading the pythia card, check if it contains the same energy specified for the output path.
+CHANGE: (!440) Gaudi Application: When using Delphes, after looking in the local folder, look up the pythia cards in outside folder defined by OperationsOption "/ProcessList/PythiaCardsLocation". Reading the pythia card, check if it contains the same energy specified for the output path.
+FIX: (!437) Update release notes
 NEW: Depend on DIRAC version 7.3
 NEW: Python3 only
-NEW: (!430) Implementation of the Delphes Application interface.
 NEW: (!430) Addition of some functionalities to the Gaudi Application interface.
 NEW: (!430) Correct paths for storing FCC simulations outputs.
+NEW: (!430) Implementation of the Delphes Application interface.
+NEW: (!440) Documentation for FCC production code.
 FIX: (!421) client installation: corrected (a typo in) the URL of the configuration service, fixes problems during dirac-configure.
 
 [v32r0p3]
 Release date: 2021-11-18
 
 *Core
 NEW: Based on Dirac v7r2p34
```

### Comparing `iLCDirac-34.0.0a4/releases.cfg` & `iLCDirac-34.0.0a5/releases.cfg`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/setup.cfg` & `iLCDirac-34.0.0a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Client/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/TODO` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/TODO`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Test/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/dev_create_events.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/CalibrationSystem/dev_create_events.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Configuration.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/Configuration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/DetectOS.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/DetectOS.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FileUtils.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/FileUtils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/GeneratorModels.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/GeneratorModels.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/HTML.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/HTML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InputDataResolution.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InstalledFiles.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/InstalledFiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
            "sidloi3_trackingStrategies_default.xml",
            "ild_00.gear",
            "ild_00_steering.xml",
            "ild_00.steer",
            "cuts_quarks_1400.txt", "cuts_taus_1400.txt",
            "cuts_h_gammaZ_1400.txt", "cuts_h_gammagamma_1400.txt",
            "cuts_h_mumu_3000.txt", 
-           "delphes_card_IDEA.tcl", "edm4hep_output_config.tcl",
+           "card_IDEA.tcl", "edm4hep_IDEA.tcl",
            "geant_fullsim_fccee_lar_pgun.py", 
            "k4simdelphesalg_pythia.py",
            "pythia.py",
            ]
   if myfile in files:
     return S_OK()
   elif configversion is None or platform is None:
```

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/JobPathResolution.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/JobPathResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/MarlinXML.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/MarlinXML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/OverlayFiles.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/OverlayFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/PrepareLibs.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/PrepareLibs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from ILCDIRAC.Core.Utilities.ResolveDependencies import resolveDeps
 from ILCDIRAC.Core.Utilities.PrepareLibs import removeLibc
 from ILCDIRAC.Core.Utilities.OverlayFiles import getOverlayFiles
 from ILCDIRAC.Core.Utilities.CombinedSoftwareInstallation import getSoftwareFolder
 from ILCDIRAC.Core.Utilities.MarlinXML import setOverlayFilesParameter, setOutputFileParameter
 from ILCDIRAC.Workflow.Modules.OverlayInput import allowedBkg
 import six
+import re
 
 LOG = gLogger.getSubLogger(__name__)
 __RCSID__ = "$Id$"
 
 
 def getNewLDLibs(platform, application, applicationVersion):
   """Prepare the LD_LIBRARY_PATH environment variable: make sure all lib folder are included.
@@ -815,53 +816,78 @@
             com = Comment('Collections to analyse changed')
             param.insert(0, com)
             subparam.text = collection
 
   tree.write(outputxml)
   return S_OK()
 
-def preparePythia8Card(pythia8CardContent, NumberOfEvents, randomSeed, pythia8Card=None):
+def preparePythia8Card(pythia8CardContent, NumberOfEvents, randomSeed, energy, pythia8Card=None):
   """Make the pythiacard file, using the string read in input. Edit it with the correct parameters of the task."""
   
   lines = pythia8CardContent.splitlines(keepends=True)
 
   for i, line in enumerate(lines):
     if line.lstrip().startswith('Beams:LHEF'):
-      LOG.info('Field `Beams:LHEF` found in your pythia card, Assuming it is a pythia card for reading LHE.')
+      LOG.notice('Field `Beams:LHEF` found in your pythia card, Assuming it is a pythia card for reading LHE.')
       card = 'reader'
       break
     elif line.replace(" ", "").startswith('Beams:eCM'):
-      LOG.info('Field `Beams:eCM` found in your pythia card, Assuming it is a pythia card for generating new events.')
+      LOG.notice('Field `Beams:eCM` found in your pythia card, Assuming it is a pythia card for generating new events.')
       card = 'generator'
       break
   else:
     LOG.error('Pythia card with unusual content: neither `Beams:LHEF` nor `Beams:eCM` fields present. Please check the content of your card.')
     return S_ERROR('Pythia card with unusual content: neither `Beams:LHEF` nor `Beams:eCM` fields present. Please check the content of your card.')
   
   modifiedEventNumber = False
   for i, line in enumerate(lines):
     if line.lstrip().startswith('Main:numberOfEvents'):
       lines[i] = f'Main:numberOfEvents = {NumberOfEvents}'+' '*(13-len(str(NumberOfEvents)))+'! number of events to generate\n'
       modifiedEventNumber = True
   if not modifiedEventNumber:
-    LOG.error('Not found any line in the pythia card for setting the number of events')
-    return S_ERROR('Not found any line in the pythia card for setting the number of events')
+    LOG.notice('Not found any line in the pythia card for setting the number of events. Appending in the end.')
+    lines.append(f'Main:numberOfEvents = {NumberOfEvents}'+' '*(13-len(str(NumberOfEvents)))+'! number of events to generate\n')
   
   modifiedEventNumber = False
   for i, line in enumerate(lines):
     # setting seed instructions: https://pythia.org/latest-manual/RandomNumberSeed.html
     if line.lstrip().startswith('Random:setSeed'): 
       lines[i] = f'Random:setSeed = on\n'
       lines.insert(i+1, f'Random:seed = {randomSeed}\n')
       modifiedEventNumber = True
   if not modifiedEventNumber:
     if card == 'reader':
-      LOG.info('Not found any line for setting the seed in your pythia card. That is fine, since your card appears to be a LHE reader.')
+      LOG.notice('Not found any line for setting the seed in your pythia card. That is fine, since your card appears to be a LHE reader.')
     elif card == 'generator':
-      LOG.info('Not found any line for setting the seed in your pythia card. Your card appears to be used for generation: I will add two lines for setting the seed by myself in the pythia card.')
+      LOG.notice('Not found any line for setting the seed in your pythia card. Your card appears to be used for generation: I will add two lines for setting the seed by myself in the pythia card.')
       lines.insert(0, f'Random:seed = {randomSeed}\n')
       lines.insert(0, f'Random:setSeed = on\n')
     
+  for i, line in enumerate(lines):
+    if line.lstrip().startswith('Beams:eCM'):
+      modifiedEventNumber = True
+      match = re.search(r'\d+(\.\d+)?', line)
+      if match:
+        cardenergy = float(metaEnergy(float(match.group())))
+        energy = float(metaEnergy(float(energy)))
+        if energy == cardenergy:
+          LOG.notice('Found in the pythia card a line containing a value compatible with the energy chosen for the process. Good.')
+        else:
+          LOG.error('Problem when checking the pythia card. The energy value found in the line starting with `Beams:eCM` was incompatible with the energy assigned to the process')
+          return S_ERROR('Problem when checking the pythia card. The energy value found in the line starting with `Beams:eCM` was incompatible with the energy assigned to the process')
+      else:
+        LOG.error('Problem when checking the pythia card. The energy value found in the line starting with `Beams:eCM` was missing.')
+        return S_ERROR('Problem when checking the pythia card. The energy value found in the line starting with `Beams:eCM` was missing.')
+  if not modifiedEventNumber:
+    LOG.info('Not found any line for setting the energy in your pythia card. That is fine, since your card appears to be a LHE reader.')
+
   if pythia8Card:
     with open(pythia8Card, 'w') as f:
       f.writelines(lines)    
   return S_OK()
+
+def metaEnergy(energy):
+  """Return string of the energy with no non-zero digits."""
+  if isinstance(energy, six.string_types):
+    return energy
+  energy = ("%1.2f" % energy).rstrip('0').rstrip('.')
+  return energy
```

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ProcessList.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/ProcessList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ProductionData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/ProductionData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/RemoveSoft.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/RemoveSoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ResolveSE.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/ResolveSE.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Splitting.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/Splitting.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/TARsoft.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/TARsoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Utilities.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/WasteCPU.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/WasteCPU.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/WhizardOptions.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/WhizardOptions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1347,36 +1347,40 @@
       assertEqualsXml(current_tree.findall('global/parameter')[-1],
                       expected_element, self)
       expected_tuples = [('default.xml', 'w')]
       FileUtil.checkFileInteractions(self, mo, expected_tuples, expected,
                                       handles)
 
   @parameterized.expand([('ciao\n', 'Pythia card with unusual content: neither `Beams:LHEF` nor `Beams:eCM` fields present. Please check the content of your card.'),
-                         ('Beams:LHEF\n', 'Not found any line in the pythia card for setting the number of events'),
+                         ('Beams:LHEF\n', None),
                          ('Beams:LHEF\nMain:numberOfEvents', None),
                          ('Beams:LHEF\nMain:numberOfEvents\nRandom:setSeed', None),
-                         ('Beams:eCM\n', 'Not found any line in the pythia card for setting the number of events'),
-                         ('Beams:eCM\nMain:numberOfEvents', None),
-                         ('Beams:eCM\nMain:numberOfEvents\nRandom:setSeed', None)])
-  def test_preparePythia8Card(self, cardcontent, outmessage):
+                         ('Beams:eCM\n', 'Problem when checking the pythia card. The energy value found in the line starting with `Beams:eCM` was missing.'),
+                         ('Beams:eCM\nMain:numberOfEvents', 'Problem when checking the pythia card. The energy value found in the line starting with `Beams:eCM` was missing.'),
+                         ('Beams:eCM = 91.19 \nMain:numberOfEvents\nRandom:setSeed', None),
+                         ('Beams:eCM = 91.188 \nMain:numberOfEvents\nRandom:setSeed', None),
+                         ('Beams:eCM = 91.2\nMain:numberOfEvents\nRandom:setSeed', 'Problem when checking the pythia card. The energy value found in the line starting with `Beams:eCM` was incompatible with the energy assigned to the process'),
+                         ('Beams:eCM = 240\nMain:numberOfEvents\nRandom:setSeed', 'Problem when checking the pythia card. The energy value found in the line starting with `Beams:eCM` was incompatible with the energy assigned to the process')])
+  def test_preparePythia8Card(self, cardcontent, outmessage, energy = 91.19):
     randomSeed = 12345
     pythia8CardContent = cardcontent
     pythia8Card = 'pythia8Card'
     NumberOfEvents = 1234000
-    res = PrepareOptionFiles.preparePythia8Card(pythia8CardContent, NumberOfEvents, randomSeed, pythia8Card)
+    res = PrepareOptionFiles.preparePythia8Card(pythia8CardContent, NumberOfEvents, randomSeed, energy, pythia8Card)
     if outmessage:
       self.assertEqual(outmessage, res['Message'])
     else:
       self.assertEqual(outmessage, res['Value'])
 
   def test_preparePythia8Card_nofilename(self):
     randomSeed = 12345
-    pythia8CardContent = 'Beams:eCM\nMain:numberOfEvents\nRandom:setSeed'
+    pythia8CardContent = 'Beams:eCM = 91.2\nMain:numberOfEvents\nRandom:setSeed'
     NumberOfEvents = 1234000
-    res = PrepareOptionFiles.preparePythia8Card(pythia8CardContent, NumberOfEvents, randomSeed)
+    energy = 91.2
+    res = PrepareOptionFiles.preparePythia8Card(pythia8CardContent, NumberOfEvents, randomSeed, energy)
     self.assertEqual(None, res['Value'])
 
 def createXMLTreeForXML(flag=0):
   """Creates a XML Tree to test prepareXMLFile()"""
   root = ET.Element("root")
   ex = ET.SubElement(root, 'execute')
   ET.SubElement(ex, 'processor', name='MYOVERLAYTIMING', type='OverlayTiming')
```

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac-architecture` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac-architecture`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/DataManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/FrameworkSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,76 +18,83 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
-"""Create productions for the Whizard2/DDSim/Marlin software chain.
+"""Create productions for the generation/simulation/reconstruction software chain.
 
 First create a config file template::
 
-  dirac-clic-make-productions -p
+  dirac-fcc-make-productions -p
 
 Then modify the template to describe the productions::
 
-    [Production Parameters]
-    detectorModel = CLIC_o3_v14
-    version = 2018-08-10
-    softwareVersion = ILCSoft-%(version)s_gcc62
-    configVersion = ILCSoft-%(version)s
-    generatorVersion = 2.6.3
-    productionLogLevel = VERBOSE
-    outputSE = CERN-DST-EOS
-    finalOutputSE = CERN-SRM
-    DRC=200
-    machine = ee
-    prodGroup = %(detectorModel)s_DiJets
-    ProdTypes = Gen, Sim, Rec, RecOver
-    energies =                100, 200
-    processes =          DY_uds
-    eventsPerJobs =           100
-    MoveTypes = REC, GEN, SIM
-    MoveStatus = Active
-    MoveGroupSize = 10
-    move = True
-    overlayEvents = 380GeV
-    cliReco = --Config.Tracking=Conformal --MyDDMarlinPandora.D0TrackCut=%(DRC)s
-        --MyDDMarlinPandora.Z0TrackCut=%(DRC)s --MyDDMarlinPandora.MaxBarrelTrackerInnerRDistance=%(DRC)s
-    additionalName = 3
-    generatorSteeringFile = dy_uds.sin
+  [delphesapp]
+  ExecutableName = DelphesPythia8_EDM4HEP
+  DetectorCard = delphes_card_IDEA.tcl
+  OutputCard = edm4hep_output_config.tcl
+  Version = key4hep-latest
+
+  [Production Parameters]
+  machine = ee
+  prodGroup = several
+  softwareVersion = key4hep-latest
+  generatorApplication = delphesapp
+  generatorSteeringFile = p8_ee_ggqq_ecm91.cmd, p8_ee_WW_ecm240.cmd, p8_ee_ZH_ecm240.cmd, p8_ee_ZZ_ecm240.cmd
+  configVersion = key4hep-devel-2
+  configPackage = fccConfig
+  eventsPerJobs = 1000, 2000, 3000, 1500
+  numberOfTasks = 1, 1, 1, 1
+  campaign = winter2023
+  energies = 91.188, 240, 240, 240
+  processes = qqbar, WW_incl, ZZ_incl, ZH_incl
+  detectorModel = idea
+  datatype = delphesapp
+  productionLogLevel = VERBOSE
+  outputSE = CERN-DST-EOS
+  finalOutputSE = CERN-SRM
+  MoveStatus = Stopped
+  MoveGroupSize = 10
+  ProdTypes = Gen
+  move = False
 
 Further options can be found in the created template file. Many options can contain comma separated values to submit
-multiple chains of productions in one command. The example above will create two chains of Generation, Simulation,
-Reconstruction and Reconstruction with overlay transformations, one for 100 GeV and one for 200 GeV.
+multiple chains of productions in one command. The example above will create a chain of Generation with pythia and processing
+with delphes, everything using a delphes standalone executable.
 
 Then test if everything works::
 
-  dirac-clic-make-productions -f myProd
+  dirac-fcc-make-productions -f myProd
 
 And finally submit to the system::
 
-  dirac-clic-make-productions -f myProd -x
+  dirac-fcc-make-productions -f myProd -x
 
 Options:
 
    -p, --printConfigFile      Create the template to create productions
    -f, --configFile <file>    Defines the file with the parameters to create a production
    -x, --enable               Disable dry-run mode and actually create the production
    --additionalName       Define a string to add to the production name if the original name already exists
 
 
 Parameters in the steering file
 
   :configPackage: Steering file package to use for simulation and reconstruction
   :configVersion: Steering file version to use for simulation and reconstruction
-  :detectorModel: Detector Model to use in simulation and reconstruction
   :outputSE: output SE for transformation jobs
   :finalOutputSE: final destination for files when moving transformations are enabled
-  :machine: the name of the machine, ee, hh, eh
+  :machine: the name of the machine: ee
+  :campaign: season and year of the simulations
+  :energies: energies of the processes
+  :processes: name informative of process and final state
+  :detectorModel: Detector Model appearing in the filepath
+  :datatype: data type (sim/rec, delphes, hepmc, lhe...)
   :prodGroup: basename of the production group the productions are part of
   :productionLogLevel: log level to use in production jobs
   :softwareVersion: softwareVersion to use for generation/simulation/reconstruction
   :additionalName: additionalName to add to the transformation name in case a transformation
      with that name already exists
 
   :ProdTypes: Which transformations to create: Gen, Split, Sim, Rec, RecOver
@@ -97,22 +104,14 @@
   :move: Whether or not to create the transformations to the output files to the finalOutputSE
 
   :energies: energy to use for generation or meta data search for each transformation chain
   :eventsPerJobs: number of events per job
   :processes: name of the processes to generate or use in meta data search
   :prodids: transformation IDs to use in meta data search for the first transformation of each chain
 
-  :simSteeringFile: path to steering file for the generator
-  :simVersion: specify which version of the generator to use
-  :simApplication: specify which application to use for event generation
-
-  :recoSteeringFile: path to steering file for the generator
-  :recoVersion: specify which version of the generator to use
-  :recoApplication: specify which application to use for event generation
-
   :generatorSteeringFile: path to steering file for the generator
   :generatorVersion: specify which version of the generator to use
   :generatorApplication: specify which application to use for event generation
   :numberOfTasks: number of production jobs/task to create for Gen transformations (default is 1)
 
   :eventsInSplitFiles: For split transformations, number of events in the input files
 
@@ -120,31 +119,27 @@
 
   :overlayEvents: For ``RecOver`` transformations use these events for Overlay. By default the gghad
      events with the process energy are used for overlay. E.g.: ``380GeV``
 
 
 The individual applications can be further modified in their respective section::
 
-  [Marlin]
-  #ApplicationAttributeName=Value
-
-  [DDSim]
+  [KKMC]
   #ApplicationAttributeName=Value
 
-  [Overlay]
+  [gaudiapp]
   #ApplicationAttributeName=Value
 
-  [Whizard2]
+  [delphesapp]
   #ApplicationAttributeName=Value
 
 All attributes with a ``set`` method can be changed. See
-:mod:`~ILCDIRAC.Interfaces.API.NewInterface.Applications.Whizard2`,
-:mod:`~ILCDIRAC.Interfaces.API.NewInterface.Applications.Marlin`,
-:mod:`~ILCDIRAC.Interfaces.API.NewInterface.Applications.OverlayInput`,
-:mod:`~ILCDIRAC.Interfaces.API.NewInterface.Applications.DDSim`.
+:mod:`~ILCDIRAC.Interfaces.API.NewInterface.Applications.KKMC`,
+:mod:`~ILCDIRAC.Interfaces.API.NewInterface.Applications.GaudiApp`,
+:mod:`~ILCDIRAC.Interfaces.API.NewInterface.Applications.DelphesApp`,
 
 
 
 :since: July 14, 2017
 :author: A Sailer
 """
 
@@ -160,23 +155,24 @@
 import six.moves.configparser
 import os
 
 from DIRAC.Core.Base import Script
 from DIRAC.Core.Utilities.DIRACScript import DIRACScript
 from DIRAC import S_OK, S_ERROR, gLogger
 
+from ILCDIRAC.Core.Utilities.PrepareOptionFiles import metaEnergy
 from ILCDIRAC.Core.Utilities.OverlayFiles import energyWithUnit, energyToInt
 from ILCDIRAC.Core.Utilities.Utilities import listify, lowerFirst
 from ILCDIRAC.ILCTransformationSystem.Utilities.Utilities import Task
 import six
 from six.moves import zip_longest
 
 PRODUCTION_PARAMETERS = 'Production Parameters'
 PP = PRODUCTION_PARAMETERS
-APPLICATION_LIST = ['Marlin', 'DDSim', 'Overlay', 'Whizard2', 'KKMC', 'delphesapp', 'gaudiapp']
+APPLICATION_LIST = ['KKMC', 'delphesapp', 'gaudiapp']
 LIST_ATTRIBUTES = ['ignoreMetadata',
                    'generatorSteeringFile',
                    'energies',
                    'eventsPerJobs',
                    'numberOfTasks',
                    'processes',
                    'prodIDs',
@@ -236,19 +232,19 @@
     return S_OK()
 
   def registerSwitches(self):
     Script.registerSwitch("f:", "configFile=", "Set config file for production", self.setProdConf)
     Script.registerSwitch("x", "enable", "create productions, if off dry-run", self.setEnable)
     Script.registerSwitch("p", "printConfigFile", "Print a config file to stdout", self.setDumpConf)
     Script.registerSwitch("", "additionalName=", "Name to add to the production", self.setAddName)
-    Script.setUsageMessage("""%s --configFile=myProduction""" % ("dirac-clic-make-productions", ))
+    Script.setUsageMessage("""%s --configFile=myProduction""" % ("dirac-fcc-make-productions", ))
 
 
 class FCCDetProdChain(object):
-  """Create applications and productions for CLIC physics studies."""
+  """Create applications and productions for FCC physics studies."""
 
   class Flags(object):
     """flags to enable or disable productions.
 
     :param bool dryRun: if False no productions are created
     :param bool gen: if True create generation production
     :param bool spl: if True create split production
@@ -382,15 +378,15 @@
 
   def __init__(self, params=None, group='fcc_prod'):
 
     from DIRAC.ConfigurationSystem.Client.Helpers.Operations import Operations
     self._ops = Operations(group=group)
 
     self.machine = {'ilc_prod': 'clic',
-                    'fcc_prod': 'fccee',
+                    'fcc_prod': 'ee',
                     }[group]
 
     self.overlayEventType = {'ilc_prod': 'gghad',
                              'fcc_prod': 'pairs',
                              }[group]
 
     self.prodGroup = 'several'
@@ -458,15 +454,15 @@
       self._basepath = self._ops.getValue(os.path.join(prodPath, 'BasePath'))
     return os.path.join(self._basepath, self.campaign) + '/'
   
   def meta(self, prodID, process, energy):
     """return meta data dictionary, always new."""
     metaD = {'ProdID': str(prodID),
              'EvtType': process,
-             'Energy': self.metaEnergy(energy),
+             'Energy': metaEnergy(energy),
              'Machine': self.machine,
              }
     for key in self.ignoreMetadata:
       metaD.pop(key)
     return metaD
 
   def loadParameters(self, parameter):
@@ -606,41 +602,33 @@
     pDict.update({'ProductionParameters': PRODUCTION_PARAMETERS})
     pDict.update({'ApplicationOptions': appOptionString})
     return """
 %(ApplicationOptions)s
 [%(ProductionParameters)s]
 machine = %(machine)s
 prodGroup = %(prodGroup)s
-detectorModel = %(detectorModel)s
 softwareVersion = %(softwareVersion)s
 
 generatorApplication = %(generatorApplication)s
 generatorVersion = %(generatorVersion)s
 generatorSteeringFile = %(generatorSteeringFile)s
 processingAfterGen = %(processingAfterGen)s
 
-datatype = %(datatype)s
 campaign = %(campaign)s
-
-simApplication = %(simApplication)s
-simVersion = %(simVersion)s
-simSteeringFile = %(simSteeringFile)s
-
-recoApplication = %(recoApplication)s
-recoVersion = %(recoVersion)s
-recoSteeringFile = %(recoSteeringFile)s
+energies = %(energies)s
+processes = %(processes)s
+detectorModel = %(detectorModel)s
+datatype = %(datatype)s
 
 configVersion = %(configVersion)s
 configPackage = %(configPackage)s
 eventsPerJobs = %(eventsPerJobs)s
 ## Number of jobs/task to generate (default = 1)
 # numberOfTasks =
 
-energies = %(energies)s
-processes = %(processes)s
 ## optional prodid to search for input files
 # prodIDs =
 
 ## number of events for input files to split productions
 eventsInSplitFiles = %(eventsInSplitFiles)s
 
 productionLogLevel = %(productionLogLevel)s
@@ -651,63 +639,38 @@
 MoveGroupSize = %(moveGroupSize)s
 
 ## optional additional name
 # additionalName = %(additionalName)s
 ## optional additional names, for for each process, prodID, etc.
 # taskNames =
 
-## optional marlin CLI options
-# cliReco = %(cliReco)s
-
 overlayEventType = %(overlayEventType)s
 ## optional energy to use for overlay: e.g. 3TeV
 # overlayEvents = %(overlayEvents)s
 
 %(_flags)s
 
 """ % (pDict)
 
-  @staticmethod
-  def metaEnergy(energy):
-    """Return string of the energy with no non-zero digits."""
-    if isinstance(energy, six.string_types):
-      return energy
-    energy = ("%1.2f" % energy).rstrip('0').rstrip('.')
-    return energy
-
   def createGeneratorApplication(self, task):
     """Create the selected generator application."""
     genApp =  {'kkmc': self.createKKMCApplication,
-               'whizard2': self.createWhizard2Application,
                'delphesapp': self.createDelphesApplication,
                'gaudiapp': self.createGaudiApplication,
              }[self.generatorApplication.lower()](task)
     if task.datatype:
       genApp.datatype = task.datatype
     return genApp
 
   def createSimulationApplication(self, task):
     """Create the selected Simulation application."""
 
     return {'genericapp': self.createGenericApplication,
             }[self.simApplication.lower()](task)
 
-  def createWhizard2Application(self, task):
-    """create Whizard2 Application."""
-    from ILCDIRAC.Interfaces.API.NewInterface.Applications import Whizard2
-    whiz = Whizard2()
-    whiz.setVersion(self.generatorVersion)
-    whiz.setNumberOfEvents(task.eventsPerJob)
-    whiz.setSinFile(task.genFile)
-    whiz.setEvtType(task.meta['EvtType'])
-    whiz.setEnergy(task.meta['Energy'])
-    whiz.datatype = 'lhef'
-    self._setApplicationOptions('Whizard2', whiz, task.applicationOptions)
-    return whiz
-
   def createKKMCApplication(self, task):
     """create KKMCee Application."""
     from ILCDIRAC.Interfaces.API.NewInterface.Applications import KKMC
     kkmcee = KKMC()
     kkmcee.setVersion(self.generatorVersion)
     kkmcee.setNumberOfEvents(task.eventsPerJob)
     if task.genFile:
@@ -767,16 +730,16 @@
     genApp = self.createGeneratorApplication(task)
     if task.generator:
       genProd.generator = task.generator
     res = genProd.append(genApp)
     if not res['OK']:
       raise RuntimeError("Error creating generation production: %s" % res['Message'])
     if self.processingAfterGen:
-      processingapp = {'delphes': self.createDelphesApplication,
-                       'gaudi': self.createGaudiApplication,
+      processingapp = {'delphesapp': self.createDelphesApplication,
+                       'gaudiapp': self.createGaudiApplication,
                        }[self.processingAfterGen](task)
       res = genProd.append(processingapp)
       if not res['OK']:
         raise RuntimeError("Error creating generation production: %s" % res['Message'])
         
     genProd.addFinalization(True, True, True, True)
     if not prodName:
@@ -1027,23 +990,23 @@
 
   def createTransformations(self, taskDict):
     """Create all the transformations we want to create."""
     for pType, createProduction in [('GEN', self.createGenerationProduction),
                                     ('SPLIT', self.createSplitProduction)]:
       for task in taskDict.get(pType, []):
         meta = createProduction(task)
-        self.addSimTask(taskDict, meta, originalTask=task)
+        # self.addSimTask(taskDict, meta, originalTask=task)
         taskDict['MOVE_' + pType].append(dict(meta))
 
     for task in taskDict.get('SIM', []):
       if not self._flags.sim:
         continue
       gLogger.notice("Creating task %s" % task)
       simMeta = self.createSimulationProduction(task)
-      self.addRecTask(taskDict, simMeta, originalTask=task)
+      # self.addRecTask(taskDict, simMeta, originalTask=task)
       taskDict['MOVE_SIM'].append(dict(simMeta))
 
     for task in taskDict.get('REC', []):
       for name, over, enabled in [('REC', False, self._flags.rec),
                                   ('OVER', True, self._flags.over)]:
         if enabled:
           recMeta = self.createReconstructionProduction(task, over=over)
```

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/DiracILC.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/DiracILC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 .. versionadded:: v34r0
 
 Usage:
 
 >>> delphes = DelphesApp()
 >>> delphes.setVersion('key4hep-latest')
 >>> delphes.setExecutable("DelphesPythia8_EDM4HEP")
->>> delphes.setDetectorCard('delphes_card_IDEA.tcl')
->>> delphes.setOutputCard('edm4hep_output_config.tcl')
+>>> delphes.setDetectorCard('card_IDEA.tcl')
+>>> delphes.setOutputCard('edm4hep_IDEA.tcl')
 >>> delphes.setPythia8Card('p8_ee_ggqq_ecm91.cmd')
 >>> delphes.setRandomSeed(12340)
 >>> delphes.setEnergy(91.2)
 >>> delphes.setNumberOfEvents(100)
 >>> delphes.setOutputFile('output.root')
 
 """
@@ -128,19 +128,27 @@
 
 
   def setPythia8Card(self, pythia8CardPath):
     """Set the pythia8 card.
 
     :param str pythia8CardPath: Name of the Pythia8 configuration file path.
     """
+    pythiaCardsLocations = Operations().getValue("/ProcessList/PythiaCardsLocation", [])
     self._checkArgs({'pythia8CardPath': (str,)})
-    if not os.path.isfile(pythia8CardPath):
+    if os.path.isfile(pythia8CardPath):
+      self.pythia8CardContent = open(pythia8CardPath).read()
+      return S_OK()
+    else:
+      for PythiaCardsLocation in pythiaCardsLocations:
+        pythia8CardEOS = os.path.join(PythiaCardsLocation, pythia8CardPath)
+        if os.path.isfile(pythia8CardEOS):
+          LOG.notice(f"Reading pythia card from {pythia8CardEOS}")
+          self.pythia8CardContent = open(pythia8CardEOS).read()
+          return S_OK()
       return self._reportError('Pythia8 configuration file does not exist!')
-    self.pythia8CardContent = open(pythia8CardPath).read()
-    return S_OK()
 
 
   def _userjobmodules(self, stepdefinition):
     res1 = self._setApplicationModuleAndParameters(stepdefinition)
     res2 = self._setUserJobFinalization(stepdefinition)
     if not res1["OK"] or not res2["OK"]:
       return S_ERROR('userjobmodules failed')
@@ -200,15 +208,15 @@
     else:
       return S_ERROR('Missing output-config-file.')
             
     if self.executableName == "DelphesPythia8_EDM4HEP" and not self.pythia8CardContent:
       return S_ERROR('Missing Pythia 8 Card. The execution of DelphesPythia8_EDM4HEP would not succeed')
 
     if self.pythia8CardContent:
-      res = preparePythia8Card(self.pythia8CardContent, 0, self.randomSeed)
+      res = preparePythia8Card(self.pythia8CardContent, 0, self.randomSeed, self.energy)
       if not res['OK']:
         return res
       
     if self._jobtype != 'User':
       self._listofoutput.append({"outputFile": "@{OutputFile}", "outputPath": "@{OutputPath}",
                                  "outputDataSE": '@{OutputSE}'})
```

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 Usage:
 
 >>> ga = GaudiApp()
 >>> ga.setVersion('key4hep-latest')
 >>> ga.setExecutable("k4run")
 >>> ga.setSteeringFile('k4simdelphesalg_pythia.py')
 >>> ga.setPythia8Card('p8_ee_ggqq_ecm91.cmd')
->>> ga.setExtraCLIArguments("--GenAlg.PythiaInterface.pythiacard pythia8card.cmd --k4SimDelphesAlg.DelphesCard delphes_card_IDEA.tcl --k4SimDelphesAlg.DelphesOutputSettings edm4hep_output_config.tcl")
+>>> ga.setExtraCLIArguments("--GenAlg.PythiaInterface.pythiacard pythia8card.cmd --k4SimDelphesAlg.DelphesCard card_IDEA.tcl --k4SimDelphesAlg.DelphesOutputSettings edm4hep_IDEA.tcl")
 >>> ga.setEnergy(91.2)
 >>> ga.setNumberOfEvents(50)
 >>> ga.setOutputFile('output.root')
 
 """
 from __future__ import absolute_import
 import types
@@ -164,19 +164,27 @@
     self.executableName = executableName
 
   def setPythia8Card(self, pythia8CardPath):
     """Set the pythia8 card.
 
     :param str pythia8CardPath: Name of the Pythia8 configuration file path.
     """
+    pythiaCardsLocations = Operations().getValue("/ProcessList/PythiaCardsLocation", [])
     self._checkArgs({'pythia8CardPath': (str,)})
-    if not os.path.isfile(pythia8CardPath):
+    if os.path.isfile(pythia8CardPath):
+      self.pythia8CardContent = open(pythia8CardPath).read()
+      return S_OK()
+    else:
+      for PythiaCardsLocation in pythiaCardsLocations:
+        pythia8CardEOS = os.path.join(PythiaCardsLocation, pythia8CardPath)
+        if os.path.isfile(pythia8CardEOS):
+          LOG.notice(f"Reading pythia card from {pythia8CardEOS}")
+          self.pythia8CardContent = open(pythia8CardEOS).read()
+          return S_OK()
       return self._reportError('Pythia8 configuration file does not exist!')
-    self.pythia8CardContent = open(pythia8CardPath).read()
-    return S_OK()
     
   def setKeepRecFile(self, val):
     """Set the ``keepRecFile`` flag.
 
     Only relevant for ProductionJobs
 
     :param bool val: If ``False`` REC file is not stored
@@ -262,15 +270,15 @@
       self._listofoutput.append({"outputFile": "@{OutputFile}", "outputPath": "@{OutputPath}",
                                  "outputDataSE": '@{OutputSE}'})
 
       self.prodparameters['detectorType'] = self.detectortype
       self.prodparameters['slic_detectormodel'] = self.detectorModel
 
     if self.pythia8CardContent:
-      res = preparePythia8Card(self.pythia8CardContent, 0, self.randomSeed)
+      res = preparePythia8Card(self.pythia8CardContent, 0, self.randomSeed, self.energy)
       if not res['OK']:
         return res
 
     if not self.startFrom:
       LOG.verbose('No startFrom defined for GaudiApp : start from the beginning')
 
     return S_OK()
```

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,22 @@
     self.assertFalse(self.delphes._errorDict)
     with patch("builtins.open", mock_open(read_data='content')), \
          patch('os.path.isfile', new=Mock(return_value=True)):
       res = self.delphes.setPythia8Card("pythia8card.cmd")
       assertDiracSucceeds(res, self)
       assertEqualsImproved(self.delphes.pythia8CardContent, 'content', self)
 
+  def test_setPythia8CardEOS(self):
+    self.assertFalse(self.delphes._errorDict)
+    with patch("builtins.open", mock_open(read_data='content')), \
+      patch("os.path.isfile", new=Mock(side_effect=[False, True])):
+      res = self.delphes.setPythia8Card("p8_ee_tt_ecm365.cmd")
+      assertDiracSucceeds(res, self)
+      assertEqualsImproved(self.delphes.pythia8CardContent, 'content', self)
+
   def test_setPythia8Card_fails_file(self):
     self.assertFalse(self.delphes._errorDict)
     res = self.delphes.setPythia8Card("content")
     assertDiracFailsWith(res, 'Pythia8 configuration file does not exist!', self)
 
   def test_setPythia8Card_fails_argument(self):
     self.assertFalse(self.delphes._errorDict)
@@ -241,37 +249,37 @@
     self.delphes.randomSeed = -1
     assertDiracFailsWith(self.delphes._checkConsistency(Mock()), 'Missing detector config-file.', self)
 
   def test_checkconsistency_nooutputcard(self):
     self.delphes.version = '134'
     self.delphes.executableName = 'DelphesPythia8_EDM4HEP'
     self.delphes.randomSeed = -1
-    self.delphes.detectorCard = 'delphes_card_IDEA.tcl'
+    self.delphes.detectorCard = 'card_IDEA.tcl'
     assertDiracFailsWith(self.delphes._checkConsistency(Mock()), 'Missing output-config-file.', self)
 
   def test_checkconsistency_nopythia8card(self):
     self.delphes.version = '134'
     self.delphes.executableName = 'DelphesPythia8_EDM4HEP'
     self.delphes.randomSeed = -1
-    self.delphes.detectorCard = 'delphes_card_IDEA.tcl'
-    self.delphes.outputCard = 'edm4hep_output_config.tcl'
+    self.delphes.detectorCard = 'card_IDEA.tcl'
+    self.delphes.outputCard = 'edm4hep_IDEA.tcl'
     assertDiracFailsWith(self.delphes._checkConsistency(Mock()), 'Missing Pythia 8 Card. The execution of DelphesPythia8_EDM4HEP would not succeed', self)
 
   def test_checkconsistency_baddetectorcard(self):
     self.delphes.version = '134'
     self.delphes.executableName = 'DelphesPythia8_EDM4HEP'
     self.delphes.randomSeed = -1
     self.delphes.detectorCard = 'badname'
     assertDiracFailsWith(self.delphes._checkConsistency(Mock()), 'Wrong name for the detector config file. Hint: they all end in ".tcl"', self)
 
   def test_checkconsistency_badoutputcard(self):
     self.delphes.version = '134'
     self.delphes.executableName = 'DelphesPythia8_EDM4HEP'
     self.delphes.randomSeed = -1
-    self.delphes.detectorCard = 'delphes_card_IDEA.tcl'
+    self.delphes.detectorCard = 'card_IDEA.tcl'
     self.delphes.outputCard = 'badname'
     assertDiracFailsWith(self.delphes._checkConsistency(Mock()), 'Wrong name for the output config file. Hint: they all end in ".tcl"', self)
 
   def test_checkconsistency_detectorcardnotavailable(self):
     self.delphes.version = '134'
     self.delphes.executableName = 'DelphesPythia8_EDM4HEP'
     self.delphes.randomSeed = -1
@@ -279,62 +287,62 @@
     res = self.delphes._checkConsistency(Mock())
     assertDiracFailsWith(res, 'badname.tcl is not available locally nor in the software installation', self)
 
   def test_checkconsistency_outputcardnotavailable(self):
     self.delphes.version = '134'
     self.delphes.executableName = 'DelphesPythia8_EDM4HEP'
     self.delphes.randomSeed = -1
-    self.delphes.detectorCard = 'delphes_card_IDEA.tcl'
+    self.delphes.detectorCard = 'card_IDEA.tcl'
     self.delphes.outputCard = 'badname.tcl'
     res = self.delphes._checkConsistency(Mock())
     assertDiracFailsWith(res, 'badname.tcl is not available locally nor in the software installation', self)
 
   def test_checkconsistency_badpythia8card(self):
     self.delphes.version = '134'
     self.delphes.executableName = 'DelphesPythia8_EDM4HEP'
     self.delphes.randomSeed = -1
-    self.delphes.detectorCard = 'delphes_card_IDEA.tcl'
-    self.delphes.outputCard = 'edm4hep_output_config.tcl'
+    self.delphes.detectorCard = 'card_IDEA.tcl'
+    self.delphes.outputCard = 'edm4hep_IDEA.tcl'
     self.delphes.pythia8CardContent = 'poorcontent'
     res = self.delphes._checkConsistency(Mock())
     assertDiracFailsWith(res, 'Pythia card with unusual content: neither `Beams:LHEF` nor `Beams:eCM` fields present. Please check the content of your card.', self)
 
   def test_checkconsistency(self):
     self.delphes.version = '134'
     self.delphes.executableName = 'DelphesPythia8_EDM4HEP'
-    self.delphes.detectorCard = 'delphes_card_IDEA.tcl'
-    self.delphes.outputCard = 'edm4hep_output_config.tcl'
+    self.delphes.detectorCard = 'card_IDEA.tcl'
+    self.delphes.outputCard = 'edm4hep_IDEA.tcl'
     self.delphes.pythia8CardContent = 'Beams:LHEF\nMain:numberOfEvents'
     self.delphes.outputFile = 'myoutput.file'
     self.delphes._jobtype = 'User'
     assertDiracSucceeds(self.delphes._checkConsistency(Mock()), self)
     self.assertNotIn({'outputFile': '@{OutputFile}', 'outputPath': '@{OutputPath}',
                         'outputDataSE': '@{OutputSE}'}, self.delphes._listofoutput)
     self.assertNotIn('nbevts', self.delphes.prodparameters)
     self.assertNotIn('Process', self.delphes.prodparameters)
 
   def test_checkconsistency_longfilenames(self):
     self.delphes.version = '134'
     self.delphes.executableName = 'DelphesPythia8_EDM4HEP'
-    self.delphes.detectorCard = 'lfn:delphes_card_IDEA.tcl'
-    self.delphes.outputCard = 'lfn:edm4hep_output_config.tcl'
+    self.delphes.detectorCard = 'lfn:card_IDEA.tcl'
+    self.delphes.outputCard = 'lfn:edm4hep_IDEA.tcl'
     self.delphes.pythia8CardContent = 'Beams:LHEF\nMain:numberOfEvents'
     self.delphes.outputFile = 'myoutput.file'
     self.delphes._jobtype = 'User'
     assertDiracSucceeds(self.delphes._checkConsistency(Mock()), self)
     self.assertNotIn({'outputFile': '@{OutputFile}', 'outputPath': '@{OutputPath}',
                         'outputDataSE': '@{OutputSE}'}, self.delphes._listofoutput)
     self.assertNotIn('nbevts', self.delphes.prodparameters)
     self.assertNotIn('Process', self.delphes.prodparameters)
 
   def test_checkconsistency_notuserjobtype(self):
     self.delphes.version = '134'
     self.delphes.executableName = 'DelphesSTDHEP_EDM4HEP'
-    self.delphes.detectorCard = 'delphes_card_IDEA.tcl'
-    self.delphes.outputCard = 'edm4hep_output_config.tcl'
+    self.delphes.detectorCard = 'card_IDEA.tcl'
+    self.delphes.outputCard = 'edm4hep_IDEA.tcl'
     self.delphes.outputFile = 'myoutput.file'
     self.delphes._jobtype = 'NotaUser'
     assertDiracSucceeds(self.delphes._checkConsistency(Mock()), self)
     self.assertIn({'outputFile': '@{OutputFile}', 'outputPath': '@{OutputPath}',
                         'outputDataSE': '@{OutputSE}'}, self.delphes._listofoutput)
     self.assertNotIn('nbevts', self.delphes.prodparameters)
     self.assertNotIn('Process', self.delphes.prodparameters)
```

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,22 @@
     self.assertFalse(self.gaudi._errorDict)
     with patch("builtins.open", mock_open(read_data='content')), \
          patch('os.path.isfile', new=Mock(return_value=True)):
       res = self.gaudi.setPythia8Card("pythia8card.cmd")
       assertDiracSucceeds(res, self)
       assertEqualsImproved(self.gaudi.pythia8CardContent, 'content', self)
 
+  def test_setPythia8CardEOS(self):
+    self.assertFalse(self.gaudi._errorDict)
+    with patch("builtins.open", mock_open(read_data='content')), \
+      patch("os.path.isfile", new=Mock(side_effect=[False, True])):
+      res = self.gaudi.setPythia8Card("p8_ee_tt_ecm365.cmd")
+      assertDiracSucceeds(res, self)
+      assertEqualsImproved(self.gaudi.pythia8CardContent, 'content', self)
+
   def test_setPythia8Card_fails_file(self):
     self.assertFalse(self.gaudi._errorDict)
     res = self.gaudi.setPythia8Card("content")
     assertDiracFailsWith(res, 'Pythia8 configuration file does not exist!', self)
 
   def test_setPythia8Card_fails_argument(self):
     self.assertFalse(self.gaudi._errorDict)
```

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/API/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Agent/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Client/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Service/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/OverlaySystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Calibration.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/CheckCollections.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     with open(scriptName, 'w') as scriptFile:
       scriptFile.write("\n".join(script))
 
     if os.path.exists(self.applicationLog):
       os.remove(self.applicationLog)
 
     if self.executableName == "DelphesPythia8_EDM4HEP":
-      res = preparePythia8Card(self.pythia8CardContent, self.NumberOfEvents, self.randomSeed, self.pythia8Card)
+      res = preparePythia8Card(self.pythia8CardContent, self.NumberOfEvents, self.randomSeed, self.energy, self.pythia8Card)
       if not res['OK']:
         return res
     
     os.chmod(scriptName, 0o755)
     comm = 'bash "./%s"' % scriptName
     self.setApplicationStatus('DelphesApp %s step %s' % (self.applicationVersion, self.STEP_NUMBER))
     self.stdError = ''
```

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DummyModule.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/DummyModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     with open(scriptName, 'w') as scriptFile:
       scriptFile.write("\n".join(script))
 
     if os.path.exists(self.applicationLog):
       os.remove(self.applicationLog)
 
     if self.pythia8CardContent:
-      res = preparePythia8Card(self.pythia8CardContent, self.NumberOfEvents, self.randomSeed, self.pythia8Card)
+      res = preparePythia8Card(self.pythia8CardContent, self.NumberOfEvents, self.randomSeed, self.energy, self.pythia8Card)
       if not res['OK']:
         return res
     
     os.chmod(scriptName, 0o755)
     comm = 'bash "./%s"' % scriptName
     self.setApplicationStatus('GaudiApp %s step %s' % (self.applicationVersion, self.STEP_NUMBER))
     self.stdError = ''
```

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ModuleBase.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/ModuleBase.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MoveInFC.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/MoveInFC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/OverlayInput.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ReportErrors.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/ReportErrors.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepCut.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/StdHepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Modules/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/RootMixin.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Utilities/RootMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/Workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/WorkloadManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/ILCDIRAC/__init__.py` & `iLCDirac-34.0.0a5/src/ILCDIRAC/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/iLCDirac.egg-info/PKG-INFO` & `iLCDirac-34.0.0a5/src/iLCDirac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iLCDirac
-Version: 34.0.0a4
+Version: 34.0.0a5
 Summary: iLCDirac is the iLC/CLIC/FCC extension of DIRAC
 Home-page: https://gitlab.cern.ch/clicdp/ilcdirac/ilcdirac.git
 Maintainer: Andre Sailer
 Maintainer-email: ilcdirac-support@cern.ch
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://its.cern.ch/jira/browse/ILCDIRAC
 Project-URL: Documentation, https://ilcdirac-doc.web.cern.ch/
```

### Comparing `iLCDirac-34.0.0a4/src/iLCDirac.egg-info/SOURCES.txt` & `iLCDirac-34.0.0a5/src/iLCDirac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a4/src/iLCDirac.egg-info/entry_points.txt` & `iLCDirac-34.0.0a5/src/iLCDirac.egg-info/entry_points.txt`

 * *Files identical despite different names*

