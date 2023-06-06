# Comparing `tmp/pyarmor-8.2.dev1.zip` & `tmp/pyarmor-8.2.dev2.zip`

## zipinfo {}

```diff
@@ -1,139 +1,139 @@
-Zip file size: 2309199 bytes, number of entries: 137
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/
--rw-r--r--  2.0 unx     3004 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/PKG-INFO
--rwxr-xr-x  2.0 unx      191 b- defN 23-Mar-04 11:58 pyarmor-8.2.dev1/MANIFEST.in
--rw-r--r--  2.0 unx     6692 b- defN 23-Apr-20 10:36 pyarmor-8.2.dev1/README.md
--rw-r--r--  2.0 unx     4296 b- defN 23-Apr-28 08:42 pyarmor-8.2.dev1/setup.py
--rw-r--r--  2.0 unx       38 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/setup.cfg
--rw-r--r--  2.0 unx     3004 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     2911 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      135 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/requires.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/dependency_links.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/plugins/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/cli/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/polyfills/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/helper/
--rw-r--r--  2.0 unx      234 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/pyshield.lic
--rwxr-xr-x  2.0 unx     2038 b- defN 23-Apr-28 08:40 pyarmor-8.2.dev1/src/config.py
--rwxr-xr-x  2.0 unx    10197 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/benchmark.py
--rw-r--r--  2.0 unx     7265 b- defN 22-Feb-25 10:48 pyarmor-8.2.dev1/src/register.py
--rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/product.key
--rwxr-xr-x  2.0 unx    65827 b- defN 23-Mar-26 00:20 pyarmor-8.2.dev1/src/pyarmor.py
--rw-r--r--  2.0 unx     2664 b- defN 22-Jan-29 09:20 pyarmor-8.2.dev1/src/protect_code.pt
--rw-r--r--  2.0 unx    13587 b- defN 21-Nov-02 17:34 pyarmor-8.2.dev1/src/pytransform.py
--rw-r--r--  2.0 unx     3363 b- defN 22-Jun-27 00:08 pyarmor-8.2.dev1/src/sppmode.py
--rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/public.key
--rwxr-xr-x  2.0 unx      113 b- defN 20-Jan-02 11:09 pyarmor-8.2.dev1/src/__init__.py
--rw-r--r--  2.0 unx     2191 b- defN 22-Dec-04 19:13 pyarmor-8.2.dev1/src/reform.py
--rwxr-xr-x  2.0 unx    25832 b- defN 22-Nov-20 13:42 pyarmor-8.2.dev1/src/packer.py
--rw-r--r--  2.0 unx     5200 b- defN 23-Jan-06 00:02 pyarmor-8.2.dev1/src/cobuilder.py
--rwxr-xr-x  2.0 unx    67431 b- defN 22-Dec-23 17:42 pyarmor-8.2.dev1/src/utils.py
--rw-r--r--  2.0 unx       37 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/pyarmor-webui.py
--rw-r--r--  2.0 unx     4028 b- defN 21-Dec-16 08:28 pyarmor-8.2.dev1/src/build_meta.py
--rw-r--r--  2.0 unx      256 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/license.tri
--rw-r--r--  2.0 unx     1598 b- defN 23-Mar-04 17:07 pyarmor-8.2.dev1/src/README.rst
--rw-r--r--  2.0 unx     1596 b- defN 22-Jan-30 11:51 pyarmor-8.2.dev1/src/protect_code2.pt
--rw-r--r--  2.0 unx     2487 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/public_capsule.zip
--rwxr-xr-x  2.0 unx     8023 b- defN 22-Jun-28 09:01 pyarmor-8.2.dev1/src/project.py
--rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/pyshield.key
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/linux/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/darwin/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/windows/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/linux/x86/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/linux/x86_64/
--rwxr-xr-x  2.0 unx  1421600 b- defN 22-Sep-28 20:59 pyarmor-8.2.dev1/src/platforms/linux/x86/_pytransform.so
--rwxr-xr-x  2.0 unx  1198080 b- defN 22-Sep-28 20:59 pyarmor-8.2.dev1/src/platforms/linux/x86_64/_pytransform.so
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/darwin/x86_64/
--rwxr-xr-x  2.0 unx  1469620 b- defN 22-Sep-28 18:28 pyarmor-8.2.dev1/src/platforms/darwin/x86_64/_pytransform.dylib
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/windows/x86/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/windows/x86_64/
--rw-r--r--  2.0 unx  1373710 b- defN 22-Sep-28 21:00 pyarmor-8.2.dev1/src/platforms/windows/x86/_pytransform.dll
--rwxr-xr-x  2.0 unx  1165824 b- defN 22-Sep-28 20:59 pyarmor-8.2.dev1/src/platforms/windows/x86_64/_pytransform.dll
--rw-r--r--  2.0 unx     6360 b- defN 22-Jul-14 19:38 pyarmor-8.2.dev1/src/plugins/README.md
--rw-r--r--  2.0 unx    13688 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/plugins/check_ntp_time.py
--rw-r--r--  2.0 unx    10694 b- defN 23-Apr-20 15:01 pyarmor-8.2.dev1/src/cli/config.py
--rw-r--r--  2.0 unx    17413 b- defN 23-Apr-29 08:43 pyarmor-8.2.dev1/src/cli/register.py
--rw-r--r--  2.0 unx     5553 b- defN 23-Apr-22 08:21 pyarmor-8.2.dev1/src/cli/generate.py
--rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 22:43 pyarmor-8.2.dev1/src/cli/shell.py
--rw-r--r--  2.0 unx     6398 b- defN 23-Apr-13 14:46 pyarmor-8.2.dev1/src/cli/resource.py
--rw-r--r--  2.0 unx     1479 b- defN 23-Apr-25 09:18 pyarmor-8.2.dev1/src/cli/__init__.py
--rw-r--r--  2.0 unx    17255 b- defN 23-Apr-29 06:34 pyarmor-8.2.dev1/src/cli/context.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Apr-22 22:15 pyarmor-8.2.dev1/src/cli/plugin.py
--rw-r--r--  2.0 unx     3956 b- defN 23-Apr-20 15:02 pyarmor-8.2.dev1/src/cli/mixer.py
--rw-r--r--  2.0 unx     2487 b- defN 23-Mar-26 06:51 pyarmor-8.2.dev1/src/cli/public_capsule.zip
--rw-r--r--  2.0 unx     7475 b- defN 23-Apr-27 08:20 pyarmor-8.2.dev1/src/cli/default.cfg
--rw-r--r--  2.0 unx    22591 b- defN 23-Apr-29 07:46 pyarmor-8.2.dev1/src/cli/__main__.py
--rw-r--r--  2.0 unx    11386 b- defN 23-Apr-20 15:01 pyarmor-8.2.dev1/src/cli/repack.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/helloworld/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/cx_Freeze/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/simple/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/pybench/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/testpkg/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/testmod/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/py2exe/
--rwxr-xr-x  2.0 unx     2048 b- defN 22-Mar-10 20:03 pyarmor-8.2.dev1/src/examples/obfuscate-pkg.bat
--rwxr-xr-x  2.0 unx     1645 b- defN 22-Mar-10 20:03 pyarmor-8.2.dev1/src/examples/obfuscate-app.bat
--rwxr-xr-x  2.0 unx     1103 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/obfuscate-app.sh
--rwxr-xr-x  2.0 unx     1685 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/obfuscate-pkg.sh
--rwxr-xr-x  2.0 unx     4102 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/build-with-project.bat
--rw-r--r--  2.0 unx     6876 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/README.md
--rwxr-xr-x  2.0 unx      773 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.sh
--rwxr-xr-x  2.0 unx      928 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.bat
--rwxr-xr-x  2.0 unx     3146 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/build-with-project.sh
--rwxr-xr-x  2.0 unx     4395 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/build-for-freeze.bat
--rw-r--r--  2.0 unx     7078 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/README-ZH.md
--rwxr-xr-x  2.0 unx     4231 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/build-for-exe.bat
--rw-r--r--  2.0 unx     1747 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/helloworld/foo.py
--rwxr-xr-x  2.0 unx       49 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/cx_Freeze/hello.py
--rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/cx_Freeze/queens.py
--rwxr-xr-x  2.0 unx      641 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/cx_Freeze/setup.py
--rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/simple/queens.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/pybench/package/
--rwxr-xr-x  2.0 unx    13565 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Arithmetic.py
--rwxr-xr-x  2.0 unx     4134 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/With.py
--rwxr-xr-x  2.0 unx     6460 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Lists.py
--rwxr-xr-x  2.0 unx     8034 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Tuples.py
--rwxr-xr-x  2.0 unx     1388 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Instances.py
--rwxr-xr-x  2.0 unx     6672 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/systimes.py
--rwxr-xr-x  2.0 unx     1193 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/clockres.py
--rwxr-xr-x  2.0 unx    15254 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Lookups.py
--rwxr-xr-x  2.0 unx    16870 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/CommandLine.py
--rwxr-xr-x  2.0 unx    16198 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Numbers.py
--rwxr-xr-x  2.0 unx     2941 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Imports.py
--rwxr-xr-x  2.0 unx      961 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Setup.py
--rwxr-xr-x  2.0 unx    13400 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Exceptions.py
--rwxr-xr-x  2.0 unx     9261 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Dict.py
--rwxr-xr-x  2.0 unx    31828 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/pybench.py
--rwxr-xr-x  2.0 unx     1561 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/NewInstances.py
--rwxr-xr-x  2.0 unx     9252 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Calls.py
--rwxr-xr-x  2.0 unx    10946 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Strings.py
--rwxr-xr-x  2.0 unx    13207 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Constructs.py
--rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/package/__init__.py
--rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/package/submodule.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/testpkg/mypkg/
--rw-r--r--  2.0 unx       66 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/testpkg/main.py
--rw-r--r--  2.0 unx      202 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/testpkg/mypkg/__init__.py
--rw-r--r--  2.0 unx       45 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/testpkg/mypkg/foo.py
--rwxr-xr-x  2.0 unx     1734 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/testmod/hello.py
--rwxr-xr-x  2.0 unx     3694 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/testmod/queens.py
--rwxr-xr-x  2.0 unx       44 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/py2exe/hello.py
--rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/py2exe/queens.py
--rwxr-xr-x  2.0 unx     1081 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/py2exe/setup.py
--rw-r--r--  2.0 unx       28 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/polyfills/__init__.py
--rwxr-xr-x  2.0 unx    88440 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/polyfills/argparse.py
--rw-r--r--  2.0 unx     1505 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/superuntime.py
--rw-r--r--  2.0 unx     9191 b- defN 22-Jan-06 22:40 pyarmor-8.2.dev1/src/helper/merge.py
--rw-r--r--  2.0 unx    11618 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/buildext.py
--rw-r--r--  2.0 unx     2144 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/get_platform_name.py
--rw-r--r--  2.0 unx      778 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/get_license_info.py
--rw-r--r--  2.0 unx      728 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/get_bind_key.py
--rw-r--r--  2.0 unx        1 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/__init__.py
--rw-r--r--  2.0 unx     3821 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/build_data_module.py
--rw-r--r--  2.0 unx    12719 b- defN 23-Mar-21 13:48 pyarmor-8.2.dev1/src/helper/repack.py
-137 files, 7373641 bytes uncompressed, 2287475 bytes compressed:  69.0%
+Zip file size: 2309362 bytes, number of entries: 137
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/pyarmor.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/
+-rw-r--r--  2.0 unx     3004 b- defN 23-May-01 10:26 pyarmor-8.2.dev2/PKG-INFO
+-rwxr-xr-x  2.0 unx      191 b- defN 23-Mar-04 11:58 pyarmor-8.2.dev2/MANIFEST.in
+-rw-r--r--  2.0 unx     6692 b- defN 23-Apr-20 10:36 pyarmor-8.2.dev2/README.md
+-rw-r--r--  2.0 unx     4296 b- defN 23-Apr-30 20:14 pyarmor-8.2.dev2/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-May-01 10:26 pyarmor-8.2.dev2/setup.cfg
+-rw-r--r--  2.0 unx     3004 b- defN 23-May-01 10:26 pyarmor-8.2.dev2/pyarmor.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     2911 b- defN 23-May-01 10:26 pyarmor-8.2.dev2/pyarmor.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      135 b- defN 23-May-01 10:26 pyarmor-8.2.dev2/pyarmor.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-May-01 10:26 pyarmor-8.2.dev2/pyarmor.egg-info/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-01 10:26 pyarmor-8.2.dev2/pyarmor.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-01 10:26 pyarmor-8.2.dev2/pyarmor.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/platforms/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/plugins/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/cli/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/examples/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/polyfills/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/helper/
+-rw-r--r--  2.0 unx      234 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev2/src/pyshield.lic
+-rwxr-xr-x  2.0 unx     2038 b- defN 23-Apr-30 20:13 pyarmor-8.2.dev2/src/config.py
+-rwxr-xr-x  2.0 unx    10197 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/benchmark.py
+-rw-r--r--  2.0 unx     7265 b- defN 22-Feb-25 10:48 pyarmor-8.2.dev2/src/register.py
+-rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev2/src/product.key
+-rwxr-xr-x  2.0 unx    65827 b- defN 23-Mar-26 00:20 pyarmor-8.2.dev2/src/pyarmor.py
+-rw-r--r--  2.0 unx     2664 b- defN 22-Jan-29 09:20 pyarmor-8.2.dev2/src/protect_code.pt
+-rw-r--r--  2.0 unx    13587 b- defN 21-Nov-02 17:34 pyarmor-8.2.dev2/src/pytransform.py
+-rw-r--r--  2.0 unx     3363 b- defN 22-Jun-27 00:08 pyarmor-8.2.dev2/src/sppmode.py
+-rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev2/src/public.key
+-rwxr-xr-x  2.0 unx      113 b- defN 20-Jan-02 11:09 pyarmor-8.2.dev2/src/__init__.py
+-rw-r--r--  2.0 unx     2191 b- defN 22-Dec-04 19:13 pyarmor-8.2.dev2/src/reform.py
+-rwxr-xr-x  2.0 unx    25832 b- defN 22-Nov-20 13:42 pyarmor-8.2.dev2/src/packer.py
+-rw-r--r--  2.0 unx     5200 b- defN 23-Jan-06 00:02 pyarmor-8.2.dev2/src/cobuilder.py
+-rwxr-xr-x  2.0 unx    67431 b- defN 22-Dec-23 17:42 pyarmor-8.2.dev2/src/utils.py
+-rw-r--r--  2.0 unx       37 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/pyarmor-webui.py
+-rw-r--r--  2.0 unx     4028 b- defN 21-Dec-16 08:28 pyarmor-8.2.dev2/src/build_meta.py
+-rw-r--r--  2.0 unx      256 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev2/src/license.tri
+-rw-r--r--  2.0 unx     1598 b- defN 23-Mar-04 17:07 pyarmor-8.2.dev2/src/README.rst
+-rw-r--r--  2.0 unx     1596 b- defN 22-Jan-30 11:51 pyarmor-8.2.dev2/src/protect_code2.pt
+-rw-r--r--  2.0 unx     2487 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev2/src/public_capsule.zip
+-rwxr-xr-x  2.0 unx     8023 b- defN 22-Jun-28 09:01 pyarmor-8.2.dev2/src/project.py
+-rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev2/src/pyshield.key
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/platforms/linux/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/platforms/darwin/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/platforms/windows/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/platforms/linux/x86/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/platforms/linux/x86_64/
+-rwxr-xr-x  2.0 unx  1421600 b- defN 22-Sep-28 20:59 pyarmor-8.2.dev2/src/platforms/linux/x86/_pytransform.so
+-rwxr-xr-x  2.0 unx  1198080 b- defN 22-Sep-28 20:59 pyarmor-8.2.dev2/src/platforms/linux/x86_64/_pytransform.so
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/platforms/darwin/x86_64/
+-rwxr-xr-x  2.0 unx  1469620 b- defN 22-Sep-28 18:28 pyarmor-8.2.dev2/src/platforms/darwin/x86_64/_pytransform.dylib
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/platforms/windows/x86/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/platforms/windows/x86_64/
+-rw-r--r--  2.0 unx  1373710 b- defN 22-Sep-28 21:00 pyarmor-8.2.dev2/src/platforms/windows/x86/_pytransform.dll
+-rwxr-xr-x  2.0 unx  1165824 b- defN 22-Sep-28 20:59 pyarmor-8.2.dev2/src/platforms/windows/x86_64/_pytransform.dll
+-rw-r--r--  2.0 unx     6360 b- defN 22-Jul-14 19:38 pyarmor-8.2.dev2/src/plugins/README.md
+-rw-r--r--  2.0 unx    13688 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/plugins/check_ntp_time.py
+-rw-r--r--  2.0 unx    10694 b- defN 23-Apr-20 15:01 pyarmor-8.2.dev2/src/cli/config.py
+-rw-r--r--  2.0 unx    17413 b- defN 23-Apr-29 13:01 pyarmor-8.2.dev2/src/cli/register.py
+-rw-r--r--  2.0 unx     5532 b- defN 23-Apr-30 16:53 pyarmor-8.2.dev2/src/cli/generate.py
+-rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 22:43 pyarmor-8.2.dev2/src/cli/shell.py
+-rw-r--r--  2.0 unx     6398 b- defN 23-Apr-13 14:46 pyarmor-8.2.dev2/src/cli/resource.py
+-rw-r--r--  2.0 unx     1479 b- defN 23-Apr-29 22:32 pyarmor-8.2.dev2/src/cli/__init__.py
+-rw-r--r--  2.0 unx    17473 b- defN 23-Apr-30 18:02 pyarmor-8.2.dev2/src/cli/context.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Apr-22 22:15 pyarmor-8.2.dev2/src/cli/plugin.py
+-rw-r--r--  2.0 unx     3956 b- defN 23-Apr-20 15:02 pyarmor-8.2.dev2/src/cli/mixer.py
+-rw-r--r--  2.0 unx     2487 b- defN 23-Mar-26 06:51 pyarmor-8.2.dev2/src/cli/public_capsule.zip
+-rw-r--r--  2.0 unx     8186 b- defN 23-May-01 10:05 pyarmor-8.2.dev2/src/cli/default.cfg
+-rw-r--r--  2.0 unx    22526 b- defN 23-Apr-30 05:18 pyarmor-8.2.dev2/src/cli/__main__.py
+-rw-r--r--  2.0 unx    11386 b- defN 23-Apr-20 15:01 pyarmor-8.2.dev2/src/cli/repack.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/examples/helloworld/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/examples/cx_Freeze/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/examples/simple/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/examples/pybench/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/examples/testpkg/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/examples/testmod/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/examples/py2exe/
+-rwxr-xr-x  2.0 unx     2048 b- defN 22-Mar-10 20:03 pyarmor-8.2.dev2/src/examples/obfuscate-pkg.bat
+-rwxr-xr-x  2.0 unx     1645 b- defN 22-Mar-10 20:03 pyarmor-8.2.dev2/src/examples/obfuscate-app.bat
+-rwxr-xr-x  2.0 unx     1103 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/examples/obfuscate-app.sh
+-rwxr-xr-x  2.0 unx     1685 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/examples/obfuscate-pkg.sh
+-rwxr-xr-x  2.0 unx     4102 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/examples/build-with-project.bat
+-rw-r--r--  2.0 unx     6876 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/examples/README.md
+-rwxr-xr-x  2.0 unx      773 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/examples/pack-obfuscated-scripts.sh
+-rwxr-xr-x  2.0 unx      928 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/examples/pack-obfuscated-scripts.bat
+-rwxr-xr-x  2.0 unx     3146 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/examples/build-with-project.sh
+-rwxr-xr-x  2.0 unx     4395 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/build-for-freeze.bat
+-rw-r--r--  2.0 unx     7078 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/examples/README-ZH.md
+-rwxr-xr-x  2.0 unx     4231 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/build-for-exe.bat
+-rw-r--r--  2.0 unx     1747 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/helloworld/foo.py
+-rwxr-xr-x  2.0 unx       49 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/cx_Freeze/hello.py
+-rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/cx_Freeze/queens.py
+-rwxr-xr-x  2.0 unx      641 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/cx_Freeze/setup.py
+-rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/simple/queens.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/examples/pybench/package/
+-rwxr-xr-x  2.0 unx    13565 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Arithmetic.py
+-rwxr-xr-x  2.0 unx     4134 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/With.py
+-rwxr-xr-x  2.0 unx     6460 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Lists.py
+-rwxr-xr-x  2.0 unx     8034 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Tuples.py
+-rwxr-xr-x  2.0 unx     1388 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Instances.py
+-rwxr-xr-x  2.0 unx     6672 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/systimes.py
+-rwxr-xr-x  2.0 unx     1193 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/clockres.py
+-rwxr-xr-x  2.0 unx    15254 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Lookups.py
+-rwxr-xr-x  2.0 unx    16870 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/CommandLine.py
+-rwxr-xr-x  2.0 unx    16198 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Numbers.py
+-rwxr-xr-x  2.0 unx     2941 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Imports.py
+-rwxr-xr-x  2.0 unx      961 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Setup.py
+-rwxr-xr-x  2.0 unx    13400 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Exceptions.py
+-rwxr-xr-x  2.0 unx     9261 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Dict.py
+-rwxr-xr-x  2.0 unx    31828 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/pybench.py
+-rwxr-xr-x  2.0 unx     1561 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/NewInstances.py
+-rwxr-xr-x  2.0 unx     9252 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Calls.py
+-rwxr-xr-x  2.0 unx    10946 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Strings.py
+-rwxr-xr-x  2.0 unx    13207 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/Constructs.py
+-rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/package/__init__.py
+-rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/pybench/package/submodule.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 10:26 pyarmor-8.2.dev2/src/examples/testpkg/mypkg/
+-rw-r--r--  2.0 unx       66 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/testpkg/main.py
+-rw-r--r--  2.0 unx      202 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/testpkg/mypkg/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/testpkg/mypkg/foo.py
+-rwxr-xr-x  2.0 unx     1734 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/testmod/hello.py
+-rwxr-xr-x  2.0 unx     3694 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/testmod/queens.py
+-rwxr-xr-x  2.0 unx       44 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/py2exe/hello.py
+-rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/py2exe/queens.py
+-rwxr-xr-x  2.0 unx     1081 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/examples/py2exe/setup.py
+-rw-r--r--  2.0 unx       28 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/polyfills/__init__.py
+-rwxr-xr-x  2.0 unx    88440 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev2/src/polyfills/argparse.py
+-rw-r--r--  2.0 unx     1505 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/helper/superuntime.py
+-rw-r--r--  2.0 unx     9191 b- defN 22-Jan-06 22:40 pyarmor-8.2.dev2/src/helper/merge.py
+-rw-r--r--  2.0 unx    11618 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/helper/buildext.py
+-rw-r--r--  2.0 unx     2144 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/helper/get_platform_name.py
+-rw-r--r--  2.0 unx      778 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/helper/get_license_info.py
+-rw-r--r--  2.0 unx      728 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/helper/get_bind_key.py
+-rw-r--r--  2.0 unx        1 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/helper/__init__.py
+-rw-r--r--  2.0 unx     3821 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev2/src/helper/build_data_module.py
+-rw-r--r--  2.0 unx    12719 b- defN 23-Mar-21 13:48 pyarmor-8.2.dev2/src/helper/repack.py
+137 files, 7374484 bytes uncompressed, 2287638 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,412 +1,412 @@
-Filename: pyarmor-8.2.dev1/
+Filename: pyarmor-8.2.dev2/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/pyarmor.egg-info/
+Filename: pyarmor-8.2.dev2/pyarmor.egg-info/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/
+Filename: pyarmor-8.2.dev2/src/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/PKG-INFO
+Filename: pyarmor-8.2.dev2/PKG-INFO
 Comment: 
 
-Filename: pyarmor-8.2.dev1/MANIFEST.in
+Filename: pyarmor-8.2.dev2/MANIFEST.in
 Comment: 
 
-Filename: pyarmor-8.2.dev1/README.md
+Filename: pyarmor-8.2.dev2/README.md
 Comment: 
 
-Filename: pyarmor-8.2.dev1/setup.py
+Filename: pyarmor-8.2.dev2/setup.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/setup.cfg
+Filename: pyarmor-8.2.dev2/setup.cfg
 Comment: 
 
-Filename: pyarmor-8.2.dev1/pyarmor.egg-info/PKG-INFO
+Filename: pyarmor-8.2.dev2/pyarmor.egg-info/PKG-INFO
 Comment: 
 
-Filename: pyarmor-8.2.dev1/pyarmor.egg-info/SOURCES.txt
+Filename: pyarmor-8.2.dev2/pyarmor.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pyarmor-8.2.dev1/pyarmor.egg-info/entry_points.txt
+Filename: pyarmor-8.2.dev2/pyarmor.egg-info/entry_points.txt
 Comment: 
 
-Filename: pyarmor-8.2.dev1/pyarmor.egg-info/requires.txt
+Filename: pyarmor-8.2.dev2/pyarmor.egg-info/requires.txt
 Comment: 
 
-Filename: pyarmor-8.2.dev1/pyarmor.egg-info/top_level.txt
+Filename: pyarmor-8.2.dev2/pyarmor.egg-info/top_level.txt
 Comment: 
 
-Filename: pyarmor-8.2.dev1/pyarmor.egg-info/dependency_links.txt
+Filename: pyarmor-8.2.dev2/pyarmor.egg-info/dependency_links.txt
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/
+Filename: pyarmor-8.2.dev2/src/platforms/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/plugins/
+Filename: pyarmor-8.2.dev2/src/plugins/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/
+Filename: pyarmor-8.2.dev2/src/cli/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/
+Filename: pyarmor-8.2.dev2/src/examples/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/polyfills/
+Filename: pyarmor-8.2.dev2/src/polyfills/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/helper/
+Filename: pyarmor-8.2.dev2/src/helper/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/pyshield.lic
+Filename: pyarmor-8.2.dev2/src/pyshield.lic
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/config.py
+Filename: pyarmor-8.2.dev2/src/config.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/benchmark.py
+Filename: pyarmor-8.2.dev2/src/benchmark.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/register.py
+Filename: pyarmor-8.2.dev2/src/register.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/product.key
+Filename: pyarmor-8.2.dev2/src/product.key
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/pyarmor.py
+Filename: pyarmor-8.2.dev2/src/pyarmor.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/protect_code.pt
+Filename: pyarmor-8.2.dev2/src/protect_code.pt
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/pytransform.py
+Filename: pyarmor-8.2.dev2/src/pytransform.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/sppmode.py
+Filename: pyarmor-8.2.dev2/src/sppmode.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/public.key
+Filename: pyarmor-8.2.dev2/src/public.key
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/__init__.py
+Filename: pyarmor-8.2.dev2/src/__init__.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/reform.py
+Filename: pyarmor-8.2.dev2/src/reform.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/packer.py
+Filename: pyarmor-8.2.dev2/src/packer.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cobuilder.py
+Filename: pyarmor-8.2.dev2/src/cobuilder.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/utils.py
+Filename: pyarmor-8.2.dev2/src/utils.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/pyarmor-webui.py
+Filename: pyarmor-8.2.dev2/src/pyarmor-webui.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/build_meta.py
+Filename: pyarmor-8.2.dev2/src/build_meta.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/license.tri
+Filename: pyarmor-8.2.dev2/src/license.tri
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/README.rst
+Filename: pyarmor-8.2.dev2/src/README.rst
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/protect_code2.pt
+Filename: pyarmor-8.2.dev2/src/protect_code2.pt
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/public_capsule.zip
+Filename: pyarmor-8.2.dev2/src/public_capsule.zip
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/project.py
+Filename: pyarmor-8.2.dev2/src/project.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/pyshield.key
+Filename: pyarmor-8.2.dev2/src/pyshield.key
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/linux/
+Filename: pyarmor-8.2.dev2/src/platforms/linux/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/darwin/
+Filename: pyarmor-8.2.dev2/src/platforms/darwin/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/windows/
+Filename: pyarmor-8.2.dev2/src/platforms/windows/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/linux/x86/
+Filename: pyarmor-8.2.dev2/src/platforms/linux/x86/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/linux/x86_64/
+Filename: pyarmor-8.2.dev2/src/platforms/linux/x86_64/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/linux/x86/_pytransform.so
+Filename: pyarmor-8.2.dev2/src/platforms/linux/x86/_pytransform.so
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/linux/x86_64/_pytransform.so
+Filename: pyarmor-8.2.dev2/src/platforms/linux/x86_64/_pytransform.so
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/darwin/x86_64/
+Filename: pyarmor-8.2.dev2/src/platforms/darwin/x86_64/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/darwin/x86_64/_pytransform.dylib
+Filename: pyarmor-8.2.dev2/src/platforms/darwin/x86_64/_pytransform.dylib
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/windows/x86/
+Filename: pyarmor-8.2.dev2/src/platforms/windows/x86/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/windows/x86_64/
+Filename: pyarmor-8.2.dev2/src/platforms/windows/x86_64/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/windows/x86/_pytransform.dll
+Filename: pyarmor-8.2.dev2/src/platforms/windows/x86/_pytransform.dll
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/platforms/windows/x86_64/_pytransform.dll
+Filename: pyarmor-8.2.dev2/src/platforms/windows/x86_64/_pytransform.dll
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/plugins/README.md
+Filename: pyarmor-8.2.dev2/src/plugins/README.md
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/plugins/check_ntp_time.py
+Filename: pyarmor-8.2.dev2/src/plugins/check_ntp_time.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/config.py
+Filename: pyarmor-8.2.dev2/src/cli/config.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/register.py
+Filename: pyarmor-8.2.dev2/src/cli/register.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/generate.py
+Filename: pyarmor-8.2.dev2/src/cli/generate.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/shell.py
+Filename: pyarmor-8.2.dev2/src/cli/shell.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/resource.py
+Filename: pyarmor-8.2.dev2/src/cli/resource.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/__init__.py
+Filename: pyarmor-8.2.dev2/src/cli/__init__.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/context.py
+Filename: pyarmor-8.2.dev2/src/cli/context.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/plugin.py
+Filename: pyarmor-8.2.dev2/src/cli/plugin.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/mixer.py
+Filename: pyarmor-8.2.dev2/src/cli/mixer.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/public_capsule.zip
+Filename: pyarmor-8.2.dev2/src/cli/public_capsule.zip
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/default.cfg
+Filename: pyarmor-8.2.dev2/src/cli/default.cfg
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/__main__.py
+Filename: pyarmor-8.2.dev2/src/cli/__main__.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/cli/repack.py
+Filename: pyarmor-8.2.dev2/src/cli/repack.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/helloworld/
+Filename: pyarmor-8.2.dev2/src/examples/helloworld/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/cx_Freeze/
+Filename: pyarmor-8.2.dev2/src/examples/cx_Freeze/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/simple/
+Filename: pyarmor-8.2.dev2/src/examples/simple/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/
+Filename: pyarmor-8.2.dev2/src/examples/pybench/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/testpkg/
+Filename: pyarmor-8.2.dev2/src/examples/testpkg/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/testmod/
+Filename: pyarmor-8.2.dev2/src/examples/testmod/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/py2exe/
+Filename: pyarmor-8.2.dev2/src/examples/py2exe/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/obfuscate-pkg.bat
+Filename: pyarmor-8.2.dev2/src/examples/obfuscate-pkg.bat
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/obfuscate-app.bat
+Filename: pyarmor-8.2.dev2/src/examples/obfuscate-app.bat
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/obfuscate-app.sh
+Filename: pyarmor-8.2.dev2/src/examples/obfuscate-app.sh
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/obfuscate-pkg.sh
+Filename: pyarmor-8.2.dev2/src/examples/obfuscate-pkg.sh
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/build-with-project.bat
+Filename: pyarmor-8.2.dev2/src/examples/build-with-project.bat
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/README.md
+Filename: pyarmor-8.2.dev2/src/examples/README.md
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.sh
+Filename: pyarmor-8.2.dev2/src/examples/pack-obfuscated-scripts.sh
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.bat
+Filename: pyarmor-8.2.dev2/src/examples/pack-obfuscated-scripts.bat
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/build-with-project.sh
+Filename: pyarmor-8.2.dev2/src/examples/build-with-project.sh
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/build-for-freeze.bat
+Filename: pyarmor-8.2.dev2/src/examples/build-for-freeze.bat
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/README-ZH.md
+Filename: pyarmor-8.2.dev2/src/examples/README-ZH.md
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/build-for-exe.bat
+Filename: pyarmor-8.2.dev2/src/examples/build-for-exe.bat
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/helloworld/foo.py
+Filename: pyarmor-8.2.dev2/src/examples/helloworld/foo.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/cx_Freeze/hello.py
+Filename: pyarmor-8.2.dev2/src/examples/cx_Freeze/hello.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/cx_Freeze/queens.py
+Filename: pyarmor-8.2.dev2/src/examples/cx_Freeze/queens.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/cx_Freeze/setup.py
+Filename: pyarmor-8.2.dev2/src/examples/cx_Freeze/setup.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/simple/queens.py
+Filename: pyarmor-8.2.dev2/src/examples/simple/queens.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/package/
+Filename: pyarmor-8.2.dev2/src/examples/pybench/package/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Arithmetic.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Arithmetic.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/With.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/With.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Lists.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Lists.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Tuples.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Tuples.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Instances.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Instances.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/systimes.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/systimes.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/clockres.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/clockres.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Lookups.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Lookups.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/CommandLine.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/CommandLine.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Numbers.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Numbers.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Imports.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Imports.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Setup.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Setup.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Exceptions.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Exceptions.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Dict.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Dict.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/pybench.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/pybench.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/NewInstances.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/NewInstances.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Calls.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Calls.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Strings.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Strings.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/Constructs.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/Constructs.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/package/__init__.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/package/__init__.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/pybench/package/submodule.py
+Filename: pyarmor-8.2.dev2/src/examples/pybench/package/submodule.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/testpkg/mypkg/
+Filename: pyarmor-8.2.dev2/src/examples/testpkg/mypkg/
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/testpkg/main.py
+Filename: pyarmor-8.2.dev2/src/examples/testpkg/main.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/testpkg/mypkg/__init__.py
+Filename: pyarmor-8.2.dev2/src/examples/testpkg/mypkg/__init__.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/testpkg/mypkg/foo.py
+Filename: pyarmor-8.2.dev2/src/examples/testpkg/mypkg/foo.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/testmod/hello.py
+Filename: pyarmor-8.2.dev2/src/examples/testmod/hello.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/testmod/queens.py
+Filename: pyarmor-8.2.dev2/src/examples/testmod/queens.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/py2exe/hello.py
+Filename: pyarmor-8.2.dev2/src/examples/py2exe/hello.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/py2exe/queens.py
+Filename: pyarmor-8.2.dev2/src/examples/py2exe/queens.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/examples/py2exe/setup.py
+Filename: pyarmor-8.2.dev2/src/examples/py2exe/setup.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/polyfills/__init__.py
+Filename: pyarmor-8.2.dev2/src/polyfills/__init__.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/polyfills/argparse.py
+Filename: pyarmor-8.2.dev2/src/polyfills/argparse.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/helper/superuntime.py
+Filename: pyarmor-8.2.dev2/src/helper/superuntime.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/helper/merge.py
+Filename: pyarmor-8.2.dev2/src/helper/merge.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/helper/buildext.py
+Filename: pyarmor-8.2.dev2/src/helper/buildext.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/helper/get_platform_name.py
+Filename: pyarmor-8.2.dev2/src/helper/get_platform_name.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/helper/get_license_info.py
+Filename: pyarmor-8.2.dev2/src/helper/get_license_info.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/helper/get_bind_key.py
+Filename: pyarmor-8.2.dev2/src/helper/get_bind_key.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/helper/__init__.py
+Filename: pyarmor-8.2.dev2/src/helper/__init__.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/helper/build_data_module.py
+Filename: pyarmor-8.2.dev2/src/helper/build_data_module.py
 Comment: 
 
-Filename: pyarmor-8.2.dev1/src/helper/repack.py
+Filename: pyarmor-8.2.dev2/src/helper/repack.py
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor-8.2.dev1/PKG-INFO` & `pyarmor-8.2.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor
-Version: 8.2.dev1
+Version: 8.2.dev2
 Summary: A tool used to obfuscate python scripts, bind obfuscated scripts to fixed machine or expire obfuscated scripts.
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Description: Protect Python Scripts By Pyarmor
         =================================
```

## Comparing `pyarmor-8.2.dev1/README.md` & `pyarmor-8.2.dev2/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/setup.py` & `pyarmor-8.2.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     package_dir={'pyarmor': 'src'},
     package_data={
         'pyarmor': pyarmor_data_files + platform_data_files,
         'pyarmor.cli': ['default.cfg', 'public_capsule.zip'],
     },
 
     install_requires=[
-        'pyarmor.cli.core~=3.2.dev1'
+        'pyarmor.cli.core~=3.2.dev2'
     ],
 
     entry_points={
         'console_scripts': [
             'pyarmor=pyarmor.pyarmor:main_entry_8',
             'pyarmor-7=pyarmor.pyarmor:main_entry',
             'pyarmor-8=pyarmor.cli.__main__:main',
```

## Comparing `pyarmor-8.2.dev1/pyarmor.egg-info/PKG-INFO` & `pyarmor-8.2.dev2/pyarmor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor
-Version: 8.2.dev1
+Version: 8.2.dev2
 Summary: A tool used to obfuscate python scripts, bind obfuscated scripts to fixed machine or expire obfuscated scripts.
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Description: Protect Python Scripts By Pyarmor
         =================================
```

## Comparing `pyarmor-8.2.dev1/pyarmor.egg-info/SOURCES.txt` & `pyarmor-8.2.dev2/pyarmor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/config.py` & `pyarmor-8.2.dev2/src/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sys import platform
 
-version = '8.2.dev1'
+version = '8.2.dev2'
 
 # The corresponding version of pytransform.so
 core_version = 'r52.6'
 
 version_info = '''
 PyArmor is a command line tool used to obfuscate python scripts, bind
 obfuscated scripts to fixed machine or expire obfuscated scripts.
```

## Comparing `pyarmor-8.2.dev1/src/benchmark.py` & `pyarmor-8.2.dev2/src/benchmark.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/register.py` & `pyarmor-8.2.dev2/src/register.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/pyarmor.py` & `pyarmor-8.2.dev2/src/pyarmor.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/protect_code.pt` & `pyarmor-8.2.dev2/src/protect_code.pt`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/pytransform.py` & `pyarmor-8.2.dev2/src/pytransform.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/sppmode.py` & `pyarmor-8.2.dev2/src/sppmode.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/reform.py` & `pyarmor-8.2.dev2/src/reform.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/packer.py` & `pyarmor-8.2.dev2/src/packer.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/cobuilder.py` & `pyarmor-8.2.dev2/src/cobuilder.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/utils.py` & `pyarmor-8.2.dev2/src/utils.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/build_meta.py` & `pyarmor-8.2.dev2/src/build_meta.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/README.rst` & `pyarmor-8.2.dev2/src/README.rst`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/protect_code2.pt` & `pyarmor-8.2.dev2/src/protect_code2.pt`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/public_capsule.zip` & `pyarmor-8.2.dev2/src/public_capsule.zip`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/project.py` & `pyarmor-8.2.dev2/src/project.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/platforms/linux/x86/_pytransform.so` & `pyarmor-8.2.dev2/src/platforms/linux/x86/_pytransform.so`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/platforms/linux/x86_64/_pytransform.so` & `pyarmor-8.2.dev2/src/platforms/linux/x86_64/_pytransform.so`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/platforms/darwin/x86_64/_pytransform.dylib` & `pyarmor-8.2.dev2/src/platforms/darwin/x86_64/_pytransform.dylib`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/platforms/windows/x86/_pytransform.dll` & `pyarmor-8.2.dev2/src/platforms/windows/x86/_pytransform.dll`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/platforms/windows/x86_64/_pytransform.dll` & `pyarmor-8.2.dev2/src/platforms/windows/x86_64/_pytransform.dll`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/plugins/README.md` & `pyarmor-8.2.dev2/src/plugins/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/plugins/check_ntp_time.py` & `pyarmor-8.2.dev2/src/plugins/check_ntp_time.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/cli/config.py` & `pyarmor-8.2.dev2/src/cli/config.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/cli/register.py` & `pyarmor-8.2.dev2/src/cli/register.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/cli/generate.py` & `pyarmor-8.2.dev2/src/cli/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         repacker(bundle, output, buildpath, entry=entry, codesign=codesign)
         shutil.rmtree(buildpath)
 
     def _obfuscate_scripts(self):
         rev = self.ctx.version_info()
         template = self.ctx.bootstrap_template
         relative = self.ctx.import_prefix
-        pkgname = self.ctx.runtime_package + self.ctx.runtime_suffix
+        pkgname = self.ctx.runtime_package_name
         bootpath = self.ctx.cfg.get('builder', 'bootstrap_file')
 
         namelist = []
         for res in self.ctx.resources:
             logger.info('process resource "%s"', res.fullname)
             name = res.name
             path = self.format_output(self.ctx.outputs, namelist.count(name))
```

## Comparing `pyarmor-8.2.dev1/src/cli/shell.py` & `pyarmor-8.2.dev2/src/cli/shell.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/cli/resource.py` & `pyarmor-8.2.dev2/src/cli/resource.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/cli/__init__.py` & `pyarmor-8.2.dev2/src/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-__VERSION__ = '8.1'
+__VERSION__ = '8.2'
 
 logger = logging.getLogger('cli')
 
 
 class CliError(Exception):
     pass
```

## Comparing `pyarmor-8.2.dev1/src/cli/context.py` & `pyarmor-8.2.dev2/src/cli/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
         # self.encoding is just for reading config file
         self.encoding = encoding
         cfglist = self.default_config, self.global_config, self.local_config
         self.cfg = self._read_config(cfglist, encoding=encoding)
 
         self.inline_plugin_marker = '# pyarmor: '
-        self.runtime_package = 'pyarmor_runtime'
+        # self.runtime_package = 'pyarmor_runtime'
         # self.runtime_suffix = '_000000'
         # default inner key filename within runtime package
         self.runtime_keyfile = '.pyarmor.ikey'
 
         self.bootstrap_template = bootstrap_template
         self.runtime_package_templates = (
             runtime_package_template,
@@ -218,14 +218,15 @@
         rev = '.'.join([str(x) for x in self.version])
         if not verbose:
             return rev
 
         licinfo = self.license_info
         lictype = 'basic' if licinfo['features'] == 1 else \
             'pro' if licinfo['features'] == 7 else \
+            'group' if licinfo['features'] == 15 else \
             'trial' if licinfo['token'] == 0 else 'unknown'
         verinfo = ['%s (%s)' % (rev, lictype)]
 
         if verbose > 1:
             verinfo.append(licinfo['licno'][-6:])
 
         if verbose > 2:
@@ -284,18 +285,14 @@
 
     @property
     def license_info(self):
         from .register import parse_token
         return parse_token(self.read_token())
 
     @property
-    def runtime_suffix(self):
-        return '_' + self.license_info['licno'][-6:]
-
-    @property
     def native_platform(self):
         from platform import system, machine
         return '.'.join([system().lower(), machine().lower()])
 
     @property
     def pyarmor_platform(self):
         platname = os.getenv('PYARMOR_PLATFORM', self.native_platform)
@@ -444,14 +441,23 @@
     #
     # runtime configuration
     #
     def _rt_opt(self, opt):
         return self.cmd_options.get(opt, self.cfg['runtime'].get(opt))
 
     @property
+    def runtime_suffix(self):
+        return self.license_info['licno'][-6:]
+
+    @property
+    def runtime_package_name(self):
+        fmt = self.cfg.get('runtime', 'package_name_format')
+        return fmt.format(suffix=self.runtime_suffix)
+
+    @property
     def runtime_platforms(self):
         return self._rt_opt('platforms')
 
     @property
     def runtime_on_error(self):
         return self._opti('runtime', 'on_error')
```

## Comparing `pyarmor-8.2.dev1/src/cli/plugin.py` & `pyarmor-8.2.dev2/src/cli/plugin.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/cli/mixer.py` & `pyarmor-8.2.dev2/src/cli/mixer.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/cli/public_capsule.zip` & `pyarmor-8.2.dev2/src/cli/public_capsule.zip`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/cli/default.cfg` & `pyarmor-8.2.dev2/src/cli/default.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -129,17 +129,23 @@
 ;; assert: call import
 assert_call = 0
 assert_import = 0
 
 ;; mix string constant
 mix_str = 0
 
+;; hide function name in traceback
+;;   1: hide function.__name__
+;;   2: also hide function.__qualname__ (not implemented)
 mix_coname = 0
+
+;; mix local variables
 mix_localnames = 1
-;; Enable it may result in annotations error
+
+;; mix argument names, it also clears annotations
 mix_argnames = 0
 
 obf_module = 1
 obf_code = 1
 wrap_mode = 1
 
 restrict_module = 1
@@ -173,14 +179,17 @@
 rft_mix_import_name = 0
 
 [runtime]
 
 ;; Generate extension for all Python3.7+
 universal = 0
 
+;; Default runtime package name
+package_name_format = pyarmor_runtime_{suffix}
+
 ;; The file ext only keep .so/.pyd, for example
 ;;     pyarmor_runtime.cpython-37m-darwin.so
 ;;     if simple_extension_name == 1 then
 ;;     pyarmor_runtime.so
 simple_extension_name = 1
 
 ;; Enable outer runtime key
@@ -307,18 +316,28 @@
 ;; Convert comprehensions to bcc code
 enable_comprehension = 1
 
 [windows.x86_64.bcc]
 cc = clang.exe
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-windows -c
 
+[windows.x86.bcc]
+cc = clang.exe
+cflags = --target=i686-elf-linux -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -fPIC -mno-sse -std=c99 -c
+
 [linux.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
 
 [linux.aarch64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -Tlinux.aarch64.ldscript
 
+[linux.x86.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -fPIC -c
+
+[linux.armv7.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -shared -nostdlib -Tlinux.armv7.ldscript
+
 [darwin.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-gnu_linux -fPIC -c
 
 [darwin.aarch64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=arm64-macho-darwin -fPIC -fno-addrsig -fno-stack-protector -shared -nostdlib -lsystem
```

## Comparing `pyarmor-8.2.dev1/src/cli/__main__.py` & `pyarmor-8.2.dev2/src/cli/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,17 +102,14 @@
         options['use_runtime'] = args.use_runtime
 
     if options.get('assert_call') or options.get('assert_import'):
         if options.get('restrict_module', 0) < 2:
             logger.debug('implicitly set restrict_module = 2')
             options['restrict_module'] = 2
 
-    if options.get('restrict_module', 0) > 1:
-        options['mix_coname'] = 1
-
     if args.enables:
         for x in args.enables:
             options['enable_' + x] = True
     if options.get('enable_themida'):
         raise NotImplementedError('--enable_themida is still not implemented')
 
     if args.prefix:
@@ -166,15 +163,15 @@
             raise CliError('--enable_themida only works for Windows')
         if enable_bcc:
             raise CliError('bcc mode does not support cross platform')
         check_cross_platform(ctx, ctx.runtime_platforms)
 
     if enable_bcc:
         plat, arch = ctx.pyarmor_platform.split('.')
-        if arch not in ('x86_64', 'aarch64'):
+        if arch not in ('x86_64', 'aarch64', 'x86', 'armv7'):
             raise CliError('bcc mode still not support arch "%s"' % arch)
 
     if ctx.cmd_options['no_runtime'] and not ctx.runtime_outer:
         raise CliError('--no_runtime must be used with --outer')
 
     if ctx.use_runtime and not ctx.runtime_outer:
         if os.path.exists(ctx.use_runtime):
```

## Comparing `pyarmor-8.2.dev1/src/cli/repack.py` & `pyarmor-8.2.dev2/src/cli/repack.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/obfuscate-pkg.bat` & `pyarmor-8.2.dev2/src/examples/obfuscate-pkg.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/obfuscate-app.bat` & `pyarmor-8.2.dev2/src/examples/obfuscate-app.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/obfuscate-app.sh` & `pyarmor-8.2.dev2/src/examples/obfuscate-app.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/obfuscate-pkg.sh` & `pyarmor-8.2.dev2/src/examples/obfuscate-pkg.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/build-with-project.bat` & `pyarmor-8.2.dev2/src/examples/build-with-project.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/README.md` & `pyarmor-8.2.dev2/src/examples/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.sh` & `pyarmor-8.2.dev2/src/examples/pack-obfuscated-scripts.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.bat` & `pyarmor-8.2.dev2/src/examples/pack-obfuscated-scripts.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/build-with-project.sh` & `pyarmor-8.2.dev2/src/examples/build-with-project.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/build-for-freeze.bat` & `pyarmor-8.2.dev2/src/examples/build-for-freeze.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/README-ZH.md` & `pyarmor-8.2.dev2/src/examples/README-ZH.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/build-for-exe.bat` & `pyarmor-8.2.dev2/src/examples/build-for-exe.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/helloworld/foo.py` & `pyarmor-8.2.dev2/src/examples/helloworld/foo.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/cx_Freeze/queens.py` & `pyarmor-8.2.dev2/src/examples/cx_Freeze/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/cx_Freeze/setup.py` & `pyarmor-8.2.dev2/src/examples/cx_Freeze/setup.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/simple/queens.py` & `pyarmor-8.2.dev2/src/examples/simple/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Arithmetic.py` & `pyarmor-8.2.dev2/src/examples/pybench/Arithmetic.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/With.py` & `pyarmor-8.2.dev2/src/examples/pybench/With.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Lists.py` & `pyarmor-8.2.dev2/src/examples/pybench/Lists.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Tuples.py` & `pyarmor-8.2.dev2/src/examples/pybench/Tuples.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Instances.py` & `pyarmor-8.2.dev2/src/examples/pybench/Instances.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/systimes.py` & `pyarmor-8.2.dev2/src/examples/pybench/systimes.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/clockres.py` & `pyarmor-8.2.dev2/src/examples/pybench/clockres.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Lookups.py` & `pyarmor-8.2.dev2/src/examples/pybench/Lookups.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/CommandLine.py` & `pyarmor-8.2.dev2/src/examples/pybench/CommandLine.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Numbers.py` & `pyarmor-8.2.dev2/src/examples/pybench/Numbers.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Imports.py` & `pyarmor-8.2.dev2/src/examples/pybench/Imports.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Setup.py` & `pyarmor-8.2.dev2/src/examples/pybench/Setup.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Exceptions.py` & `pyarmor-8.2.dev2/src/examples/pybench/Exceptions.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Dict.py` & `pyarmor-8.2.dev2/src/examples/pybench/Dict.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/pybench.py` & `pyarmor-8.2.dev2/src/examples/pybench/pybench.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/NewInstances.py` & `pyarmor-8.2.dev2/src/examples/pybench/NewInstances.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Calls.py` & `pyarmor-8.2.dev2/src/examples/pybench/Calls.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Strings.py` & `pyarmor-8.2.dev2/src/examples/pybench/Strings.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/pybench/Constructs.py` & `pyarmor-8.2.dev2/src/examples/pybench/Constructs.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/testmod/hello.py` & `pyarmor-8.2.dev2/src/examples/testmod/hello.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/testmod/queens.py` & `pyarmor-8.2.dev2/src/examples/testmod/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/py2exe/queens.py` & `pyarmor-8.2.dev2/src/examples/py2exe/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/examples/py2exe/setup.py` & `pyarmor-8.2.dev2/src/examples/py2exe/setup.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/polyfills/argparse.py` & `pyarmor-8.2.dev2/src/polyfills/argparse.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/helper/superuntime.py` & `pyarmor-8.2.dev2/src/helper/superuntime.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/helper/merge.py` & `pyarmor-8.2.dev2/src/helper/merge.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/helper/buildext.py` & `pyarmor-8.2.dev2/src/helper/buildext.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/helper/get_platform_name.py` & `pyarmor-8.2.dev2/src/helper/get_platform_name.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/helper/get_license_info.py` & `pyarmor-8.2.dev2/src/helper/get_license_info.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/helper/get_bind_key.py` & `pyarmor-8.2.dev2/src/helper/get_bind_key.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/helper/build_data_module.py` & `pyarmor-8.2.dev2/src/helper/build_data_module.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.2.dev1/src/helper/repack.py` & `pyarmor-8.2.dev2/src/helper/repack.py`

 * *Files identical despite different names*

