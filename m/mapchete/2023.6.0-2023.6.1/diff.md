# Comparing `tmp/mapchete-2023.6.0.tar.gz` & `tmp/mapchete-2023.6.1.tar.gz`

## Comparing `mapchete-2023.6.0.tar` & `mapchete-2023.6.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/__init__.py
--rw-r--r--   0        0        0    29098 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_core.py
--rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_executor.py
--rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_processing.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_registered.py
--rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_tasks.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_timer.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_user_process.py
--rw-r--r--   0        0        0    48597 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/config.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/errors.py
--rw-r--r--   0        0        0    17748 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/index.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/log.py
--rw-r--r--   0        0        0    24446 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/path.py
--rw-r--r--   0        0        0    17498 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/stac.py
--rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/testing.py
--rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/tile.py
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/types.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/main.py
--rw-r--r--   0        0        0    11007 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     4995 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/__init__.py
--rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/_convert.py
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/_cp.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/_execute.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/_index.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/_rm.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commons/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commons/clip.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commons/contours.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commons/hillshade.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    20802 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/base.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/loaders.py
--rw-r--r--   0        0        0    12520 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/geobuf.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    15914 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/__init__.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/_json.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/_misc.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/_path.py
--rw-r--r--   0        0        0    44018 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/raster.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/settings.py
--rw-r--r--   0        0        0    21813 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/vector.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/convert.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/static/__init__.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/static/index.html
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/static/process_template.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.6.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.6.0/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.6.0/README.rst
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 mapchete-2023.6.0/pyproject.toml
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 mapchete-2023.6.0/PKG-INFO
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/__init__.py
+-rw-r--r--   0        0        0    29098 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_core.py
+-rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_executor.py
+-rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_processing.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_registered.py
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_tasks.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_timer.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_user_process.py
+-rw-r--r--   0        0        0    48597 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/config.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/errors.py
+-rw-r--r--   0        0        0    17748 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/index.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/log.py
+-rw-r--r--   0        0        0    24483 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/path.py
+-rw-r--r--   0        0        0    17481 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/stac.py
+-rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/testing.py
+-rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/tile.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/types.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/main.py
+-rw-r--r--   0        0        0    11007 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     4995 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/_convert.py
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/_cp.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/_execute.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/_index.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/_rm.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commons/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commons/clip.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commons/contours.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commons/hillshade.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    20802 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/base.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0    12520 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/geobuf.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    15914 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/_json.py
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/_misc.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/_path.py
+-rw-r--r--   0        0        0    44018 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/raster.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/settings.py
+-rw-r--r--   0        0        0    21813 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/static/index.html
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.6.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.6.1/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.6.1/README.rst
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 mapchete-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 mapchete-2023.6.1/PKG-INFO
```

### Comparing `mapchete-2023.6.0/mapchete/__init__.py` & `mapchete-2023.6.1/mapchete/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     "ProcessInfo",
     "Timer",
     "Executor",
     "FakeFuture",
     "SkippedFuture",
     "Job",
 ]
-__version__ = "2023.6.0"
+__version__ = "2023.6.1"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `mapchete-2023.6.0/mapchete/_core.py` & `mapchete-2023.6.1/mapchete/_core.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/_executor.py` & `mapchete-2023.6.1/mapchete/_executor.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/_processing.py` & `mapchete-2023.6.1/mapchete/_processing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/_registered.py` & `mapchete-2023.6.1/mapchete/_registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/_tasks.py` & `mapchete-2023.6.1/mapchete/_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from collections import namedtuple
 from itertools import chain
-from traceback import format_exc
 from uuid import uuid4
 
 from shapely.geometry import box, mapping
 
 from mapchete._timer import Timer
 from mapchete._user_process import MapcheteProcess
 from mapchete.config import get_process_func
```

### Comparing `mapchete-2023.6.0/mapchete/_timer.py` & `mapchete-2023.6.1/mapchete/_timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/_user_process.py` & `mapchete-2023.6.1/mapchete/_user_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/config.py` & `mapchete-2023.6.1/mapchete/config.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/errors.py` & `mapchete-2023.6.1/mapchete/errors.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/index.py` & `mapchete-2023.6.1/mapchete/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/log.py` & `mapchete-2023.6.1/mapchete/log.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/path.py` & `mapchete-2023.6.1/mapchete/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,25 +349,32 @@
             gdal_opts.update(user_opts)
         else:
             gdal_opts = user_opts
         logger.debug("using GDAL options: %s", gdal_opts)
         return gdal_opts
 
     @cached_property
+    def _endpoint_url(self):
+        # GDAL parses the paths in a weird way, so we have to be careful with a custom
+        # endpoint
+        if hasattr(self.fs, "endpoint_url") and isinstance(self.fs.endpoint_url, str):
+            return self.fs.endpoint_url.lstrip("http://").lstrip("https://")
+        else:
+            return None
+
+    @cached_property
     def rio_session(self) -> "rasterio.session.Session":
         if self.fs_session:
             # rasterio accepts a Session object but only a boto3.session.Session
             # object and not a aiobotocore.session.AioSession which we get from fsspec
             return RioSession.from_path(
                 self._path_str,
                 aws_access_key_id=self.fs.key,
                 aws_secret_access_key=self.fs.secret,
-                # GDAL parses the paths in a weird way, so we have to be careful with a custom
-                # endpoint
-                endpoint_url=self.fs.endpoint_url.lstrip("http://").lstrip("https://"),
+                endpoint_url=self._endpoint_url,
                 requester_pays=self.fs.storage_options.get("requester_pays", False),
             )
         else:
             return RioSession.from_path(self._path_str)
 
     def rio_env_config(self, opts=None, allowed_remote_extensions=None) -> dict:
         """Return configuration parameters for rasterio.Env()."""
@@ -394,17 +401,15 @@
         if self.fs_session:
             # fiona accepts a Session object but only a boto3.session.Session
             # object and not a aiobotocore.session.AioSession which we get from fsspec
             return FioSession.from_path(
                 self._path_str,
                 aws_access_key_id=self.fs.key,
                 aws_secret_access_key=self.fs.secret,
-                # GDAL parses the paths in a weird way, so we have to be careful with a custom
-                # endpoint
-                endpoint_url=self.fs.endpoint_url.lstrip("http://").lstrip("https://"),
+                endpoint_url=self._endpoint_url,
                 requester_pays=self.fs.storage_options.get("requester_pays", False),
             )
         else:
             return FioSession.from_path(self._path_str)
 
     def fio_env_config(self, opts=None, allowed_remote_extensions=None) -> dict:
         """Return configuration parameters for fiona.Env()."""
```

### Comparing `mapchete-2023.6.0/mapchete/stac.py` & `mapchete-2023.6.1/mapchete/stac.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,14 @@
     # for each zoom level get tile output for 0/0
     for zoom in mp.config.init_zoom_levels:
         prototype_tile = mp.config.output_pyramid.tile(zoom, 0, 0)
         tile_path = mp.config.output.get_path(prototype_tile)
         # if tile exists, skip
         if mp.config.output.tiles_exist(output_tile=prototype_tile):
             logger.debug("prototype tile %s already exists", tile_path)
-            pass
         # if not, write empty tile
         else:
             logger.debug("creating prototype tile %s", tile_path)
             out_profile = mp.config.output.profile(prototype_tile)
             tile_path.makedirs()
             write_raster_window(
                 in_tile=prototype_tile,
```

### Comparing `mapchete-2023.6.0/mapchete/testing.py` & `mapchete-2023.6.1/mapchete/testing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/tile.py` & `mapchete-2023.6.1/mapchete/tile.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/types.py` & `mapchete-2023.6.1/mapchete/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from collections.abc import Iterable
-
-
 class Bounds(list):
     """
     Class to handle geographic bounds.
     """
 
     left: float = None
     bottom: float = None
```

### Comparing `mapchete-2023.6.0/mapchete/validate.py` & `mapchete-2023.6.1/mapchete/validate.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/options.py` & `mapchete-2023.6.1/mapchete/cli/options.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/default/convert.py` & `mapchete-2023.6.1/mapchete/cli/default/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/default/cp.py` & `mapchete-2023.6.1/mapchete/cli/default/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/default/create.py` & `mapchete-2023.6.1/mapchete/cli/default/create.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/default/execute.py` & `mapchete-2023.6.1/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/default/formats.py` & `mapchete-2023.6.1/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/default/index.py` & `mapchete-2023.6.1/mapchete/cli/default/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/default/processes.py` & `mapchete-2023.6.1/mapchete/cli/default/processes.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/default/rm.py` & `mapchete-2023.6.1/mapchete/cli/default/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/default/serve.py` & `mapchete-2023.6.1/mapchete/cli/default/serve.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/cli/default/stac.py` & `mapchete-2023.6.1/mapchete/cli/default/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/commands/_convert.py` & `mapchete-2023.6.1/mapchete/commands/_convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/commands/_cp.py` & `mapchete-2023.6.1/mapchete/commands/_cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/commands/_execute.py` & `mapchete-2023.6.1/mapchete/commands/_execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/commands/_index.py` & `mapchete-2023.6.1/mapchete/commands/_index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/commands/_rm.py` & `mapchete-2023.6.1/mapchete/commands/_rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/commons/clip.py` & `mapchete-2023.6.1/mapchete/commons/clip.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/commons/contours.py` & `mapchete-2023.6.1/mapchete/commons/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/commons/hillshade.py` & `mapchete-2023.6.1/mapchete/commons/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/__init__.py` & `mapchete-2023.6.1/mapchete/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/base.py` & `mapchete-2023.6.1/mapchete/formats/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/loaders.py` & `mapchete-2023.6.1/mapchete/formats/loaders.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/tools.py` & `mapchete-2023.6.1/mapchete/formats/tools.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/_fiona_base.py` & `mapchete-2023.6.1/mapchete/formats/default/_fiona_base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/flatgeobuf.py` & `mapchete-2023.6.1/mapchete/formats/default/flatgeobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/geobuf.py` & `mapchete-2023.6.1/mapchete/formats/default/geobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/geojson.py` & `mapchete-2023.6.1/mapchete/formats/default/geojson.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/gtiff.py` & `mapchete-2023.6.1/mapchete/formats/default/gtiff.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/mapchete_input.py` & `mapchete-2023.6.1/mapchete/formats/default/mapchete_input.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/png.py` & `mapchete-2023.6.1/mapchete/formats/default/png.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/png_hillshade.py` & `mapchete-2023.6.1/mapchete/formats/default/png_hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/raster_file.py` & `mapchete-2023.6.1/mapchete/formats/default/raster_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/tile_directory.py` & `mapchete-2023.6.1/mapchete/formats/default/tile_directory.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/formats/default/vector_file.py` & `mapchete-2023.6.1/mapchete/formats/default/vector_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/io/__init__.py` & `mapchete-2023.6.1/mapchete/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/io/_geometry_operations.py` & `mapchete-2023.6.1/mapchete/io/_geometry_operations.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/io/_json.py` & `mapchete-2023.6.1/mapchete/io/_json.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/io/_misc.py` & `mapchete-2023.6.1/mapchete/io/_misc.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/io/raster.py` & `mapchete-2023.6.1/mapchete/io/raster.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/io/settings.py` & `mapchete-2023.6.1/mapchete/io/settings.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/io/vector.py` & `mapchete-2023.6.1/mapchete/io/vector.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/processes/__init__.py` & `mapchete-2023.6.1/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/processes/contours.py` & `mapchete-2023.6.1/mapchete/processes/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/processes/convert.py` & `mapchete-2023.6.1/mapchete/processes/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/processes/hillshade.py` & `mapchete-2023.6.1/mapchete/processes/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/processes/examples/example_process.py` & `mapchete-2023.6.1/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/static/index.html` & `mapchete-2023.6.1/mapchete/static/index.html`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/mapchete/static/process_template.py` & `mapchete-2023.6.1/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/LICENSE` & `mapchete-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/README.rst` & `mapchete-2023.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/pyproject.toml` & `mapchete-2023.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.0/PKG-INFO` & `mapchete-2023.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapchete
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

