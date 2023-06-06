# Comparing `tmp/oda_api-1.1.8.tar.gz` & `tmp/oda_api-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oda_api-1.1.8.tar", last modified: Mon May 10 09:30:43 2021, max compression
+gzip compressed data, was "dist/oda_api-1.1.9.tar", last modified: Thu May 20 09:32:51 2021, max compression
```

## Comparing `oda_api-1.1.8.tar` & `oda_api-1.1.9.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.465108 oda_api-1.1.8/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       50 2021-02-17 11:00:26.000000 oda_api-1.1.8/.gitattributes
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.453108 oda_api-1.1.8/.github/
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.453108 oda_api-1.1.8/.github/styles/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       64 2021-04-13 06:45:56.000000 oda_api-1.1.8/.github/styles/vocab.txt
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.453108 oda_api-1.1.8/.github/workflows/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1591 2021-04-26 15:02:34.000000 oda_api-1.1.8/.github/workflows/ci.yml
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      653 2021-04-13 06:45:56.000000 oda_api-1.1.8/.github/workflows/prose.yml
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1839 2021-04-13 06:45:56.000000 oda_api-1.1.8/.github/workflows/python-package.yml
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      621 2021-02-17 11:00:26.000000 oda_api-1.1.8/.github/workflows/python-publish.yml
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      408 2021-04-13 06:45:56.000000 oda_api-1.1.8/.gitignore
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       89 2021-04-13 06:45:56.000000 oda_api-1.1.8/.vale.ini
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      189 2021-02-17 11:00:26.000000 oda_api-1.1.8/CL.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      396 2021-02-17 11:00:26.000000 oda_api-1.1.8/Dockerfile
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2832 2021-02-17 11:00:26.000000 oda_api-1.1.8/Dockerfile_oginal
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1172 2021-02-17 11:00:26.000000 oda_api-1.1.8/LICENSE.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       98 2021-02-17 11:00:26.000000 oda_api-1.1.8/MANIFEST.in
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      278 2021-05-10 09:30:43.465108 oda_api-1.1.8/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1693 2021-03-09 14:54:59.000000 oda_api-1.1.8/README.md
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.453108 oda_api-1.1.8/doc/
--rwxrwxr-x   0 savchenk  (1000) savchenk  (1000)       46 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/CL.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      584 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/Makefile
--rwxrwxr-x   0 savchenk  (1000) savchenk  (1000)     1844 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/make_apidoc_and_uml_graphs.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       69 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/requirements.txt
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.453108 oda_api-1.1.8/doc/source/
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.453108 oda_api-1.1.8/doc/source/_templates/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      464 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/_templates/my_side_bar.html
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.457108 oda_api-1.1.8/doc/source/api/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       28 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/api.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       38 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/data_products.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      204 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/modules.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      929 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.api.DispatcherAPI.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      130 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.api.NoTraceBackWithLineNumber.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      100 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.api.RemoteException.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       94 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.api.Request.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      281 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.data_products.ApiCatalog.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      308 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.data_products.BinaryData.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      837 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.data_products.NumpyDataProduct.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      531 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.data_products.NumpyDataUnit.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      109 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.data_products._chekc_enc_data.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      112 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.data_products.sanitize_encoded.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      291 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.plot_tools.OdaImage.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      262 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/oda_api.plot_tools.OdaLightCurve.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       35 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/api/plot_tools.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     9501 2021-04-13 06:46:02.000000 oda_api-1.1.8/doc/source/conf.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      677 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/index.rst
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      382 2021-04-13 06:45:56.000000 oda_api-1.1.8/doc/source/install.rst
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.457108 oda_api-1.1.8/doc/source/user_guide/
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.457108 oda_api-1.1.8/doc/source/user_guide/.ipynb_checkpoints/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)   515387 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/.ipynb_checkpoints/TestAPI-checkpoint.ipynb
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    15927 2021-04-13 06:45:56.000000 oda_api-1.1.8/doc/source/user_guide/AsynchronousAPI.ipynb
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)   472859 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI.ipynb
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    73764 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI.rst
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.461108 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    88816 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_36_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    88815 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_37_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     6956 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_47_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     6950 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_48_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8299 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_55_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8283 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_56_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    13763 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_64_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    13763 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_65_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    13751 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_66_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8698 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_82_2.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8698 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_83_2.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10731 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_84_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10731 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_85_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12046 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_85_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12046 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_85_2.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12024 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_86_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12024 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_86_2.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10731 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_87_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12001 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_88_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12001 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_88_2.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    63100 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_89_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    63100 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_89_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8692 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_89_2.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    64004 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_90_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10734 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_90_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10698 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_91_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10506 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_91_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10506 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_91_2.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12002 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_92_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12002 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_92_2.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    57256 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_93_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    57256 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_93_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10634 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_94_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10634 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_94_2.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    46123 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_96_0.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    46123 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_96_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     9716 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_97_1.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     9716 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_97_2.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5354 2021-02-17 11:00:26.000000 oda_api-1.1.8/doc/source/user_guide/tutorial_main.rst
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.465108 oda_api-1.1.8/oda_api/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      878 2021-02-17 11:00:26.000000 oda_api-1.1.8/oda_api/__init__.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    33865 2021-05-06 13:36:10.000000 oda_api-1.1.8/oda_api/api.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1852 2021-04-13 06:45:56.000000 oda_api-1.1.8/oda_api/cli.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      361 2021-02-17 11:00:26.000000 oda_api-1.1.8/oda_api/colors.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1109 2021-05-06 14:00:03.000000 oda_api-1.1.8/oda_api/custom_formatters.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    16618 2021-05-02 08:50:14.000000 oda_api-1.1.8/oda_api/data_products.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       21 2021-05-10 09:30:39.000000 oda_api-1.1.8/oda_api/pkg_info.json
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2187 2021-02-17 11:00:26.000000 oda_api-1.1.8/oda_api/plot_tools.py
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.465108 oda_api-1.1.8/oda_api.egg-info/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      278 2021-05-10 09:30:43.000000 oda_api-1.1.8/oda_api.egg-info/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3848 2021-05-10 09:30:43.000000 oda_api-1.1.8/oda_api.egg-info/SOURCES.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2021-05-10 09:30:43.000000 oda_api-1.1.8/oda_api.egg-info/dependency_links.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       46 2021-05-10 09:30:43.000000 oda_api-1.1.8/oda_api.egg-info/entry_points.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       69 2021-05-10 09:30:43.000000 oda_api-1.1.8/oda_api.egg-info/requires.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        8 2021-05-10 09:30:43.000000 oda_api-1.1.8/oda_api.egg-info/top_level.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       99 2021-05-06 13:30:39.000000 oda_api-1.1.8/pytest.ini
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      125 2021-05-10 09:13:31.000000 oda_api-1.1.8/requirements.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       70 2021-02-17 11:00:26.000000 oda_api-1.1.8/requirements_docker.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      433 2021-05-10 09:30:43.465108 oda_api-1.1.8/setup.cfg
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1318 2021-05-10 09:14:06.000000 oda_api-1.1.8/setup.py
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-10 09:30:43.465108 oda_api-1.1.8/tests/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     6272 2021-05-06 13:30:39.000000 oda_api-1.1.8/tests/test_live.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.398554 oda_api-1.1.9/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       50 2021-02-17 11:00:26.000000 oda_api-1.1.9/.gitattributes
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.370554 oda_api-1.1.9/.github/
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.374554 oda_api-1.1.9/.github/styles/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       64 2021-04-13 06:45:56.000000 oda_api-1.1.9/.github/styles/vocab.txt
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.374554 oda_api-1.1.9/.github/workflows/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1591 2021-04-26 15:02:34.000000 oda_api-1.1.9/.github/workflows/ci.yml
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      653 2021-04-13 06:45:56.000000 oda_api-1.1.9/.github/workflows/prose.yml
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1851 2021-05-20 09:29:07.000000 oda_api-1.1.9/.github/workflows/python-package.yml
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      621 2021-02-17 11:00:26.000000 oda_api-1.1.9/.github/workflows/python-publish.yml
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      448 2021-05-20 09:22:59.000000 oda_api-1.1.9/.gitignore
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       89 2021-04-13 06:45:56.000000 oda_api-1.1.9/.vale.ini
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      189 2021-02-17 11:00:26.000000 oda_api-1.1.9/CL.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      396 2021-02-17 11:00:26.000000 oda_api-1.1.9/Dockerfile
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2832 2021-02-17 11:00:26.000000 oda_api-1.1.9/Dockerfile_oginal
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1172 2021-02-17 11:00:26.000000 oda_api-1.1.9/LICENSE.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       98 2021-02-17 11:00:26.000000 oda_api-1.1.9/MANIFEST.in
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      278 2021-05-20 09:32:51.402554 oda_api-1.1.9/PKG-INFO
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1693 2021-03-09 14:54:59.000000 oda_api-1.1.9/README.md
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.374554 oda_api-1.1.9/doc/
+-rwxrwxr-x   0 savchenk  (1000) savchenk  (1000)       46 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/CL.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      584 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/Makefile
+-rwxrwxr-x   0 savchenk  (1000) savchenk  (1000)     1844 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/make_apidoc_and_uml_graphs.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       69 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/requirements.txt
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.374554 oda_api-1.1.9/doc/source/
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.374554 oda_api-1.1.9/doc/source/_templates/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      464 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/_templates/my_side_bar.html
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.378554 oda_api-1.1.9/doc/source/api/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       28 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/api.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       38 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/data_products.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      204 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/modules.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      929 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.api.DispatcherAPI.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      130 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.api.NoTraceBackWithLineNumber.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      100 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.api.RemoteException.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       94 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.api.Request.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      281 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.data_products.ApiCatalog.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      308 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.data_products.BinaryData.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      837 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.data_products.NumpyDataProduct.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      531 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.data_products.NumpyDataUnit.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      109 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.data_products._chekc_enc_data.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      112 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.data_products.sanitize_encoded.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      291 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.plot_tools.OdaImage.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      262 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/oda_api.plot_tools.OdaLightCurve.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       35 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/api/plot_tools.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     9501 2021-04-13 06:46:02.000000 oda_api-1.1.9/doc/source/conf.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      677 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/index.rst
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      382 2021-04-13 06:45:56.000000 oda_api-1.1.9/doc/source/install.rst
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.382554 oda_api-1.1.9/doc/source/user_guide/
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.382554 oda_api-1.1.9/doc/source/user_guide/.ipynb_checkpoints/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)   515387 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/.ipynb_checkpoints/TestAPI-checkpoint.ipynb
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    15927 2021-04-13 06:45:56.000000 oda_api-1.1.9/doc/source/user_guide/AsynchronousAPI.ipynb
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)   472859 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI.ipynb
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    73764 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI.rst
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.398554 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    88816 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_36_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    88815 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_37_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     6956 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_47_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     6950 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_48_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8299 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_55_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8283 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_56_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    13763 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_64_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    13763 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_65_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    13751 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_66_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8698 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_82_2.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8698 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_83_2.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10731 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_84_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10731 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_85_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12046 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_85_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12046 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_85_2.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12024 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_86_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12024 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_86_2.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10731 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_87_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12001 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_88_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12001 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_88_2.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    63100 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_89_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    63100 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_89_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8692 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_89_2.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    64004 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_90_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10734 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_90_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10698 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_91_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10506 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_91_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10506 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_91_2.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12002 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_92_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12002 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_92_2.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    57256 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_93_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    57256 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_93_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10634 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_94_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10634 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_94_2.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    46123 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_96_0.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    46123 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_96_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     9716 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_97_1.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     9716 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_97_2.png
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5354 2021-02-17 11:00:26.000000 oda_api-1.1.9/doc/source/user_guide/tutorial_main.rst
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.398554 oda_api-1.1.9/oda_api/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      878 2021-02-17 11:00:26.000000 oda_api-1.1.9/oda_api/__init__.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    34970 2021-05-20 09:08:09.000000 oda_api-1.1.9/oda_api/api.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1852 2021-04-13 06:45:56.000000 oda_api-1.1.9/oda_api/cli.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      361 2021-02-17 11:00:26.000000 oda_api-1.1.9/oda_api/colors.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1109 2021-05-06 14:00:03.000000 oda_api-1.1.9/oda_api/custom_formatters.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    17105 2021-05-20 05:46:51.000000 oda_api-1.1.9/oda_api/data_products.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       21 2021-05-20 09:32:48.000000 oda_api-1.1.9/oda_api/pkg_info.json
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2187 2021-02-17 11:00:26.000000 oda_api-1.1.9/oda_api/plot_tools.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.398554 oda_api-1.1.9/oda_api.egg-info/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      278 2021-05-20 09:32:51.000000 oda_api-1.1.9/oda_api.egg-info/PKG-INFO
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3866 2021-05-20 09:32:51.000000 oda_api-1.1.9/oda_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2021-05-20 09:32:51.000000 oda_api-1.1.9/oda_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       46 2021-05-20 09:32:51.000000 oda_api-1.1.9/oda_api.egg-info/entry_points.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       69 2021-05-20 09:32:51.000000 oda_api-1.1.9/oda_api.egg-info/requires.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        8 2021-05-20 09:32:51.000000 oda_api-1.1.9/oda_api.egg-info/top_level.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      120 2021-05-20 09:15:25.000000 oda_api-1.1.9/pytest.ini
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      214 2021-05-20 09:26:11.000000 oda_api-1.1.9/requirements.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       70 2021-02-17 11:00:26.000000 oda_api-1.1.9/requirements_docker.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      433 2021-05-20 09:32:51.402554 oda_api-1.1.9/setup.cfg
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1318 2021-05-20 09:26:20.000000 oda_api-1.1.9/setup.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-05-20 09:32:51.398554 oda_api-1.1.9/tests/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      194 2021-05-03 06:48:14.000000 oda_api-1.1.9/tests/conftest.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     8082 2021-05-20 09:21:33.000000 oda_api-1.1.9/tests/test_live.py
```

### Comparing `oda_api-1.1.8/.github/workflows/ci.yml` & `oda_api-1.1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/.github/workflows/prose.yml` & `oda_api-1.1.9/.github/workflows/prose.yml`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/.github/workflows/python-package.yml` & `oda_api-1.1.9/.github/workflows/python-package.yml`

 * *Files 17% similar despite different names*

```diff
@@ -30,17 +30,17 @@
         python -m pip install flake8 pytest wheel coverage pylint mypy
         python -m pip install oda-knowledge-base[rdf,cwl]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
 
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
-        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
+        flake8 oda_api --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-        flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+        flake8 oda_api --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
 
     - name: PyLint - more lint
       run: |
         pylint -E oda_api
 
     - name: MyPy
       run: |
```

### Comparing `oda_api-1.1.8/.github/workflows/python-publish.yml` & `oda_api-1.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/Dockerfile_oginal` & `oda_api-1.1.9/Dockerfile_oginal`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/LICENSE.rst` & `oda_api-1.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/README.md` & `oda_api-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/Makefile` & `oda_api-1.1.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/make_apidoc_and_uml_graphs.py` & `oda_api-1.1.9/doc/make_apidoc_and_uml_graphs.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/api/oda_api.api.DispatcherAPI.rst` & `oda_api-1.1.9/doc/source/api/oda_api.api.DispatcherAPI.rst`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/api/oda_api.data_products.NumpyDataProduct.rst` & `oda_api-1.1.9/doc/source/api/oda_api.data_products.NumpyDataProduct.rst`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/api/oda_api.data_products.NumpyDataUnit.rst` & `oda_api-1.1.9/doc/source/api/oda_api.data_products.NumpyDataUnit.rst`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/conf.py` & `oda_api-1.1.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/index.rst` & `oda_api-1.1.9/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/.ipynb_checkpoints/TestAPI-checkpoint.ipynb` & `oda_api-1.1.9/doc/source/user_guide/.ipynb_checkpoints/TestAPI-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/AsynchronousAPI.ipynb` & `oda_api-1.1.9/doc/source/user_guide/AsynchronousAPI.ipynb`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI.ipynb` & `oda_api-1.1.9/doc/source/user_guide/TestAPI.ipynb`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI.rst` & `oda_api-1.1.9/doc/source/user_guide/TestAPI.rst`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_36_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_36_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_37_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_37_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_47_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_47_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_48_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_48_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_55_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_55_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_56_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_56_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_64_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_64_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_65_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_65_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_66_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_66_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_82_2.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_82_2.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_83_2.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_83_2.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_84_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_84_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_85_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_85_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_85_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_85_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_85_2.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_85_2.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_86_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_86_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_86_2.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_86_2.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_87_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_87_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_88_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_88_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_88_2.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_88_2.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_89_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_89_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_89_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_89_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_89_2.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_89_2.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_90_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_90_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_90_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_90_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_91_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_91_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_91_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_91_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_91_2.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_91_2.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_92_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_92_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_92_2.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_92_2.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_93_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_93_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_93_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_93_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_94_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_94_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_94_2.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_94_2.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_96_0.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_96_0.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_96_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_96_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_97_1.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_97_1.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/TestAPI_files/TestAPI_97_2.png` & `oda_api-1.1.9/doc/source/user_guide/TestAPI_files/TestAPI_97_2.png`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/doc/source/user_guide/tutorial_main.rst` & `oda_api-1.1.9/doc/source/user_guide/tutorial_main.rst`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/oda_api/__init__.py` & `oda_api-1.1.9/oda_api/__init__.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/oda_api/api.py` & `oda_api-1.1.9/oda_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,44 +267,48 @@
         if v in allowed_request_methods:
             self._preferred_request_method = v
         else:
             raise RuntimeError(f'unable to set preferred request method to {v}, allowed {allowed_request_methods}')
 
     @property
     def selected_request_method(self):
-        request_size = len(json.dumps(self.parameters_dict_payload))
-        max_get_method_size = getattr(self, 'max_get_method_size', 1000)
-        if request_size > max_get_method_size:
-            self.logger.warning(
-                'switching to POST request due to large payload: %s > %s', request_size, max_get_method_size)
-            return 'POST'
+        if self.parameters_dict_payload is not None:
+            request_size = len(json.dumps(self.parameters_dict_payload))
+            max_get_method_size = getattr(self, 'max_get_method_size', 1000)
+
+            self.logger.debug('payload size %s, max for GET is %s', request_size, max_get_method_size)
+
+            if request_size > max_get_method_size:
+                self.logger.warning(
+                    'switching to POST request due to large payload: %s > %s', request_size, max_get_method_size)
+                return 'POST'
 
         return self.preferred_request_method
 
     def request_to_json(self, verbose=False):
         self.progress_logger.info(
             f'- waiting for remote response (since {time.strftime("%Y-%m-%d %H:%M:%S")}), please wait for {self.url}/{self.run_analysis_handle}')
 
         try:
             timeout = getattr(self, 'timeout', 120)
 
             self.last_request_t0 = time.time()
 
-            if self.preferred_request_method == 'GET':
+            if self.selected_request_method == 'GET':
                 response = requests.get(
                     "%s/%s" % (self.url, self.run_analysis_handle),
                     params=self.parameters_dict_payload,
                     cookies=self.cookies,
                     headers={
                         'Request-Timeout': str(timeout),
                         'Connection-Timeout': str(timeout),
                     },
                     timeout=timeout,
                 )
-            elif self.preferred_request_method == 'POST':
+            elif self.selected_request_method == 'POST':
                 response = requests.post(
                     "%s/%s" % (self.url, self.run_analysis_handle),
                     data=self.parameters_dict_payload,
                     cookies=self.cookies,
                     headers={
                         'Request-Timeout': str(timeout),
                         'Connection-Timeout': str(timeout),
@@ -321,36 +325,56 @@
             self.last_request_t_complete = time.time()
 
             self.note_request_time()
 
             response_json = self._decode_res_json(response)
 
             validate_json(response_json, self.dispatcher_response_schema)
+            
+            self.returned_analysis_parameters = response_json['products'].get('analysis_parameters', None)
 
             return response_json
         except json.decoder.JSONDecodeError as e:
             self.logger.error(
                 f"{C.RED}{C.BOLD}unable to decode json from response:{C.NC}")
             self.logger.error(f"{C.RED}{response.text}{C.NC}")
             raise
 
+    def returned_analysis_parameters_consistency(self):    
+        mismatching_parameters = []
+        for k in self.parameters_dict.keys():
+            # these do not correspond to meaning
+            if k in ['query_status', 'off_line', 'verbose', 'dry_run']:                
+                continue
+
+            returned = self.returned_analysis_parameters.get(k, None)
+            requested = self.parameters_dict.get(k, None)
+            if str(returned) != str(requested):
+                mismatching_parameters.append(f"{k}: returned {returned} != requested {requested}")
+
+        if mismatching_parameters != []:
+            raise RuntimeError(f"dispatcher return different parameters: {'; '.join(mismatching_parameters)}")
+    
     @property
     def parameters_dict(self):
         """
         as provided in request, not modified by state changes
         """
         return getattr(self, '_parameters_dict', None)
 
     @parameters_dict.setter
     def parameters_dict(self, value):
         self._parameters_dict = value
         self.query_status = 'prepared'
 
     @property
     def parameters_dict_payload(self):
+        if self.parameters_dict is None:
+            return None
+
         p = {
             **self.parameters_dict,
             'api': 'True',
             'oda_api_version': __version__,
         }
 
         if self.is_submitted:
```

### Comparing `oda_api-1.1.8/oda_api/cli.py` & `oda_api-1.1.9/oda_api/cli.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/oda_api/custom_formatters.py` & `oda_api-1.1.9/oda_api/custom_formatters.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/oda_api/data_products.py` & `oda_api-1.1.9/oda_api/data_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,15 +362,15 @@
                 gzip_file = gzip.GzipFile(fileobj=in_file, mode='rb')
                 _data = gzip_file.read()
                 _data = _data.decode('utf-8')
                 _data = pickle.loads(_data)
                 gzip_file.close()
             else:
                 if version_info[0] > 2:
-                    _data=pickle.loads(_binarys,encoding='bytes')
+                    _data = pickle.loads(_binarys,encoding='bytes')
                 else:
                     _data = pickle.loads(_binarys)
 
         elif encoded_data is not None:
             #print('using JsonCustomEncoder')
             encoded_data=eval(encoded_data)
 
@@ -411,26 +411,33 @@
     def show_meta(self):
         print('------------------------------')
         for k,v in self.meta_data.items():
             print(k,':',v)
         print ('------------------------------')
 
 
-    def get_data_unit(self,ID   ):
-        return self.data_unit[ID]
+    def get_data_unit(self, ID):
+        try:
+            return self.data_unit[ID]
+        except IndexError as e:
+            raise RuntimeError(f"problem get_data_unit ID:{ID} in self.data_unit:{self.data_unit}")
 
     def get_data_unit_by_name(self,name):
         _du=None
+
         for du in self.data_unit:
             if du.name == name:
-
-                _du=du
+                if _du is not None:
+                    print(f"\033[31mWARNING: get_data_unit_by_name found multiple du for name {name}\033[0m")
+                _du = du
             print('--> NAME',du.name)
 
-        #TODO raise RuntimeError if _du is None
+        if _du is None:
+            found_names = '; '.join([ str(_du.name) + ":" + repr(du) for _du in self.data_unit ])
+            print(f"\033[31mWARNING: get_data_unit_by_name found no du for name {name}, have {found_names}\033[0m")
 
         return _du
 
     def _seta_data(self,data):
         if type(data) == list:
             _dl = data
         else:
```

### Comparing `oda_api-1.1.8/oda_api/plot_tools.py` & `oda_api-1.1.9/oda_api/plot_tools.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/oda_api.egg-info/SOURCES.txt` & `oda_api-1.1.9/oda_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -94,8 +94,9 @@
 oda_api/plot_tools.py
 oda_api.egg-info/PKG-INFO
 oda_api.egg-info/SOURCES.txt
 oda_api.egg-info/dependency_links.txt
 oda_api.egg-info/entry_points.txt
 oda_api.egg-info/requires.txt
 oda_api.egg-info/top_level.txt
+tests/conftest.py
 tests/test_live.py
```

### Comparing `oda_api-1.1.8/setup.py` & `oda_api-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.1.8/tests/test_live.py` & `oda_api-1.1.9/tests/test_live.py`

 * *Files 18% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             print("this raised something else", e)
             raise
     else:
         yield
 
 
 @pytest.mark.slow
-@pytest.mark.parametrize("platform", ["staging-1-3", "staging-1-2", "production-1-2"])
+@pytest.mark.parametrize("platform", ["staging", "staging-1-2", "production-1-2"])
 @pytest.mark.parametrize("scw_kind", ["crab", "any", "failing"])
 def test_waiting(scw_kind, platform):
     from oda_api.api import UserError, FailedToFindAnyUsefulResults
 
     disp = get_disp(wait=True, platform=platform)
 
     with pytest.raises(UserError):
@@ -127,15 +127,15 @@
 
         print(data._n_list)
 
         validate_data(data, scw_kind)
 
 
 @pytest.mark.slow
-@pytest.mark.parametrize("platform", ["staging-1-3", "staging-1-2", "production-1-2"])
+@pytest.mark.parametrize("platform", ["staging", "staging-1-2", "production-1-2"])
 @pytest.mark.parametrize("scw_kind", ["crab", "any", "failing"])
 def test_not_waiting(scw_kind, platform):
     from oda_api.api import DispatcherAPI, UserError, FailedToFindAnyUsefulResults
 
     disp = get_disp(wait=False, platform=platform)
     disp2 = get_disp(wait=False, platform=platform)
 
@@ -199,24 +199,78 @@
             time.sleep(2)
 
         validate_data(data, scw_kind)
         validate_data(data2, scw_kind)
 
 
 @pytest.mark.slow
-@pytest.mark.parametrize("platform", ["staging-1-3", "staging-1-2", "production-1-2"])
+@pytest.mark.parametrize("platform", ["staging", "staging-1-2", "production-1-2"])
 def test_large_request(platform):
-    disp = get_disp(wait=False, platform=platform)
-
-    'isgri' in disp.get_instruments_list()
 
-    disp.preferred_request_method = 'POST'
-
-    product = disp.get_product(
+    dummy_request_parameters = dict(
         instrument="isgri",
         product="isgri_image",
         product_type="Dummy",
         osa_version="OSA10.2",
         E1_keV=40.0,
         E2_keV=200.0,
-        scw_list=[f"0665{i:04d}0010.001" for i in range(200)],
+        scw_list="066500550010.001"*300,
+        # this needs role
+        #scw_list=[f"0665{i:04d}0010.001" for i in range(200)],
+    )
+
+
+    disp = get_disp(wait=True, platform=platform)
+
+    'isgri' in disp.get_instruments_list()
+
+    assert disp.preferred_request_method == "GET"
+    assert disp.selected_request_method == "GET"
+
+    product = disp.get_product(
+        **dummy_request_parameters
+    )
+    disp.returned_analysis_parameters_consistency()
+
+    assert disp.preferred_request_method == "GET"
+    assert disp.selected_request_method == "POST"
+
+    product = disp.get_product(
+        **{            
+            **dummy_request_parameters,
+            'scw_list': "066500550010.001"
+        }
     )
+    disp.returned_analysis_parameters_consistency()
+
+    assert disp.preferred_request_method == "GET"
+    assert disp.selected_request_method == "GET"
+
+
+@pytest.mark.slow
+@pytest.mark.parametrize("platform", ["staging", "staging-1-2", "production-1-2"])
+def test_peculiar_request_causing_pickling_problem(platform):
+    import logging
+    logging.basicConfig(level='DEBUG')
+    logging.getLogger('oda_api').setLevel('DEBUG')
+    logging.getLogger('oda_api.api').setLevel('DEBUG')
+
+
+    import oda_api.api
+    disp = oda_api.api.DispatcherAPI(url="http://dispatcher.staging.internal.odahub.io")
+    print(disp.get_instruments_list())
+
+    disp.get_product(
+        'isgri_image',
+        scw_list='193200210010.001,193300510010.001,193400100010.001,193600090010.001,193600150010.001,193800020010.001,193900120010.001,193900160010.001,194000130010.001,194100100010.001,194100130010.001,194300090010.001,194400490010.001,194500020010.001,194500100010.001,194800270010.001,194800310010.001,194900080010.001,194900110010.001,195000330010.001',
+        E1_keV='28.0',
+        E2_keV='80.0',
+        osa_version='OSA11.0',
+        RA='275.0914266666666',
+        DEC='7.185355',
+        detection_threshold=7.0,
+        instrument='isgri',
+        query_type='Real',
+        session_id='EV49GW1UN9427QD9',
+     )
+
+
```

