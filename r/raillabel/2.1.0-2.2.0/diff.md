# Comparing `tmp/raillabel-2.1.0.tar.gz` & `tmp/raillabel-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raillabel-2.1.0.tar", last modified: Fri May  5 13:39:13 2023, max compression
+gzip compressed data, was "raillabel-2.2.0.tar", last modified: Tue Jun  6 10:55:49 2023, max compression
```

## Comparing `raillabel-2.1.0.tar` & `raillabel-2.2.0.tar`

### file list

```diff
@@ -1,123 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-05 13:38:57.000000 raillabel-2.1.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-05 13:38:57.000000 raillabel-2.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.949673 raillabel-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-05 13:38:57.000000 raillabel-2.1.0/.github/workflows/build-test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-05 13:38:57.000000 raillabel-2.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-05 13:38:57.000000 raillabel-2.1.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-05 13:38:57.000000 raillabel-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-05 13:38:57.000000 raillabel-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-05 13:38:57.000000 raillabel-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-05 13:38:57.000000 raillabel-2.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 13:38:57.000000 raillabel-2.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 13:38:57.000000 raillabel-2.1.0/LICENSES/.license_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 13:38:57.000000 raillabel-2.1.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-05 13:38:57.000000 raillabel-2.1.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-05 13:39:13.961673 raillabel-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-05 13:38:57.000000 raillabel-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/_static/github-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/howto.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/docs/source/howtos/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/howtos/1 Validating Annotation Files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/howtos/2 Loading Annotation Files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/howtos/3 Saving Annotation Files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/howtos/4 Filtering Scenes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 13:38:57.000000 raillabel-2.1.0/git-conventional-commits.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/git-conventional-commits.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-05 13:38:57.000000 raillabel-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/raillabel/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.957673 raillabel-2.1.0/raillabel/_filter_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_annotation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_end.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_object_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_object_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.957673 raillabel-2.1.0/raillabel/_util/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_util/_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/raillabel/format/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/frame_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/intrinsics_pinhole.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/intrinsics_radar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/num.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/object_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/point3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/poly2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/poly3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/seg3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/sensor_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/size2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/size3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/raillabel/format_loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format_loaders/_loader_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format_loaders/loader_raillabel_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format_loaders/translation.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format_loaders/translation.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/raillabel/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    39070 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/schemas/raillabel_v2_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/schemas/raillabel_v2_schema.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.957673 raillabel-2.1.0/raillabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:39:13.961673 raillabel-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/master_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/test_raillabel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/test_raillabel/__test_assets__/
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/metaschema.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/metaschema.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    85872 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60789 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5.license
--rw-r--r--   0 runner    (1001) docker     (123)    54074 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/test_raillabel/format/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/format/test_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/test_raillabel/format_loaders/
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/format_loaders/test_loader_raillabel_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/test_raillabel/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/schemas/test_raillabel_v2_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-06 10:55:31.000000 raillabel-2.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-06 10:55:31.000000 raillabel-2.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.810411 raillabel-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.814411 raillabel-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-06 10:55:31.000000 raillabel-2.2.0/.github/workflows/build-test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-06 10:55:31.000000 raillabel-2.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-06 10:55:31.000000 raillabel-2.2.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-06 10:55:31.000000 raillabel-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-06 10:55:31.000000 raillabel-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-06 10:55:31.000000 raillabel-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-06 10:55:31.000000 raillabel-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 10:55:31.000000 raillabel-2.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.814411 raillabel-2.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 10:55:31.000000 raillabel-2.2.0/LICENSES/.license_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-06 10:55:31.000000 raillabel-2.2.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-06 10:55:31.000000 raillabel-2.2.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-06 10:55:49.838411 raillabel-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 10:55:31.000000 raillabel-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.814411 raillabel-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/_static/github-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/howto.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/docs/source/howtos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/howtos/1 Validating Annotation Files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/howtos/2 Loading Annotation Files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/howtos/3 Saving Annotation Files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/howtos/4 Filtering Scenes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 10:55:31.000000 raillabel-2.2.0/git-conventional-commits.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/git-conventional-commits.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-06 10:55:31.000000 raillabel-2.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/raillabel/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/raillabel/_filter_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_annotation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_object_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_object_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.822411 raillabel-2.2.0/raillabel/_understand_ai_t4_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/bounding_box_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/bounding_box_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/point_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/polygon_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/polyline_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/sensor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/size_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.822411 raillabel-2.2.0/raillabel/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_util/_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.826411 raillabel-2.2.0/raillabel/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/frame_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/intrinsics_pinhole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/intrinsics_radar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/num.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/object_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/point3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/poly2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/poly3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/seg3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/sensor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/size2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/size3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.826411 raillabel-2.2.0/raillabel/format_loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/_loader_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/loader_raillabel_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/loader_understand_ai_t4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/translation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/translation.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.826411 raillabel-2.2.0/raillabel/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    41712 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/schemas/raillabel_v2_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/schemas/raillabel_v2_schema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/schemas/understand_ai_t4_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/schemas/understand_ai_t4_schema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/raillabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 10:55:49.838411 raillabel-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.826411 raillabel-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/master_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.826411 raillabel-2.2.0/tests/test_raillabel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.830411 raillabel-2.2.0/tests/test_raillabel/__test_assets__/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_cs_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_cs_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_stream_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_stream_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar_stream_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar_stream_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar_stream_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar_stream_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_camera.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_camera.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_lidar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_lidar.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/metaschema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/metaschema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    85872 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60789 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5.license
+-rw-r--r--   0 runner    (1001) docker     (123)    54074 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   295329 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/understand_ai_real_life.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/understand_ai_real_life.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/understand_ai_t4_short.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/understand_ai_t4_short.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_bounding_box_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_bounding_box_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_point_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_polygon_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_polyline_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_sensor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_size_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/tests/test_raillabel/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/format/test_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/tests/test_raillabel/format_loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/format_loaders/test_loader_raillabel_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/format_loaders/test_loader_understand_ai_t4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/tests/test_raillabel/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/schemas/test_raillabel_v2_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/schemas/test_understand_ai_t4_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/test_validate.py
```

### Comparing `raillabel-2.1.0/.github/workflows/build-test-publish.yml` & `raillabel-2.2.0/.github/workflows/build-test-publish.yml`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/.github/workflows/docs.yml` & `raillabel-2.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/.github/workflows/lint.yml` & `raillabel-2.2.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/.gitignore` & `raillabel-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/.pre-commit-config.yaml` & `raillabel-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/CHANGELOG.md` & `raillabel-2.2.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 <!--
  ~ Copyright DB Netz AG and contributors
  ~ SPDX-License-Identifier: Apache-2.0
  -->
 
-[[_TOC_]]
-
-## 1.0.0
+# 1.0.0
 Release
 
-### 1.1.0
+## 1.1.0
 - Added raillabel.filter() and raillabel.Scene.filter()
 - Fixed a bug when comparing raillabel.CoordinateSystems with differing base children
 
-#### 1.1.1
+### 1.1.1
 - Fixed a naming dispute in raillabel.save()
 - Tested the package for Python 3.8 and 3.10
 - Created a requirements.txt
 - The filter() function is now accessible via raillabel.filter() instead of raillabel.io.filter()
 
-### 1.2.0
+## 1.2.0
 - Implemented frame specific data, that does not belong to any object
 - Implemented the Num annotation type
 
-## 2.0.0
+# 2.0.0
 - Made the saved data VCD-compatible
   - URIs of the annotation files (like the .png, where a bounding box is located) are now stored in the "frame_properties" under "sensors"
   - Implemented object data pointers
   - Devkit version is now stored in the metadata
 - FrameInterval.\_\_len\_\_() now returns the number of frames in the FrameInterval
 - Frame.annotations returns a dict of all annotations in the frame regardless of type or object
 - Removed proprietary parts
 - Added poly3d as a supported annotation type
 - All annotations are now stored in object_data.annotations (before they were stored in different fields according to their type)
 - raillabel.Scene.filter() has been removed. Use raillabel.filter() instead
 - Fields "coordinate_system" and "frame_intervals" have been removed from the raillabel.format.Object class
 - stream and coordinate system have been combined into a single sensor type
 
-## 2.0.1
+### 2.0.1
 - Changed name of PyPI package from 'raillabel' to 'pyraillabel' due to name collision
 
-## 2.0.2
+### 2.0.2
 - Changed name of PyPI package back to 'raillabel' because the problematic package has been removed
 
-## 2.0.3
+### 2.0.3
 - Fixed bug related to saving the annotator field in the metadata
 
-## 2.0.4
+### 2.0.4
 - Fixed bug related to the package version
 
-# 2.1.0
+## 2.1.0
 - Added IntrinsicsRadar to the devkit and the json-schema
+
+## 2.2.0
+- Raillabel schema is now more restrictive regarding intrinsic calibration
+- Support for understand.ai t4 format
+- Renaming of raillabel.format.Frame.data to frame_data
```

### Comparing `raillabel-2.1.0/CONTRIBUTING.md` & `raillabel-2.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/LICENSE` & `raillabel-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/LICENSES/Apache-2.0.txt` & `raillabel-2.2.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/LICENSES/CC0-1.0.txt` & `raillabel-2.2.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/PKG-INFO` & `raillabel-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raillabel
-Version: 2.1.0
+Version: 2.2.0
 Summary: A devkit for working with recorded and annotated train ride data from Deutsche Bahn.
 Author: DB Netz AG
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/DSD-DBS/raillabel
 Project-URL: Documentation, https://dsd-dbs.github.io/raillabel
 Platform: any
 Classifier: Development Status :: 1 - Planning
```

### Comparing `raillabel-2.1.0/README.md` & `raillabel-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/docs/Makefile` & `raillabel-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/docs/make.bat` & `raillabel-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/docs/source/_static/github-logo.svg` & `raillabel-2.2.0/docs/source/_static/github-logo.svg`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/docs/source/conf.py` & `raillabel-2.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/docs/source/howtos/1 Validating Annotation Files.rst` & `raillabel-2.2.0/docs/source/howtos/1 Validating Annotation Files.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/docs/source/howtos/2 Loading Annotation Files.rst` & `raillabel-2.2.0/docs/source/howtos/2 Loading Annotation Files.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/docs/source/howtos/3 Saving Annotation Files.rst` & `raillabel-2.2.0/docs/source/howtos/3 Saving Annotation Files.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/docs/source/howtos/4 Filtering Scenes.rst` & `raillabel-2.2.0/docs/source/howtos/4 Filtering Scenes.rst`

 * *Files 24% similar despite different names*

```diff
@@ -13,38 +13,38 @@
     import raillabel
     import decimal
 
     scene = raillabel.load('path/to/file.json')
 
     scene_with_only_trains = raillabel.filter(
         scene,
-        include_classes='train'
+        include_object_types=['train']
     )
     scene_without_bboxs = raillabel.filter(
         scene,
         exclude_annotation_types=['bbox']
     )
     cut_scene_with_only_red_trains = raillabel.filter(
         scene,
         start_timestamp=decimal.Decimal('1587349200.004200000'),
         exclude_frames=[4, 2],
-        include_classes='train',
+        include_object_types=['train'],
         include_attributes={
             'color': 'red'
         }
     )
     scene_with_annotations_with_an_attribute = raillabel.filter(
         scene,
         include_attributes={ # All annotations with the color
             'color': None    # attribute will be included,
         }                    # regardless of color value.
     )
 
-Most filter categories have an include and exclude parameter (i.e ``include_classes`` and ``exclude_classes``). When include is set, all annotations, that meet the criterium are *included* into the filtered scene. Excluded parameters are *excluded* from the scene. These two parameters are mutually exclusive and can not both be set.
+Most filter categories have an include and exclude parameter (i.e ``include_object_types`` and ``exclude_object_types``). When include is set, all annotations, that meet the criterium are *included* into the filtered scene. Excluded parameters are *excluded* from the scene. These two parameters are mutually exclusive and can not both be set.
 
 .. code-block:: python
 
     invalid_scene = raillabel.filter(
         scene,
-        include_classes='person',  # Will raise a ValueError due
-        exclude_classes='train'    # to mutual exclusivity.
+        include_object_types=['person'],  # Will raise a ValueError due
+        exclude_object_types=['train']    # to mutual exclusivity.
     )
```

### Comparing `raillabel-2.1.0/docs/source/index.rst` & `raillabel-2.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/docs/source/intro.rst` & `raillabel-2.2.0/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/pyproject.toml` & `raillabel-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/__init__.py` & `raillabel-2.2.0/raillabel/_filter_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/_filter_abc.py` & `raillabel-2.2.0/raillabel/_filter_classes/_filter_abc.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/_filter_annotation_ids.py` & `raillabel-2.2.0/raillabel/_filter_classes/_filter_annotation_ids.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/_filter_annotation_types.py` & `raillabel-2.2.0/raillabel/_filter_classes/_filter_annotation_types.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/_filter_attributes.py` & `raillabel-2.2.0/raillabel/_filter_classes/_filter_attributes.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/_filter_end.py` & `raillabel-2.2.0/raillabel/_filter_classes/_filter_end.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/_filter_frames.py` & `raillabel-2.2.0/raillabel/_filter_classes/_filter_frames.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/_filter_object_ids.py` & `raillabel-2.2.0/raillabel/_filter_classes/_filter_object_ids.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/_filter_object_types.py` & `raillabel-2.2.0/raillabel/_filter_classes/_filter_object_types.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/_filter_sensors.py` & `raillabel-2.2.0/raillabel/_filter_classes/_filter_sensors.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/_filter_classes/_filter_start.py` & `raillabel-2.2.0/raillabel/_filter_classes/_filter_start.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/exceptions.py` & `raillabel-2.2.0/raillabel/exceptions.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/filter.py` & `raillabel-2.2.0/raillabel/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,21 +114,21 @@
 
     for frame_id, frame in scene.frames.items():
 
         if not _passes_filters(frame, frame_filters):
             del filtered_scene.frames[frame_id]
             continue
 
-        for frame_data_id, frame_data in frame.data.items():
+        for frame_data_id, frame_data in frame.frame_data.items():
 
             if _passes_filters(frame_data, frame_data_filters):
                 used_sensors.add(frame_data.sensor.uid)
 
             else:
-                del filtered_scene.frames[frame_id].data[frame_data_id]
+                del filtered_scene.frames[frame_id].frame_data[frame_data_id]
 
         for object_id, object_data in frame.object_data.items():
 
             if not _passes_filters(scene.objects[object_id], object_filters):
                 continue
 
             for annotation_id, annotation in object_data.annotations.items():
```

### Comparing `raillabel-2.1.0/raillabel/format/__init__.py` & `raillabel-2.2.0/raillabel/format/__init__.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/_annotation.py` & `raillabel-2.2.0/raillabel/format/_annotation.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/bbox.py` & `raillabel-2.2.0/raillabel/format/bbox.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/cuboid.py` & `raillabel-2.2.0/raillabel/format/cuboid.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/frame.py` & `raillabel-2.2.0/raillabel/format/frame.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright DB Netz AG and contributors
 # SPDX-License-Identifier: Apache-2.0
 
 import decimal
 import typing as t
 import uuid
+import warnings
 from dataclasses import dataclass, field
 
 from .._util._warning import _warning
 from .num import Num
 from .object import Object
 from .object_data import ObjectData
 from .sensor import Sensor
@@ -17,52 +18,66 @@
 @dataclass
 class Frame:
     """A container of dynamic, timewise, information.
 
     Parameters
     ----------
     uid: int
-        Number of the frame withing the annotation file. Must be unique.
+        Number of the frame within the annotation file. Must be unique.
     timestamp: decimal.Decimal, optional
         Timestamp containing the Unix epoch time of the frame with up to nanosecond precision.
     sensors: dict of raillabel.format.SensorReference, optional
         References to the sensors with frame specific information like timestamp and uri.
         Default is {}.
-    data: dict, optional
-        Dictionary containing data directly connected to the frame and not to anny object.
-        Dictionary keys are the ID-strings of the variable the data belongs to. Default is {}.
+    frame_data: dict, optional
+        Dictionary containing data directly connected to the frame and not to any object, like
+        gps/imu data. Dictionary keys are the ID-strings of the variable the data belongs to.
+        Default is {}.
     object_data: dict of raillabel.format.ObjectData, optional
         Dictionary containing the annotations per object. Dictionary keys are the object uids.
         Default is {}.
 
     Read-Only Attributes
     --------------------
     annotations: dict
-        Dictionary containing all annotations of this frame, regardless of object or annotation
-        type. Dictionary keys are annotation UIDs.
+        Consolidation of all annotations in the object_data. Only use this field if you don't need
+        object tracking information. Dictionary keys are annotation UIDs.
     """
 
     uid: int
     timestamp: t.Optional[decimal.Decimal] = None
     sensors: t.Dict[str, SensorReference] = field(default_factory=dict)
-    data: t.Dict[str, Num] = field(default_factory=dict)
+    frame_data: t.Dict[str, Num] = field(default_factory=dict)
     object_data: t.Dict[uuid.UUID, ObjectData] = field(default_factory=dict)
 
     @property
     def annotations(self) -> t.Dict[uuid.UUID, t.Any]:
         """Return dict containing all annotations of this frame.
 
-        Dictionary keys are annotation UIDs.
+        Only use this field if you don't need object tracking
+        information. Dictionary keys are annotation UIDs.
         """
         annotations = {}
         for object in self.object_data.values():
             annotations.update(object.annotations)
 
         return annotations
 
+    @property
+    def data(self) -> t.Dict[str, Num]:
+        """Return frame data under alias.
+
+        Will be deprecated soon.
+        """
+        warnings.warn(
+            "data is a deprecated field and will be removed soon. Use Frame.frame_data instead.",
+            category=DeprecationWarning,
+        )
+        return self.frame_data
+
     @classmethod
     def fromdict(
         cls,
         uid: str,
         data_dict: dict,
         objects: t.Dict[str, Object],
         sensors: t.Dict[str, Sensor],
@@ -89,15 +104,15 @@
             Converted Frame object.
         """
 
         frame = Frame(
             uid=int(uid),
             timestamp=cls._timestamp_fromdict(data_dict),
             sensors=cls._sensors_fromdict(data_dict, int(uid), sensors),
-            data=cls._frame_data_fromdict(data_dict, int(uid), annotation_classes, sensors),
+            frame_data=cls._frame_data_fromdict(data_dict, int(uid), annotation_classes, sensors),
             object_data=cls._objects_fromdict(
                 data_dict, int(uid), objects, sensors, annotation_classes
             ),
         )
 
         frame = cls._fix_sensor_uri_attribute(frame)
 
@@ -126,17 +141,17 @@
             dict_repr["frame_properties"]["timestamp"] = str(self.timestamp)
 
         if self.sensors != {}:
             dict_repr["frame_properties"]["streams"] = {
                 str(k): v.asdict() for k, v in self.sensors.items()
             }
 
-        if self.data != {}:
+        if self.frame_data != {}:
             dict_repr["frame_properties"]["frame_data"] = {
-                "num": [v.asdict() for v in self.data.values()]
+                "num": [v.asdict() for v in self.frame_data.values()]
             }
 
         if self.object_data != {}:
             dict_repr["objects"] = {str(k): v.asdict() for k, v in self.object_data.items()}
 
         return dict_repr
```

### Comparing `raillabel-2.1.0/raillabel/format/frame_interval.py` & `raillabel-2.2.0/raillabel/format/frame_interval.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/intrinsics_pinhole.py` & `raillabel-2.2.0/raillabel/format/intrinsics_pinhole.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/intrinsics_radar.py` & `raillabel-2.2.0/raillabel/format/intrinsics_radar.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/metadata.py` & `raillabel-2.2.0/raillabel/format/metadata.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/num.py` & `raillabel-2.2.0/raillabel/format/num.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/object.py` & `raillabel-2.2.0/raillabel/format/object.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/object_data.py` & `raillabel-2.2.0/raillabel/format/object_data.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/point2d.py` & `raillabel-2.2.0/raillabel/format/point2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/point3d.py` & `raillabel-2.2.0/raillabel/format/point3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/poly2d.py` & `raillabel-2.2.0/raillabel/format/poly2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/poly3d.py` & `raillabel-2.2.0/raillabel/format/poly3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/quaternion.py` & `raillabel-2.2.0/raillabel/format/quaternion.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/scene.py` & `raillabel-2.2.0/raillabel/format/scene.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/seg3d.py` & `raillabel-2.2.0/raillabel/format/seg3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/sensor.py` & `raillabel-2.2.0/raillabel/format/sensor.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/sensor_reference.py` & `raillabel-2.2.0/raillabel/format/sensor_reference.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format/transform.py` & `raillabel-2.2.0/raillabel/format/transform.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format_loaders/__init__.py` & `raillabel-2.2.0/raillabel/format_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format_loaders/_loader_abc.py` & `raillabel-2.2.0/raillabel/format_loaders/_loader_abc.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format_loaders/loader_raillabel_v2.py` & `raillabel-2.2.0/raillabel/format_loaders/loader_raillabel_v2.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/format_loaders/translation.json` & `raillabel-2.2.0/raillabel/format_loaders/translation.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9911960132890366%*

 * *Differences: {"'stream_resolutions'": "{'radar': OrderedDict([('resolution_px_per_m', 2.856), ('x', 2856), "*

 * *                         "('y', 1428)])}",*

 * * "'streams'": "{'lidar_merged': 'lidar'}"}*

```diff
@@ -101,14 +101,19 @@
             "x": 640,
             "y": 480
         },
         "ir_right": {
             "x": 640,
             "y": 480
         },
+        "radar": {
+            "resolution_px_per_m": 2.856,
+            "x": 2856,
+            "y": 1428
+        },
         "rgb_highres_left": {
             "x": 4112,
             "y": 2504
         },
         "rgb_highres_middle": {
             "x": 4112,
             "y": 2504
@@ -188,14 +193,15 @@
         "S1213755_image": "rgb_highres_right",
         "S1213755_image_1": "rgb_highres_right",
         "base_link": "base",
         "imu": "gps_imu",
         "ir_left": "ir_left",
         "ir_middle": "ir_middle",
         "ir_right": "ir_right",
+        "lidar_merged": "lidar",
         "new_left_rect": "rgb_highres_left",
         "new_middle_rect": "rgb_highres_middle",
         "new_right_rect": "rgb_highres_right",
         "points_raw": "lidar",
         "points_raw_1": "lidar",
         "radar": "radar",
         "rgb_left_rect": "rgb_left",
```

### Comparing `raillabel-2.1.0/raillabel/load.py` & `raillabel-2.2.0/raillabel/load.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/save.py` & `raillabel-2.2.0/raillabel/save.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel/schemas/raillabel_v2_schema.json` & `raillabel-2.2.0/raillabel/schemas/raillabel_v2_schema.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9903615900383141%*

 * *Differences: {"'definitions'": "{'streams': {'patternProperties': {'^': {replace: OrderedDict([('oneOf', "*

 * *                  "[OrderedDict([('$ref', '#/definitions/stream_camera')]), OrderedDict([('$ref', "*

 * *                  "'#/definitions/stream_radar')]), OrderedDict([('$ref', "*

 * *                  "'#/definitions/stream_other')])])])}}}, 'stream_camera': "*

 * *                  "OrderedDict([('additionalProperties', False), ('description', 'A stream "*

 * *                  'describes the source of a data sequence, usually a s […]*

```diff
@@ -607,106 +607,151 @@
             "required": [
                 "name",
                 "val",
                 "closed"
             ],
             "type": "object"
         },
-        "stream": {
+        "stream_camera": {
             "additionalProperties": false,
-            "description": "A stream describes the source of a data sequence, usually a sensor.",
+            "description": "A stream describes the source of a data sequence, usually a sensor. This specific object contains the intrinsics of a camera sensor.",
             "properties": {
                 "description": {
                     "description": "Description of the stream.",
                     "type": "string"
                 },
                 "stream_properties": {
-                    "$ref": "#/definitions/stream_properties"
+                    "additionalProperties": false,
+                    "description": "Additional properties of the stream.",
+                    "properties": {
+                        "intrinsics_pinhole": {
+                            "additionalProperties": false,
+                            "description": "This JSON object defines an instance of the intrinsic parameters of a pinhole camera.",
+                            "properties": {
+                                "camera_matrix": {
+                                    "description": "This is a 3x4 camera matrix which projects 3D homogeneous points (4x1) from a camera coordinate system into the image plane (3x1). This is the usual K matrix for camera projection as in OpenCV. It is extended from 3x3 to 3x4 to enable its direct utilisation to project 4x1 homogeneous 3D points. The matrix is defined to follow the camera model: x-to-right, y-down, z-forward. The following equation applies: x_img = camera_matrix * X_ccs.",
+                                    "items": {
+                                        "type": "number"
+                                    },
+                                    "maxItems": 12,
+                                    "minItems": 12,
+                                    "type": "array"
+                                },
+                                "distortion_coeffs": {
+                                    "description": "This is the array 1xN radial and tangential distortion coefficients.",
+                                    "items": {
+                                        "type": "number"
+                                    },
+                                    "maxItems": 14,
+                                    "minItems": 5,
+                                    "type": "array"
+                                },
+                                "height_px": {
+                                    "type": "integer"
+                                },
+                                "width_px": {
+                                    "type": "integer"
+                                }
+                            },
+                            "required": [
+                                "camera_matrix",
+                                "distortion_coeffs",
+                                "height_px",
+                                "width_px"
+                            ],
+                            "type": "object"
+                        }
+                    }
+                },
+                "type": {
+                    "description": "A string encoding the type of the stream.",
+                    "enum": [
+                        "camera"
+                    ],
+                    "type": "string"
+                },
+                "uri": {
+                    "description": "A string encoding the subdirectory containing the sensor files.",
+                    "type": "string"
+                }
+            },
+            "type": "object"
+        },
+        "stream_other": {
+            "additionalProperties": false,
+            "description": "A stream describes the source of a data sequence, usually a sensor. This specific object is used for streams without intrinsic calibration.",
+            "properties": {
+                "description": {
+                    "description": "Description of the stream.",
+                    "type": "string"
                 },
                 "type": {
                     "description": "A string encoding the type of the stream.",
                     "enum": [
-                        "camera",
                         "lidar",
-                        "radar",
                         "gps_imu",
                         "other"
                     ],
                     "type": "string"
                 },
                 "uri": {
                     "description": "A string encoding the subdirectory containing the sensor files.",
                     "type": "string"
                 }
             },
             "type": "object"
         },
-        "stream_properties": {
+        "stream_radar": {
             "additionalProperties": false,
-            "description": "Additional properties of the stream.",
+            "description": "A stream describes the source of a data sequence, usually a sensor. This specific object contains the intrinsics of a camera sensor.",
             "properties": {
-                "intrinsics_pinhole": {
+                "description": {
+                    "description": "Description of the stream.",
+                    "type": "string"
+                },
+                "stream_properties": {
                     "additionalProperties": false,
-                    "description": "This JSON object defines an instance of the intrinsic parameters of a pinhole camera.",
+                    "description": "Additional properties of the stream.",
                     "properties": {
-                        "camera_matrix": {
-                            "description": "This is a 3x4 camera matrix which projects 3D homogeneous points (4x1) from a camera coordinate system into the image plane (3x1). This is the usual K matrix for camera projection as in OpenCV. It is extended from 3x3 to 3x4 to enable its direct utilisation to project 4x1 homogeneous 3D points. The matrix is defined to follow the camera model: x-to-right, y-down, z-forward. The following equation applies: x_img = camera_matrix * X_ccs.",
-                            "items": {
-                                "type": "number"
-                            },
-                            "maxItems": 12,
-                            "minItems": 12,
-                            "type": "array"
-                        },
-                        "distortion_coeffs": {
-                            "description": "This is the array 1xN radial and tangential distortion coefficients.",
-                            "items": {
-                                "type": "number"
+                        "intrinsics_radar": {
+                            "additionalProperties": false,
+                            "description": "This JSON object defines an instance of the intrinsic parameters of a radar.",
+                            "properties": {
+                                "height_px": {
+                                    "type": "integer"
+                                },
+                                "resolution_px_per_m": {
+                                    "type": "number"
+                                },
+                                "width_px": {
+                                    "type": "integer"
+                                }
                             },
-                            "maxItems": 14,
-                            "minItems": 5,
-                            "type": "array"
-                        },
-                        "height_px": {
-                            "type": "integer"
-                        },
-                        "width_px": {
-                            "type": "integer"
+                            "required": [
+                                "resolution_px_per_m",
+                                "height_px",
+                                "width_px"
+                            ],
+                            "type": "object"
                         }
-                    },
-                    "required": [
-                        "camera_matrix",
-                        "distortion_coeffs",
-                        "height_px",
-                        "width_px"
-                    ],
-                    "type": "object"
+                    }
                 },
-                "intrinsics_radar": {
-                    "additionalProperties": false,
-                    "description": "This JSON object defines an instance of the intrinsic parameters of a radar.",
-                    "properties": {
-                        "height_px": {
-                            "type": "integer"
-                        },
-                        "resolution_px_per_m": {
-                            "type": "number"
-                        },
-                        "width_px": {
-                            "type": "integer"
-                        }
-                    },
-                    "required": [
-                        "resolution_px_per_m",
-                        "height_px",
-                        "width_px"
+                "type": {
+                    "description": "A string encoding the type of the stream.",
+                    "enum": [
+                        "radar"
                     ],
-                    "type": "object"
+                    "type": "string"
+                },
+                "uri": {
+                    "description": "A string encoding the subdirectory containing the sensor files.",
+                    "type": "string"
                 }
-            }
+            },
+            "type": "object"
         },
         "stream_sync": {
             "additionalProperties": false,
             "description": "Syncronization information of a stream in a frame.",
             "properties": {
                 "stream_properties": {
                     "additionalProperties": false,
@@ -739,15 +784,25 @@
             "type": "object"
         },
         "streams": {
             "additionalProperties": false,
             "description": "This is a JSON object which contains OpenLABEL streams. Stream keys can be any string, for example, a friendly stream name.",
             "patternProperties": {
                 "^": {
-                    "$ref": "#/definitions/stream"
+                    "oneOf": [
+                        {
+                            "$ref": "#/definitions/stream_camera"
+                        },
+                        {
+                            "$ref": "#/definitions/stream_radar"
+                        },
+                        {
+                            "$ref": "#/definitions/stream_other"
+                        }
+                    ]
                 }
             },
             "type": "object"
         },
         "text_attribute": {
             "additionalProperties": false,
             "description": "A text attribute.",
```

### Comparing `raillabel-2.1.0/raillabel/validate.py` & `raillabel-2.2.0/raillabel/validate.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/raillabel.egg-info/PKG-INFO` & `raillabel-2.2.0/raillabel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raillabel
-Version: 2.1.0
+Version: 2.2.0
 Summary: A devkit for working with recorded and annotated train ride data from Deutsche Bahn.
 Author: DB Netz AG
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/DSD-DBS/raillabel
 Project-URL: Documentation, https://dsd-dbs.github.io/raillabel
 Platform: any
 Classifier: Development Status :: 1 - Planning
```

### Comparing `raillabel-2.1.0/tests/conftest.py` & `raillabel-2.2.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,51 +27,69 @@
 
     with json5_file_path.open() as f:
         data = json5.load(f)
 
     with open(str(json5_file_path)[:-1], "w") as f:
         json.dump(data, f, indent=4)
 
+
 @pytest.fixture
 def json_paths(request) -> t.Dict[str, Path]:
     json_paths = _fetch_json_paths_from_cache(request)
 
     if json_paths is None:
-        json_paths = {p.stem: p for p in _collect_json_paths()}
+        json_paths = {_get_file_identifier(p): p for p in _collect_json_paths()}
 
     return json_paths
 
 def _fetch_json_paths_from_cache(request) -> t.Optional[t.Dict[str, Path]]:
     return request.config.cache.get("json_paths", None)
 
 def _collect_json_paths() -> t.List[Path]:
     json_paths = []
 
     for dir in json_data_directories:
-        json_paths.extend([Path(p) for p in glob.glob(str(dir) + "/**.json")])
+        json_paths.extend([Path(p) for p in glob.glob(str(dir) + "/**/**.json", recursive=True)])
 
     return json_paths
 
+def _get_file_identifier(path: Path) -> str:
+    """Return relative path from test asset dir as string."""
+
+    if "__test_assets__" not in path.parts:
+        return path.stem
+
+    test_assets_dir_index = path.parts.index("__test_assets__")
+
+    relative_path = ""
+    for part in path.parts[test_assets_dir_index+1:-1]:
+        relative_path += part + "/"
+
+    relative_path += path.stem
+
+    return relative_path
+
 @pytest.fixture
 def json_data(request) -> t.Dict[str, dict]:
     json_data = _fetch_json_data_from_cache(request)
 
     if json_data is None:
-        json_data = {p.stem: _load_json_data(p) for p in _collect_json_paths()}
+        json_data = {_get_file_identifier(p): _load_json_data(p) for p in _collect_json_paths()}
 
     return json_data
 
 def _fetch_json_data_from_cache(request) -> t.Optional[t.Dict[str, Path]]:
     return request.config.cache.get("json_data", None)
 
 def _load_json_data(path: Path) -> dict:
     with path.open() as f:
         json_data = json.load(f)
     return json_data
 
+
 @pytest.fixture
 def annotation_compare_methods() -> t.Dict[str, t.Callable]:
     methods = {}
 
     def compare_bbox(annotation: raillabel.format.Bbox, ground_truth: dict) -> bool:
 
         assert type(annotation) == raillabel.format.Bbox
```

### Comparing `raillabel-2.1.0/tests/test_raillabel/__test_assets__/metaschema.json` & `raillabel-2.2.0/tests/test_raillabel/__test_assets__/metaschema.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json` & `raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5` & `raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json` & `raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/tests/test_raillabel/format/test_annotation.py` & `raillabel-2.2.0/tests/test_raillabel/format/test_annotation.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/tests/test_raillabel/format_loaders/test_loader_raillabel_v2.py` & `raillabel-2.2.0/tests/test_raillabel/format_loaders/test_loader_raillabel_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,19 +131,19 @@
 
     for frame_id, frame in scene.frames.items():
 
         accumulative_frame_data = []
         for frame_data_type in ground_truth["frames"][str(frame_id)]["frame_properties"]["frame_data"].values():
             accumulative_frame_data.extend(frame_data_type)
 
-        assert len(frame.data) == len(accumulative_frame_data)
+        assert len(frame.frame_data) == len(accumulative_frame_data)
 
         for frame_data_type, frame_data in ground_truth["frames"][str(frame_id)]["frame_properties"]["frame_data"].items():
             for annotation in frame_data:
-                annotation_compare_methods[frame_data_type](frame.data[annotation["name"]], annotation)
+                annotation_compare_methods[frame_data_type](frame.frame_data[annotation["name"]], annotation)
 
 
 def test_load_frame_annotations(json_data, loader, annotation_compare_methods):
     scene = loader.load(json_data["openlabel_v1_short"], validate=False)
 
     ground_truth = json_data["openlabel_v1_short"]["openlabel"]
 
@@ -177,17 +177,17 @@
         json_data["openlabel_v1_vcd_incompatible"],
         validate=False
     )
 
     # The UUIDs of the frame data have been generated and therefore do not match the ground truth.
     # They are set equal here.
     for frame_id in scene_ground_truth.frames:
-        for frame_data in scene_ground_truth.frames[frame_id].data:
-            scene.frames[frame_id].data[frame_data].uid = (
-                scene_ground_truth.frames[frame_id].data[frame_data].uid
+        for frame_data in scene_ground_truth.frames[frame_id].frame_data:
+            scene.frames[frame_id].frame_data[frame_data].uid = (
+                scene_ground_truth.frames[frame_id].frame_data[frame_data].uid
             )
 
     assert scene == scene_ground_truth
 
 
 # Tests the warnings and errors
 def test_no_warnings(json_data, loader):
@@ -321,15 +321,15 @@
     scene = loader.load(data, validate=False)
 
     for frame in scene.frames.values():
 
         for sensor_reference in frame.sensors.values():
             assert sensor_reference.sensor is scene.sensors[sensor_reference.sensor.uid]
 
-        for frame_data in frame.data.values():
+        for frame_data in frame.frame_data.values():
             assert frame_data.sensor is scene.sensors[frame_data.sensor.uid]
 
         for annotation in frame.annotations.values():
             assert annotation.sensor is scene.sensors[annotation.sensor.uid]
 
 
 # Executes the test if the file is called
```

### Comparing `raillabel-2.1.0/tests/test_raillabel/schemas/test_raillabel_v2_schema.py` & `raillabel-2.2.0/tests/test_raillabel/schemas/test_raillabel_v2_schema.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/tests/test_raillabel/test_filter.py` & `raillabel-2.2.0/tests/test_raillabel/test_filter.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/tests/test_raillabel/test_save.py` & `raillabel-2.2.0/tests/test_raillabel/test_save.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.1.0/tests/test_raillabel/test_validate.py` & `raillabel-2.2.0/tests/test_raillabel/test_validate.py`

 * *Files identical despite different names*

