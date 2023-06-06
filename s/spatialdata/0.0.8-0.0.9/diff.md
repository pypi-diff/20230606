# Comparing `tmp/spatialdata-0.0.8.tar.gz` & `tmp/spatialdata-0.0.9.tar.gz`

## Comparing `spatialdata-0.0.8.tar` & `spatialdata-0.0.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.bumpversion.cfg
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.editorconfig
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.gitmodules
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.mypy.ini
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata-0.0.8/_version.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.github/codecov.yml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/Makefile
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/changelog.md
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/conf.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/contributing.md
--rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/design_doc.md
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/index.md
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/installation.md
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_static/.gitkeep
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_static/css/custom.css
--rw-r--r--   0        0        0    51748 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_static/img/spatialdata_horizontal.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_templates/autosummary/function.rst
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/__init__.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/__main__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_compat.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_logging.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_types.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_utils.py
--rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/__init__.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/concatenate.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/data_extent.py
--rw-r--r--   0        0        0    62038 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/spatialdata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/operations/__init__.py
--rw-r--r--   0        0        0     9463 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/operations/aggregate.py
--rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/operations/rasterize.py
--rw-r--r--   0        0        0    17348 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/operations/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/query/__init__.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/query/_utils.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/query/relational_query.py
--rw-r--r--   0        0        0    30119 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/query/spatial_query.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/__init__.py
--rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/_utils.py
--rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/format.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/io_points.py
--rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/io_raster.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/io_shapes.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/io_table.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/io_zarr.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/dataloader/__init__.py
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/dataloader/datasets.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/models/__init__.py
--rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/models/_utils.py
--rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/models/models.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/__init__.py
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/_utils.py
--rw-r--r--   0        0        0    19686 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/operations.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/ngff/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/ngff/_utils.py
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/ngff/ngff_coordinate_system.py
--rw-r--r--   0        0        0    48233 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/ngff/ngff_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/operations/__init__.py
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/operations/test_aggregations.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/operations/test_rasterize.py
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/operations/test_spatialdata_operations.py
--rw-r--r--   0        0        0    19768 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/operations/test_transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/query/__init__.py
--rw-r--r--   0        0        0    16426 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/query/test_spatial_query.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/data/multipolygon.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/data/points.json
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/data/polygon.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/dataloader/__init__.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/dataloader/test_datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/dataloader/test_transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/datasets/__init__.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/datasets/test_datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/io/__init__.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/io/test_format.py
--rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/io/test_readwrite.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/io/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/models/__init__.py
--rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/models/test_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/__init__.py
--rw-r--r--   0        0        0    28221 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/test_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/ngff/__init__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/ngff/conftest.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/ngff/test_ngff_coordinate_system.py
--rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/ngff/test_ngff_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/utils/__init__.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/utils/test_element_utils.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata-0.0.8/LICENSE
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 spatialdata-0.0.8/README.md
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 spatialdata-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 spatialdata-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 spatialdata-0.0.9/.bumpversion.cfg
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 spatialdata-0.0.9/.editorconfig
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata-0.0.9/.gitmodules
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata-0.0.9/.mypy.ini
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spatialdata-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 spatialdata-0.0.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata-0.0.9/_version.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 spatialdata-0.0.9/.github/codecov.yml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata-0.0.9/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 spatialdata-0.0.9/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/changelog.md
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/conf.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/contributing.md
+-rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/design_doc.md
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/index.md
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/installation.md
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    51748 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/_static/img/spatialdata_horizontal.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/_templates/autosummary/function.rst
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata-0.0.9/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/__init__.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/__main__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_compat.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_logging.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_types.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_utils.py
+-rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/__init__.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/concatenate.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/data_extent.py
+-rw-r--r--   0        0        0    62038 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/spatialdata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/operations/__init__.py
+-rw-r--r--   0        0        0     9463 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/operations/aggregate.py
+-rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/operations/rasterize.py
+-rw-r--r--   0        0        0    17348 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/operations/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/query/__init__.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/query/_utils.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/query/relational_query.py
+-rw-r--r--   0        0        0    30119 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_core/query/spatial_query.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_io/__init__.py
+-rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_io/_utils.py
+-rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_io/format.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_io/io_points.py
+-rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_io/io_raster.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_io/io_shapes.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_io/io_table.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/_io/io_zarr.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/dataloader/__init__.py
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/dataloader/datasets.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/models/__init__.py
+-rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/models/_utils.py
+-rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/models/models.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/transformations/__init__.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/transformations/_utils.py
+-rw-r--r--   0        0        0    19686 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/transformations/operations.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/transformations/transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/transformations/ngff/__init__.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/transformations/ngff/_utils.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/transformations/ngff/ngff_coordinate_system.py
+-rw-r--r--   0        0        0    48233 2020-02-02 00:00:00.000000 spatialdata-0.0.9/src/spatialdata/transformations/ngff/ngff_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/core/operations/__init__.py
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/core/operations/test_aggregations.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/core/operations/test_rasterize.py
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/core/operations/test_spatialdata_operations.py
+-rw-r--r--   0        0        0    19768 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/core/operations/test_transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/core/query/__init__.py
+-rw-r--r--   0        0        0    16426 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/core/query/test_spatial_query.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/data/multipolygon.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/data/points.json
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/data/polygon.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/dataloader/__init__.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/dataloader/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/dataloader/test_transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/datasets/__init__.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/datasets/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/io/__init__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/io/test_format.py
+-rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/io/test_readwrite.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/io/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/models/__init__.py
+-rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/models/test_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/transformations/__init__.py
+-rw-r--r--   0        0        0    28221 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/transformations/test_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/transformations/ngff/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/transformations/ngff/conftest.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/transformations/ngff/test_ngff_coordinate_system.py
+-rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/transformations/ngff/test_ngff_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 spatialdata-0.0.9/tests/utils/test_element_utils.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 spatialdata-0.0.9/README.md
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 spatialdata-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 spatialdata-0.0.9/PKG-INFO
```

### Comparing `spatialdata-0.0.8/.mypy.ini` & `spatialdata-0.0.9/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/.pre-commit-config.yaml` & `spatialdata-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/.github/workflows/build.yaml` & `spatialdata-0.0.9/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/.github/workflows/test_and_deploy.yaml` & `spatialdata-0.0.9/.github/workflows/test_and_deploy.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/Makefile` & `spatialdata-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/api.md` & `spatialdata-0.0.9/docs/api.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/conf.py` & `spatialdata-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/contributing.md` & `spatialdata-0.0.9/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/design_doc.md` & `spatialdata-0.0.9/docs/design_doc.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/index.md` & `spatialdata-0.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/installation.md` & `spatialdata-0.0.9/docs/installation.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/references.bib` & `spatialdata-0.0.9/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/_static/css/custom.css` & `spatialdata-0.0.9/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/_static/img/spatialdata_horizontal.png` & `spatialdata-0.0.9/docs/_static/img/spatialdata_horizontal.png`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/_templates/autosummary/class.rst` & `spatialdata-0.0.9/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/docs/extensions/typed_returns.py` & `spatialdata-0.0.9/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/__init__.py` & `spatialdata-0.0.9/src/spatialdata/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/__main__.py` & `spatialdata-0.0.9/src/spatialdata/__main__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_compat.py` & `spatialdata-0.0.9/src/spatialdata/_compat.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_logging.py` & `spatialdata-0.0.9/src/spatialdata/_logging.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_utils.py` & `spatialdata-0.0.9/src/spatialdata/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/datasets.py` & `spatialdata-0.0.9/src/spatialdata/datasets.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_core/concatenate.py` & `spatialdata-0.0.9/src/spatialdata/_core/concatenate.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_core/data_extent.py` & `spatialdata-0.0.9/src/spatialdata/_core/data_extent.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_core/spatialdata.py` & `spatialdata-0.0.9/src/spatialdata/_core/spatialdata.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_core/operations/aggregate.py` & `spatialdata-0.0.9/src/spatialdata/_core/operations/aggregate.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_core/operations/rasterize.py` & `spatialdata-0.0.9/src/spatialdata/_core/operations/rasterize.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_core/operations/transform.py` & `spatialdata-0.0.9/src/spatialdata/_core/operations/transform.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_core/query/_utils.py` & `spatialdata-0.0.9/src/spatialdata/_core/query/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_core/query/relational_query.py` & `spatialdata-0.0.9/src/spatialdata/_core/query/relational_query.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_core/query/spatial_query.py` & `spatialdata-0.0.9/src/spatialdata/_core/query/spatial_query.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_io/_utils.py` & `spatialdata-0.0.9/src/spatialdata/_io/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_io/format.py` & `spatialdata-0.0.9/src/spatialdata/_io/format.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_io/io_points.py` & `spatialdata-0.0.9/src/spatialdata/_io/io_points.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_io/io_raster.py` & `spatialdata-0.0.9/src/spatialdata/_io/io_raster.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_io/io_shapes.py` & `spatialdata-0.0.9/src/spatialdata/_io/io_shapes.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_io/io_table.py` & `spatialdata-0.0.9/src/spatialdata/_io/io_table.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/_io/io_zarr.py` & `spatialdata-0.0.9/src/spatialdata/_io/io_zarr.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/dataloader/datasets.py` & `spatialdata-0.0.9/src/spatialdata/dataloader/datasets.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/models/__init__.py` & `spatialdata-0.0.9/src/spatialdata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/models/_utils.py` & `spatialdata-0.0.9/src/spatialdata/models/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/models/models.py` & `spatialdata-0.0.9/src/spatialdata/models/models.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/transformations/__init__.py` & `spatialdata-0.0.9/src/spatialdata/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/transformations/_utils.py` & `spatialdata-0.0.9/src/spatialdata/transformations/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/transformations/operations.py` & `spatialdata-0.0.9/src/spatialdata/transformations/operations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/transformations/transformations.py` & `spatialdata-0.0.9/src/spatialdata/transformations/transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/transformations/ngff/_utils.py` & `spatialdata-0.0.9/src/spatialdata/transformations/ngff/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/transformations/ngff/ngff_coordinate_system.py` & `spatialdata-0.0.9/src/spatialdata/transformations/ngff/ngff_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/src/spatialdata/transformations/ngff/ngff_transformations.py` & `spatialdata-0.0.9/src/spatialdata/transformations/ngff/ngff_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/conftest.py` & `spatialdata-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/core/operations/test_aggregations.py` & `spatialdata-0.0.9/tests/core/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/core/operations/test_rasterize.py` & `spatialdata-0.0.9/tests/core/operations/test_rasterize.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/core/operations/test_spatialdata_operations.py` & `spatialdata-0.0.9/tests/core/operations/test_spatialdata_operations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/core/operations/test_transform.py` & `spatialdata-0.0.9/tests/core/operations/test_transform.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/core/query/test_spatial_query.py` & `spatialdata-0.0.9/tests/core/query/test_spatial_query.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/data/multipolygon.json` & `spatialdata-0.0.9/tests/data/multipolygon.json`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/data/polygon.json` & `spatialdata-0.0.9/tests/data/polygon.json`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/dataloader/test_datasets.py` & `spatialdata-0.0.9/tests/dataloader/test_datasets.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/datasets/test_datasets.py` & `spatialdata-0.0.9/tests/datasets/test_datasets.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/io/test_format.py` & `spatialdata-0.0.9/tests/io/test_format.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/io/test_readwrite.py` & `spatialdata-0.0.9/tests/io/test_readwrite.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/io/test_utils.py` & `spatialdata-0.0.9/tests/io/test_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/models/test_models.py` & `spatialdata-0.0.9/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/transformations/test_transformations.py` & `spatialdata-0.0.9/tests/transformations/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/transformations/ngff/conftest.py` & `spatialdata-0.0.9/tests/transformations/ngff/conftest.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/transformations/ngff/test_ngff_coordinate_system.py` & `spatialdata-0.0.9/tests/transformations/ngff/test_ngff_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/transformations/ngff/test_ngff_transformations.py` & `spatialdata-0.0.9/tests/transformations/ngff/test_ngff_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/tests/utils/test_element_utils.py` & `spatialdata-0.0.9/tests/utils/test_element_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/.gitignore` & `spatialdata-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/LICENSE` & `spatialdata-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/README.md` & `spatialdata-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.8/pyproject.toml` & `spatialdata-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "multiscale_spatial_image>=0.11.2",
     "xarray-schema",
     "pygeos",
     "geopandas",
     "shapely>=2.0.1",
     "rich",
     "pyarrow",
-    "typing_extensions>=4.0.0",
+    "typing_extensions>=4.0.0,<4.6.0",
     "dask-image",
     "networkx",
     "xarray-spatial>=0.3.5",
     "tqdm",
 ]
 
 [project.optional-dependencies]
@@ -62,15 +62,15 @@
     "pytest",
     "pytest-cov",
 ]
 torch = [
     "torch"
 ]
 extra  = [
-    "napari-spatialdata>=0.2.3",
+    "napari-spatialdata>=0.2.4",
     "spatialdata-plot",
     "spatialdata-io",
 ]
 
 [tool.coverage.run]
 source = ["spatialdata"]
 omit = [
```

### Comparing `spatialdata-0.0.8/PKG-INFO` & `spatialdata-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialdata
-Version: 0.0.8
+Version: 0.0.9
 Summary: Spatial data format.
 Project-URL: Documentation, https://spatialdata.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata.git
 Project-URL: Home-page, https://github.com/scverse/spatialdata.git
 Author: scverse
 Maintainer-email: scverse <giov.pll@gmail.com>
 License: BSD 3-Clause License
@@ -47,15 +47,15 @@
 Requires-Dist: ome-zarr>=0.7.0
 Requires-Dist: pyarrow
 Requires-Dist: pygeos
 Requires-Dist: rich
 Requires-Dist: shapely>=2.0.1
 Requires-Dist: spatial-image>=0.3.0
 Requires-Dist: tqdm
-Requires-Dist: typing-extensions>=4.0.0
+Requires-Dist: typing-extensions<4.6.0,>=4.0.0
 Requires-Dist: xarray
 Requires-Dist: xarray-schema
 Requires-Dist: xarray-spatial>=0.3.5
 Requires-Dist: zarr
 Provides-Extra: dev
 Requires-Dist: bump2version; extra == 'dev'
 Provides-Extra: docs
@@ -65,15 +65,15 @@
 Requires-Dist: sphinx-book-theme>=1.0.0; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Requires-Dist: sphinx>=4.5; extra == 'docs'
 Requires-Dist: sphinxcontrib-bibtex>=1.0.0; extra == 'docs'
 Provides-Extra: extra
-Requires-Dist: napari-spatialdata>=0.2.3; extra == 'extra'
+Requires-Dist: napari-spatialdata>=0.2.4; extra == 'extra'
 Requires-Dist: spatialdata-io; extra == 'extra'
 Requires-Dist: spatialdata-plot; extra == 'extra'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Provides-Extra: torch
 Requires-Dist: torch; extra == 'torch'
```

