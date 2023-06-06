# Comparing `tmp/mippy-2.9.4.tar.gz` & `tmp/mippy-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mippy-2.9.4.tar", last modified: Thu Jan 23 16:24:24 2020, max compression
+gzip compressed data, was "dist/mippy-2.9.5.tar", last modified: Mon May 18 11:56:55 2020, max compression
```

## Comparing `mippy-2.9.4.tar` & `mippy-2.9.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-23 16:24:24.000000 mippy-2.9.4/
--rw-r--r--   0 root         (0) root         (0)      317 2020-01-23 16:24:24.000000 mippy-2.9.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1828 2020-01-23 16:24:05.000000 mippy-2.9.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy/
--rw-rw-rw-   0 root         (0) root         (0)      113 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    56795 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/application.py
--rw-rw-rw-   0 root         (0) root         (0)     5882 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/fileio.py
--rw-rw-rw-   0 root         (0) root         (0)     2941 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/html.py
--rw-rw-rw-   0 root         (0) root         (0)    10628 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/improcess.py
--rw-rw-rw-   0 root         (0) root         (0)     4258 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy/luts/
--rw-rw-rw-   0 root         (0) root         (0)     3351 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/16_colors.csv
--rw-rw-rw-   0 root         (0) root         (0)     2873 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/blue.csv
--rw-rw-rw-   0 root         (0) root         (0)     3274 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/colours_roman.csv
--rw-rw-rw-   0 root         (0) root         (0)     3275 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/cyan.csv
--rw-rw-rw-   0 root         (0) root         (0)     3460 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/fire.csv
--rw-rw-rw-   0 root         (0) root         (0)     2873 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/green.csv
--rw-rw-rw-   0 root         (0) root         (0)     3405 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/green_fire_blue.csv
--rw-rw-rw-   0 root         (0) root         (0)     3675 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/hi_lo.csv
--rw-rw-rw-   0 root         (0) root         (0)     3650 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/ice.csv
--rw-rw-rw-   0 root         (0) root         (0)     3275 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/magenta.csv
--rw-rw-rw-   0 root         (0) root         (0)     3723 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/phase.csv
--rw-rw-rw-   0 root         (0) root         (0)     3570 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/physics.csv
--rw-rw-rw-   0 root         (0) root         (0)     3395 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/rainbow.csv
--rw-rw-rw-   0 root         (0) root         (0)     2873 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/red.csv
--rw-rw-rw-   0 root         (0) root         (0)     2873 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/red_green.csv
--rw-rw-rw-   0 root         (0) root         (0)     3385 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/spectrum.csv
--rw-rw-rw-   0 root         (0) root         (0)     3275 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/luts/yellow.csv
--rw-rw-rw-   0 root         (0) root         (0)      137 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/math.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy/mdicom/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mdicom/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mdicom/anon.py
--rw-rw-rw-   0 root         (0) root         (0)    15025 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mdicom/io.py
--rw-rw-rw-   0 root         (0) root         (0)     4415 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mdicom/mrenhanced.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mdicom/mrspectroscopy.py
--rw-rw-rw-   0 root         (0) root         (0)    19667 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mdicom/pixel.py
--rw-rw-rw-   0 root         (0) root         (0)    21710 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mdicom/reading.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mdicom/siemens.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mdicom/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     1483 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1871 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mlogging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy/mviewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mviewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mviewer/config
--rw-rw-rw-   0 root         (0) root         (0)     6601 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/mviewer/module_main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy/resources/
--rw-rw-rw-   0 root         (0) root         (0)    51299 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/brain_bw.xbm
--rw-rw-rw-   0 root         (0) root         (0)    67646 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/brain_orange.ico
--rw-rw-rw-   0 root         (0) root         (0)  2485808 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/dcmdjpeg_linux
--rwxrwxrwx   0 root         (0) root         (0)  3547912 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/dcmdjpeg_mac
--rw-rw-rw-   0 root         (0) root         (0)  1343488 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/dcmdjpeg_win.exe
--rw-rw-rw-   0 root         (0) root         (0)      941 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/ellipse_roi.png
--rw-rw-rw-   0 root         (0) root         (0)      975 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/freehand_roi.png
--rw-rw-rw-   0 root         (0) root         (0)      580 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/line_roi.png
--rw-rw-rw-   0 root         (0) root         (0)     3223 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/mrs.png
--rw-rw-rw-   0 root         (0) root         (0)   115181 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/splash11.jpg
--rw-rw-rw-   0 root         (0) root         (0)   720054 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/splash20.bmp
--rw-rw-rw-   0 root         (0) root         (0)    61572 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/splash20.jpg
--rw-rw-rw-   0 root         (0) root         (0)    61572 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/splash3.jpg
--rw-rw-rw-   0 root         (0) root         (0)      578 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/resources/square_roi.png
--rw-rw-rw-   0 root         (0) root         (0)     1990 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/splash.py
--rw-rw-rw-   0 root         (0) root         (0)      878 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/threading.py
--rw-rw-rw-   0 root         (0) root         (0)   105200 2020-01-23 16:24:05.000000 mippy-2.9.4/mippy/viewing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      317 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1547 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2020-01-23 16:24:24.000000 mippy-2.9.4/mippy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-23 16:24:24.000000 mippy-2.9.4/scripts/
--rw-rw-rw-   0 root         (0) root         (0)       80 2020-01-23 16:24:05.000000 mippy-2.9.4/scripts/_mippy.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2020-01-23 16:24:05.000000 mippy-2.9.4/scripts/install_mippy.bat
--rw-rw-rw-   0 root         (0) root         (0)     2379 2020-01-23 16:24:05.000000 mippy-2.9.4/scripts/install_mippy.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2020-01-23 16:24:05.000000 mippy-2.9.4/scripts/mippy.bat
--rw-r--r--   0 root         (0) root         (0)       38 2020-01-23 16:24:24.000000 mippy-2.9.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2810 2020-01-23 16:24:05.000000 mippy-2.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-18 11:56:55.000000 mippy-2.9.5/
+-rw-r--r--   0 root         (0) root         (0)      317 2020-05-18 11:56:55.000000 mippy-2.9.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2020-05-18 11:56:38.000000 mippy-2.9.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    56795 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     5882 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/fileio.py
+-rw-rw-rw-   0 root         (0) root         (0)     2941 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/html.py
+-rw-rw-rw-   0 root         (0) root         (0)    10628 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/improcess.py
+-rw-rw-rw-   0 root         (0) root         (0)     4258 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy/luts/
+-rw-rw-rw-   0 root         (0) root         (0)     3351 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/16_colors.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2873 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/blue.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/colours_roman.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/cyan.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3460 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/fire.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2873 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/green.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3405 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/green_fire_blue.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/hi_lo.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3650 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/ice.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/magenta.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/phase.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3570 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/physics.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/rainbow.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2873 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/red.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2873 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/red_green.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3385 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/spectrum.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/luts/yellow.csv
+-rw-rw-rw-   0 root         (0) root         (0)      137 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/math.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy/mdicom/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mdicom/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mdicom/anon.py
+-rw-rw-rw-   0 root         (0) root         (0)    15025 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mdicom/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     4415 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mdicom/mrenhanced.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mdicom/mrspectroscopy.py
+-rw-rw-rw-   0 root         (0) root         (0)    19667 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mdicom/pixel.py
+-rw-rw-rw-   0 root         (0) root         (0)    22027 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mdicom/reading.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mdicom/siemens.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mdicom/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1871 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mlogging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy/mviewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mviewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mviewer/config
+-rw-rw-rw-   0 root         (0) root         (0)     6601 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/mviewer/module_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy/resources/
+-rw-rw-rw-   0 root         (0) root         (0)    51299 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/brain_bw.xbm
+-rw-rw-rw-   0 root         (0) root         (0)    67646 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/brain_orange.ico
+-rw-rw-rw-   0 root         (0) root         (0)  2485808 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/dcmdjpeg_linux
+-rwxrwxrwx   0 root         (0) root         (0)  3547912 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/dcmdjpeg_mac
+-rw-rw-rw-   0 root         (0) root         (0)  1343488 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/dcmdjpeg_win.exe
+-rw-rw-rw-   0 root         (0) root         (0)      941 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/ellipse_roi.png
+-rw-rw-rw-   0 root         (0) root         (0)      975 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/freehand_roi.png
+-rw-rw-rw-   0 root         (0) root         (0)      580 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/line_roi.png
+-rw-rw-rw-   0 root         (0) root         (0)     3223 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/mrs.png
+-rw-rw-rw-   0 root         (0) root         (0)   115181 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/splash11.jpg
+-rw-rw-rw-   0 root         (0) root         (0)   720054 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/splash20.bmp
+-rw-rw-rw-   0 root         (0) root         (0)    61572 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/splash20.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    61572 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/splash3.jpg
+-rw-rw-rw-   0 root         (0) root         (0)      578 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/resources/square_roi.png
+-rw-rw-rw-   0 root         (0) root         (0)     1990 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/splash.py
+-rw-rw-rw-   0 root         (0) root         (0)      878 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/threading.py
+-rw-rw-rw-   0 root         (0) root         (0)   105200 2020-05-18 11:56:38.000000 mippy-2.9.5/mippy/viewing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      317 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1547 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2020-05-18 11:56:55.000000 mippy-2.9.5/mippy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-18 11:56:55.000000 mippy-2.9.5/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2020-05-18 11:56:38.000000 mippy-2.9.5/scripts/_mippy.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2020-05-18 11:56:38.000000 mippy-2.9.5/scripts/install_mippy.bat
+-rw-rw-rw-   0 root         (0) root         (0)     2379 2020-05-18 11:56:38.000000 mippy-2.9.5/scripts/install_mippy.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2020-05-18 11:56:38.000000 mippy-2.9.5/scripts/mippy.bat
+-rw-r--r--   0 root         (0) root         (0)       38 2020-05-18 11:56:55.000000 mippy-2.9.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2810 2020-05-18 11:56:38.000000 mippy-2.9.5/setup.py
```

### Comparing `mippy-2.9.4/README.md` & `mippy-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/application.py` & `mippy-2.9.5/mippy/application.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/fileio.py` & `mippy-2.9.5/mippy/fileio.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/html.py` & `mippy-2.9.5/mippy/html.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/improcess.py` & `mippy-2.9.5/mippy/improcess.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/launcher.py` & `mippy-2.9.5/mippy/launcher.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/16_colors.csv` & `mippy-2.9.5/mippy/luts/16_colors.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/blue.csv` & `mippy-2.9.5/mippy/luts/blue.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/colours_roman.csv` & `mippy-2.9.5/mippy/luts/colours_roman.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/cyan.csv` & `mippy-2.9.5/mippy/luts/cyan.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/fire.csv` & `mippy-2.9.5/mippy/luts/fire.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/green.csv` & `mippy-2.9.5/mippy/luts/green.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/green_fire_blue.csv` & `mippy-2.9.5/mippy/luts/green_fire_blue.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/hi_lo.csv` & `mippy-2.9.5/mippy/luts/hi_lo.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/ice.csv` & `mippy-2.9.5/mippy/luts/ice.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/magenta.csv` & `mippy-2.9.5/mippy/luts/magenta.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/phase.csv` & `mippy-2.9.5/mippy/luts/phase.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/physics.csv` & `mippy-2.9.5/mippy/luts/physics.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/rainbow.csv` & `mippy-2.9.5/mippy/luts/rainbow.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/red.csv` & `mippy-2.9.5/mippy/luts/red.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/red_green.csv` & `mippy-2.9.5/mippy/luts/red_green.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/spectrum.csv` & `mippy-2.9.5/mippy/luts/spectrum.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/luts/yellow.csv` & `mippy-2.9.5/mippy/luts/yellow.csv`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/mdicom/io.py` & `mippy-2.9.5/mippy/mdicom/io.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/mdicom/mrenhanced.py` & `mippy-2.9.5/mippy/mdicom/mrenhanced.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/mdicom/pixel.py` & `mippy-2.9.5/mippy/mdicom/pixel.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/mdicom/reading.py` & `mippy-2.9.5/mippy/mdicom/reading.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,37 +336,39 @@
                                 'ACQUISITION TIME',
                                 'CONTENT TIME',
                                 'CREATION TIME',
                                 'PIXEL VALUE',
                                 'WINDOW',
                                 'CSA',                # Still don't really know what CSA is
                                 'PIXEL DATA',
-                                'PADDING']
+                                'PADDING',
+                                'PHOENIX',
+                                'PRIVATE TAG DATA']
         for element in ds1:
                 if any(s in element.name.upper() for s in exclude_list):
                         continue
                 val1 = element.value
                 try:
                         val2 = ds2[element.tag].value
                 except:
-                        diffs.append((name+str(element.name)+num,str(val1),'--MISSING--'))
+                        diffs.append((name+str(element.name)+num+' '+str(element.tag.group).zfill(4)+','+str(element.tag.element).zfill(4),str(val1),'--MISSING--'))
                         continue
                 if element.VR=="SQ":
                         for i in range(len(val1)):
                                 compare_dicom(val1[i],val2[i],diffs=diffs,num=i,name=str(element.name)+' >> ')
                         continue
                 if not val1==val2:
                         if not any(s in element.name.upper() for s in exclude_list):
-                                diffs.append((name+str(element.name)+num,str(val1),str(val2)))
+                                diffs.append((name+str(element.name)+num+' '+str(element.tag.group).zfill(4)+','+str(element.tag.element).zfill(4),str(val1),str(val2)))
         for element in ds2:
                 val2 = element.value
                 try:
                         val1 = ds1[element.tag].value
                 except:
-                        diffs.append((name+str(element.name)+num,'--MISSING--',str(val2)))
+                        diffs.append((name+str(element.name)+num+' '+str(element.tag.group).zfill(4)+','+str(element.tag.element).zfill(4),'--MISSING--',str(val2)))
                         continue
 
         return diffs
 
 def load_images_from_uids(list_of_tags,uids_to_match,tempdir,multiprocess=False):
         datasets_to_pass = []
         dcm_info = []
```

### Comparing `mippy-2.9.4/mippy/misc.py` & `mippy-2.9.5/mippy/misc.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/mlogging.py` & `mippy-2.9.5/mippy/mlogging.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/mviewer/module_main.py` & `mippy-2.9.5/mippy/mviewer/module_main.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/brain_bw.xbm` & `mippy-2.9.5/mippy/resources/brain_bw.xbm`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/brain_orange.ico` & `mippy-2.9.5/mippy/resources/brain_orange.ico`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/dcmdjpeg_linux` & `mippy-2.9.5/mippy/resources/dcmdjpeg_linux`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/dcmdjpeg_mac` & `mippy-2.9.5/mippy/resources/dcmdjpeg_mac`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/dcmdjpeg_win.exe` & `mippy-2.9.5/mippy/resources/dcmdjpeg_win.exe`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/ellipse_roi.png` & `mippy-2.9.5/mippy/resources/ellipse_roi.png`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/freehand_roi.png` & `mippy-2.9.5/mippy/resources/freehand_roi.png`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/line_roi.png` & `mippy-2.9.5/mippy/resources/line_roi.png`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/mrs.png` & `mippy-2.9.5/mippy/resources/mrs.png`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/splash11.jpg` & `mippy-2.9.5/mippy/resources/splash11.jpg`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/splash20.bmp` & `mippy-2.9.5/mippy/resources/splash20.bmp`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/splash20.jpg` & `mippy-2.9.5/mippy/resources/splash20.jpg`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/splash3.jpg` & `mippy-2.9.5/mippy/resources/splash3.jpg`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/resources/square_roi.png` & `mippy-2.9.5/mippy/resources/square_roi.png`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/splash.py` & `mippy-2.9.5/mippy/splash.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/threading.py` & `mippy-2.9.5/mippy/threading.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy/viewing.py` & `mippy-2.9.5/mippy/viewing.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/mippy.egg-info/SOURCES.txt` & `mippy-2.9.5/mippy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/scripts/install_mippy.py` & `mippy-2.9.5/scripts/install_mippy.py`

 * *Files identical despite different names*

### Comparing `mippy-2.9.4/setup.py` & `mippy-2.9.5/setup.py`

 * *Files identical despite different names*

