# Comparing `tmp/porespy-2.2.2.tar.gz` & `tmp/porespy-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porespy-2.2.2.tar", last modified: Wed Nov 16 01:00:30 2022, max compression
+gzip compressed data, was "porespy-2.3.0.tar", last modified: Tue Jun  6 17:24:08 2023, max compression
```

## Comparing `porespy-2.2.2.tar` & `porespy-2.3.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.620844 porespy-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-11-16 00:59:44.000000 porespy-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9034 2022-11-16 01:00:30.620844 porespy-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6677 2022-11-16 00:59:44.000000 porespy-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.616844 porespy-2.2.2/porespy/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.616844 porespy-2.2.2/porespy/dns/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/dns/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.616844 porespy-2.2.2/porespy/filters/
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/filters/_fftmorphology.py
--rw-r--r--   0 runner    (1001) docker     (121)    50592 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/filters/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7180 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/filters/_ibip.py
--rw-r--r--   0 runner    (1001) docker     (121)     7361 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/filters/_ibip_gpu.py
--rw-r--r--   0 runner    (1001) docker     (121)     3162 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/filters/_nlmeans.py
--rw-r--r--   0 runner    (1001) docker     (121)     7864 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/filters/_size_seq_satn.py
--rw-r--r--   0 runner    (1001) docker     (121)    36811 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/filters/_snows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.616844 porespy-2.2.2/porespy/filters/imagej/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/filters/imagej/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5332 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/filters/imagej/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.620844 porespy-2.2.2/porespy/generators/
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/generators/_borders.py
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/generators/_cylinder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/generators/_fractals.py
--rw-r--r--   0 runner    (1001) docker     (121)    41908 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/generators/_imgen.py
--rw-r--r--   0 runner    (1001) docker     (121)     3838 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/generators/_noise.py
--rw-r--r--   0 runner    (1001) docker     (121)     8183 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/generators/_pseudo_packings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.620844 porespy-2.2.2/porespy/io/
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    77875 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/io/_comsol.py
--rw-r--r--   0 runner    (1001) docker     (121)    17518 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/io/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.620844 porespy-2.2.2/porespy/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/metrics/_fractal_dims.py
--rw-r--r--   0 runner    (1001) docker     (121)    41456 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/metrics/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9794 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/metrics/_meshtools.py
--rw-r--r--   0 runner    (1001) docker     (121)     9091 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/metrics/_regionprops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.620844 porespy-2.2.2/porespy/networks/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/networks/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11618 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/networks/_getnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/networks/_maximal_ball.py
--rw-r--r--   0 runner    (1001) docker     (121)    13593 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/networks/_size_factors.py
--rw-r--r--   0 runner    (1001) docker     (121)    10398 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/networks/_snow2.py
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/networks/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.620844 porespy-2.2.2/porespy/simulations/
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4438 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/simulations/_dns.py
--rw-r--r--   0 runner    (1001) docker     (121)    10924 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/simulations/_drainage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.620844 porespy-2.2.2/porespy/tools/
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39860 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/tools/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7972 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/tools/_sphere_insertions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/tools/_unpad.py
--rw-r--r--   0 runner    (1001) docker     (121)     7941 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/tools/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.620844 porespy-2.2.2/porespy/visualization/
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10551 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/visualization/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/visualization/_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)     5071 2022-11-16 00:59:45.000000 porespy-2.2.2/porespy/visualization/_views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 01:00:30.616844 porespy-2.2.2/porespy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9034 2022-11-16 01:00:30.000000 porespy-2.2.2/porespy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-11-16 01:00:30.000000 porespy-2.2.2/porespy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 01:00:30.000000 porespy-2.2.2/porespy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 01:00:30.000000 porespy-2.2.2/porespy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-11-16 01:00:30.000000 porespy-2.2.2/porespy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-16 01:00:30.000000 porespy-2.2.2/porespy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-11-16 01:00:30.620844 porespy-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2841 2022-11-16 00:59:45.000000 porespy-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.082442 porespy-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-06 17:23:18.000000 porespy-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-06 17:24:08.082442 porespy-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-06 17:23:18.000000 porespy-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.074442 porespy-2.3.0/porespy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.078442 porespy-2.3.0/porespy/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/dns/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.078442 porespy-2.3.0/porespy/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/filters/_fftmorphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54857 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/filters/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/filters/_nlmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/filters/_size_seq_satn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37067 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/filters/_snows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.078442 porespy-2.3.0/porespy/filters/imagej/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/filters/imagej/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/filters/imagej/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.078442 porespy-2.3.0/porespy/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/generators/_borders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/generators/_fractals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52491 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/generators/_imgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/generators/_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/generators/_pseudo_packings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/generators/_spheres_from_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.078442 porespy-2.3.0/porespy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77875 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/io/_comsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/io/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/io/_unzipper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.078442 porespy-2.3.0/porespy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44387 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/metrics/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/metrics/_meshtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/metrics/_regionprops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.078442 porespy-2.3.0/porespy/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/networks/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/networks/_getnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/networks/_maximal_ball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21353 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/networks/_size_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/networks/_snow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/networks/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.078442 porespy-2.3.0/porespy/simulations/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/simulations/_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/simulations/_drainage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/simulations/_ibip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/simulations/_ibip_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.078442 porespy-2.3.0/porespy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43173 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/tools/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/tools/_sphere_insertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/tools/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.082442 porespy-2.3.0/porespy/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/visualization/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/visualization/_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-06 17:23:18.000000 porespy-2.3.0/porespy/visualization/_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:24:08.074442 porespy-2.3.0/porespy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-06 17:24:07.000000 porespy-2.3.0/porespy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-06 17:24:08.000000 porespy-2.3.0/porespy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:24:07.000000 porespy-2.3.0/porespy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:24:07.000000 porespy-2.3.0/porespy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-06 17:24:07.000000 porespy-2.3.0/porespy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 17:24:07.000000 porespy-2.3.0/porespy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-06 17:24:08.082442 porespy-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-06 17:23:18.000000 porespy-2.3.0/setup.py
```

### Comparing `porespy-2.2.2/LICENSE` & `porespy-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `porespy-2.2.2/PKG-INFO` & `porespy-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porespy
-Version: 2.2.2
+Version: 2.3.0
 Summary: A set of tools for analyzing 3D images of porous materials
 Home-page: http://porespy.org
 Author: PoreSpy Team
 Author-email: jgostick@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/PMEAL/porespy/
 Project-URL: Documentation, https://porespy.org/
@@ -68,15 +68,15 @@
         > *Gostick J, Khan ZA, Tranter TG, Kok MDR, Agnaou M, Sadeghi MA, Jervis
         > R.* **PoreSpy: A Python Toolkit for Quantitative Analysis of Porous Media
         > Images.** Journal of Open Source Software, 2019.
         > [doi:10.21105/joss.01296](https://doi.org/10.21105/joss.01296)
         
         # Installation
         
-        For detailed and up to date installation instructions, [see here](https://porespy.org/user_guide/installation.html)
+        For detailed and up to date installation instructions, [see here](https://porespy.org/installation.html)
         
         # Contributing
         
         If you think you may be interested in contributing to PoreSpy and wish
         to both *use* and *edit* the source code, then you should clone the
         [repository](https://github.com/PMEAL/porespy) to your local machine,
         and install it using the following PIP command:
@@ -182,11 +182,12 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `porespy-2.2.2/README.md` & `porespy-2.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 > *Gostick J, Khan ZA, Tranter TG, Kok MDR, Agnaou M, Sadeghi MA, Jervis
 > R.* **PoreSpy: A Python Toolkit for Quantitative Analysis of Porous Media
 > Images.** Journal of Open Source Software, 2019.
 > [doi:10.21105/joss.01296](https://doi.org/10.21105/joss.01296)
 
 # Installation
 
-For detailed and up to date installation instructions, [see here](https://porespy.org/user_guide/installation.html)
+For detailed and up to date installation instructions, [see here](https://porespy.org/installation.html)
 
 # Contributing
 
 If you think you may be interested in contributing to PoreSpy and wish
 to both *use* and *edit* the source code, then you should clone the
 [repository](https://github.com/PMEAL/porespy) to your local machine,
 and install it using the following PIP command:
```

### Comparing `porespy-2.2.2/porespy/__init__.py` & `porespy-2.3.0/porespy/__init__.py`

 * *Files identical despite different names*

### Comparing `porespy-2.2.2/porespy/filters/_fftmorphology.py` & `porespy-2.3.0/porespy/filters/_fftmorphology.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import numpy as np
 from scipy.signal import fftconvolve
 
 
+__all__ = [
+    "fftmorphology",
+]
+
+
 def fftmorphology(im, strel, mode='opening'):
     r"""
     Perform morphological operations on binary images using fft approach for
     improved performance
 
     Parameters
     ----------
```

### Comparing `porespy-2.2.2/porespy/filters/_funcs.py` & `porespy-2.3.0/porespy/filters/_funcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,155 @@
 import inspect as insp
 import logging
 import dask
 import numpy as np
 from edt import edt
 import operator as op
 import scipy.ndimage as spim
+from deprecated import deprecated
 from skimage.morphology import reconstruction
 from skimage.segmentation import clear_border
 from skimage.morphology import ball, disk, square, cube, diamond, octahedron
 from porespy.tools import _check_for_singleton_axes
-from porespy.tools import get_border, subdivide, recombine
+from porespy.tools import get_border, subdivide, recombine, make_contiguous
 from porespy.tools import unpad, extract_subsection
-from porespy.tools import ps_disk, ps_ball
+from porespy.tools import ps_disk, ps_ball, ps_round
 from porespy import settings
 from porespy.tools import get_tqdm
 
 
+__all__ = [
+    "apply_chords",
+    "apply_chords_3D",
+    "apply_padded",
+    "chunked_func",
+    "distance_transform_lin",
+    "fill_blind_pores",
+    "find_disconnected_voxels",
+    "find_trapped_regions",
+    "find_dt_artifacts",
+    "flood",
+    "flood_func",
+    "hold_peaks",
+    "ibip",
+    "ibip_gpu",
+    "local_thickness",
+    "nphase_border",
+    "porosimetry",
+    "prune_branches",
+    "region_size",
+    "trim_disconnected_blobs",
+    "trim_extrema",
+    "trim_floating_solid",
+    "trim_nonpercolating_paths",
+    "trim_small_clusters",
+]
+
+
 tqdm = get_tqdm()
 logger = logging.getLogger(__name__)
 
 
+@deprecated("The ibip function will be moved to the"
+            + " ``simulations`` module in a future version")
+def ibip(**kwargs):
+    r"""
+    This function has been moved to the ``simulations`` module, please use that.
+    """
+    from porespy.simulations import ibip
+    return ibip(**kwargs)
+
+
+@deprecated("The ibip_gpu function will be moved to the"
+            + " ``simulations`` module in a future version")
+def ibip_gpu(**kwargs):
+    r"""
+    This function has been moved to the ``simulations`` module, please use that.
+    """
+    from porespy.simulations import ibip_gpu
+    return ibip_gpu(**kwargs)
+
+
+def find_trapped_regions(seq, outlets=None, bins=25, return_mask=True):
+    r"""
+    Find the trapped regions given an invasion sequence image
+
+    Parameters
+    ----------
+    seq : ndarray
+        An image with invasion sequence values in each voxel.  Regions
+        labelled -1 are considered uninvaded, and regions labelled 0 are
+        considered solid.
+    outlets : ndarray, optional
+        An image the same size as ``seq`` with ``True`` indicating outlets
+        and ``False`` elsewhere.  If not given then all image boundaries
+        are considered outlets.
+    bins : int
+        The resolution to use when thresholding the ``seq`` image.  By default
+        the invasion sequence will be broken into 25 discrete steps and
+        trapping will be identified at each step. A higher value of ``bins``
+        will provide a more accurate trapping analysis, but is more time
+        consuming. If ``None`` is specified, then *all* the steps will
+        analyzed, providing the highest accuracy.
+    return_mask : bool
+        If ``True`` (default) then the returned image is a boolean mask
+        indicating which voxels are trapped.  If ``False``, then a copy of
+        ``seq`` is returned with the trapped voxels set to uninvaded and
+        the invasion sequence values adjusted accordingly.
+
+    Returns
+    -------
+    trapped : ND-image
+        An image, the same size as ``seq``.  If ``return_mask`` is ``True``,
+        then the image has ``True`` values indicating the trapped voxels.  If
+        ``return_mask`` is ``False``, then a copy of ``seq`` is returned with
+        trapped voxels set to 0.
+
+    Examples
+    --------
+    `Click here
+    <https://porespy.org/examples/filters/reference/find_trapped_regions.html>`_
+    to view online example.
+
+    """
+    seq = np.copy(seq)
+    if outlets is None:
+        outlets = get_border(seq.shape, mode='faces')
+    trapped = np.zeros_like(outlets)
+    if bins is None:
+        bins = np.unique(seq)[-1::-1]
+        bins = bins[bins > 0]
+    elif isinstance(bins, int):
+        # starting the max_bin at: minimum sequence at outlets
+        # This means soon as the fluid reaches the outlets
+        # outlet_seq = np.setdiff1d(seq[outlets], np.array([0]))
+        # bins_start = outlet_seq.min()
+        # starting the max_bin at: maximum sequence available
+        # in the image. No matter if it's after percolation
+        # threshold (reaching the outlets):
+        bins_start = seq.max()
+        bins = np.linspace(bins_start, 1, bins)
+    for i in tqdm(bins, **settings.tqdm):
+        temp = seq >= i
+        labels = spim.label(temp)[0]
+        keep = np.unique(labels[outlets])
+        # In cases where entire outlet is filled, the
+        # first indice is not necessarily the
+        # void space. Only the element with value
+        # of zero needs to be removed, if it's in keep.
+        keep = np.setdiff1d(keep, np.array([0]))
+        trapped += temp*np.isin(labels, keep, invert=True)
+    if return_mask:
+        return trapped
+    else:
+        seq[trapped] = -1
+        seq = make_contiguous(seq, mode='symmetric')
+        return seq
+
+
 def apply_padded(im, pad_width, func, pad_val=1, **kwargs):
     r"""
     Applies padding to an image before sending to ``func``, then extracts
     the result corresponding to the original image shape.
 
     Parameters
     ----------
@@ -81,20 +207,15 @@
     Examples
     --------
     `Click here
     <https://porespy.org/examples/filters/reference/trim_small_clusters.html>`_
     to view online example.
 
     """
-    if im.ndim == 2:
-        strel = disk(1)
-    elif im.ndim == 3:
-        strel = ball(1)
-    else:
-        raise Exception("Only 2D or 3D images are accepted")
+    strel = ps_round(r=1, ndim=im.ndim, smooth=False)
     filtered_array = np.copy(im)
     labels, N = spim.label(filtered_array, structure=strel)
     id_sizes = np.array(spim.sum(im, labels, range(N + 1)))
     area_mask = id_sizes <= size
     filtered_array[area_mask[labels]] = 0
     return filtered_array
 
@@ -922,31 +1043,32 @@
             non-wetting fluid configuration.
         'dt'
             Same as 'hybrid', except uses a second distance
             transform, relative to the thresholded mask, to find the
             invading fluid configuration. The choice of 'dt' or 'hybrid'
             depends on speed, which is system and installation specific.
         'mio'
-            Uses bindary erosion followed by dilation to obtain the invading
-            fluid confirguration directly. If ``access_limitations`` is
+            Uses binary erosion followed by dilation to obtain the invading
+            fluid configuration directly. If ``access_limitated`` is
             ``True`` then disconnected blobs are trimmmed before the dilation.
             This is the only method that can be parallelized by chunking (see
             ``divs`` and ``cores``).
 
     divs : int or array_like
-        The number of times to divide the image for parallel processing.  If ``1``
-        then parallel processing does not occur.  ``2`` is equivalent to
-        ``[2, 2, 2]`` for a 3D image.  The number of cores used is specified in
-        ``porespy.settings.ncores`` and defaults to all cores.
+        The number of times to divide the image for parallel processing.
+        If ``1`` then parallel processing does not occur.  ``2`` is
+        equivalent to ``[2, 2, 2]`` for a 3D image.  The number of cores
+        used is specified in ``porespy.settings.ncores`` and defaults to
+        all cores.
 
     Returns
     -------
     image : ndarray
         A copy of ``im`` with voxel values indicating the sphere radius at
-        which it becomes accessible from the inlets.  This image can be
+        which it becomes accessible from the ``inlets``.  This image can be
         used to find invading fluid configurations as a function of
         applied capillary pressure by applying a boolean comparison:
         ``inv_phase = im > r`` where ``r`` is the radius (in voxels) of
         the invading sphere.  Of course, ``r`` can be converted to
         capillary pressure using a preferred model.
 
     Notes
```

### Comparing `porespy-2.2.2/porespy/filters/_ibip.py` & `porespy-2.3.0/porespy/simulations/_ibip.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import numpy as np
 from edt import edt
 from porespy.tools import get_tqdm
-import scipy.ndimage as spim
 from porespy.tools import get_border, make_contiguous
 from porespy.tools import _insert_disk_at_points
 from porespy.tools import Results
-import numba
+from numba import njit
 from porespy import settings
 tqdm = get_tqdm()
 
 
+__all__ = [
+    "ibip",
+]
+
+
 def ibip(im, inlets=None, dt=None, maxiter=10000):
     r"""
     Performs invasion percolation on given image using iterative image dilation
 
     Parameters
     ----------
     im : ND-array
@@ -95,112 +99,48 @@
     sizes[temp] = -1
     results = Results()
     results.inv_sequence = inv
     results.inv_sizes = sizes
     return results
 
 
-@numba.jit(nopython=True, parallel=False)
+@njit(parallel=False)
 def _where(arr):
     inds = np.where(arr)
     result = np.vstack(inds)
     return result
 
 
-@numba.jit(nopython=True)
+@njit()
 def _update_dt_and_bd(dt, bd, pt):
     if dt.ndim == 2:
         for i in range(pt.shape[1]):
             bd[pt[0, i], pt[1, i]] = True
             dt[pt[0, i], pt[1, i]] = 0
     else:
         for i in range(pt.shape[1]):
             bd[pt[0, i], pt[1, i], pt[2, i]] = True
             dt[pt[0, i], pt[1, i], pt[2, i]] = 0
     return dt, bd
 
 
-def find_trapped_regions(seq, outlets=None, bins=25, return_mask=True):
-    r"""
-    Find the trapped regions given an invasion sequence image
-
-    Parameters
-    ----------
-    seq : ndarray
-        An image with invasion sequence values in each voxel.  Regions
-        labelled -1 are considered uninvaded, and regions labelled 0 are
-        considered solid.
-    outlets : ndarray, optional
-        An image the same size as ``seq`` with ``True`` indicating outlets
-        and ``False`` elsewhere.  If not given then all image boundaries
-        are considered outlets.
-    bins : int
-        The resolution to use when thresholding the ``seq`` image.  By default
-        the invasion sequence will be broken into 25 discrete steps and
-        trapping will be identified at each step. A higher value of ``bins``
-        will provide a more accurate trapping analysis, but is more time
-        consuming. If ``None`` is specified, then *all* the steps will
-        analyzed, providing the highest accuracy.
-    return_mask : bool
-        If ``True`` (default) then the returned image is a boolean mask
-        indicating which voxels are trapped.  If ``False``, then a copy of
-        ``seq`` is returned with the trapped voxels set to uninvaded and
-        the invasion sequence values adjusted accordingly.
-
-    Returns
-    -------
-    trapped : ND-image
-        An image, the same size as ``seq``.  If ``return_mask`` is ``True``,
-        then the image has ``True`` values indicating the trapped voxels.  If
-        ``return_mask`` is ``False``, then a copy of ``seq`` is returned with
-        trapped voxels set to 0.
-
-    Examples
-    --------
-    `Click here
-    <https://porespy.org/examples/filters/reference/find_trapped_regions.html>`_
-    to view online example.
-
-    """
-    seq = np.copy(seq)
-    if outlets is None:
-        outlets = get_border(seq.shape, mode='faces')
-    trapped = np.zeros_like(outlets)
-    if bins is None:
-        bins = np.unique(seq)[-1::-1]
-        bins = bins[bins > 0]
-    elif isinstance(bins, int):
-        bins = np.linspace(seq.max(), 1, bins)
-    for i in tqdm(bins, **settings.tqdm):
-        temp = seq >= i
-        labels = spim.label(temp)[0]
-        keep = np.unique(labels[outlets])[1:]
-        trapped += temp*np.isin(labels, keep, invert=True)
-    if return_mask:
-        return trapped
-    else:
-        seq[trapped] = -1
-        seq = make_contiguous(seq, mode='symmetric')
-        return seq
-
-
 if __name__ == "__main__":
     import numpy as np
     import porespy as ps
     import matplotlib.pyplot as plt
     from copy import copy
 
     # %% Run this cell to regenerate the variables in drainage
     np.random.seed(6)
     bg = 'white'
     plots = True
     im = ps.generators.blobs(shape=[300, 300], porosity=0.7, blobiness=2)
     inlets = np.zeros_like(im)
     inlets[0, :] = True
-    ip = ps.filters.ibip(im=im, inlets=inlets)
+    ip = ps.simulations.ibip(im=im, inlets=inlets)
 
     # %% Generate some plots
     if plots:
         cmap = copy(plt.cm.plasma)
         cmap.set_under(color='black')
         cmap.set_over(color='grey')
         fig, ax = plt.subplots(1, 1)
```

### Comparing `porespy-2.2.2/porespy/filters/_ibip_gpu.py` & `porespy-2.3.0/porespy/simulations/_ibip_gpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import logging
 import numpy as np
 from edt import edt
 from porespy.tools import get_tqdm, get_border
 from porespy.tools import Results
 
 
+__all__ = [
+    "ibip_gpu",
+]
+
+
 tqdm = get_tqdm()
 logger = logging.getLogger(__name__)
 
 
 def ibip_gpu(im, dt=None, inlets=None, maxiter=10000):  # pragma: no cover
     """
     Performs invasion percolation on given image using iterative image
```

### Comparing `porespy-2.2.2/porespy/filters/_nlmeans.py` & `porespy-2.3.0/porespy/filters/_nlmeans.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import numpy as np
-from skimage.restoration import denoise_nl_means, estimate_sigma
+from skimage.restoration.non_local_means import denoise_nl_means
+from skimage.restoration import estimate_sigma
 from skimage.exposure import rescale_intensity, match_histograms
 import dask
 dask.config.set(scheduler="threads")
 # from dask.diagnostics import ProgressBar
 
 
-def nl_means_layered(im, cores=None, axis=0, patch_size=5, patch_distance=15, h=4):
+__all__ = [
+    "nl_means_layered",
+]
+
+
+def nl_means_layered(im, cores=None, axis=0, patch_size=5, patch_distance=5, h=4):
     r"""
     Apply the non-local means filter to each 2D layer of a stack in parallel.
 
     This applies ``skimage.restoration.denoise_nl_means`` to each slice, so
     refer to the documentation of that function for further information.
 
     Parameters
@@ -54,33 +60,31 @@
 
     """
 
     @dask.delayed
     def apply_func(func, **kwargs):
         return func(**kwargs)
 
-    temp = np.copy(im)
-    for i in range(im.shape[2]):
-        temp[:, :, i] = match_histograms(temp[:, :, i], temp[:, :, 0],
-                                         multichannel=False)
+    # Move axis of interest to first axis
+    temp = np.swapaxes(im, 0, axis)
+    for i in range(im.shape[0]):
+        temp[i, ...] = match_histograms(temp[i, ...], temp[0, ...])
     p2, p98 = np.percentile(temp, (2, 98))
     temp = rescale_intensity(temp, in_range=(p2, p98))
     temp = temp / temp.max()
-    sigma_est = np.mean(estimate_sigma(temp[:, :, 0], multichannel=False))
+    sigma_est = np.mean(estimate_sigma(temp[0, ...]))
 
     kw = {'image': temp,
           'patch_size': patch_size,
           'patch_distance': patch_distance,
           'h': h * sigma_est,
-          'multichannel': False,
           'fast_mode': True}
 
-    temp = np.swapaxes(temp, 0, axis)
     results = []
-    for i in range(im.shape[2]):
+    for i in range(im.shape[0]):
         layer = temp[i, ...]
         kw["image"] = layer
         t = apply_func(func=denoise_nl_means, **kw)
         results.append(t)
     # with ProgressBar():
     #     ims = dask.compute(results, num_workers=cores)[0]
     ims = dask.compute(results, num_workers=cores)[0]
```

### Comparing `porespy-2.2.2/porespy/filters/_snows.py` & `porespy-2.3.0/porespy/filters/_snows.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,26 @@
 from porespy.tools import extend_slice, ps_rect, ps_round
 from porespy.tools import Results
 from porespy.tools import get_tqdm
 from porespy.filters import chunked_func
 from porespy import settings
 
 
+__all__ = [
+    "snow_partitioning",
+    "snow_partitioning_n",
+    "snow_partitioning_parallel",
+    "find_peaks",
+    "reduce_peaks",
+    "trim_nearby_peaks",
+    "trim_saddle_points",
+    "trim_saddle_points_legacy",
+]
+
+
 tqdm = get_tqdm()
 logger = logging.getLogger(__name__)
 
 
 def snow_partitioning(im, dt=None, r_max=4, sigma=0.4, peaks=None):
     r"""
     Partition the void space into pore regions using a marker-based
@@ -406,15 +418,15 @@
             iters += 1
             peaks_dil = spim.binary_dilation(input=peaks_i, structure=cube(3))
             peaks_max = peaks_dil * np.amax(dt_i * peaks_dil)
             peaks_extended = (peaks_max == dt_i) * im_i
             if np.all(peaks_extended == peaks_i):
                 new_peaks[sx] += peaks_i
                 break  # Found a true peak
-            elif np.sum(peaks_extended * peaks_i) == 0:
+            elif np.sum(peaks_extended * peaks_i, dtype=np.int64) == 0:
                 break  # Found a saddle point
             peaks_i = peaks_extended
         if iters >= maxiter:
             logger.debug(
                 "Maximum number of iterations reached, consider "
                 + "running again with a larger value of max_iters"
             )
@@ -479,15 +491,15 @@
         while iters < maxiter:
             iters += 1
             peaks_dil = spim.binary_dilation(input=peaks_i, structure=cube(3))
             peaks_max = peaks_dil * np.amax(dt_i * peaks_dil)
             peaks_extended = (peaks_max == dt_i) * im_i
             if np.all(peaks_extended == peaks_i):
                 break  # Found a true peak
-            elif np.sum(peaks_extended * peaks_i) == 0:
+            elif np.sum(peaks_extended * peaks_i, dtype=np.int64) == 0:
                 peaks_i = False
                 break  # Found a saddle point
             # The following line was also missing from the original.  It has
             # no effect on the result but without this the "maxiters" is
             # reached very often.
             peaks_i = peaks_extended
         # The following line is essentially a bug.  It should be:
```

### Comparing `porespy-2.2.2/porespy/filters/imagej/_funcs.py` & `porespy-2.3.0/porespy/filters/imagej/_funcs.py`

 * *Files identical despite different names*

### Comparing `porespy-2.2.2/porespy/generators/_borders.py` & `porespy-2.3.0/porespy/generators/_borders.py`

 * *Files identical despite different names*

### Comparing `porespy-2.2.2/porespy/generators/_imgen.py` & `porespy-2.3.0/porespy/generators/_imgen.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,96 @@
 from edt import edt
 import porespy as ps
 from numba import njit
 import scipy.spatial as sptl
 import scipy.ndimage as spim
 import scipy.stats as spst
 from deprecated import deprecated
-from porespy.tools import norm_to_uniform, ps_ball, ps_disk, get_border
+from porespy.tools import norm_to_uniform, ps_ball, ps_disk, get_border, ps_round
 from porespy.tools import extract_subsection
 from porespy.tools import insert_sphere
+from porespy.tools import _insert_disk_at_points
 from porespy import settings
 from typing import List
 
 
+__all__ = [
+    "blobs",
+    "bundle_of_tubes",
+    "cylinders",
+    "cylindrical_plug",
+    "insert_shape",
+    "lattice_spheres",
+    "line_segment",
+    "overlapping_spheres",
+    "polydisperse_spheres",
+    "RSA",
+    "rsa",
+    "random_spheres",
+    "voronoi_edges",
+    "_get_Voronoi_edges",
+]
+
+
 tqdm = ps.tools.get_tqdm()
 logger = logging.getLogger(__name__)
 
 
+def cylindrical_plug(shape, r=None, axis=2):
+    r"""
+    Generates a cylindrical plug suitable for use as a mask on a tomogram
+
+    Parameters
+    ----------
+    shape : array_like
+        The shape of the image to create.  Can be 3D, or 2D in which case
+        a circle is returned.
+    r : int (optional)
+        The diameter of the cylinder to create. If not provided then the
+        largest possible radius is used to fit within the image.
+    axis : int
+        The direction along with the cylinder's axis of rotation should be
+        oriented.  The default is 2, which is the z-direction.
+
+    Returns
+    -------
+    cylinder : ndarray
+        A boolean image of the size given by ``shape`` with ``True``'s
+        inside the cylinder and ``False``'s outside.
+
+    Examples
+    --------
+    `Click here
+    <https://porespy.org/examples/generators/reference/cylindrical_plug.html>`_
+    to view online example.
+
+    """
+    shape = np.array(shape, dtype=int)
+    axes = np.array(list(set([0, 1, 2]).difference(set([axis]))), dtype=int)
+    if len(shape) == 3:
+        im2d = np.ones(shape=shape[axes])
+        im2d[int(shape[axes[0]]/2), int(shape[axes[1]]/2)] = 0
+        dt = edt(im2d)
+        if r is None:
+            r = int(min(shape[axes])/2)
+        circ = dt < r
+        tile_ax = [1, 1, 1]
+        tile_ax[axis] = shape[axis]
+        circ = np.expand_dims(circ, axis)
+        cyl = np.tile(circ, tile_ax)
+    if len(shape) == 2:
+        im2d = np.ones(shape=shape)
+        im2d[int(shape[0]/2), int(shape[1]/2)] = 0
+        dt = edt(im2d)
+        if r is None:
+            r = int(min(shape[axes])/2)
+        cyl = dt < r
+    return cyl
+
+
 def insert_shape(im, element, center=None, corner=None, value=1, mode="overwrite"):
     r"""
     Inserts sub-image into a larger image at the specified location.
 
     If the inserted image extends beyond the boundaries of the image it will
     be cropped accordingly.
 
@@ -100,27 +171,31 @@
     elif mode == "overwrite":
         im[tuple(s_im)] = element[tuple(s_el)] * value
     else:
         raise Exception("Invalid mode " + mode)
     return im
 
 
-@deprecated("This function has been renamed to rsa (lowercase to meet pep8")
+@deprecated("This function has been renamed to rsa (lowercase to meet pep8)")
 def RSA(*args, **kwargs):
     return rsa(*args, **kwargs)
 
 
-def rsa(im_or_shape: np.array,
-        r: int,
-        volume_fraction: int = 1,
-        clearance: int = 0,
-        n_max: int = 100000,
-        mode: str = "contained",
-        return_spheres: bool = False,
-        smooth: bool = True):
+def random_spheres(
+    im_or_shape: np.array,
+    r: int,
+    volume_fraction: int = 1,
+    clearance: int = 0,
+    protrusion: int = 0,
+    n_max: int = 100000,
+    edges: str = "contained",
+    return_spheres: bool = False,
+    smooth: bool = True,
+    seed: int = None,
+):
     r"""
     Generates a sphere or disk packing using Random Sequential Addition
 
     Parameters
     ----------
     im_or_shape : ndarray or list
         To provide flexibility, this argument accepts either an image into
@@ -131,41 +206,168 @@
     r : int
         The radius of the disk or sphere to insert.
     volume_fraction : scalar (default is 1.0)
         The fraction of the image that should be filled with spheres.  The
         spheres are added as ``True``'s, so each sphere addition increases the
         ``volume_fraction`` until the specified limit is reached.  Note that if
         ``n_max`` is reached first, then ``volume_fraction`` will not be
-        acheived.  Also, ``volume_fraction`` is not counted correctly if the
+        achieved.  Also, ``volume_fraction`` is not counted correctly if the
         ``mode`` is ``'extended'``.
     clearance : int (optional, default = 0)
         The amount of space to put between each sphere. Negative values are
         acceptable to create overlaps, so long as ``abs(clearance) < r``.
+    protrusion : int (optional, default = 0)
+        The amount by which inserted spheres are allowed to protrude outside of
+        the given background.  If set to 0 (the default) then all spheres will
+        be fully inside the region marked ``False`` in the input image. If > 0, then
+        spheres will extend into the region marked ``True`` in the input image.
+    n_max : int (default is 100,000)
+        The maximum number of spheres to add.  Using a low value may halt
+        the addition process prior to reaching the specified
+        ``volume_fraction``.  If ``None`` is given, then no limit is used.
+    edges : string (default is 'contained')
+        Controls how the edges of the image are handled.  Options are:
+
+        ============ ===============================================================
+        edges        description
+        ============ ===============================================================
+        'contained'  Spheres are all completely within the image
+        'extended'   Spheres are allowed to extend beyond the edge of the
+                     image.  In this mode the volume fraction will be less than
+                     requested since some spheres extend beyond the image, but their
+                     entire volume is counted as added for computational efficiency.
+        ============ ===============================================================
+
+    return_spheres : bool
+        If ``True`` then an image containing only the spheres is returned
+        rather than the input image with the spheres added, which is the
+        default behavior.
+    smooth : bool
+        Indicates whether balls should have smooth faces (``True``) or should
+        include the bumps on the extremities (``False``).
+    seed : int
+        The seed to supply to the random number generators. Because this function
+        uses ``numba`` for speed, calling the normal ``numpy.random.seed(<seed>)``
+        has no effect. To get a repeatable image, the seed must be passed to the
+        function so it can be initialized the way ``numba`` requires. The default
+        is ``None``, which means each call will produce a new realization.
+
+    Returns
+    -------
+    image : ndarray
+        An image with spheres of specified radius *added* to the background.
+
+    See Also
+    --------
+    pseudo_gravity_packing
+    pseudo_electrostatic_packing
+
+    Notes
+    -----
+    This algorithm ensures that spheres do not overlap but does not
+    guarantee they are tightly packed.
+
+    This function adds spheres to the background of the received ``im``, which
+    allows iteratively adding spheres of different radii to the unfilled space
+    by repeatedly passing in the result of previous calls to RSA.
+
+    References
+    ----------
+    [1] Random Heterogeneous Materials, S. Torquato (2001)
+
+    Examples
+    --------
+    `Click here
+    <https://porespy.org/examples/generators/reference/random_spheres.html>`_
+    to view online example.
+
+    """
+    im = rsa(
+        im_or_shape=im_or_shape,
+        r=r,
+        volume_fraction=volume_fraction,
+        clearance=clearance,
+        protrusion=protrusion,
+        n_max=n_max,
+        mode=edges,
+        return_spheres=return_spheres,
+        smooth=smooth,
+        seed=seed)
+    return im
+
+
+@deprecated("This function will be renamed random_spheres in a future version")
+def rsa(
+    im_or_shape: np.array,
+    r: int,
+    volume_fraction: int = 1,
+    clearance: int = 0,
+    protrusion: int = 0,
+    n_max: int = 100000,
+    mode: str = "contained",
+    return_spheres: bool = False,
+    smooth: bool = True,
+    seed: int = None,
+):
+    r"""
+    Generates a sphere or disk packing using Random Sequential Addition
+
+    Parameters
+    ----------
+    im_or_shape : ndarray or list
+        To provide flexibility, this argument accepts either an image into
+        which the spheres are inserted, or a shape which is used to create an
+        empty image.  In both cases the spheres are added as ``True`` values
+        to the background.  Since ``True`` is considered the pore space, then
+        the added spheres represent holes.
+    r : int
+        The radius of the disk or sphere to insert.
+    volume_fraction : scalar (default is 1.0)
+        The fraction of the image that should be filled with spheres.  The
+        spheres are added as ``True``'s, so each sphere addition increases the
+        ``volume_fraction`` until the specified limit is reached.  Note that if
+        ``n_max`` is reached first, then ``volume_fraction`` will not be
+        achieved.  Also, ``volume_fraction`` is not counted correctly if the
+        ``mode`` is ``'extended'``.
+    clearance : int (optional, default = 0)
+        The amount of space to put between each sphere. Negative values are
+        acceptable to create overlaps, so long as ``abs(clearance) < r``.
+    protrusion : int (optional, default = 0)
+        The amount by which inserted spheres are allowed to protrude outside of
+        the given background.  If set to 0 (the default) then all spheres will
+        be fully inside the region marked ``False`` in the input image. If > 0, then
+        spheres will extend into the region marked ``True`` in the input image.
     n_max : int (default is 100,000)
         The maximum number of spheres to add.  Using a low value may halt
         the addition process prior to reaching the specified
         ``volume_fraction``.  If ``None`` is given, then no limit is used.
     mode : string (default is 'contained')
         Controls how the edges of the image are handled.  Options are:
 
         'contained'
             Spheres are all completely within the image
         'extended'
             Spheres are allowed to extend beyond the edge of the
-            image.  In this mode the volume fraction will be less that
+            image.  In this mode the volume fraction will be less than
             requested since some spheres extend beyond the image, but their
             entire volume is counted as added for computational efficiency.
 
     return_spheres : bool
         If ``True`` then an image containing only the spheres is returned
         rather than the input image with the spheres added, which is the
         default behavior.
     smooth : bool
         Indicates whether balls should have smooth faces (``True``) or should
         include the bumps on the extremities (``False``).
+    seed : int
+        The seed to supply to the random number generators. Because this function
+        uses ``numba`` for speed, calling the normal ``numpy.random.seed(<seed>)``
+        has no effect. To get a repeatable image, the seed must be passed to the
+        function so it can be initialized the way ``numba`` requires. The default
+        is ``None``, which means each call will produce a new realization.
 
     Returns
     -------
     image : ndarray
         An image with spheres of specified radius *added* to the background.
 
     See Also
@@ -189,85 +391,97 @@
     Examples
     --------
     `Click here
     <https://porespy.org/examples/generators/reference/rsa.html>`_
     to view online example.
 
     """
-    logger.debug(f"RSA: Adding spheres of size {r}")
-    if len(im_or_shape) <= 3:
+    logger.debug(f"rsa: Adding spheres of size {r}")
+    if np.array(im_or_shape).ndim < 2:
         im = np.zeros(shape=im_or_shape, dtype=bool)
+        input_im = np.copy(im)
     else:
-        im = im_or_shape
+        input_im = np.copy(im_or_shape)
+        im = np.zeros_like(im_or_shape, dtype=bool)
+    if seed is not None:  # Initialize rng so numba sees it
+        _set_seed(seed)
     im = im.astype(bool)
-    if return_spheres:
-        im_temp = np.copy(im)
+    shape_orig = im.shape  # Store original image shape, to undo padding at the end
     if n_max is None:
         n_max = np.inf
+    # Compute volume fraction info
     vf_final = volume_fraction
-    vf_start = im.sum() / im.size
+    vf_start = im.sum(dtype=np.int64) / im.size
+    vf_template = ps_round(r, ndim=im.ndim, smooth=smooth).sum(dtype=np.int64) / im.size
     logger.debug(f"Initial volume fraction: {vf_start}")
-    if im.ndim == 2:
-        template_lg = ps_disk((r + clearance) * 2)
-        template_sm = ps_disk(r, smooth=smooth)
-    else:
-        template_lg = ps_ball((r + clearance) * 2)
-        template_sm = ps_ball(r, smooth=smooth)
-    vf_template = template_sm.sum() / im.size
-    # Pad image by the radius of large template to enable insertion near edges
-    im = np.pad(im, pad_width=2 * (r + clearance), mode="edge")
-    # Depending on mode, adjust mask to remove options around edge
+    # Dilate existing objects by strel to remove pixels near them
+    # from consideration for sphere placement
+    logger.info("Dilating foreground features by sphere radius")
+    dt = edt(input_im == 0)
+    options_im = dt >= (r - protrusion)
+    # Depending on mode, adjust options_im to remove options around edge
     if mode == "contained":
-        border = get_border(im.shape, thickness=2 * (r + clearance),
-                            mode="faces")
+        border = get_border(im.shape, thickness=r, mode="faces")
+        options_im[border] = False
     elif mode == "extended":
-        border = get_border(im.shape, thickness=(r + clearance) + 1,
-                            mode="faces")
+        im = np.pad(im, pad_width=r, mode="edge")
+        options_im = np.pad(options_im, r, mode='symmetric')
     else:
         raise Exception("Unrecognized mode: ", mode)
-    # Remove border pixels
-    im[border] = True
-    # Dilate existing objects by strel to remove pixels near them
-    # from consideration for sphere placement
-    logger.info("Dilating foreground features by sphere radius")
-    dt = edt(im == 0)
-    options_im = dt >= r
     # Begin inserting the spheres
     vf = vf_start
     free_sites = np.flatnonzero(options_im)
     i = 0
     while (vf <= vf_final) and (i < n_max) and (len(free_sites) > 0):
+        # Choose a random site from free_sites
         c, count = _make_choice(options_im, free_sites=free_sites)
         # The 100 below is arbitrary and may change performance
         if count > 100:
             # Regenerate list of free_sites
             logger.debug(f"Regenerating `free_sites` after {i} iterations")
             free_sites = np.flatnonzero(options_im)
         if all(np.array(c) == -1):
             break
-        s_sm = tuple([slice(x - r, x + r + 1, None) for x in c])
-        s_lg = tuple([slice(x - 2 * (r + clearance),
-                            x + 2 * (r + clearance) + 1, None) for x in c])
-        im[s_sm] += template_sm  # Add ball to image
-        options_im[s_lg][template_lg] = False  # Update extended region
+        im = _insert_disk_at_points(im=im,
+                                    coords=np.vstack(c),
+                                    r=r,
+                                    v=True,
+                                    smooth=smooth)
+        options_im = _insert_disk_at_points(im=options_im,
+                                            coords=np.vstack(c),
+                                            r=2*r + int(np.round(clearance/2)),
+                                            v=False,
+                                            smooth=smooth,
+                                            overwrite=True)
         vf += vf_template
         i += 1
     logger.info(f"Number of spheres inserted: {i}")
-    # Get slice into returned image to retain original size
-    s = tuple([slice(2 * (r + clearance), d - 2 * (r + clearance), None)
-               for d in im.shape])
-    im = im[s]
-    vf = im.sum() / im.size
+    im = extract_subsection(im, shape_orig)
     logger.debug("Final volume fraction:", vf)
-    if return_spheres:
-        im = im * (~im_temp)
+    if not return_spheres:
+        im = im + input_im
     return im
 
 
 @njit
+def _set_seed(a):
+    np.random.seed(a)
+
+
+@njit
+def _get_rand_float(*args):
+    return np.random.rand(*args)
+
+
+@njit
+def _get_rand_int(*args):
+    return np.random.randint(*args)
+
+
+@njit
 def _make_choice(options_im, free_sites):
     r"""
     This function is called by _begin_inserting to find valid insertion
     points.
 
     Parameters
     ----------
@@ -298,42 +512,48 @@
     if options_im.ndim == 2:
         coords = [-1, -1]
         Nx, Ny = options_im.shape
         while not choice:
             if count >= maxiter:
                 coords = [-1, -1]
                 break
-            ind = np.random.randint(0, upper_limit)
+            ind = _get_rand_int(0, upper_limit)
             # This numpy function is not supported by numba yet
             # c1, c2 = np.unravel_index(free_sites[ind], options_im.shape)
             # So using manual unraveling
             coords[1] = free_sites[ind] % Ny
             coords[0] = (free_sites[ind] // Ny) % Nx
             choice = options_im[coords[0], coords[1]]
             count += 1
     if options_im.ndim == 3:
         coords = [-1, -1, -1]
         Nx, Ny, Nz = options_im.shape
         while not choice:
             if count >= maxiter:
                 coords = [-1, -1, -1]
                 break
-            ind = np.random.randint(0, upper_limit)
+            ind = _get_rand_int(0, upper_limit)
             # This numpy function is not supported by numba yet
             # c1, c2, c3 = np.unravel_index(free_sites[ind], options_im.shape)
             # So using manual unraveling
             coords[2] = free_sites[ind] % Nz
             coords[1] = (free_sites[ind] // Nz) % Ny
             coords[0] = (free_sites[ind] // (Nz * Ny)) % Nx
             choice = options_im[coords[0], coords[1], coords[2]]
             count += 1
     return coords, count
 
 
-def bundle_of_tubes(shape: List[int], spacing: int, distribution=None, smooth=True):
+def bundle_of_tubes(
+    shape: List[int],
+    spacing: int,
+    distribution=None,
+    smooth=True,
+    seed=None,
+):
     r"""
     Create a 3D image of a bundle of tubes, in the form of a rectangular
     plate with randomly sized holes through it.
 
     Parameters
     ----------
     shape : list
@@ -341,37 +561,43 @@
         thickness.  If the 3rd dimension is not given then a thickness of
         1 voxel is assumed.
     spacing : int
         The center to center distance of the holes.  The hole sizes will
         be distributed between this values down to 3 voxels.
     distribution : scipy.stats object
         A handle to a scipy stats object with the desired parameters.
+    seed : int, optional, default = `None`
+        Initializes numpy's random number generator to the specified state. If not
+        provided, the current global value is used. This means calls to
+        ``np.random.state(seed)`` prior to calling this function will be respected.
 
     Returns
     -------
     image : ndarray
         A boolean array with ``True`` values denoting the pore space
 
     Examples
     --------
     `Click here
     <https://porespy.org/examples/generators/reference/bundle_of_tubes.html>`_
     to view online example.
 
     """
+    if seed is not None:
+        np.random.seed(seed)
     shape = np.array(shape)
     if len(shape) == 2:
         shape = np.hstack((shape, [1]))
     shape2 = shape[shape > 1]
     im = ~lattice_spheres(shape=shape2,
                           r=1,
                           offset=0.5*spacing,
                           spacing=spacing,
                           lattice='sc')
-    N = im.sum()
+    N = im.sum(dtype=np.int64)
     if distribution is None:
         # +1 below is because randint 4.X gives a max of 3
         distribution = spst.randint(low=3, high=int(spacing/2 + 1))
         Rs = distribution.rvs(N)
     else:
         Rs = distribution.rvs(N)
         Rs = np.around(np.clip(Rs, a_min=1, a_max=spacing/2), decimals=0).astype(int)
@@ -385,15 +611,16 @@
     return temp
 
 
 def polydisperse_spheres(shape: List[int],
                          porosity: float,
                          dist,
                          nbins: int = 5,
-                         r_min: int = 5):
+                         r_min: int = 5,
+                         seed=None):
     r"""
     Create an image of randomly placed, overlapping spheres with a
     distribution of radii.
 
     Parameters
     ----------
     shape : list
@@ -413,77 +640,98 @@
         ``dist = scipy.stats.norm(loc=20, scale=10)``
     nbins : int
         The number of discrete sphere sizes that will be used to generate
         the image. This function generates ``nbins`` images of
         monodisperse spheres that span 0.05 and 0.95 of the possible
         values produced by the provided distribution, then overlays them
         to get polydispersivity.
+    seed : int, optional, default = `None`
+        Initializes numpy's random number generator to the specified state. If not
+        provided, the current global value is used. This means calls to
+        ``np.random.state(seed)`` prior to calling this function will be respected.
 
     Returns
     -------
     image : ndarray
         A boolean array with ``True`` values denoting the pore space
 
     Examples
     --------
     `Click here
     <https://porespy.org/examples/generators/reference/polydisperse_spheres.html>`_
     to view online example.
 
     """
+    if seed is not None:
+        np.random.seed(seed)
     shape = np.array(shape)
     if np.size(shape) == 1:
         shape = np.full((3,), int(shape))
     Rs = dist.interval(np.linspace(0.05, 0.95, nbins))
     Rs = np.vstack(Rs).T
     Rs = (Rs[:-1] + Rs[1:]) / 2
     Rs = np.clip(Rs.flatten(), a_min=r_min, a_max=None)
     phi_desired = 1 - (1 - porosity) / (len(Rs))
     im = np.ones(shape, dtype=bool)
     for r in Rs:
-        phi_im = im.sum() / np.prod(shape)
+        phi_im = im.sum(dtype=np.int64) / np.prod(shape)
         phi_corrected = 1 - (1 - phi_desired) / phi_im
         temp = overlapping_spheres(shape=shape, r=r, porosity=phi_corrected)
         im = im * temp
     return im
 
 
-def voronoi_edges(shape: List[int], ncells: int, r: int = 0,
-                  flat_faces: bool = True):
+def voronoi_edges(
+    shape: List[int],
+    ncells: int,
+    r: int = 0,
+    flat_faces: bool = True,
+    seed=None,
+    **kwargs,
+):
     r"""
     Create an image from the edges of a Voronoi tessellation.
 
     Parameters
     ----------
     shape : array_like
         The size of the image to generate in [Nx, Ny, <Nz>] where Ni is the
         number of voxels in each direction.  If Nz is not given a 2D image
         is returned.
     ncells : int
         The number of Voronoi cells to include in the tesselation.
-    radius : int, optional
+    r : int, optional
         The radius to which Voronoi edges should be dilated in the final
         image.  If not given then edges are a single pixel/voxel thick.
     flat_faces : bool
         Whether the Voronoi edges should lie on the boundary of the
         image (``True``), or if edges outside the image should be removed
         (``False``).
+    seed : int, optional, default = `None`
+        Initializes numpy's random number generator to the specified state. If not
+        provided, the current global value is used. This means calls to
+        ``np.random.state(seed)`` prior to calling this function will be respected.
 
     Returns
     -------
     image : ndarray
         A boolean array with ``True`` values denoting the pore space
 
     Examples
     --------
     `Click here
     <https://porespy.org/examples/generators/reference/voronoi_edges.html>`_
     to view online example.
 
     """
+    if 'radius' in kwargs.keys():
+        r = kwargs['radius']
+        print('radius keyword is deprecated in favor of just r')
+    if seed is not None:
+        np.random.seed(seed)
     logger.info(f"Generating {ncells} cells")
     shape = np.array(shape)
     if np.size(shape) == 1:
         shape = np.full((3,), int(shape))
     im = np.zeros(shape, dtype=bool)
     base_pts = tuple(np.around(np.random.rand(ncells, im.ndim) * (shape-1),
                                decimals=0).T.astype(int))
@@ -508,15 +756,15 @@
     im = edt(~im) > r
     return im
 
 
 def _get_Voronoi_edges(vor):
     r"""
     Given a Voronoi object as produced by the scipy.spatial.Voronoi class,
-    this function calculates the start and end points of eeach edge in the
+    this function calculates the start and end points of each edge in the
     Voronoi diagram, in terms of the vertex indices used by the received
     Voronoi object.
 
     Parameters
     ----------
     vor : scipy.spatial.Voronoi object
 
@@ -679,19 +927,22 @@
     if smooth:
         im = ~(edt(~im) < r)
     else:
         im = ~(edt(~im) <= r)
     return im
 
 
-def overlapping_spheres(shape: List[int],
-                        r: int,
-                        porosity: float,
-                        maxiter: int = 10,
-                        tol: float = 0.01):
+def overlapping_spheres(
+    shape: List[int],
+    r: int,
+    porosity: float,
+    maxiter: int = 10,
+    tol: float = 0.01,
+    seed=None,
+):
     r"""
     Generate a packing of overlapping mono-disperse spheres
 
     Parameters
     ----------
     shape : list
         The size of the image to generate in [Nx, Ny, Nz] where Ni is the
@@ -701,14 +952,18 @@
     porosity : scalar
         The porosity of the final image, accurate to the given tolerance.
     maxiter : int
         Maximum number of iterations for the iterative algorithm that improves
         the porosity of the final image to match the given value.
     tol : float
         Tolerance for porosity of the final image compared to the given value.
+    seed : int, optional, default = `None`
+        Initializes numpy's random number generator to the specified state. If not
+        provided, the current global value is used. This means calls to
+        ``np.random.state(seed)`` prior to calling this function will be respected.
 
     Returns
     -------
     image : ndarray
         A boolean array with ``True`` values denoting the pore space
 
     Notes
@@ -720,31 +975,34 @@
     Examples
     --------
     `Click here
     <https://porespy.org/examples/generators/reference/overlapping_spheres.html>`_
     to view online example.
 
     """
+    if seed is not None:
+        np.random.seed(seed)
     shape = np.array(shape)
     if np.size(shape) == 1:
         shape = np.full((3, ), int(shape))
-    ndim = (shape != 1).sum()
-    s_vol = ps_disk(r).sum() if ndim == 2 else ps_ball(r).sum()
+    ndim = (shape != 1).sum(dtype=np.int64)
+    s_vol = ps_disk(r).sum(dtype=np.int64) if ndim == 2 \
+        else ps_ball(r).sum(dtype=np.int64)
 
     bulk_vol = np.prod(shape)
     N = int(np.ceil((1 - porosity) * bulk_vol / s_vol))
     im = np.random.random(size=shape)
 
     # Helper functions for calculating porosity: phi = g(f(N))
     def f(N):
         return edt(im > N / bulk_vol) < r
 
     def g(im):
         r"""Returns fraction of 0s, given a binary image"""
-        return 1 - im.sum() / np.prod(shape)
+        return 1 - im.sum(dtype=np.int64) / np.prod(shape)
 
     # # Newton's method for getting image porosity match the given
     # w = 1.0                         # Damping factor
     # dN = 5 if ndim == 2 else 25     # Perturbation
     # for i in range(maxiter):
     #     err = g(f(N)) - porosity
     #     d_err = (g(f(N+dN)) - g(f(N))) / dN
@@ -766,16 +1024,21 @@
             N_high = N
         if abs(err) <= tol:
             break
 
     return ~f(N)
 
 
-def blobs(shape: List[int], porosity: float = 0.5, blobiness: int = 1,
-          divs: int = 1):
+def blobs(
+    shape: List[int],
+    porosity: float = 0.5,
+    blobiness: int = 1,
+    divs: int = 1,
+    seed=None,
+):
     """
     Generates an image containing amorphous blobs
 
     Parameters
     ----------
     shape : list
         The size of the image to generate in [Nx, Ny, Nz] where N is the
@@ -791,14 +1054,18 @@
         blobs are anisotropic.
     divs : int or array_like
         The number of times to divide the image for parallel processing.
         If ``1`` then parallel processing does not occur.  ``2`` is
         equivalent to ``[2, 2, 2]`` for a 3D image.  The number of cores
         used is specified in ``porespy.settings.ncores`` and defaults to
         all cores.
+    seed : int, optional, default = `None`
+        Initializes numpy's random number generator to the specified state. If not
+        provided, the current global value is used. This means calls to
+        ``np.random.state(seed)`` prior to calling this function will be respected.
 
     Returns
     -------
     image : ndarray
         A boolean array with ``True`` values denoting the pore space
 
     See Also
@@ -818,14 +1085,16 @@
     Examples
     --------
     `Click here
     <https://porespy.org/examples/generators/reference/blobs.html>`_
     to view online example.
 
     """
+    if seed is not None:
+        np.random.seed(seed)
     if isinstance(shape, int):
         shape = [shape]*3
     if len(shape) == 1:
         shape = [shape[0]]*3
     shape = np.array(shape)
     if isinstance(blobiness, int):
         blobiness = [blobiness]*len(shape)
@@ -835,33 +1104,36 @@
         divs = [divs]*len(shape)
     if max(divs) > 1:
         parallel = True
         logger.info(f'Performing {insp.currentframe().f_code.co_name} in parallel')
     sigma = np.mean(shape) / (40 * blobiness)
     im = np.random.random(shape)
     if parallel:
-        overlap = max([int(s*4) for s in sigma])
+        overlap = max([int(s*4) for s in np.array(sigma, ndmin=1)])
         im = ps.filters.chunked_func(func=spim.gaussian_filter,
                                      input=im, sigma=sigma,
                                      divs=divs, overlap=overlap)
     else:
         im = spim.gaussian_filter(im, sigma=sigma)
     im = norm_to_uniform(im, scale=[0, 1])
     if porosity:
         im = im < porosity
     return im
 
 
-def _cylinders(shape: List[int],
-               r: int,
-               ncylinders: int,
-               phi_max: float = 0,
-               theta_max: float = 90,
-               length: float = None,
-               verbose: bool = True):
+def _cylinders(
+    shape: List[int],
+    r: int,
+    ncylinders: int,
+    phi_max: float = 0,
+    theta_max: float = 90,
+    length: float = None,
+    verbose: bool = True,
+    seed=None,
+):
     r"""
     Generates a binary image of overlapping cylinders.
 
     This is a good approximation of a fibrous mat.
 
     Parameters
     ----------
@@ -888,28 +1160,34 @@
         The length of the cylinders to add.  If ``None`` (default) then
         the cylinders will extend beyond the domain in both directions so
         no ends will exist. If a scalar value is given it will be
         interpreted as the Euclidean distance between the two ends of the
         cylinder. Note that one or both of the ends *may* still lie
         outside the domain, depending on the randomly chosen center point
         of the cylinder.
+    seed : int, optional, default = `None`
+        Initializes numpy's random number generator to the specified state. If not
+        provided, the current global value is used. This means calls to
+        ``np.random.state(seed)`` prior to calling this function will be respected.
 
     Returns
     -------
     image : ndarray
         A boolean array with ``True`` values denoting the pore space
 
     """
+    if seed is not None:
+        np.random.seed(seed)
     shape = np.array(shape)
     if np.size(shape) == 1:
         shape = np.full((3, ), int(shape))
     elif np.size(shape) == 2:
         raise Exception("2D cylinders don't make sense")
     # Find hypotenuse of domain from [0,0,0] to [Nx,Ny,Nz]
-    H = np.sqrt(np.sum(np.square(shape))).astype(int)
+    H = np.sqrt(np.sum(np.square(shape), dtype=np.int64)).astype(int)
     if length is None:  # Assume cylinders span domain if length not given
         length = 2 * H
     R = min(int(length / 2), 2 * H)  # Trim given length to 2H if too long
     # Adjust max angles to be between 0 and 90
     if (phi_max > 90) or (phi_max < 0):
         raise Exception('phi_max must be betwen 0 and 90')
     if (theta_max > 90) or (theta_max < 0):
@@ -942,22 +1220,25 @@
                 n += 1
                 pbar.update()
     im = np.array(im, dtype=bool)
     dt = edt(~im) < r
     return ~dt
 
 
-def cylinders(shape: List[int],
-              r: int,
-              ncylinders: int = None,
-              porosity: float = None,
-              phi_max: float = 0,
-              theta_max: float = 90,
-              length: float = None,
-              maxiter: int = 3):
+def cylinders(
+    shape: List[int],
+    r: int,
+    ncylinders: int = None,
+    porosity: float = None,
+    phi_max: float = 0,
+    theta_max: float = 90,
+    length: float = None,
+    maxiter: int = 3,
+    seed=None,
+):
     r"""
     Generates a binary image of overlapping cylinders given porosity OR
     number of cylinders.
 
     This is a good approximation of a fibrous mat.
 
     Parameters
@@ -996,14 +1277,18 @@
         of the cylinder.
     maxiter : int
         The number of fractional fiber insertions used to target the
         requested porosity. By default a value of 3 is used (and this is
         typically effective in getting very close to the targeted
         porosity), but a greater number can be input to improve the
         achieved porosity.
+    seed : int, optional, default = `None`
+        Initializes numpy's random number generator to the specified state. If not
+        provided, the current global value is used. This means calls to
+        ``np.random.state(seed)`` prior to calling this function will be respected.
 
     Returns
     -------
     image : ndarray
         A boolean array with ``True`` values denoting the pore space
 
     Notes
@@ -1028,14 +1313,17 @@
     Examples
     --------
     `Click here
     <https://porespy.org/examples/generators/reference/cylinders.html>`_
     to view online example.
 
     """
+    if seed is not None:
+        np.random.seed(seed)
+
     if ncylinders is not None:
         im = _cylinders(
             shape=shape,
             r=r,
             ncylinders=ncylinders,
             phi_max=phi_max,
             theta_max=theta_max,
@@ -1063,15 +1351,15 @@
     # Rough fiber volume estimate
     vol_fiber = length_estimate * np.pi * r * r
     n_pixels_to_add = get_num_pixels(porosity)
 
     # Rough estimate of n_fibers
     n_fibers_added = 0
     # Calculate fraction of fibers to be added in each iteration.
-    subdif = 0.8 / np.sum(np.arange(1, maxiter) ** 2)
+    subdif = 0.8 / np.sum(np.arange(1, maxiter) ** 2, dtype=np.int64)
     fractions = [0.2]
     for i in range(1, maxiter):
         fractions.append(fractions[i - 1] + (maxiter - i) ** 2 * subdif)
 
     im = np.ones(shape, dtype=bool)
     for frac in tqdm(fractions, **settings.tqdm):
         n_fibers_total = n_pixels_to_add / vol_fiber
@@ -1115,15 +1403,17 @@
     <https://porespy.org/examples/generators/reference/line_segment.html>`_
     to view online example.
 
     """
     X0 = np.around(X0).astype(int)
     X1 = np.around(X1).astype(int)
     if len(X0) == 3:
-        L = np.amax(np.absolute([[X1[0] - X0[0]], [X1[1] - X0[1]], [X1[2] - X0[2]]])) + 1
+        L = np.amax(
+            np.absolute([[X1[0] - X0[0]], [X1[1] - X0[1]], [X1[2] - X0[2]]])
+        ) + 1
         x = np.rint(np.linspace(X0[0], X1[0], L)).astype(int)
         y = np.rint(np.linspace(X0[1], X1[1], L)).astype(int)
         z = np.rint(np.linspace(X0[2], X1[2], L)).astype(int)
         return [x, y, z]
     else:
         L = np.amax(np.absolute([[X1[0] - X0[0]], [X1[1] - X0[1]]])) + 1
         x = np.rint(np.linspace(X0[0], X1[0], L)).astype(int)
```

### Comparing `porespy-2.2.2/porespy/generators/_noise.py` & `porespy-2.3.0/porespy/generators/_noise.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 import numpy as np
 from porespy.tools import norm_to_uniform
 import psutil
 
 
-def fractal_noise(shape, frequency=0.05, octaves=4, gain=0.5, mode='simplex',
-                  seed=None, cores=None, uniform=True):
+__all__ = [
+    'fractal_noise',
+]
+
+
+def fractal_noise(
+    shape,
+    frequency=0.05,
+    octaves=4,
+    gain=0.5,
+    mode='simplex',
+    seed=None,
+    cores=None,
+    uniform=True,
+):
     r"""
     Generate fractal noise which can be thresholded to create binary
     images with realistic structures across scales.
 
     Parameters
     ----------
     shape : array_like
@@ -21,25 +34,29 @@
         generated, with larger values giving more scale.
     gain : scalar, default=0.5
         Controls the intensity of successively higher octaves. Values
         below 1.0 mean the higher octaves are less prominent.
     mode : string
         The type of noise to generate. Options are:
 
-        - 'perlin'
-            classic Perlin noise
-
-        - 'simplex'
-            updated Perlin noise for more realistic textures
-
-        - 'value'
-            bilnear interpolation of white noise
-
-        - 'cubic'
-            cubic interpolation of white noise
+        ========== ==================================================================
+        mode       description
+        ========== ==================================================================
+        'perlin'   Classic Perlin noise. For more information on ``perlin noise`` see
+                   `here <https://en.wikipedia.org/wiki/Perlin_noise>`__.
+        'simplex'  Updated Perlin noise for more realistic textures. For more
+                   information on ``simplex noise`` see
+                   `here <https://en.wikipedia.org/wiki/Simplex_noise>`__.
+        'value'    Bilnear interpolation of white noise. For more information on
+                   ``value noise`` see
+                   `here <https://en.wikipedia.org/wiki/Value_noise>`__.
+        'cubic'    Cubic interpolation of white noise. For more information on
+                   ``cubic noise`` see
+                   `here <https://github.com/jobtalle/CubicNoise>`__.
+        ========== ==================================================================
 
     seed : int, optional
         The seed of the random number generator.  Using the same
         ``seed`` between runs will produce the same image.
     cores : int, optional
         The number of cores to use. This function uses ``pyfastnoisesimd``,
         which has implemented SIMD processing which can be spread across
@@ -56,26 +73,14 @@
     the `pyfastnoisesimd <https://github.com/robbmcleod/pyfastnoisesimd>`_
     package. ``pyfastnoisesimd`` is itself a wrapper for a C-library
     called `FastNoiseSIMD <https://github.com/Auburn/FastNoiseSIMD>`_.
     To access the more elaborate functionality and options of these
     packages, explore the `pyfastnoisesimd documentation
     <https://pyfastnoisesimd.readthedocs.io/en/latest/overview.html>`_.
 
-    For more information on ``simplex noise`` see
-    `here <https://en.wikipedia.org/wiki/Simplex_noise>`__.
-
-    For more information on ``perlin noise`` see
-    `here <https://en.wikipedia.org/wiki/Perlin_noise>`__.
-
-    For more information on ``value noise`` see
-    `here <https://en.wikipedia.org/wiki/Value_noise>`__.
-
-    For more information on ``cubic noise`` see
-    `here <https://github.com/jobtalle/CubicNoise>`__.
-
     Examples
     --------
     `Click here
     <https://porespy.org/examples/generators/reference/fractal_noise.html>`_
     to view online example.
 
     """
```

### Comparing `porespy-2.2.2/porespy/generators/_pseudo_packings.py` & `porespy-2.3.0/porespy/generators/_pseudo_packings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,44 @@
 import logging
-import numba
 import numpy as np
 import scipy.ndimage as spim
 from edt import edt
 from skimage.morphology import disk, ball
 from porespy import settings
 from porespy.tools import get_tqdm, ps_round, get_border
 from porespy.tools import _insert_disks_at_points
 from porespy.filters import trim_disconnected_blobs, fftmorphology
-import random
+# import random
+from numba import njit
+
+
+__all__ = [
+    "pseudo_gravity_packing",
+    "pseudo_electrostatic_packing",
+]
 
 
 tqdm = get_tqdm()
 logger = logging.getLogger(__name__)
 
 
-def pseudo_gravity_packing(im, r, clearance=0, axis=0, maxiter=1000,
-                           edges='contained'):
+@njit
+def _set_seed(a):
+    np.random.seed(a)
+
+
+def pseudo_gravity_packing(
+    im,
+    r,
+    clearance=0,
+    axis=0,
+    maxiter=1000,
+    edges='contained',
+    seed=None,
+):
     r"""
     Iteratively inserts spheres at the lowest accessible point in an image,
     mimicking a gravity packing.
 
     Parameters
     ----------
     im : ndarray
@@ -33,23 +51,32 @@
         The amount space to add between neighboring spheres. The value can be
         negative for overlapping spheres, but ``abs(clearance) > r``.
     axis : int (default is 0)
         The axis along which gravity acts.
     maxiter : int (default is 1000)
         The maximum number of spheres to add
     edges : string (default is 'contained')
-        Controls how the edges of the image are handled.  Options are:
+        Controls how spheres at the edges of the image are handled.  Options are:
 
-        'contained'
-            Spheres are all completely within the image
-        'extended'
-            Spheres are allowed to extend beyond the edge of the
-            image.  In this mode the volume fraction will be less that
-            requested since some spheres extend beyond the image, but their
-            entire volume is counted as added for computational efficiency.
+        ============ ================================================================
+        edges        description
+        ============ ================================================================
+        'contained'  Spheres are all completely within the image
+        'extended'   Spheres are allowed to extend beyond the edge of the
+                     image.  In this mode the volume fraction will be less that
+                     requested since some spheres extend beyond the image, but their
+                     entire volume is counted as added for computational efficiency.
+        ============ ================================================================
+
+    seed : int, optional, default = `None`
+        The seed to supply to the random number generator. Because this function
+        uses ``numba`` for speed, calling the normal ``numpy.random.seed(<seed>)``
+        has no effect. To get a repeatable image, the seed must be passed to the
+        function so it can be initialized the way ``numba`` requires. The default
+        is ``None``, which means each call will produce a new realization.
 
     Returns
     -------
     spheres : ndarray
         An image the same size as ``im`` with spheres indicated by ``True``.
         The spheres are only inserted at locations that are accessible
         from the top of the image.
@@ -59,14 +86,18 @@
     `Click here
     <https://porespy.org/examples/generators/reference/pseudo_gravity_packing.html>`_
     to view online example.
 
     """
     logger.debug(f'Adding spheres of radius {r}')
 
+    if seed is not None:  # Initialize rng so numba sees it
+        _set_seed(seed)
+        np.random.seed(seed)
+
     im = np.swapaxes(im, 0, axis)
     im_temp = np.zeros_like(im, dtype=bool)
     r = r - 1
     strel = disk if im.ndim == 2 else ball
     sites = fftmorphology(im == 1, strel=strel(r), mode='erosion')
     inlets = np.zeros_like(im)
     inlets[-(r+1), ...] = True
@@ -98,19 +129,24 @@
                                         overwrite=True)
         x_min += x.min()
     logger.debug(f'A total of {n} spheres were added')
     im_temp = np.swapaxes(im_temp, 0, axis)
     return im_temp
 
 
-def pseudo_electrostatic_packing(im, r, sites=None,
-                                 clearance=0,
-                                 protrusion=0,
-                                 edges='extended',
-                                 maxiter=1000):
+def pseudo_electrostatic_packing(
+    im,
+    r,
+    sites=None,
+    clearance=0,
+    protrusion=0,
+    edges='extended',
+    maxiter=1000,
+    seed=None,
+):
     r"""
     Iterativley inserts spheres as close to the given sites as possible.
 
     Parameters
     ----------
     im : ndarray
         Image with ``True`` values indicating the phase where spheres should be
@@ -125,37 +161,49 @@
         The amount of space to put between each sphere. Negative values are
         acceptable to create overlaps, but ``abs(clearance) < r``.
     protrusion : int (optional, default=0)
         The amount that spheres are allowed to protrude beyond the active phase.
     maxiter : int (optional, default=1000)
         The maximum number of spheres to insert.
     edges : string (default is 'contained')
-        Controls how the edges of the image are handled.  Options are:
+        Controls how spheres at the edges of the image are handled.  Options are:
 
-        'contained'
-            Spheres are all completely within the image
-        'extended'
-            Spheres are allowed to extend beyond the edge of the
-            image.  In this mode the volume fraction will be less that
-            requested since some spheres extend beyond the image, but their
-            entire volume is counted as added for computational efficiency.
+        ============ ================================================================
+        edges        description
+        ============ ================================================================
+        'contained'  Spheres are all completely within the image
+        'extended'   Spheres are allowed to extend beyond the edge of the
+                     image.  In this mode the volume fraction will be less that
+                     requested since some spheres extend beyond the image, but their
+                     entire volume is counted as added for computational efficiency.
+        ============ ================================================================
+
+    seed : int, optional, default = `None`
+        The seed to supply to the random number generator. Because this function
+        uses ``numba`` for speed, calling the normal ``numpy.random.seed(<seed>)``
+        has no effect. To get a repeatable image, the seed must be passed to the
+        function so it can be initialized the way ``numba`` requires. The default
+        is ``None``, which means each call will produce a new realization.
 
     Returns
     -------
     im : ndarray
         An image with inserted spheres indicated by ``True``
 
     Examples
     --------
     `Click here
     <https://porespy.org/examples/generators/reference/pseudo_electrostatic_packing.html>`_
     to view online example.
 
     """
-    random.seed(0)
+    if seed is not None:  # Initialize rng so numba sees it
+        _set_seed(seed)
+        np.random.seed(seed)
+
     im_temp = np.zeros_like(im, dtype=bool)
     dt_im = edt(im)
     if sites is None:
         dt2 = spim.gaussian_filter(dt_im, sigma=0.5)
         strel = ps_round(r, ndim=im.ndim, smooth=True)
         sites = (spim.maximum_filter(dt2, footprint=strel) == dt2)*im
     dt = edt(sites == 0).astype(int)
@@ -169,22 +217,22 @@
         borders = get_border(im.shape, thickness=r, mode='faces')
         dt[borders] = dtmax
     r = r + clearance
     # Get initial options
     options = np.where(dt == 1)
     for _ in tqdm(range(maxiter), **settings.tqdm):
         hits = dt[options] < dtmax
-        if hits.sum() == 0:
+        if hits.sum(dtype=np.int64) == 0:
             if dt.min() == dtmax:
                 break
             options = np.where(dt == dt.min())
             hits = dt[options] < dtmax
         if hits.size == 0:
             break
-        choice = random.choice(np.where(hits)[0])
+        choice = np.random.choice(np.where(hits)[0])
         cen = np.vstack([options[i][choice] for i in range(im.ndim)])
         im_temp = _insert_disks_at_points(im_temp, coords=cen,
                                           radii=np.array([r-clearance]),
                                           v=True,
                                           overwrite=True)
         dt = _insert_disks_at_points(dt, coords=cen,
                                      radii=np.array([2*r-clearance]),
@@ -197,18 +245,18 @@
     import porespy as ps
     import matplotlib.pyplot as plt
     shape = [200, 200]
 
     fig, ax = plt.subplots(1, 2)
     im = ps.generators.pseudo_gravity_packing(im=np.ones(shape, dtype=bool),
                                               r=7, clearance=3,
-                                              edges='contained')
+                                              edges='contained', seed=0)
     ax[0].imshow(im, origin='lower')
 
     sites = np.zeros(shape, dtype=bool)
     sites[100, 100] = True
     im = ps.generators.pseudo_electrostatic_packing(im=np.ones(shape,
                                                                dtype=bool),
                                                     r=5, sites=sites,
                                                     clearance=4,
-                                                    maxiter=50)
+                                                    maxiter=50, seed=0)
     ax[1].imshow(im, origin='lower')
```

### Comparing `porespy-2.2.2/porespy/io/__init__.py` & `porespy-2.3.0/porespy/io/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,7 +24,8 @@
 from ._funcs import dict_to_vtk
 from ._funcs import to_palabos
 from ._funcs import openpnm_to_im
 from ._funcs import to_stl
 from ._funcs import to_paraview
 from ._funcs import open_paraview
 from ._funcs import spheres_to_comsol
+from ._unzipper import *
```

### Comparing `porespy-2.2.2/porespy/io/_comsol.py` & `porespy-2.3.0/porespy/io/_comsol.py`

 * *Files identical despite different names*

### Comparing `porespy-2.2.2/porespy/io/_funcs.py` & `porespy-2.3.0/porespy/io/_funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import os
-import imageio
 import subprocess
 import numpy as np
-from stl import mesh
 import scipy.ndimage as nd
 import skimage.measure as ms
 from porespy.tools import sanitize_filename
 from porespy.networks import generate_voxel_image
 from porespy.filters import reduce_peaks
-from pyevtk.hl import imageToVTK
 from skimage.morphology import ball
 from edt import edt
 
 
 def dict_to_vtk(data, filename, voxel_size=1, origin=(0, 0, 0)):
     r"""
     Accepts multiple images as a dictionary and compiles them into a vtk file
@@ -37,14 +34,19 @@
     Examples
     --------
     `Click here
     <https://porespy.org/examples/io/reference/dict_to_vtk.html>`_
     to view online example.
 
     """
+    try:
+        from pyevtk.hl import imageToVTK
+    except ModuleNotFoundError:
+        msg = 'The pyevtk package can be installed with pip install pyevtk'
+        raise ModuleNotFoundError(msg)
     vs = voxel_size
     for entry in data:
         if data[entry].dtype == bool:
             data[entry] = data[entry].astype(np.int8)
         if data[entry].flags["C_CONTIGUOUS"]:
             data[entry] = np.ascontiguousarray(data[entry])
     imageToVTK(filename, cellData=data, spacing=(vs, vs, vs), origin=origin)
@@ -81,14 +83,19 @@
     Examples
     --------
     `Click here
     <https://porespy.org/examples/io/reference/to_vtk.html>`_
     to view online example.
 
     """
+    try:
+        from pyevtk.hl import imageToVTK
+    except ModuleNotFoundError:
+        msg = 'The pyevtk package can be installed with pip install pyevtk'
+        raise ModuleNotFoundError(msg)
     if len(im.shape) == 2:
         im = im[:, :, np.newaxis]
     if im.dtype == bool:
         vox = True
     if vox:
         im = im.astype(np.int8)
     vs = voxel_size
@@ -274,14 +281,19 @@
         The image of the porous material
     voxel_size : int
         The side length of the voxels (voxels are cubic)
     filename : string
         Path to output file
 
     """
+    try:
+        from stl import mesh
+    except ModuleNotFoundError:
+        msg = 'numpy-stl can be installed with pip install numpy-stl'
+        ModuleNotFoundError(msg)
     im = np.pad(im, pad_width=10, mode="constant", constant_values=True)
     vertices, faces, norms, values = ms.marching_cubes(im)
     vertices *= vs
     # Export the STL file
     export = mesh.Mesh(np.zeros(faces.shape[0], dtype=mesh.Mesh.dtype))
     for i, f in enumerate(faces):
         for j in range(3):
@@ -312,14 +324,19 @@
     --------
     `Click here
     <https://porespy.org/examples/io/reference/to_paraview.html>`_
     to view online example.
 
     """
     try:
+        import imageio
+    except ModuleNotFoundError:
+        msg = "The imageio package can be installed with pip install imageio"
+        raise ModuleNotFoundError(msg)
+    try:
         import paraview.simple
     except ModuleNotFoundError:
         msg = ("The paraview python bindings must be installed using conda"
                " install -c conda-forge paraview, however this may require"
                " using a virtualenv since conflicts with other packages are"
                " common. This is why it is not explicitly included as a"
                " dependency in porespy.")
```

### Comparing `porespy-2.2.2/porespy/metrics/_funcs.py` & `porespy-2.3.0/porespy/metrics/_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,109 @@
 from porespy.tools import _check_for_singleton_axes
 from porespy.tools import Results
 from porespy import settings
 from porespy.tools import get_tqdm
 from numba import njit
 
 
+__all__ = [
+    "boxcount",
+    "chord_counts",
+    "chord_length_distribution",
+    "find_h",
+    "lineal_path_distribution",
+    "pore_size_distribution",
+    "radial_density_distribution",
+    "porosity",
+    "porosity_profile",
+    "representative_elementary_volume",
+    "satn_profile",
+    "two_point_correlation",
+    "phase_fraction",
+    "pc_curve",
+    "pc_curve_from_ibip",
+    "pc_curve_from_mio",
+]
+
+
 tqdm = get_tqdm()
 logger = logging.getLogger(__name__)
 
 
+def boxcount(im, bins=10):
+    r"""
+    Calculates fractal dimension of an image using the tiled box counting
+    method [1]_
+
+    Parameters
+    ----------
+    im : ndarray
+        The image of the porous material.
+    bins : int or array_like, optional
+        The number of box sizes to use. The default is 10 sizes
+        logarithmically spaced between 1 and ``min(im.shape)``.
+        If an array is provided, this is used directly.
+
+    Returns
+    -------
+    results
+        An object possessing the following attributes:
+
+        size : ndarray
+            The box sizes used
+        count : ndarray
+            The number of boxes of each size that contain both solid and void
+        slope : ndarray
+            The gradient of ``count``. This has the same number of elements as
+            ``count`` and
+
+    References
+    ----------
+    .. [1] See Boxcounting on `Wikipedia <https://en.wikipedia.org/wiki/Box_counting>`_
+
+    Examples
+    --------
+    `Click here
+    <https://porespy.org/examples/metrics/reference/box_counting.html>`_
+    to view online example.
+
+    """
+    im = np.array(im, dtype=bool)
+
+    if (len(im.shape) != 2 and len(im.shape) != 3):
+        raise Exception('Image must be 2-dimensional or 3-dimensional')
+
+    if isinstance(bins, int):
+        Ds = np.unique(np.logspace(1, np.log10(min(im.shape)), bins).astype(int))
+    else:
+        Ds = np.array(bins).astype(int)
+
+    N = []
+    for d in tqdm(Ds, **settings.tqdm):
+        result = 0
+        for i in range(0, im.shape[0], d):
+            for j in range(0, im.shape[1], d):
+                if len(im.shape) == 2:
+                    temp = im[i:i+d, j:j+d]
+                    result += np.any(temp)
+                    result -= np.all(temp)
+                else:
+                    for k in range(0, im.shape[2], d):
+                        temp = im[i:i+d, j:j+d, k:k+d]
+                        result += np.any(temp)
+                        result -= np.all(temp)
+        N.append(result)
+    slope = -1*np.gradient(np.log(np.array(N)), np.log(Ds))
+    data = Results()
+    data.size = Ds
+    data.count = N
+    data.slope = slope
+    return data
+
+
 def representative_elementary_volume(im, npoints=1000):
     r"""
     Calculates the porosity of an image as a function subdomain size.
 
     This function extracts a specified number of subdomains of random size,
     then finds their porosity.
 
@@ -77,15 +168,15 @@
     porosity = np.zeros(shape=(N,), dtype=float)
     volume = np.zeros(shape=(N,), dtype=int)
     for i in tqdm(np.arange(0, N), **settings.tqdm):
         s = slices[i]
         p = pads[i]
         new_s = extend_slice(s, shape=im.shape, pad=p)
         temp = im[new_s]
-        Vp = np.sum(temp)
+        Vp = np.sum(temp, dtype=np.int64)
         Vt = np.size(temp)
         porosity[i] = Vp / Vt
         volume[i] = Vt
     profile = Results()
     profile.volume = volume
     profile.porosity = porosity
     return profile
@@ -130,17 +221,17 @@
     Examples
     --------
     `Click here
     <https://porespy.org/examples/metrics/reference/porosity.html>`_
     to view online example.
 
     """
-    im = np.array(im, dtype=int)
-    Vp = np.sum(im == 1)
-    Vs = np.sum(im == 0)
+    im = np.array(im, dtype=np.int64)
+    Vp = np.sum(im == 1, dtype=np.int64)
+    Vs = np.sum(im == 0, dtype=np.int64)
     e = Vp / (Vs + Vp)
     return e
 
 
 def porosity_profile(im, axis=0):
     r"""
     Computes the porosity profile along the specified axis
@@ -168,15 +259,16 @@
 
     """
     if axis >= im.ndim:
         raise Exception('axis out of range')
     im = np.atleast_3d(im)
     a = set(range(im.ndim)).difference(set([axis]))
     a1, a2 = a
-    prof = np.sum(np.sum(im == 1, axis=a2), axis=a1) / (im.shape[a2] * im.shape[a1])
+    tmp = np.sum(np.sum(im == 1, axis=a2, dtype=np.int64), axis=a1, dtype=np.int64)
+    prof = tmp / (im.shape[a2] * im.shape[a1])
     return prof
 
 
 def radial_density_distribution(dt, bins=10, log=False, voxel_size=1):
     r"""
     Computes radial density function by analyzing the histogram of voxel
     values in the distance transform.  This function is defined by
@@ -438,16 +530,18 @@
     if bins is None:
         bins = np.array(range(0, x.max() + 2)) * voxel_size
     x = x * voxel_size
     if log:
         x = np.log10(x)
     if normalization == 'length':
         h = list(np.histogram(x, bins=bins, density=False))
-        h[0] = h[0] * (h[1][1:] + h[1][:-1]) / 2  # Scale bin heigths by length
-        h[0] = h[0] / h[0].sum() / (h[1][1:] - h[1][:-1])  # Normalize h[0] manually
+        # Scale bin heigths by length
+        h[0] = h[0] * (h[1][1:] + h[1][:-1]) / 2
+        # Normalize h[0] manually
+        h[0] = h[0] / h[0].sum(dtype=np.int64) / (h[1][1:] - h[1][:-1])
     elif normalization in ['number', 'count']:
         h = np.histogram(x, bins=bins, density=True)
     else:
         raise Exception('Unsupported normalization:', normalization)
     h = _parse_histogram(h)
     cld = Results()
     cld[f"{log*'Log' + 'L'}"] = h.bin_centers
@@ -670,20 +764,21 @@
     tpcf.probability = norm_autoc_radial
     tpcf.probability_scaled = norm_autoc_radial * pf
     tpcf.pdf = h.pdf * pf
     tpcf.relfreq = h.relfreq
     return tpcf
 
 
-@njit(parallel=True)
+@njit(parallel=False)
 def _get_radial_sum(dt, bins, bin_size, autocorr):
     radial_sum = np.zeros_like(bins[:-1])
     for i, r in enumerate(bins[:-1]):
         mask = (dt <= r) * (dt > (r - bin_size[i]))
-        radial_sum[i] = np.sum(np.ravel(autocorr)[np.ravel(mask)]) / np.sum(mask)
+        radial_sum[i] = np.sum(np.ravel(autocorr)[np.ravel(mask)], dtype=np.int64) \
+            / np.sum(mask)
     return radial_sum
 
 
 def two_point_correlation(im, voxel_size=1, bins=100):
     r"""
     Calculate the two-point correlation function using Fourier transforms
 
@@ -814,15 +909,15 @@
     `Click here
     <https://porespy.org/examples/reference/metrics/chord_counts.html>`_
     to view online example.
 
     """
     labels, N = spim.label(im > 0)
     props = regionprops(labels)
-    chord_lens = np.array([i.filled_area for i in props])
+    chord_lens = np.array([i.filled_area for i in props], dtype=int)
     return chord_lens
 
 
 def phase_fraction(im, normed=True):
     r"""
     Calculate the fraction of each phase in an image
 
@@ -853,15 +948,16 @@
 
     """
     if im.dtype == bool:
         im = im.astype(int)
     labels = np.unique(im)
     results = {}
     for label in labels:
-        results[label] = np.sum(im == label) * (1 / im.size if normed else 1)
+        results[label] = np.sum(im == label, dtype=np.int64) * \
+            (1 / im.size if normed else 1)
     return results
 
 
 @deprecated("This function is deprecated, use pc_curve instead")
 def pc_curve_from_ibip(*args, **kwargs):
     r"""
     This function is deprecated.  Use ``pc_curve`` instead.  Note that the
@@ -959,15 +1055,16 @@
             for n in seqs:
                 pbar.update()
                 mask = seq == n
                 # The following assumes only one size found, which was confirmed
                 r = sizes[mask][0]*voxel_size
                 pc = -2*sigma*np.cos(np.deg2rad(theta))/r
                 x.append(pc)
-                snwp = ((seq <= n)*(seq > 0)*(im == 1)).sum()/im.sum()
+                snwp = ((seq <= n)*(seq > 0) *
+                        (im == 1)).sum(dtype=np.int64)/im.sum(dtype=np.int64)
                 y.append(snwp)
         pc_curve = Results()
         pc_curve.pc = x
         pc_curve.snwp = y
     elif sizes is not None:
         if im is None:
             im = ~(sizes == 0)
@@ -977,15 +1074,15 @@
         y = []
         with tqdm(sz, **settings.tqdm) as pbar:
             for n in sz:
                 pbar.update()
                 r = n*voxel_size
                 pc = -2*sigma*np.cos(np.deg2rad(theta))/r
                 x.append(pc)
-                snwp = ((sizes >= n)*(im == 1)).sum()/im.sum()
+                snwp = ((sizes >= n)*(im == 1)).sum(dtype=np.int64)/im.sum(dtype=np.int64)
                 y.append(snwp)
         pc_curve = Results()
         pc_curve.pc = x
         pc_curve.snwp = y
     elif pc is not None:
         Ps = np.unique(pc[im])
         # Utilize the fact that -inf and +inf will be at locations 0 & -1 in Ps
@@ -993,18 +1090,18 @@
             Ps[-1] = Ps[-2]*2
         if Ps[0] == -np.inf:
             Ps[0] = Ps[1] - np.abs(Ps[1]/2)
         else:
             # Add a point at begining to ensure curve starts a 0, if no residual
             Ps = np.hstack((Ps[0] - np.abs(Ps[0]/2), Ps))
         y = []
-        Vp = im.sum()
+        Vp = im.sum(dtype=np.int64)
         temp = pc[im]
         for p in tqdm(Ps, **settings.tqdm):
-            y.append((temp <= p).sum()/Vp)
+            y.append((temp <= p).sum(dtype=np.int64)/Vp)
         pc_curve = Results()
         pc_curve.pc = Ps
         pc_curve.snwp = y
     return pc_curve
 
 
 def satn_profile(satn, s, axis=0, span=10, mode='tile'):
@@ -1063,23 +1160,23 @@
         if mode == 'tile':
             y = np.zeros(int(satn.shape[0]/span))
             z = np.zeros_like(y)
             for i in range(int(satn.shape[0]/span)):
                 void = satn[i*span:(i+1)*span, ...] != 0
                 nwp = (satn[i*span:(i+1)*span, ...] < s) \
                     *(satn[i*span:(i+1)*span, ...] > 0)
-                y[i] = nwp.sum()/void.sum()
+                y[i] = nwp.sum(dtype=np.int64)/void.sum(dtype=np.int64)
                 z[i] = i*span + (span-1)/2
         if mode == 'slide':
             y = np.zeros(int(satn.shape[0]-span))
             z = np.zeros_like(y)
             for i in range(int(satn.shape[0]-span)):
                 void = satn[i:i+span, ...] != 0
                 nwp = (satn[i:i+span, ...] < s)*(satn[i:i+span, ...] > 0)
-                y[i] = nwp.sum()/void.sum()
+                y[i] = nwp.sum(dtype=np.int64)/void.sum(dtype=np.int64)
                 z[i] = i + (span-1)/2
         return z, y
 
     z, y = func(satn=satn, s=s, axis=axis, span=span, mode=mode)
 
     class results(Results):
         r"""
```

### Comparing `porespy-2.2.2/porespy/metrics/_meshtools.py` & `porespy-2.3.0/porespy/metrics/_meshtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 import logging
 import numpy as np
 import scipy.ndimage as spim
-from trimesh import Trimesh
 from porespy.tools import extend_slice, ps_round
 from porespy.tools import _check_for_singleton_axes, Results
 from porespy.tools import mesh_region
 from skimage import measure
 from porespy.tools import get_tqdm
 from porespy import settings
 
 
+__all__ = [
+    "mesh_surface_area",
+    "mesh_volume",
+    "region_interface_areas",
+    "region_surface_areas",
+    "region_volumes",
+]
+
+
 tqdm = get_tqdm()
 logger = logging.getLogger(__name__)
 
 
 def region_volumes(regions, mode='marching_cubes'):
     r"""
     Compute volume of each labelled region in an image
@@ -51,15 +59,15 @@
     vols = np.zeros([len(slices), ])
     msg = "Computing region volumes".ljust(60)
     for i, s in enumerate(tqdm(slices, desc=msg, **settings.tqdm)):
         region = regions[s] == (i + 1)
         if mode == 'marching_cubes':
             vols[i] = mesh_volume(region)
         elif mode.startswith('voxel'):
-            vols[i] = region.sum()
+            vols[i] = region.sum(dtype=np.int64)
     return vols
 
 
 def mesh_volume(region):
     r"""
     Compute the volume of a single region by meshing it
 
@@ -78,14 +86,19 @@
     Examples
     --------
     `Click here
     <https://porespy.org/examples/metrics/reference/mesh_volume.html>`_
     to view online example.
 
     """
+    try:
+        from trimesh import Trimesh
+    except ModuleNotFoundError:
+        msg = 'The trimesh package can be installed with pip install trimesh'
+        raise ModuleNotFoundError(msg)
     mc = mesh_region(region > 0)
     m = Trimesh(vertices=mc.verts, faces=mc.faces, vertex_normals=mc.norm)
     if m.is_watertight:
         vol = np.abs(m.volume)
     else:
         vol = np.nan
     return vol
```

### Comparing `porespy-2.2.2/porespy/metrics/_regionprops.py` & `porespy-2.3.0/porespy/metrics/_regionprops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 from skimage.morphology import skeletonize_3d, ball
 from skimage.measure import regionprops
 from skimage.measure._regionprops import RegionProperties
 from pandas import DataFrame
 from edt import edt
 
 
+__all__ = [
+    "regionprops_3D",
+    "props_to_DataFrame",
+    "prop_to_image",
+]
+
+
 logger = logging.getLogger(__name__)
 
 
 def props_to_DataFrame(regionprops):
     r"""
     Create a ``pandas`` DataFrame containing all the scalar metrics for each
     region, such as volume, sphericity, and so on, calculated by
```

### Comparing `porespy-2.2.2/porespy/networks/__init__.py` & `porespy-2.3.0/porespy/networks/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,20 +19,13 @@
     networks.map_to_regions
     networks.maximal_ball_wrapper
     networks.regions_to_network
     networks.snow2
 
 """
 
-from ._funcs import add_boundary_regions
-from ._funcs import generate_voxel_image
-from ._funcs import label_phases
-from ._funcs import label_boundaries
-from ._funcs import map_to_regions
-from ._maximal_ball import maximal_ball_wrapper
-from ._getnet import regions_to_network
-from ._snow2 import snow2
-from ._utils import _net_dict
-from ._snow2 import _parse_pad_width
-from ._size_factors import diffusive_size_factor_AI
-from ._size_factors import create_model
-from ._size_factors import find_conns
+from ._funcs import *
+from ._maximal_ball import *
+from ._getnet import *
+from ._snow2 import *
+from ._utils import *
+from ._size_factors import *
```

### Comparing `porespy-2.2.2/porespy/networks/_funcs.py` & `porespy-2.3.0/porespy/networks/_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,23 @@
 from porespy.tools import overlay, extend_slice
 from porespy.tools import insert_cylinder
 from porespy.generators import borders
 from porespy import settings
 from porespy.tools import get_tqdm
 
 
+__all__ = [
+    "add_boundary_regions",
+    "generate_voxel_image",
+    "label_phases",
+    "label_boundaries",
+    "map_to_regions",
+]
+
+
 tqdm = get_tqdm()
 logger = logging.getLogger(__name__)
 
 
 def map_to_regions(regions, values):
     r"""
     Maps pore values from a network onto the image from which it was extracted
@@ -256,15 +265,15 @@
     # If max_dim is not provided, find best max_dim that predicts porosity
     err = 100
     eps_old = 200
     while err > rtol:
         logger.debug(f"Maximum dimension: {max_dim} voxels")
         im = _generate_voxel_image(
             network, pore_shape, throat_shape, max_dim=max_dim)
-        eps = im.astype(bool).sum() / np.prod(im.shape)
+        eps = im.astype(bool).sum(dtype=np.int64) / np.prod(im.shape)
         err = abs(1 - eps / eps_old)
         eps_old = eps
         max_dim = int(max_dim * 1.25)
     logger.debug(f"Converged at max_dim = {max_dim} voxels")
     return im
```

### Comparing `porespy-2.2.2/porespy/networks/_getnet.py` & `porespy-2.3.0/porespy/networks/_getnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from porespy.tools import extend_slice
 from porespy import settings
 from porespy.tools import get_tqdm, make_contiguous
 from porespy.metrics import region_surface_areas, region_interface_areas
 from porespy.metrics import region_volumes
 
 
+__all__ = [
+    "regions_to_network",
+]
+
+
 tqdm = get_tqdm()
 logger = logging.getLogger(__name__)
 
 
 def regions_to_network(regions, phases=None, voxel_size=1, accuracy='standard'):
     r"""
     Analyzes an image that has been partitioned into pore regions and extracts
@@ -169,29 +174,29 @@
         p_label[pore] = i
         p_coords_cm[pore, :] = spim.center_of_mass(pore_im) + s_offset
         temp = np.vstack(np.where(pore_dt == pore_dt.max()))[:, 0]
         p_coords_dt[pore, :] = temp + s_offset
         p_phase[pore] = (phases[s]*pore_im).max()
         temp = np.vstack(np.where(sub_dt == sub_dt.max()))[:, 0]
         p_coords_dt_global[pore, :] = temp + s_offset
-        p_volume[pore] = np.sum(pore_im)
+        p_volume[pore] = np.sum(pore_im, dtype=np.int64)
         p_dia_local[pore] = 2*np.amax(pore_dt)
         p_dia_global[pore] = 2*np.amax(sub_dt)
         # The following is overwritten if accuracy is set to 'high'
-        p_area_surf[pore] = np.sum(pore_dt == 1)
+        p_area_surf[pore] = np.sum(pore_dt == 1, dtype=np.int64)
         im_w_throats = spim.binary_dilation(input=pore_im, structure=struc_elem(1))
         im_w_throats = im_w_throats*sub_im
         Pn = np.unique(im_w_throats)[1:] - 1
         for j in Pn:
             if j > pore:
                 t_conns.append([pore, j])
                 vx = np.where(im_w_throats == (j + 1))
                 t_dia_inscribed.append(2*np.amax(sub_dt[vx]))
                 # The following is overwritten if accuracy is set to 'high'
-                t_perimeter.append(np.sum(sub_dt[vx] < 2))
+                t_perimeter.append(np.sum(sub_dt[vx] < 2, dtype=np.int64))
                 # The following is overwritten if accuracy is set to 'high'
                 t_area.append(np.size(vx[0]))
                 p_area_surf[pore] -= np.size(vx[0])
                 t_inds = tuple([i+j for i, j in zip(vx, s_offset)])
                 temp = np.where(dt[t_inds] == np.amax(dt[t_inds]))[0][0]
                 t_coords.append(tuple([t_inds[k][temp] for k in range(im.ndim)]))
 
@@ -229,15 +234,15 @@
                          axis=1))
     PT2 = np.sqrt(np.sum(((p_coords[P12[:, 1]]-t_coords)*voxel_size)**2,
                          axis=1))
     net['throat.total_length'] = PT1 + PT2
     PT1 = PT1-p_dia_local[P12[:, 0]]/2*voxel_size
     PT2 = PT2-p_dia_local[P12[:, 1]]/2*voxel_size
     dist = (p_coords[P12[:, 0]] - p_coords[P12[:, 1]])*voxel_size
-    net['throat.direct_length'] = np.sqrt(np.sum(dist**2, axis=1))
+    net['throat.direct_length'] = np.sqrt(np.sum(dist**2, axis=1, dtype=np.int64))
     net['throat.perimeter'] = np.array(t_perimeter)*voxel_size
     if (accuracy == 'high') and (im.ndim == 2):
         msg = "accuracy='high' only available in 3D, reverting to 'standard'"
         logger.warning(msg)
         accuracy = 'standard'
     if (accuracy == 'high'):
         net['pore.volume'] = region_volumes(regions=im, mode='marching_cubes')
```

### Comparing `porespy-2.2.2/porespy/networks/_maximal_ball.py` & `porespy-2.3.0/porespy/networks/_maximal_ball.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import logging
 import os
 import time
 import psutil
 import subprocess
 import numpy as np
-import imageio
+
+
+__all__ = [
+    "maximal_ball_wrapper",
+]
 
 
 logger = logging.getLogger(__name__)
 
 
 def maximal_ball_wrapper(im, prefix, path_to_exe, voxel_size=1e-6):
     r"""
@@ -31,14 +35,19 @@
     outputs four DAT files:
         prefix_link1, prefix_link2, prefix_node1, prefix_node2
 
     This function only runs on Windows since the Windows compatible binary is
     provided by the Imperial College team.
 
     """
+    try:
+        import imageio
+    except ModuleNotFoundError:
+        msg = "The imageio package can be installed with pip install imageio"
+        raise ModuleNotFoundError(msg)
     file = os.path.splitext(prefix)[0]
     imageio.volsave(file + ".tif", np.array(im.astype("uint8")))
     with open(f"{file}.mhd", "w") as f:
         f.write("ObjectType =  Image\n\
                  NDims =	   3 \n\
                  ElementType = MET_UCHAR \n\
                  DimSize = " + str(im.shape[0]) + " " + str(im.shape[1]) + " " +
```

### Comparing `porespy-2.2.2/porespy/networks/_snow2.py` & `porespy-2.3.0/porespy/networks/_snow2.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 from porespy.networks import regions_to_network
 from porespy.networks import add_boundary_regions
 from porespy.networks import label_phases, label_boundaries
 from porespy.filters import snow_partitioning, snow_partitioning_parallel
 from porespy.tools import Results
 
 
+__all__ = [
+    "snow2",
+    "_parse_pad_width",
+]
+
+
 logger = logging.getLogger(__name__)
 
 
 def snow2(phases,
           phase_alias=None,
           boundary_width=3,
           accuracy='standard',
@@ -234,8 +240,8 @@
         if np.size(elem) == 1:
             tmp.append(np.tile(np.array(elem).item(), 2))
         elif np.size(elem) == 2 and np.ndim(elem) == 1:
             tmp.append(elem)
         else:
             raise Exception("pad_width components can't have 2+ elements")
 
-    return np.array(tmp)
+    return np.array(tmp, dtype=int)
```

### Comparing `porespy-2.2.2/porespy/simulations/_dns.py` & `porespy-2.3.0/porespy/simulations/_dns.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import numpy as np
 import openpnm as op
 from porespy.filters import trim_nonpercolating_paths
 from porespy.tools import Results
 from porespy.generators import faces
 
+
 logger = logging.getLogger(__name__)
 ws = op.Workspace()
 
 
 __all__ = ['tortuosity_fd']
 
 
@@ -54,24 +55,26 @@
 
     """
     if axis > (im.ndim - 1):
         raise Exception(f"'axis' must be <= {im.ndim}")
     openpnm_v3 = op.__version__.startswith('3')
 
     # Obtain original porosity
-    eps0 = im.sum() / im.size
+    eps0 = im.sum(dtype=np.int64) / im.size
 
     # Remove floating pores
     inlets = faces(im.shape, inlet=axis)
     outlets = faces(im.shape, outlet=axis)
     im = trim_nonpercolating_paths(im, inlets=inlets, outlets=outlets)
     # Check if porosity is changed after trimmimg floating pores
-    eps = im.sum() / im.size
+    eps = im.sum(dtype=np.int64) / im.size
+    if not eps:
+        raise Exception('No pores remain after trimming floating pores')
     if eps < eps0:  # pragma: no cover
-        logger.warning(f'Found non-percolating regions, were filled to percolate')
+        logger.warning('Found non-percolating regions, were filled to percolate')
 
     # Generate a Cubic network to be used as an orthogonal grid
     net = op.network.CubicTemplate(template=im, spacing=1.0)
     if openpnm_v3:
         phase = op.phase.Phase(network=net)
     else:
         phase = op.phases.GenericPhase(network=net)
```

### Comparing `porespy-2.2.2/porespy/simulations/_drainage.py` & `porespy-2.3.0/porespy/simulations/_drainage.py`

 * *Files identical despite different names*

### Comparing `porespy-2.2.2/porespy/tools/__init__.py` & `porespy-2.3.0/porespy/tools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,16 +43,14 @@
     tools.subdivide
     tools.unpad
 
 """
 
 from ._funcs import *
 from ._utils import *
-from ._funcs import _check_for_singleton_axes
-from ._unpad import unpad
 from ._sphere_insertions import *
 
 
 def _get_version():
     from porespy.__version__ import __version__ as ver
     suffix = ".dev0"
     if ver.endswith(suffix):
```

### Comparing `porespy-2.2.2/porespy/tools/_funcs.py` & `porespy-2.3.0/porespy/tools/_funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 import numpy as np
 import scipy.ndimage as spim
 from scipy.special import erfc
 from skimage.segmentation import relabel_sequential
 from edt import edt
 from skimage.morphology import ball, disk
 from ._utils import Results
-from ._unpad import unpad
 try:
     from skimage.measure import marching_cubes
 except ImportError:
     from skimage.measure import marching_cubes_lewiner as marching_cubes
 
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
+    '_check_for_singleton_axes',
     'align_image_with_openpnm',
     'bbox_to_slices',
     'extend_slice',
     'extract_cylinder',
     'extract_subsection',
     'extract_regions',
     'find_outer_region',
+    'find_bbox',
     'get_border',
     'get_planes',
     'insert_cylinder',
     'insert_sphere',
     'in_hull',
     'isolate_object',
     'marching_map',
@@ -38,17 +39,110 @@
     'randomize_colors',
     'recombine',
     'ps_ball',
     'ps_disk',
     'ps_rect',
     'ps_round',
     'subdivide',
+    'unpad',
 ]
 
 
+def unpad(im, pad_width):
+    r"""
+    Remove padding from a previously padded image given original pad widths
+
+    Parameters
+    ----------
+    im : ndarray
+        The padded image from which padding should be removed
+    pad_width : int or list of ints
+        The amount of padding previously added to each axis. This should be
+        the same as the values used to add original padding. Refer to
+        ``numpy.pad`` documentation for more details.
+
+    Notes
+    -----
+    A use case for this is when using ``skimage.morphology.skeletonize_3d``
+    to ensure that the skeleton extends beyond the edges of the image, but the
+    padding should be subsequently removed.
+
+    Examples
+    --------
+    `Click here
+    <https://porespy.org/examples/tools/reference/unpad.html>`_
+    to view online example.
+
+    """
+    pad_width = np.asarray(pad_width).squeeze()
+
+    if pad_width.ndim == 0:
+        new_pad_width = []
+        for r in range(0, len(im.shape)):
+            new_pad_width.append(pad_width)
+        pad_width = np.array(new_pad_width)
+
+    if pad_width.ndim == 1:
+        shape = im.shape - pad_width[0] - pad_width[1]
+        if shape[0] < 1:
+            shape = np.array(im.shape) * shape
+        s_im = []
+        for dim in range(im.ndim):
+            lower_im = pad_width[0]
+            upper_im = shape[dim] + pad_width[0]
+            s_im.append(slice(int(lower_im), int(upper_im)))
+
+    if pad_width.ndim == 2:
+        shape = np.asarray(im.shape)
+        s_im = []
+        for dim in range(im.ndim):
+            shape[dim] = im.shape[dim] - pad_width[dim][0] - pad_width[dim][1]
+            lower_im = pad_width[dim][0]
+            upper_im = shape[dim] + pad_width[dim][0]
+            s_im.append(slice(int(lower_im), int(upper_im)))
+
+    return im[tuple(s_im)]
+
+
+def find_bbox(im, order_by='axis'):
+    r"""
+    Finds the lower and upper corner surrounding the foreground in the image
+
+    Parameters
+    ----------
+    im : ndarray
+        The image containing the features around which the bounding box is sought
+    order_by : string
+        How the coords are returned.  Options are:
+
+        ========= ==================================================================
+        option    description
+        ========= ==================================================================
+        axis      The values are sorted by axes first, like
+                  ``[x_min, x_max], [y_min, y_max], [z_min, z_max]``.
+        corner    The values are sorted as lower corner first followed by upper
+                  corner, like ``[x_min, y_min, z_min], [x_max, y_max, z_max]``.
+        ========= ==================================================================
+
+    Returns
+    -------
+    bbox : list or list-of-lists
+        The corners of the bounding box around the forground of the image
+
+    """
+    # This might not be super fast, but I'm not sure of a faster way. There are
+    # a few suggestions on stackoverflow but I can't see how they'd be faster.
+    inds = np.where(im)
+    if order_by.startswith('ax'):
+        bbox = tuple([slice(np.amin(i), np.amax(i)+1, None) for i in inds])
+    elif order_by.startswith('corner'):
+        bbox = [[np.amin(i) for i in inds], [np.amax(i)+1 for i in inds]]
+    return bbox
+
+
 def isolate_object(region, i, s=None):
     r"""
     Given an image containing labels, removes all labels except the specified
     one.
 
     Parameters
     ----------
@@ -1244,15 +1338,15 @@
     im = np.pad(im, r)
     xyz_min = np.amin(xyz_line, axis=1) - r
     xyz_max = np.amax(xyz_line, axis=1) + r
     shape_template = xyz_max - xyz_min + 1
     template = np.zeros(shape=shape_template)
 
     # Shortcut for orthogonal cylinders
-    if (xyz0 == xyz1).sum() == 2:
+    if (xyz0 == xyz1).sum(dtype=np.int64) == 2:
         unique_dim = [xyz0[i] != xyz1[i] for i in range(3)].index(True)
         shape_template[unique_dim] = 1
         template_2D = disk(radius=r).reshape(shape_template)
         template = np.repeat(template_2D, repeats=L, axis=unique_dim)
         xyz_min[unique_dim] += r
         xyz_max[unique_dim] += -r
     else:
```

### Comparing `porespy-2.2.2/porespy/tools/_sphere_insertions.py` & `porespy-2.3.0/porespy/tools/_sphere_insertions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
-import numba
+from numba import njit
 
 
 __all__ = [
     '_make_disk',
     '_make_disks',
     '_make_ball',
     '_make_balls',
     '_insert_disk_at_points',
     '_insert_disks_at_points',
 ]
 
 
-@numba.jit(nopython=True, parallel=False)
+@njit(parallel=False)
 def _make_disks(r, smooth=True):  # pragma: no cover
     r"""
     Returns a list of disks from size 0 to ``r``
 
     Parameters
     ----------
     r : int
@@ -35,15 +35,15 @@
     disks = []
     for val in range(0, r):
         disk = _make_disk(val, smooth)
         disks.append(disk)
     return disks
 
 
-@numba.jit(nopython=True, parallel=False)
+@njit(parallel=False)
 def _make_balls(r, smooth=True):  # pragma: no cover
     r"""
     Returns a list of balls from size 0 to ``r``
 
     Parameters
     ----------
     r : int
@@ -62,15 +62,15 @@
     balls = []
     for val in range(0, r):
         ball = _make_ball(val, smooth)
         balls.append(ball)
     return balls
 
 
-@numba.jit(nopython=True, parallel=False)
+@njit(parallel=False)
 def _insert_disk_at_points(im, coords, r, v,
                            smooth=True, overwrite=False):  # pragma: no cover
     r"""
     Insert spheres (or disks) into the given ND-image at given locations
 
     This function uses numba to accelerate the process, and does not
     overwrite any existing values (i.e. only writes to locations containing
@@ -120,15 +120,15 @@
                                 if (z >= 0) and (z < zlim):
                                     if (s[a, b, c] == 1):
                                         if overwrite or (im[x, y, z] == 0):
                                             im[x, y, z] = v
     return im
 
 
-@numba.jit(nopython=True, parallel=False)
+@njit(parallel=False)
 def _insert_disks_at_points(im, coords, radii, v, smooth=True,
                             overwrite=False):  # pragma: no cover
     r"""
     Insert spheres (or disks) of specified radii into an ND-image at given locations.
 
     This function uses numba to accelerate the process, and does not overwrite
     any existing values (i.e. only writes to locations containing zeros).
@@ -181,15 +181,15 @@
                                 if (z >= 0) and (z < zlim):
                                     if s[a, b, c] == 1:
                                         if overwrite or (im[x, y, z] == 0):
                                             im[x, y, z] = v
     return im
 
 
-@numba.jit(nopython=True, parallel=False)
+@njit(parallel=False)
 def _make_disk(r, smooth=True):  # pragma: no cover
     r"""
     Generate a circular structuring element of the given radius
 
     Parameters
     ----------
     r : int
@@ -211,15 +211,15 @@
     for i in range(2*r+1):
         for j in range(2*r+1):
             if ((i - r)**2 + (j - r)**2)**0.5 <= thresh:
                 s[i, j] = 1
     return s
 
 
-@numba.jit(nopython=True, parallel=False)
+@njit(parallel=False)
 def _make_ball(r, smooth=True):  # pragma: no cover
     r"""
     Generate a spherical structuring element of the given radius
 
     Parameters
     ----------
     r : int
```

### Comparing `porespy-2.2.2/porespy/tools/_utils.py` & `porespy-2.3.0/porespy/tools/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
-import os
 import sys
 import numpy as np
 import importlib
 from dataclasses import dataclass
-from tqdm import tqdm
 import psutil
+import inspect
+import time
 
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("porespy")
 
 
 __all__ = [
     'sanitize_filename',
     'get_tqdm',
     'show_docstring',
     'Results',
@@ -88,14 +88,15 @@
                 "INFO" : 20,
                 "SUCESS" : 25,
                 "WARNING" : 30,
                 "ERROR" : 40,
                 "CRITICAL" : 50
             }
             value = options[value]
+        self._loglevel = value
         logger.setLevel(value)
 
     def __new__(cls):
         if Settings.__instance__ is None:
             Settings.__instance__ = super().__new__(cls)
         return Settings.__instance__
 
@@ -225,36 +226,43 @@
     A minimal class for use when returning multiple values from a function
 
     This class supports dict-like assignment and retrieval
     (``obj['im'] = im``), namedtuple-like attribute look-ups (``obj.im``),
     and generic class-like object assignment (``obj.im = im``)
 
     """
-    _value = "Description"
-    _key = "Item"
+
+    def __init__(self, **kwargs):
+        self._func = inspect.getouterframes(inspect.currentframe())[1].function
+        self._time = time.asctime()
 
     def __iter__(self):
-        for item in self.__dict__.values():
-            yield item
+        for k, v in self.__dict__.items():
+            if not k.startswith('_'):
+                yield v
 
     def __getitem__(self, key):
         return getattr(self, key)
 
     def __setitem__(self, key, value):
         self.__dict__[key] = value
 
     def __str__(self):
         header = "―" * 78
-        lines = [header, "{0:<25s} {1}".format(self._key, self._value), header]
+        lines = [
+            header,
+            f"Results of {self._func} generated at {self._time}",
+            header,
+        ]
         for item in list(self.__dict__.keys()):
             if item.startswith('_'):
                 continue
             if (isinstance(self[item], np.ndarray)):
                 s = np.shape(self[item])
-                if (self[item].ndim > 1):
-                    lines.append("{0:<25s} Image of size {1}".format(item, s))
-                else:
-                    lines.append("{0:<25s} Array of size {1}".format(item, s))
+                lines.append("{0:<25s} Array of size {1}".format(item, s))
+            elif hasattr(self[item], 'keys'):
+                N = len(self[item].keys())
+                lines.append("{0:<25s} Dictionary with {1} items".format(item, N))
             else:
                 lines.append("{0:<25s} {1}".format(item, self[item]))
         lines.append(header)
         return "\n".join(lines)
```

### Comparing `porespy-2.2.2/porespy/visualization/__init__.py` & `porespy-2.3.0/porespy/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `porespy-2.2.2/porespy/visualization/_funcs.py` & `porespy-2.3.0/porespy/visualization/_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,16 +197,17 @@
     for i, p in enumerate(Ps):
         temp = (satn <= p)*(satn > 0)
         im_data = prep_for_imshow(im=temp*2.0 - temp_old*1.0, mask=im,
                                   axis=axis, slice=slice)
         im_data.pop('vmax')
         [im_data.pop(i) for i in kwargs]
         ax[i // n][i % n].imshow(**im_data, vmax=2, **kwargs)
-        ax[i // n][i % n].set_title(str(np.around(temp.sum()/im.sum(),
-                                                  decimals=5)))
+        ax[i // n][i % n].set_title(
+            str(np.around(temp.sum(dtype=np.int64)/im.sum(dtype=np.int64),
+                          decimals=5)))
         temp_old = np.copy(temp)
     return fig, ax
 
 
 def prep_for_imshow(im, mask=None, axis=0, slice=None):
     r"""
     Adjusts the range of greyscale values in an image to improve visualization
```

### Comparing `porespy-2.2.2/porespy/visualization/_plots.py` & `porespy-2.3.0/porespy/visualization/_plots.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,61 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
+from porespy.tools import get_tqdm
 
 
 __all__ = [
     'bar',
     'imshow',
     'show_mesh',
+    'show_panels',
 ]
 
 
+tqdm = get_tqdm()
+
+
+def show_panels(im, rc=[3, 3], axis=0):
+    r"""
+    Show slices of a 3D image as a 2D array of panels.
+
+    Parameters
+    ----------
+    im : ndarray
+        The 3D image to visualize
+    rc : list if ints
+        The number of rows and columns to create
+    axis : int
+        The axis along which to create the slices
+
+    Returns
+    -------
+    fig, ax : Matplotlib figure and axis handles
+    """
+    from porespy.visualization import prep_for_imshow
+    i, j = rc
+    im = np.swapaxes(im, axis, 2)
+    slices = np.linspace(0, im.shape[2], i*j, endpoint=False).astype(int)
+    fig, ax = plt.subplots(i, j)
+    s = 0
+    for row in range(i):
+        for col in range(j):
+            temp = prep_for_imshow(im[..., slices[s]])
+            ax[row][col].imshow(**temp)
+            ax[row][col].text(
+                0, 1,
+                f"Slice {slices[s]}",
+                # ha="center", va="center",
+                bbox=dict(boxstyle="square,pad=0.3",
+                          fc="white", ec="white", lw=1, alpha=0.75))
+            s += 1
+    return fig, ax
+
+
 def bar(results, h='pdf', **kwargs):  # pragma: no cover
     r"""
     Convenience wrapper for matplotlib's ``bar``.
 
     This automatically:
 
         * fetches the ``bin_centers``
```

### Comparing `porespy-2.2.2/porespy/visualization/_views.py` & `porespy-2.3.0/porespy/visualization/_views.py`

 * *Files 8% similar despite different names*

```diff
@@ -179,9 +179,9 @@
     to view online example.
     """
     im = np.array(~im, dtype=int)
     if axis == 1:
         im = np.transpose(im, axes=[1, 0, 2])
     if axis == 2:
         im = np.transpose(im, axes=[2, 1, 0])
-    im = np.sum(im, axis=0)
+    im = np.sum(im, axis=0, dtype=np.int64)
     return im
```

### Comparing `porespy-2.2.2/porespy.egg-info/PKG-INFO` & `porespy-2.3.0/porespy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porespy
-Version: 2.2.2
+Version: 2.3.0
 Summary: A set of tools for analyzing 3D images of porous materials
 Home-page: http://porespy.org
 Author: PoreSpy Team
 Author-email: jgostick@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/PMEAL/porespy/
 Project-URL: Documentation, https://porespy.org/
@@ -68,15 +68,15 @@
         > *Gostick J, Khan ZA, Tranter TG, Kok MDR, Agnaou M, Sadeghi MA, Jervis
         > R.* **PoreSpy: A Python Toolkit for Quantitative Analysis of Porous Media
         > Images.** Journal of Open Source Software, 2019.
         > [doi:10.21105/joss.01296](https://doi.org/10.21105/joss.01296)
         
         # Installation
         
-        For detailed and up to date installation instructions, [see here](https://porespy.org/user_guide/installation.html)
+        For detailed and up to date installation instructions, [see here](https://porespy.org/installation.html)
         
         # Contributing
         
         If you think you may be interested in contributing to PoreSpy and wish
         to both *use* and *edit* the source code, then you should clone the
         [repository](https://github.com/PMEAL/porespy) to your local machine,
         and install it using the following PIP command:
@@ -182,11 +182,12 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `porespy-2.2.2/porespy.egg-info/SOURCES.txt` & `porespy-2.3.0/porespy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,48 +11,47 @@
 porespy.egg-info/requires.txt
 porespy.egg-info/top_level.txt
 porespy/dns/__init__.py
 porespy/dns/_funcs.py
 porespy/filters/__init__.py
 porespy/filters/_fftmorphology.py
 porespy/filters/_funcs.py
-porespy/filters/_ibip.py
-porespy/filters/_ibip_gpu.py
 porespy/filters/_nlmeans.py
 porespy/filters/_size_seq_satn.py
 porespy/filters/_snows.py
 porespy/filters/imagej/__init__.py
 porespy/filters/imagej/_funcs.py
 porespy/generators/__init__.py
 porespy/generators/_borders.py
-porespy/generators/_cylinder.py
 porespy/generators/_fractals.py
 porespy/generators/_imgen.py
 porespy/generators/_noise.py
 porespy/generators/_pseudo_packings.py
+porespy/generators/_spheres_from_coords.py
 porespy/io/__init__.py
 porespy/io/_comsol.py
 porespy/io/_funcs.py
+porespy/io/_unzipper.py
 porespy/metrics/__init__.py
-porespy/metrics/_fractal_dims.py
 porespy/metrics/_funcs.py
 porespy/metrics/_meshtools.py
 porespy/metrics/_regionprops.py
 porespy/networks/__init__.py
 porespy/networks/_funcs.py
 porespy/networks/_getnet.py
 porespy/networks/_maximal_ball.py
 porespy/networks/_size_factors.py
 porespy/networks/_snow2.py
 porespy/networks/_utils.py
 porespy/simulations/__init__.py
 porespy/simulations/_dns.py
 porespy/simulations/_drainage.py
+porespy/simulations/_ibip.py
+porespy/simulations/_ibip_gpu.py
 porespy/tools/__init__.py
 porespy/tools/_funcs.py
 porespy/tools/_sphere_insertions.py
-porespy/tools/_unpad.py
 porespy/tools/_utils.py
 porespy/visualization/__init__.py
 porespy/visualization/_funcs.py
 porespy/visualization/_plots.py
 porespy/visualization/_views.py
```

### Comparing `porespy-2.2.2/setup.cfg` & `porespy-2.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.2.2.dev0
+current_version = 2.3.0.dev0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\.(?P<release>\D+)(?P<build>\d+)?
 serialize = {major}.{minor}.{patch}.{release}{build}
 
 [bumpversion:part:release]
 values = dev
 
 [flake8]
```

### Comparing `porespy-2.2.2/setup.py` & `porespy-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Physics'
     ],
     packages=[
         'porespy',
         'porespy.tools',
         'porespy.generators',
@@ -67,30 +68,24 @@
         'porespy.visualization',
         'porespy.io'
     ],
     install_requires=[
         'dask',
         'deprecated',
         'edt',
-        'imageio',
         'matplotlib',
         'numba',
         'numpy',
-        'numpy-stl',
         'openpnm',
         'pandas',
         'psutil',
-        'pyevtk',
-        'pyfastnoisesimd',
         'rich',
-        'scikit-fmm',
         'scikit-image',
         'scipy',
         'tqdm',
-        'trimesh',
     ],
     author='PoreSpy Team',
     author_email='jgostick@gmail.com',
     download_url='https://github.com/PMEAL/porespy/',
     url='http://porespy.org',
     project_urls={
         'Documentation': 'https://porespy.org/',
```

