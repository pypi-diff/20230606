# Comparing `tmp/astroid-3.0.0a3.tar.gz` & `tmp/astroid-3.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroid-3.0.0a3.tar", last modified: Sun May 14 17:47:52 2023, max compression
+gzip compressed data, was "astroid-3.0.0a4.tar", last modified: Tue Jun  6 20:01:11 2023, max compression
```

## Comparing `astroid-3.0.0a3.tar` & `astroid-3.0.0a4.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.436113 astroid-3.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-05-14 17:47:37.000000 astroid-3.0.0a3/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-05-14 17:47:37.000000 astroid-3.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 17:47:37.000000 astroid-3.0.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-14 17:47:52.436113 astroid-3.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-14 17:47:37.000000 astroid-3.0.0a3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.424113 astroid-3.0.0a3/astroid/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/_backport_stdlib_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/astroid_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    27278 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.432113 astroid-3.0.0a3/astroid/brain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    35752 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_builtin_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_fstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_gi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_mechanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_namedtuple_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_nose.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_einsumfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_ma.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_responses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_scipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_six.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    45357 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/inference_tip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.432113 astroid-3.0.0a3/astroid/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.432113 astroid-3.0.0a3/astroid/interpreter/_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16568 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/_import/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/_import/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/dunder_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/objectmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17814 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23500 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/node_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.432113 astroid-3.0.0a3/astroid/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/const.py
--rw-r--r--   0 runner    (1001) docker     (123)   132674 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/node_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/node_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.432113 astroid-3.0.0a3/astroid/nodes/scoped_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/scoped_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/scoped_nodes/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)   100964 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/scoped_nodes/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/scoped_nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    69315 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.424113 astroid-3.0.0a3/astroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-14 17:47:52.000000 astroid-3.0.0a3/astroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-14 17:47:52.000000 astroid-3.0.0a3/astroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:47:52.000000 astroid-3.0.0a3/astroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 17:47:52.000000 astroid-3.0.0a3/astroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 17:47:52.000000 astroid-3.0.0a3/astroid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-14 17:47:37.000000 astroid-3.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-14 17:47:37.000000 astroid-3.0.0a3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-14 17:47:37.000000 astroid-3.0.0a3/requirements_full.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 17:47:37.000000 astroid-3.0.0a3/requirements_minimal.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-14 17:47:52.436113 astroid-3.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.436113 astroid-3.0.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_group_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)   221608 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_inference_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    61209 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    54462 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_nodes_lineno.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_nodes_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_object_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_python3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_regrtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    92790 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.654733 astroid-3.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-06 20:00:53.000000 astroid-3.0.0a4/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-06-06 20:00:53.000000 astroid-3.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 20:00:53.000000 astroid-3.0.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-06 20:01:11.654733 astroid-3.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-06 20:00:53.000000 astroid-3.0.0a4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.638733 astroid-3.0.0a4/astroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/_backport_stdlib_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/astroid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27278 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.646733 astroid-3.0.0a4/astroid/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35752 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_builtin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_fstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_gi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_mechanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_namedtuple_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_nose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_einsumfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_responses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_scipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45357 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/inference_tip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.646733 astroid-3.0.0a4/astroid/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.646733 astroid-3.0.0a4/astroid/interpreter/_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/_import/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/_import/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/dunder_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/objectmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17814 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23589 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/node_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.646733 astroid-3.0.0a4/astroid/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132674 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/node_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/node_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.646733 astroid-3.0.0a4/astroid/nodes/scoped_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/scoped_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/scoped_nodes/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100971 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/scoped_nodes/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/scoped_nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69315 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.638733 astroid-3.0.0a4/astroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-06 20:01:11.000000 astroid-3.0.0a4/astroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-06 20:01:11.000000 astroid-3.0.0a4/astroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:01:11.000000 astroid-3.0.0a4/astroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 20:01:11.000000 astroid-3.0.0a4/astroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 20:01:11.000000 astroid-3.0.0a4/astroid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-06 20:00:53.000000 astroid-3.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-06 20:00:53.000000 astroid-3.0.0a4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-06 20:00:53.000000 astroid-3.0.0a4/requirements_full.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-06 20:00:53.000000 astroid-3.0.0a4/requirements_minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-06 20:01:11.654733 astroid-3.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.654733 astroid-3.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:53.000000 astroid-3.0.0a4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_group_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   221727 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_inference_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22524 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61209 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54462 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_nodes_lineno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_nodes_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_object_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_python3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_regrtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92790 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tox.ini
```

### Comparing `astroid-3.0.0a3/CONTRIBUTORS.txt` & `astroid-3.0.0a4/CONTRIBUTORS.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 - Nick Drozd <nicholasdrozd@gmail.com>
 - Andrew Haigh <hello@nelf.in>
 - Julien Cristau <julien.cristau@logilab.fr>
 - David Liu <david@cs.toronto.edu>
 - Alexandre Fayolle <alexandre.fayolle@logilab.fr>
 - Eevee (Alex Munroe) <amunroe@yelp.com>
 - David Gilman <davidgilman1@gmail.com>
+- Tushar Sadhwani <tushar.sadhwani000@gmail.com>
 - Julien Jehannet <julien.jehannet@logilab.fr>
 - Calen Pennington <calen.pennington@gmail.com>
-- Tushar Sadhwani <tushar.sadhwani000@gmail.com> <86737547+tushar-deepsource@users.noreply.github.com>
 - Hugo van Kemenade <hugovk@users.noreply.github.com>
 - Tim Martin <tim@asymptotic.co.uk>
 - Phil Schaf <flying-sheep@web.de>
 - Alex Hall <alex.mojaki@gmail.com>
 - Raphael Gaschignard <raphael@makeleaps.com>
 - Radosław Ganczarek <radoslaw@ganczarek.in>
 - Paligot Gérard <androwiiid@gmail.com>
@@ -103,14 +103,15 @@
 - ostr00000 <ostr00000@gmail.com>
 - noah-weingarden <33741795+noah-weingarden@users.noreply.github.com>
 - nathannaveen <42319948+nathannaveen@users.noreply.github.com>
 - mathieui <mathieui@users.noreply.github.com>
 - markmcclain <markmcclain@users.noreply.github.com>
 - ioanatia <ioanatia@users.noreply.github.com>
 - grayjk <grayjk@gmail.com>
+- alm <alonme@users.noreply.github.com>
 - adam-grant-hendry <59346180+adam-grant-hendry@users.noreply.github.com>
 - Zbigniew Jędrzejewski-Szmek <zbyszek@in.waw.pl>
 - Zac Hatfield-Dodds <Zac-HD@users.noreply.github.com>
 - Vilnis Termanis <vilnis.termanis@iotics.com>
 - Valentin Valls <valentin.valls@esrf.fr>
 - Uilian Ries <uilianries@gmail.com>
 - Tomas Novak <ext.Tomas.Novak@skoda-auto.cz>
@@ -182,15 +183,14 @@
 - Artsiom Kaval <lezeroq@gmail.com>
 - Anubhav <35621759+anubh-v@users.noreply.github.com>
 - Antoine Boellinger <aboellinger@hotmail.com>
 - Alphadelta14 <alpha@alphaservcomputing.solutions>
 - Alexander Scheel <alexander.m.scheel@gmail.com>
 - Alexander Presnyakov <flagist0@gmail.com>
 - Ahmed Azzaoui <ahmed.azzaoui@engie.com>
-- alm <alonme@users.noreply.github.com
 
 Co-Author
 ---------
 The following persons were credited manually but did not commit themselves
 under this name, or we did not manage to find their commits in the history.
 
 - François Mockers
```

### Comparing `astroid-3.0.0a3/LICENSE` & `astroid-3.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/PKG-INFO` & `astroid-3.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a3/README.rst` & `astroid-3.0.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/__init__.py` & `astroid-3.0.0a4/astroid/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/_ast.py` & `astroid-3.0.0a4/astroid/_ast.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/_backport_stdlib_names.py` & `astroid-3.0.0a4/astroid/_backport_stdlib_names.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/arguments.py` & `astroid-3.0.0a4/astroid/arguments.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/astroid_manager.py` & `astroid-3.0.0a4/astroid/astroid_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/bases.py` & `astroid-3.0.0a4/astroid/bases.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_argparse.py` & `astroid-3.0.0a4/astroid/brain/brain_argparse.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_attrs.py` & `astroid-3.0.0a4/astroid/brain/brain_attrs.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_boto3.py` & `astroid-3.0.0a4/astroid/brain/brain_boto3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_builtin_inference.py` & `astroid-3.0.0a4/astroid/brain/brain_builtin_inference.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_collections.py` & `astroid-3.0.0a4/astroid/brain/brain_collections.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_crypt.py` & `astroid-3.0.0a4/astroid/brain/brain_crypt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_ctypes.py` & `astroid-3.0.0a4/astroid/brain/brain_ctypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_curses.py` & `astroid-3.0.0a4/astroid/brain/brain_curses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_dataclasses.py` & `astroid-3.0.0a4/astroid/brain/brain_dataclasses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_dateutil.py` & `astroid-3.0.0a4/astroid/brain/brain_dateutil.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_fstrings.py` & `astroid-3.0.0a4/astroid/brain/brain_fstrings.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_functools.py` & `astroid-3.0.0a4/astroid/brain/brain_functools.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_gi.py` & `astroid-3.0.0a4/astroid/brain/brain_gi.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_hashlib.py` & `astroid-3.0.0a4/astroid/brain/brain_hashlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_http.py` & `astroid-3.0.0a4/astroid/brain/brain_http.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_hypothesis.py` & `astroid-3.0.0a4/astroid/brain/brain_hypothesis.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_io.py` & `astroid-3.0.0a4/astroid/brain/brain_io.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_mechanize.py` & `astroid-3.0.0a4/astroid/brain/brain_mechanize.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_multiprocessing.py` & `astroid-3.0.0a4/astroid/brain/brain_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_namedtuple_enum.py` & `astroid-3.0.0a4/astroid/brain/brain_namedtuple_enum.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_nose.py` & `astroid-3.0.0a4/astroid/brain/brain_nose.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_core_einsumfunc.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_core_einsumfunc.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_core_fromnumeric.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_core_fromnumeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_core_function_base.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_core_function_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for numpy.core.function_base module."""
 
 import functools
 
-from astroid.brain.brain_numpy_utils import infer_numpy_member, looks_like_numpy_member
+from astroid.brain.brain_numpy_utils import (
+    attribute_looks_like_numpy_member,
+    infer_numpy_member,
+)
 from astroid.inference_tip import inference_tip
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import Attribute
 
 METHODS_TO_BE_INFERRED = {
     "linspace": """def linspace(start, stop, num=50, endpoint=True, retstep=False, dtype=None, axis=0):
             return numpy.ndarray([0, 0])""",
@@ -21,9 +24,9 @@
 }
 
 for func_name, func_src in METHODS_TO_BE_INFERRED.items():
     inference_function = functools.partial(infer_numpy_member, func_src)
     AstroidManager().register_transform(
         Attribute,
         inference_tip(inference_function),
-        functools.partial(looks_like_numpy_member, func_name),
+        functools.partial(attribute_looks_like_numpy_member, func_name),
     )
```

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_core_multiarray.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_core_multiarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for numpy.core.multiarray module."""
 
 import functools
 
-from astroid.brain.brain_numpy_utils import infer_numpy_member, looks_like_numpy_member
+from astroid.brain.brain_numpy_utils import (
+    attribute_looks_like_numpy_member,
+    infer_numpy_member,
+    name_looks_like_numpy_member,
+)
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import parse
 from astroid.inference_tip import inference_tip
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import Attribute, Name
 
 
@@ -87,14 +91,14 @@
 }
 
 for method_name, function_src in METHODS_TO_BE_INFERRED.items():
     inference_function = functools.partial(infer_numpy_member, function_src)
     AstroidManager().register_transform(
         Attribute,
         inference_tip(inference_function),
-        functools.partial(looks_like_numpy_member, method_name),
+        functools.partial(attribute_looks_like_numpy_member, method_name),
     )
     AstroidManager().register_transform(
         Name,
         inference_tip(inference_function),
-        functools.partial(looks_like_numpy_member, method_name),
+        functools.partial(name_looks_like_numpy_member, method_name),
     )
```

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_core_numeric.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_core_numeric.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for numpy.core.numeric module."""
 
 import functools
 
-from astroid.brain.brain_numpy_utils import infer_numpy_member, looks_like_numpy_member
+from astroid.brain.brain_numpy_utils import (
+    attribute_looks_like_numpy_member,
+    infer_numpy_member,
+)
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import parse
 from astroid.inference_tip import inference_tip
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import Attribute
 
 
@@ -38,9 +41,9 @@
 
 
 for method_name, function_src in METHODS_TO_BE_INFERRED.items():
     inference_function = functools.partial(infer_numpy_member, function_src)
     AstroidManager().register_transform(
         Attribute,
         inference_tip(inference_function),
-        functools.partial(looks_like_numpy_member, method_name),
+        functools.partial(attribute_looks_like_numpy_member, method_name),
     )
```

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_core_numerictypes.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_core_numerictypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_core_umath.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_core_umath.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_ma.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_ma.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_ndarray.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_ndarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_random_mtrand.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_random_mtrand.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_numpy_utils.py` & `astroid-3.0.0a4/astroid/brain/brain_numpy_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """Different utilities for the numpy brains."""
 
 from __future__ import annotations
 
 from astroid.builder import extract_node
 from astroid.context import InferenceContext
-from astroid.nodes.node_classes import Attribute, Import, Name, NodeNG
+from astroid.nodes.node_classes import Attribute, Import, Name
 
 # Class subscript is available in numpy starting with version 1.20.0
 NUMPY_VERSION_TYPE_HINTS_SUPPORT = ("1", "20", "0")
 
 
 def numpy_supports_type_hints() -> bool:
     """Returns True if numpy supports type hints."""
@@ -57,30 +57,25 @@
     ]
     return any(
         ("numpy", module_nickname) in target.names or ("numpy", None) in target.names
         for target in potential_import_target
     )
 
 
-def looks_like_numpy_member(member_name: str, node: NodeNG) -> bool:
+def name_looks_like_numpy_member(member_name: str, node: Name) -> bool:
     """
-    Returns True if the node is a member of numpy whose
+    Returns True if the Name is a member of numpy whose
     name is member_name.
+    """
+    return node.name == member_name and node.root().name.startswith("numpy")
 
-    :param member_name: name of the member
-    :param node: node to test
-    :return: True if the node is a member of numpy
+
+def attribute_looks_like_numpy_member(member_name: str, node: Attribute) -> bool:
     """
-    if (
-        isinstance(node, Attribute)
-        and node.attrname == member_name
+    Returns True if the Attribute is a member of numpy whose
+    name is member_name.
+    """
+    return (
+        node.attrname == member_name
         and isinstance(node.expr, Name)
         and _is_a_numpy_module(node.expr)
-    ):
-        return True
-    if (
-        isinstance(node, Name)
-        and node.name == member_name
-        and node.root().name.startswith("numpy")
-    ):
-        return True
-    return False
+    )
```

### Comparing `astroid-3.0.0a3/astroid/brain/brain_pathlib.py` & `astroid-3.0.0a4/astroid/brain/brain_pathlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_pkg_resources.py` & `astroid-3.0.0a4/astroid/brain/brain_pkg_resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_pytest.py` & `astroid-3.0.0a4/astroid/brain/brain_pytest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_qt.py` & `astroid-3.0.0a4/astroid/brain/brain_qt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_random.py` & `astroid-3.0.0a4/astroid/brain/brain_random.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_re.py` & `astroid-3.0.0a4/astroid/brain/brain_re.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_regex.py` & `astroid-3.0.0a4/astroid/brain/brain_regex.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_responses.py` & `astroid-3.0.0a4/astroid/brain/brain_responses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_scipy_signal.py` & `astroid-3.0.0a4/astroid/brain/brain_scipy_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_signal.py` & `astroid-3.0.0a4/astroid/brain/brain_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_six.py` & `astroid-3.0.0a4/astroid/brain/brain_six.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_sqlalchemy.py` & `astroid-3.0.0a4/astroid/brain/brain_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_ssl.py` & `astroid-3.0.0a4/astroid/brain/brain_ssl.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_subprocess.py` & `astroid-3.0.0a4/astroid/brain/brain_subprocess.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_threading.py` & `astroid-3.0.0a4/astroid/brain/brain_threading.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_type.py` & `astroid-3.0.0a4/astroid/brain/brain_type.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_typing.py` & `astroid-3.0.0a4/astroid/brain/brain_typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,14 +312,17 @@
         func_to_add = _extract_single_node(CLASS_GETITEM_TEMPLATE)
         class_def.locals["__class_getitem__"] = [func_to_add]
     else:
         # If not, make sure that `__class_getitem__` access is forbidden.
         # This is an issue in cases where the aliased class implements it,
         # but the typing alias isn't subscriptable. E.g., `typing.ByteString` for PY39+
         _forbid_class_getitem_access(class_def)
+
+    # Avoid re-instantiating this class every time it's seen
+    node._explicit_inference = lambda node, context: iter([class_def])
     return iter([class_def])
 
 
 def _looks_like_special_alias(node: Call) -> bool:
     """Return True if call is for Tuple or Callable alias.
 
     In PY37 and PY38 the call is to '_VariadicGenericAlias' with 'tuple' as
```

### Comparing `astroid-3.0.0a3/astroid/brain/brain_unittest.py` & `astroid-3.0.0a4/astroid/brain/brain_unittest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/brain_uuid.py` & `astroid-3.0.0a4/astroid/brain/brain_uuid.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/brain/helpers.py` & `astroid-3.0.0a4/astroid/brain/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/builder.py` & `astroid-3.0.0a4/astroid/builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/const.py` & `astroid-3.0.0a4/astroid/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/constraint.py` & `astroid-3.0.0a4/astroid/constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/context.py` & `astroid-3.0.0a4/astroid/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,14 +136,26 @@
 
     @contextlib.contextmanager
     def restore_path(self) -> Iterator[None]:
         path = set(self.path)
         yield
         self.path = path
 
+    def is_empty(self) -> bool:
+        return (
+            not self.path
+            and not self.nodes_inferred
+            and not self.callcontext
+            and not self.boundnode
+            and not self.lookupname
+            and not self.callcontext
+            and not self.extra_context
+            and not self.constraints
+        )
+
     def __str__(self) -> str:
         state = (
             f"{field}={pprint.pformat(getattr(self, field), width=80 - len(field))}"
             for field in self.__slots__
         )
         return "{}({})".format(type(self).__name__, ",\n    ".join(state))
```

### Comparing `astroid-3.0.0a3/astroid/decorators.py` & `astroid-3.0.0a4/astroid/decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/exceptions.py` & `astroid-3.0.0a4/astroid/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/filter_statements.py` & `astroid-3.0.0a4/astroid/filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/helpers.py` & `astroid-3.0.0a4/astroid/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/inference.py` & `astroid-3.0.0a4/astroid/inference.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/inference_tip.py` & `astroid-3.0.0a4/astroid/inference_tip.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Transform utilities (filters and decorator)."""
 
 from __future__ import annotations
 
+from collections import OrderedDict
 from collections.abc import Generator
 from typing import Any, TypeVar
 
 from astroid.context import InferenceContext
 from astroid.exceptions import InferenceOverwriteError, UseInferenceDefault
 from astroid.nodes import NodeNG
 from astroid.typing import (
     InferenceResult,
     InferFn,
     TransformFn,
 )
 
-_cache: dict[
+_cache: OrderedDict[
     tuple[InferFn[Any], NodeNG, InferenceContext | None], list[InferenceResult]
-] = {}
+] = OrderedDict()
 
 _CURRENTLY_INFERRING: set[tuple[InferFn[Any], NodeNG]] = set()
 
 _NodesT = TypeVar("_NodesT", bound=NodeNG)
 
 
 def clear_inference_tip_cache() -> None:
@@ -40,30 +41,46 @@
         context: InferenceContext | None = None,
         **kwargs: Any,
     ) -> Generator[InferenceResult, None, None]:
         partial_cache_key = (func, node)
         if partial_cache_key in _CURRENTLY_INFERRING:
             # If through recursion we end up trying to infer the same
             # func + node we raise here.
+            _CURRENTLY_INFERRING.remove(partial_cache_key)
             raise UseInferenceDefault
+        if context is not None and context.is_empty():
+            # Fresh, empty contexts will defeat the cache.
+            context = None
         try:
             yield from _cache[func, node, context]
             return
         except KeyError:
             # Recursion guard with a partial cache key.
             # Using the full key causes a recursion error on PyPy.
             # It's a pragmatic compromise to avoid so much recursive inference
             # with slightly different contexts while still passing the simple
             # test cases included with this commit.
             _CURRENTLY_INFERRING.add(partial_cache_key)
-            result = _cache[func, node, context] = list(func(node, context, **kwargs))
-            # Remove recursion guard.
-            _CURRENTLY_INFERRING.remove(partial_cache_key)
+            try:
+                # May raise UseInferenceDefault
+                result = _cache[func, node, context] = list(
+                    func(node, context, **kwargs)
+                )
+            finally:
+                # Remove recursion guard.
+                try:
+                    _CURRENTLY_INFERRING.remove(partial_cache_key)
+                except KeyError:
+                    pass  # Recursion may beat us to the punch.
+
+                if len(_cache) > 64:
+                    _cache.popitem(last=False)
 
-        yield from result
+        # https://github.com/pylint-dev/pylint/issues/8686
+        yield from result  # pylint: disable=used-before-assignment
 
     return inner
 
 
 def inference_tip(
     infer_function: InferFn[_NodesT], raise_on_overwrite: bool = False
 ) -> TransformFn[_NodesT]:
```

### Comparing `astroid-3.0.0a3/astroid/interpreter/_import/spec.py` & `astroid-3.0.0a4/astroid/interpreter/_import/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                     )
             except ValueError:
                 pass
             submodule_path = sys.path
 
         for entry in submodule_path:
             package_directory = os.path.join(entry, modname)
-            for suffix in (".py", importlib.machinery.BYTECODE_SUFFIXES[0]):
+            for suffix in (".py", ".pyi", importlib.machinery.BYTECODE_SUFFIXES[0]):
                 package_file_name = "__init__" + suffix
                 file_path = os.path.join(package_directory, package_file_name)
                 if os.path.isfile(file_path):
                     return ModuleSpec(
                         name=modname,
                         location=package_directory,
                         type=ModuleType.PKG_DIRECTORY,
```

### Comparing `astroid-3.0.0a3/astroid/interpreter/_import/util.py` & `astroid-3.0.0a4/astroid/interpreter/_import/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/interpreter/dunder_lookup.py` & `astroid-3.0.0a4/astroid/interpreter/dunder_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/interpreter/objectmodel.py` & `astroid-3.0.0a4/astroid/interpreter/objectmodel.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/manager.py` & `astroid-3.0.0a4/astroid/manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/mixins.py` & `astroid-3.0.0a4/astroid/mixins.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/modutils.py` & `astroid-3.0.0a4/astroid/modutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 else:
     from astroid._backport_stdlib_names import stdlib_module_names
 
 logger = logging.getLogger(__name__)
 
 
 if sys.platform.startswith("win"):
-    PY_SOURCE_EXTS = ("py", "pyw")
+    PY_SOURCE_EXTS = ("py", "pyw", "pyi")
     PY_COMPILED_EXTS = ("dll", "pyd")
 else:
-    PY_SOURCE_EXTS = ("py",)
+    PY_SOURCE_EXTS = ("py", "pyi")
     PY_COMPILED_EXTS = ("so",)
 
 
 # TODO: Adding `platstdlib` is a fix for a workaround in virtualenv. At some point we should
 # revisit whether this is still necessary. See https://github.com/pylint-dev/astroid/pull/1323.
 STD_LIB_DIRS = {sysconfig.get_path("stdlib"), sysconfig.get_path("platstdlib")}
 
@@ -270,17 +270,14 @@
     if os.path.normcase(abs_filename).startswith(path_to_check):
         importable_path = abs_filename
 
     real_filename = os.path.realpath(filename)
     if os.path.normcase(real_filename).startswith(path_to_check):
         importable_path = real_filename
 
-    # if "var" in path_to_check:
-    #     breakpoint()
-
     if importable_path:
         base_path = os.path.splitext(importable_path)[0]
         relative_base_path = base_path[len(path_to_check) :]
         return [pkg for pkg in relative_base_path.split(os.sep) if pkg]
 
     return None
 
@@ -472,15 +469,15 @@
     """
     files: list[str] = []
     for directory, dirnames, filenames in os.walk(src_directory):
         if directory in blacklist:
             continue
         _handle_blacklist(blacklist, dirnames, filenames)
         # check for __init__.py
-        if not list_all and "__init__.py" not in filenames:
+        if not list_all and {"__init__.py", "__init__.pyi"}.isdisjoint(filenames):
             dirnames[:] = ()
             continue
         for filename in filenames:
             if _is_python_file(filename):
                 src = os.path.join(directory, filename)
                 files.append(src)
     return files
@@ -495,14 +492,16 @@
 
     :raise NoSourceFile: if no source file exists on the file system
 
     :return: the absolute path of the source file if it exists
     """
     filename = os.path.abspath(_path_from_filename(filename))
     base, orig_ext = os.path.splitext(filename)
+    if orig_ext == ".pyi" and os.path.exists(f"{base}{orig_ext}"):
+        return f"{base}{orig_ext}"
     for ext in PY_SOURCE_EXTS:
         source_path = f"{base}.{ext}"
         if os.path.exists(source_path):
             return source_path
     if include_no_ext and not orig_ext and os.path.exists(base):
         return base
     raise NoSourceFile(filename)
@@ -659,15 +658,15 @@
 
 
 def _is_python_file(filename: str) -> bool:
     """Return true if the given filename should be considered as a python file.
 
     .pyc and .pyo are ignored
     """
-    return filename.endswith((".py", ".so", ".pyd", ".pyw"))
+    return filename.endswith((".py", ".pyi", ".so", ".pyd", ".pyw"))
 
 
 def _has_init(directory: str) -> str | None:
     """If the given directory has a valid __init__ file, return its path,
     else return None.
     """
     mod_or_pack = os.path.join(directory, "__init__")
```

### Comparing `astroid-3.0.0a3/astroid/node_classes.py` & `astroid-3.0.0a4/astroid/node_classes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/nodes/__init__.py` & `astroid-3.0.0a4/astroid/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/nodes/_base_nodes.py` & `astroid-3.0.0a4/astroid/nodes/_base_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/nodes/as_string.py` & `astroid-3.0.0a4/astroid/nodes/as_string.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/nodes/const.py` & `astroid-3.0.0a4/astroid/nodes/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/nodes/node_classes.py` & `astroid-3.0.0a4/astroid/nodes/node_classes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/nodes/node_ng.py` & `astroid-3.0.0a4/astroid/nodes/node_ng.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/nodes/scoped_nodes/__init__.py` & `astroid-3.0.0a4/astroid/nodes/scoped_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/nodes/scoped_nodes/mixin.py` & `astroid-3.0.0a4/astroid/nodes/scoped_nodes/mixin.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/nodes/scoped_nodes/scoped_nodes.py` & `astroid-3.0.0a4/astroid/nodes/scoped_nodes/scoped_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,32 +129,32 @@
         return
     # Found multiple Generics in mro, remove entry from inferred_bases
     # and the corresponding one from bases_mro
     inferred_bases.pop(position_in_inferred_bases)
     bases_mro.pop(position_in_inferred_bases)
 
 
-def clean_duplicates_mro(sequences, cls, context):
+def clean_duplicates_mro(
+    sequences: Iterable[Iterable[ClassDef]],
+    cls: ClassDef,
+    context: InferenceContext | None,
+) -> Iterable[Iterable[ClassDef]]:
     for sequence in sequences:
-        names = [
-            (node.lineno, node.qname()) if node.name else None for node in sequence
-        ]
-        last_index = dict(map(reversed, enumerate(names)))
-        if names and names[0] is not None and last_index[names[0]] != 0:
-            raise DuplicateBasesError(
-                message="Duplicates found in MROs {mros} for {cls!r}.",
-                mros=sequences,
-                cls=cls,
-                context=context,
-            )
-        yield [
-            node
-            for i, (node, name) in enumerate(zip(sequence, names))
-            if name is None or last_index[name] == i
-        ]
+        seen = set()
+        for node in sequence:
+            lineno_and_qname = (node.lineno, node.qname())
+            if lineno_and_qname in seen:
+                raise DuplicateBasesError(
+                    message="Duplicates found in MROs {mros} for {cls!r}.",
+                    mros=sequences,
+                    cls=cls,
+                    context=context,
+                )
+            seen.add(lineno_and_qname)
+    return sequences
 
 
 def function_to_method(n, klass):
     if isinstance(n, FunctionDef):
         if n.type == "classmethod":
             return bases.BoundMethod(n, klass)
         if n.type == "property":
@@ -2802,14 +2802,17 @@
                 continue
             if not baseobj.hide:
                 yield baseobj
             else:
                 yield from baseobj.bases
 
     def _compute_mro(self, context: InferenceContext | None = None):
+        if self.qname() == "builtins.object":
+            return [self]
+
         inferred_bases = list(self._inferred_bases(context=context))
         bases_mro = []
         for base in inferred_bases:
             if base is self:
                 continue
 
             try:
@@ -2821,15 +2824,15 @@
                 # although in Python it's possible, since the class we are
                 # currently working is in fact new style.
                 # So, we fallback to ancestors here.
                 ancestors = list(base.ancestors(context=context))
                 bases_mro.append(ancestors)
 
         unmerged_mro = [[self], *bases_mro, inferred_bases]
-        unmerged_mro = list(clean_duplicates_mro(unmerged_mro, self, context))
+        unmerged_mro = clean_duplicates_mro(unmerged_mro, self, context)
         clean_typing_generic_mro(unmerged_mro)
         return _c3_merge(unmerged_mro, self, context)
 
     def mro(self, context: InferenceContext | None = None) -> list[ClassDef]:
         """Get the method resolution order, using C3 linearization.
 
         :returns: The list of ancestors, sorted by the mro.
```

### Comparing `astroid-3.0.0a3/astroid/nodes/scoped_nodes/utils.py` & `astroid-3.0.0a4/astroid/nodes/scoped_nodes/utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/objects.py` & `astroid-3.0.0a4/astroid/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,14 +310,17 @@
 
     def infer_call_result(
         self,
         caller: SuccessfulInferenceResult | None,
         context: InferenceContext | None = None,
     ) -> Iterator[InferenceResult]:
         if context:
+            assert (
+                context.callcontext
+            ), "CallContext should be set before inferring call result"
             current_passed_keywords = {
                 keyword for (keyword, _) in context.callcontext.keywords
             }
             for keyword, value in self.filled_keywords.items():
                 if keyword not in current_passed_keywords:
                     context.callcontext.keywords.append((keyword, value))
```

### Comparing `astroid-3.0.0a3/astroid/protocols.py` & `astroid-3.0.0a4/astroid/protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/raw_building.py` & `astroid-3.0.0a4/astroid/raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/rebuilder.py` & `astroid-3.0.0a4/astroid/rebuilder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/scoped_nodes.py` & `astroid-3.0.0a4/astroid/scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/test_utils.py` & `astroid-3.0.0a4/astroid/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/transforms.py` & `astroid-3.0.0a4/astroid/transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/typing.py` & `astroid-3.0.0a4/astroid/typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid/util.py` & `astroid-3.0.0a4/astroid/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/astroid.egg-info/PKG-INFO` & `astroid-3.0.0a4/astroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a3/astroid.egg-info/SOURCES.txt` & `astroid-3.0.0a4/astroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/pyproject.toml` & `astroid-3.0.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/resources.py` & `astroid-3.0.0a4/tests/resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_builder.py` & `astroid-3.0.0a4/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_constraint.py` & `astroid-3.0.0a4/tests/test_constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_decorators.py` & `astroid-3.0.0a4/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_filter_statements.py` & `astroid-3.0.0a4/tests/test_filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_group_exceptions.py` & `astroid-3.0.0a4/tests/test_group_exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_helpers.py` & `astroid-3.0.0a4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_inference.py` & `astroid-3.0.0a4/tests/test_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     test_utils,
     util,
 )
 from astroid import decorators as decoratorsmod
 from astroid.arguments import CallSite
 from astroid.bases import BoundMethod, Instance, UnboundMethod, UnionType
 from astroid.builder import AstroidBuilder, _extract_single_node, extract_node, parse
-from astroid.const import PY39_PLUS, PY310_PLUS
+from astroid.const import IS_PYPY, PY39_PLUS, PY310_PLUS
 from astroid.context import CallContext, InferenceContext
 from astroid.exceptions import (
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
     NotFoundError,
 )
@@ -6972,14 +6972,17 @@
     parse("__dunder_var__ = ['v']", module_name="top3.mod")
     w_val = mod3.body[-1].value
     i_w_val = next(w_val.infer())
     assert i_w_val is not util.Uninferable
     assert i_w_val.as_string() == "['w', 'v']"
 
 
+@pytest.mark.skipif(
+    IS_PYPY, reason="Test run with coverage on PyPy sometimes raises a RecursionError"
+)
 def test_recursion_on_inference_tip() -> None:
     """Regression test for recursion in inference tip.
 
     Originally reported in https://github.com/pylint-dev/pylint/issues/5408.
 
     When run on PyPy with coverage enabled, the test can sometimes raise a RecursionError
     outside of the code that we actually want to test.
```

### Comparing `astroid-3.0.0a3/tests/test_inference_calls.py` & `astroid-3.0.0a4/tests/test_inference_calls.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_lookup.py` & `astroid-3.0.0a4/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_manager.py` & `astroid-3.0.0a4/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_modutils.py` & `astroid-3.0.0a4/tests/test_modutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,19 @@
         self.assertEqual(
             modutils.get_source_file(os.path.__file__), os.path.normpath(filename)
         )
 
     def test_raise(self) -> None:
         self.assertRaises(modutils.NoSourceFile, modutils.get_source_file, "whatever")
 
+    def test_(self) -> None:
+        package = resources.find("pyi_data")
+        module = os.path.join(package, "__init__.pyi")
+        self.assertEqual(modutils.get_source_file(module), os.path.normpath(module))
+
 
 class IsStandardModuleTest(resources.SysPathSetup, unittest.TestCase):
     """
     Return true if the module may be considered as a module from the standard
     library.
     """
 
@@ -413,16 +418,20 @@
     """
 
     def test_success(self) -> None:
         datadir = resources.find("")
         assert modutils.module_in_path("data.module", datadir)
         assert modutils.module_in_path("data.module", (datadir,))
         assert modutils.module_in_path("data.module", os.path.abspath(datadir))
+        assert modutils.module_in_path("pyi_data.module", datadir)
+        assert modutils.module_in_path("pyi_data.module", (datadir,))
+        assert modutils.module_in_path("pyi_data.module", os.path.abspath(datadir))
         # "" will evaluate to cwd
         assert modutils.module_in_path("data.module", "")
+        assert modutils.module_in_path("pyi_data.module", "")
 
     def test_bad_import(self) -> None:
         datadir = resources.find("")
         assert not modutils.module_in_path("this_module_is_no_more", datadir)
 
     def test_no_filename(self) -> None:
         datadir = resources.find("")
@@ -492,14 +501,27 @@
             "module.py",
             "module2.py",
             "noendingnewline.py",
             "nonregr.py",
         ]
         self.assertEqual(modules, {os.path.join(package, x) for x in expected})
 
+    def test_get_module_files_2(self) -> None:
+        package = resources.find("pyi_data/find_test")
+        modules = set(modutils.get_module_files(package, []))
+        expected = [
+            "__init__.py",
+            "__init__.pyi",
+            "module.py",
+            "module2.py",
+            "noendingnewline.py",
+            "nonregr.py",
+        ]
+        self.assertEqual(modules, {os.path.join(package, x) for x in expected})
+
     def test_get_all_files(self) -> None:
         """Test that list_all returns all Python files from given location."""
         non_package = resources.find("data/notamodule")
         modules = modutils.get_module_files(non_package, [], list_all=True)
         self.assertEqual(modules, [os.path.join(non_package, "file.py")])
 
     def test_load_module_set_attribute(self) -> None:
```

### Comparing `astroid-3.0.0a3/tests/test_nodes.py` & `astroid-3.0.0a4/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_nodes_lineno.py` & `astroid-3.0.0a4/tests/test_nodes_lineno.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_nodes_position.py` & `astroid-3.0.0a4/tests/test_nodes_position.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_object_model.py` & `astroid-3.0.0a4/tests/test_object_model.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_objects.py` & `astroid-3.0.0a4/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_protocols.py` & `astroid-3.0.0a4/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_python3.py` & `astroid-3.0.0a4/tests/test_python3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_raw_building.py` & `astroid-3.0.0a4/tests/test_raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_regrtest.py` & `astroid-3.0.0a4/tests/test_regrtest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_scoped_nodes.py` & `astroid-3.0.0a4/tests/test_scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_stdlib.py` & `astroid-3.0.0a4/tests/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_transforms.py` & `astroid-3.0.0a4/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a3/tests/test_utils.py` & `astroid-3.0.0a4/tests/test_utils.py`

 * *Files identical despite different names*

