# Comparing `tmp/pyunifiprotect-4.9.0.tar.gz` & `tmp/pyunifiprotect-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunifiprotect-4.9.0.tar", last modified: Mon May 15 01:00:11 2023, max compression
+gzip compressed data, was "pyunifiprotect-4.9.1.tar", last modified: Thu Jun  1 16:04:50 2023, max compression
```

## Comparing `pyunifiprotect-4.9.0.tar` & `pyunifiprotect-4.9.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.394236 pyunifiprotect-4.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/format-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/install-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.bin/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/lib/common.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/lint-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/test-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/update-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.docker/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.378235 pyunifiprotect-4.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.github/workflows/test-live-AngellusMortis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/LIVE_DATA_CI.md
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-15 01:00:11.394236 pyunifiprotect-4.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/TESTDATA.md
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/dev.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/docs/overrides/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/overrides/partials/toc-item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/pyunifiprotect/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47861 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.386236 pyunifiprotect-4.9.0/pyunifiprotect/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/chimes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/doorlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/lights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/liveviews.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.386236 pyunifiprotect-4.9.0/pyunifiprotect/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    73524 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    33878 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/release_cache.json
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.386236 pyunifiprotect-4.9.0/pyunifiprotect/test_util/
--rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/test_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/test_util/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 01:00:11.394236 pyunifiprotect-4.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.386236 pyunifiprotect-4.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.390236 pyunifiprotect-4.9.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27759 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_chime.py
--rw-r--r--   0 runner    (1001) docker     (123)    24435 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_doorlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_light.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.390236 pyunifiprotect-4.9.0/tests/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   239461 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_bootstrap.json
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_camera.json
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_camera_heatmap.png
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_camera_snapshot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_camera_thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_camera_video.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_chime.json
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_constants.json
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_doorlock.json
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_event_smart_track.json
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_light.json
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_liveview.json
--rw-r--r--   0 runner    (1001) docker     (123)   854579 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_raw_events.json
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_viewport.json
--rw-r--r--   0 runner    (1001) docker     (123)   159864 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_ws_messages.json
--rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/test_api_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/test_api_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.299831 pyunifiprotect-4.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.283831 pyunifiprotect-4.9.1/.bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.bin/format-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.bin/install-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.283831 pyunifiprotect-4.9.1/.bin/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.bin/lib/common.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.bin/lint-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.bin/test-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.bin/update-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.283831 pyunifiprotect-4.9.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.283831 pyunifiprotect-4.9.1/.docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.279831 pyunifiprotect-4.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.283831 pyunifiprotect-4.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.github/workflows/test-live-AngellusMortis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.283831 pyunifiprotect-4.9.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/LIVE_DATA_CI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-06-01 16:04:50.295831 pyunifiprotect-4.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/TESTDATA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.283831 pyunifiprotect-4.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/docs/dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.283831 pyunifiprotect-4.9.1/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.283831 pyunifiprotect-4.9.1/docs/overrides/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/docs/overrides/partials/toc-item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.287831 pyunifiprotect-4.9.1/pyunifiprotect/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47861 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.287831 pyunifiprotect-4.9.1/pyunifiprotect/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/chimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/doorlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/lights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/liveviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/cli/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.291831 pyunifiprotect-4.9.1/pyunifiprotect/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/data/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/data/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73524 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/data/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33878 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/data/nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/data/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/data/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/release_cache.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.291831 pyunifiprotect-4.9.1/pyunifiprotect/test_util/
+-rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/test_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/test_util/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15971 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/pyunifiprotect/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.287831 pyunifiprotect-4.9.1/pyunifiprotect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-06-01 16:04:50.000000 pyunifiprotect-4.9.1/pyunifiprotect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-01 16:04:50.000000 pyunifiprotect-4.9.1/pyunifiprotect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:04:50.000000 pyunifiprotect-4.9.1/pyunifiprotect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 16:04:50.000000 pyunifiprotect-4.9.1/pyunifiprotect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-01 16:04:50.000000 pyunifiprotect-4.9.1/pyunifiprotect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 16:04:50.000000 pyunifiprotect-4.9.1/pyunifiprotect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:04:50.299831 pyunifiprotect-4.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.291831 pyunifiprotect-4.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.291831 pyunifiprotect-4.9.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27759 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/data/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/data/test_chime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24435 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/data/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/data/test_doorlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/data/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/data/test_nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/data/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/data/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:50.295831 pyunifiprotect-4.9.1/tests/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239461 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_bootstrap.json
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_camera.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_camera_heatmap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_camera_snapshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_camera_thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_camera_video.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_chime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_constants.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_doorlock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_event_smart_track.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_light.json
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_liveview.json
+-rw-r--r--   0 runner    (1001) docker     (123)   854579 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_raw_events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_viewport.json
+-rw-r--r--   0 runner    (1001) docker     (123)   159864 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/sample_data/sample_ws_messages.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/test_api_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/test_api_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-01 16:04:39.000000 pyunifiprotect-4.9.1/tests/test_utils.py
```

### Comparing `pyunifiprotect-4.9.0/.bin/lib/common.sh` & `pyunifiprotect-4.9.1/.bin/lib/common.sh`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.bin/lint-code` & `pyunifiprotect-4.9.1/.bin/lint-code`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.bin/update-requirements` & `pyunifiprotect-4.9.1/.bin/update-requirements`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.devcontainer/devcontainer.json` & `pyunifiprotect-4.9.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.github/workflows/ci.yaml` & `pyunifiprotect-4.9.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.github/workflows/docker.yml` & `pyunifiprotect-4.9.1/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.github/workflows/docs.yml` & `pyunifiprotect-4.9.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.github/workflows/pypi.yml` & `pyunifiprotect-4.9.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.github/workflows/test-live-AngellusMortis.yml` & `pyunifiprotect-4.9.1/.github/workflows/test-live-AngellusMortis.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.gitignore` & `pyunifiprotect-4.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.vscode/launch.json` & `pyunifiprotect-4.9.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/.vscode/tasks.json` & `pyunifiprotect-4.9.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/Dockerfile` & `pyunifiprotect-4.9.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/LICENSE` & `pyunifiprotect-4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/LIVE_DATA_CI.md` & `pyunifiprotect-4.9.1/LIVE_DATA_CI.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/PKG-INFO` & `pyunifiprotect-4.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunifiprotect
-Version: 4.9.0
+Version: 4.9.1
 Summary: Unofficial UniFi Protect Python API and CLI
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
 License: MIT
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
```

### Comparing `pyunifiprotect-4.9.0/README.md` & `pyunifiprotect-4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/TESTDATA.md` & `pyunifiprotect-4.9.1/TESTDATA.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/dev-requirements.txt` & `pyunifiprotect-4.9.1/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/docs/api.md` & `pyunifiprotect-4.9.1/docs/api.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/docs/cli.md` & `pyunifiprotect-4.9.1/docs/cli.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/docs/dev.md` & `pyunifiprotect-4.9.1/docs/dev.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/mkdocs.yml` & `pyunifiprotect-4.9.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyproject.toml` & `pyunifiprotect-4.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/api.py` & `pyunifiprotect-4.9.1/pyunifiprotect/api.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/__init__.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/backup.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/backup.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/base.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/cameras.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/cameras.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/chimes.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/chimes.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/doorlocks.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/doorlocks.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/events.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/events.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/lights.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/lights.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/liveviews.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/liveviews.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/nvr.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/sensors.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/sensors.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/cli/viewers.py` & `pyunifiprotect-4.9.1/pyunifiprotect/cli/viewers.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/data/__init__.py` & `pyunifiprotect-4.9.1/pyunifiprotect/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/data/base.py` & `pyunifiprotect-4.9.1/pyunifiprotect/data/base.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/data/bootstrap.py` & `pyunifiprotect-4.9.1/pyunifiprotect/data/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/data/convert.py` & `pyunifiprotect-4.9.1/pyunifiprotect/data/convert.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/data/devices.py` & `pyunifiprotect-4.9.1/pyunifiprotect/data/devices.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/data/nvr.py` & `pyunifiprotect-4.9.1/pyunifiprotect/data/nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/data/types.py` & `pyunifiprotect-4.9.1/pyunifiprotect/data/types.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/data/user.py` & `pyunifiprotect-4.9.1/pyunifiprotect/data/user.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/data/websocket.py` & `pyunifiprotect-4.9.1/pyunifiprotect/data/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/exceptions.py` & `pyunifiprotect-4.9.1/pyunifiprotect/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/stream.py` & `pyunifiprotect-4.9.1/pyunifiprotect/stream.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/test_util/__init__.py` & `pyunifiprotect-4.9.1/pyunifiprotect/test_util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/test_util/anonymize.py` & `pyunifiprotect-4.9.1/pyunifiprotect/test_util/anonymize.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/utils.py` & `pyunifiprotect-4.9.1/pyunifiprotect/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 from aiohttp import ClientResponse
 import jwt
 from pydantic.fields import SHAPE_DICT, SHAPE_LIST, SHAPE_SET, ModelField
 from pydantic.utils import to_camel
 
 from pyunifiprotect.data.types import (
+    Color,
     SmartDetectAudioType,
     SmartDetectObjectType,
     Version,
     VideoMode,
 )
 from pyunifiprotect.exceptions import NvrError
 
@@ -70,24 +71,26 @@
 SNAKE_CASE_MATCH_2 = re.compile("__([A-Z0-9])")
 SNAKE_CASE_MATCH_3 = re.compile("([a-z0-9])([A-Z])")
 
 _LOGGER = logging.getLogger(__name__)
 
 RELEASE_CACHE = Path(__file__).parent / "release_cache.json"
 
-IP_TYPES = (
+_CREATE_TYPES = {IPv6Address, IPv4Address, UUID, Color, Decimal, Path, Version}
+
+IP_TYPES = {
     Union[IPv4Address, str, None],
     Union[IPv4Address, str],
     Union[IPv6Address, str, None],
     Union[IPv6Address, str],
     Union[IPv6Address, IPv4Address, str, None],
     Union[IPv6Address, IPv4Address, str],
     Union[IPv6Address, IPv4Address],
     Union[IPv6Address, IPv4Address, None],
-)
+}
 
 if sys.version_info[:2] < (3, 11):
     from async_timeout import (  # pylint: disable=unused-import # noqa: F401
         timeout as asyncio_timeout,
     )
 else:
     from asyncio import (  # pylint: disable=unused-import # noqa: F401
@@ -197,50 +200,47 @@
         return name[0].lower() + name[1:]
     return name
 
 
 def convert_unifi_data(value: Any, field: ModelField) -> Any:
     """Converts value from UFP data into pydantic field class"""
     from pyunifiprotect.data import (  # pylint: disable=import-outside-toplevel
-        Color,
         ProtectBaseObject,
     )
 
-    if field.shape == SHAPE_LIST and isinstance(value, list):
+    shape = field.shape
+    type_ = field.type_
+
+    if type_ == Any:
+        return value
+
+    if shape == SHAPE_LIST and isinstance(value, list):
         value = [convert_unifi_data(v, field) for v in value]
-    elif field.shape == SHAPE_SET and isinstance(value, list):
+    elif shape == SHAPE_SET and isinstance(value, list):
         value = {convert_unifi_data(v, field) for v in value}
-    elif field.shape == SHAPE_DICT and isinstance(value, dict):
+    elif shape == SHAPE_DICT and isinstance(value, dict):
         value = {k: convert_unifi_data(v, field) for k, v in value.items()}
-    elif field.type_ in IP_TYPES and value is not None:
+    elif type_ in IP_TYPES and value is not None:
         try:
             value = ip_address(value)
         except ValueError:
             pass
-    elif (
-        value is None
-        or not isclass(field.type_)
-        or issubclass(field.type_, ProtectBaseObject)
-        or isinstance(value, field.type_)
-    ):
+    elif value is None or not isclass(type_) or issubclass(type_, ProtectBaseObject) or isinstance(value, type_):
         return value
-    elif field.type_ in (IPv6Address, IPv4Address, UUID, Color, Decimal, Path, Version) or issubclass(
-        field.type_, Enum
-    ):
-        value = field.type_(value)
-    elif field.type_ == datetime:
+    elif type_ in _CREATE_TYPES or issubclass(type_, Enum):
+        value = type_(value)
+    elif type_ == datetime:
         value = from_js_time(value)
 
     return value
 
 
 def serialize_unifi_obj(value: Any) -> Any:
     """Serializes UFP data"""
     from pyunifiprotect.data import (  # pylint: disable=import-outside-toplevel
-        Color,
         ProtectModel,
     )
 
     if isinstance(value, ProtectModel):
         value = value.unifi_dict()
     if isinstance(value, dict):
         value = serialize_dict(value)
```

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect/websocket.py` & `pyunifiprotect-4.9.1/pyunifiprotect/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect.egg-info/PKG-INFO` & `pyunifiprotect-4.9.1/pyunifiprotect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunifiprotect
-Version: 4.9.0
+Version: 4.9.1
 Summary: Unofficial UniFi Protect Python API and CLI
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
 License: MIT
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
```

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect.egg-info/SOURCES.txt` & `pyunifiprotect-4.9.1/pyunifiprotect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/pyunifiprotect.egg-info/requires.txt` & `pyunifiprotect-4.9.1/pyunifiprotect.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/requirements.txt` & `pyunifiprotect-4.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/conftest.py` & `pyunifiprotect-4.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/data/test_camera.py` & `pyunifiprotect-4.9.1/tests/data/test_camera.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/data/test_chime.py` & `pyunifiprotect-4.9.1/tests/data/test_chime.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/data/test_common.py` & `pyunifiprotect-4.9.1/tests/data/test_common.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/data/test_doorlock.py` & `pyunifiprotect-4.9.1/tests/data/test_doorlock.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/data/test_light.py` & `pyunifiprotect-4.9.1/tests/data/test_light.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/data/test_nvr.py` & `pyunifiprotect-4.9.1/tests/data/test_nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/data/test_sensor.py` & `pyunifiprotect-4.9.1/tests/data/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/data/test_viewer.py` & `pyunifiprotect-4.9.1/tests/data/test_viewer.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/constants.py` & `pyunifiprotect-4.9.1/tests/sample_data/constants.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_bootstrap.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_bootstrap.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_bridge.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_bridge.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_camera.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_camera.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_camera_heatmap.png` & `pyunifiprotect-4.9.1/tests/sample_data/sample_camera_heatmap.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_camera_snapshot.png` & `pyunifiprotect-4.9.1/tests/sample_data/sample_camera_snapshot.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_camera_thumbnail.png` & `pyunifiprotect-4.9.1/tests/sample_data/sample_camera_thumbnail.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_camera_video.mp4` & `pyunifiprotect-4.9.1/tests/sample_data/sample_camera_video.mp4`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_chime.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_chime.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_constants.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_constants.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_doorlock.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_doorlock.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_event_smart_track.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_event_smart_track.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_light.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_light.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_liveview.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_liveview.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_raw_events.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_raw_events.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_sensor.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_sensor.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_viewport.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_viewport.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/sample_data/sample_ws_messages.json` & `pyunifiprotect-4.9.1/tests/sample_data/sample_ws_messages.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/test_api.py` & `pyunifiprotect-4.9.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/test_api_polling.py` & `pyunifiprotect-4.9.1/tests/test_api_polling.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/test_api_ws.py` & `pyunifiprotect-4.9.1/tests/test_api_ws.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.9.0/tests/test_utils.py` & `pyunifiprotect-4.9.1/tests/test_utils.py`

 * *Files identical despite different names*

