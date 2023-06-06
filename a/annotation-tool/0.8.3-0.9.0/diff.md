# Comparing `tmp/annotation_tool-0.8.3.tar.gz` & `tmp/annotation_tool-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annotation_tool-0.8.3.tar", max compression
+gzip compressed data, was "annotation_tool-0.9.0.tar", max compression
```

## Comparing `annotation_tool-0.8.3.tar` & `annotation_tool-0.9.0.tar`

### file list

```diff
@@ -1,96 +1,91 @@
--rw-r--r--   0        0        0     1085 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/LICENSE
--rw-r--r--   0        0        0     1280 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/README.md
--rw-r--r--   0        0        0       68 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/__init__.py
--rw-r--r--   0        0        0     8480 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/annotation_base.py
--rw-r--r--   0        0        0     5170 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/controller.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/manual/__init__.py
--rw-r--r--   0        0        0     5852 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/manual/controller.py
--rw-r--r--   0        0        0     3075 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/manual/main_widget.py
--rw-r--r--   0        0        0     2456 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/manual/tool_widget.py
--rw-r--r--   0        0        0       80 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/modes.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/__init__.py
--rw-r--r--   0        0        0    12649 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/controller.py
--rw-r--r--   0        0        0     3828 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/main_widget.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/__init__.py
--rw-r--r--   0        0        0      917 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/element.py
--rw-r--r--   0        0        0     1969 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/filter.py
--rw-r--r--   0        0        0     2184 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py
--rw-r--r--   0        0        0     6370 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/loader.py
--rw-r--r--   0        0        0    12318 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/query.py
--rw-r--r--   0        0        0     8256 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/queue.py
--rw-r--r--   0        0        0     2013 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/tool_widget.py
--rw-r--r--   0        0        0    14145 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/timeline.py
--rw-r--r--   0        0        0      479 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/data_model/__init__.py
--rw-r--r--   0        0        0     7726 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/annotation.py
--rw-r--r--   0        0        0     2077 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/annotation_scheme.py
--rw-r--r--   0        0        0     3003 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/dataset.py
--rw-r--r--   0        0        0      795 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/media_type.py
--rw-r--r--   0        0        0     4014 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/model.py
--rw-r--r--   0        0        0     2040 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/project.py
--rw-r--r--   0        0        0     3664 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/sample.py
--rw-r--r--   0        0        0     6412 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/single_annotation.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/__init__.py
--rw-r--r--   0        0        0    12197 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/annotation_dialog.py
--rw-r--r--   0        0        0    10523 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/annotation_list.py
--rw-r--r--   0        0        0     1956 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/dialog_manager.py
--rw-r--r--   0        0        0     7082 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/edit_datasets.py
--rw-r--r--   0        0        0    10994 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/import_annotation_dialog.py
--rw-r--r--   0        0        0     5706 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/load_annotation_dialog.py
--rw-r--r--   0        0        0     3670 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/local_files.py
--rw-r--r--   0        0        0    10576 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/network_list.py
--rw-r--r--   0        0        0     6899 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/new_annotation_dialog.py
--rw-r--r--   0        0        0    19491 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/settings_dialog.py
--rw-r--r--   0        0        0      197 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/file_cache/__init__.py
--rw-r--r--   0        0        0     9586 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/file_cache/_file_cache.py
--rw-r--r--   0        0        0     8506 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/gui.py
--rw-r--r--   0        0        0    12322 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/main_controller.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/__init__.py
--rw-r--r--   0        0        0    10152 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/controller.py
--rw-r--r--   0        0        0     4220 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/player.py
--rw-r--r--   0        0        0     5373 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/timer.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/type_specific_player/__init__.py
--rw-r--r--   0        0        0     8424 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/type_specific_player/mocap.py
--rw-r--r--   0        0        0     7082 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/type_specific_player/video.py
--rw-r--r--   0        0        0     2286 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/media.py
--rw-r--r--   0        0        0      357 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/__init__.py
--rw-r--r--   0        0        0     8866 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/base.py
--rw-r--r--   0        0        0     2167 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/mocap.py
--rw-r--r--   0        0        0      121 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/__init__.py
--rw-r--r--   0        0        0     3128 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/base.py
--rw-r--r--   0        0        0     4745 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/cache.py
--rw-r--r--   0        0        0     6020 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/lara_reader.py
--rw-r--r--   0        0        0     1787 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video.py
--rw-r--r--   0        0        0      157 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/__init__.py
--rw-r--r--   0        0        0     4096 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/base.py
--rw-r--r--   0        0        0     3668 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/decord_reader.py
--rw-r--r--   0        0        0     4321 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/evaluation.py
--rw-r--r--   0        0        0     7496 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/opencv_reader.py
--rw-r--r--   0        0        0     4170 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/mediator.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/LARa/__init__.py
--rw-r--r--   0        0        0    12119 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/LARa/attr_per_class.txt
--rw-r--r--   0        0        0     5583 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/LARa/lara_specifics.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/__init__.py
--rw-r--r--   0        0        0     7267 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/controller.py
--rw-r--r--   0        0        0    27224 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/network.py
--rw-r--r--   0        0        0     7556 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/playback.py
--rw-r--r--   0        0        0     1546 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py
--rw-r--r--   0        0        0     4401 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/checkable_combobox.py
--rw-r--r--   0        0        0     2170 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/display_scheme.py
--rw-r--r--   0        0        0     1798 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/histogram.py
--rw-r--r--   0        0        0      458 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/line_edit_adapted.py
--rw-r--r--   0        0        0      403 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/lines.py
--rw-r--r--   0        0        0     1077 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/own_slider.py
--rw-r--r--   0        0        0     1480 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/settings.py
--rw-r--r--   0        0        0     4037 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/user_actions.py
--rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/__init__.py
--rw-r--r--   0        0        0     4818 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/decorators.py
--rw-r--r--   0        0        0    11854 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/filehandler.py
--rw-r--r--   0        0        0     4059 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/functions.py
--rw-r--r--   0        0        0     2153 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/networking.py
--rw-r--r--   0        0        0     4469 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/priority_queue.py
--rw-r--r--   0        0        0    53863 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/resources.py
--rw-r--r--   0        0        0     1938 2023-05-04 12:28:40.291202 annotation_tool-0.8.3/main.py
--rw-r--r--   0        0        0     1949 2023-05-04 12:28:40.295202 annotation_tool-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 annotation_tool-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1280 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/README.md
+-rw-r--r--   0        0        0       68 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/annotation/__init__.py
+-rw-r--r--   0        0        0     9694 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/annotation/annotation_base.py
+-rw-r--r--   0        0        0     5170 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/annotation/controller.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/annotation/manual/__init__.py
+-rw-r--r--   0        0        0     6202 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/annotation/manual/controller.py
+-rw-r--r--   0        0        0     3075 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/annotation/manual/main_widget.py
+-rw-r--r--   0        0        0     2456 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/annotation/manual/tool_widget.py
+-rw-r--r--   0        0        0       80 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/annotation/modes.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/__init__.py
+-rw-r--r--   0        0        0    12649 2023-06-06 11:56:57.102593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/controller.py
+-rw-r--r--   0        0        0     3828 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/main_widget.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/__init__.py
+-rw-r--r--   0        0        0      917 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/element.py
+-rw-r--r--   0        0        0     1969 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/filter.py
+-rw-r--r--   0        0        0     2184 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py
+-rw-r--r--   0        0        0     5920 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/loader.py
+-rw-r--r--   0        0        0    12339 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/query.py
+-rw-r--r--   0        0        0     8256 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/queue.py
+-rw-r--r--   0        0        0     2013 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/annotation/retrieval/tool_widget.py
+-rw-r--r--   0        0        0    15091 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/annotation/timeline.py
+-rw-r--r--   0        0        0      484 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/data_model/__init__.py
+-rw-r--r--   0        0        0     5607 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/data_model/annotation.py
+-rw-r--r--   0        0        0     2253 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/data_model/annotation_scheme.py
+-rw-r--r--   0        0        0     1279 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/data_model/dataset.py
+-rw-r--r--   0        0        0      928 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/data_model/media_type.py
+-rw-r--r--   0        0        0     7365 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/data_model/model.py
+-rw-r--r--   0        0        0     3549 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/data_model/sample.py
+-rw-r--r--   0        0        0     6672 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/data_model/single_annotation.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/__init__.py
+-rw-r--r--   0        0        0    12371 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/annotation_dialog.py
+-rw-r--r--   0        0        0    10977 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/annotation_list.py
+-rw-r--r--   0        0        0     1956 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/dialog_manager.py
+-rw-r--r--   0        0        0     7159 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/edit_datasets.py
+-rw-r--r--   0        0        0    11156 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/import_annotation_dialog.py
+-rw-r--r--   0        0        0     5728 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/load_annotation_dialog.py
+-rw-r--r--   0        0        0     3279 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/local_files.py
+-rw-r--r--   0        0        0    13857 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/network_list.py
+-rw-r--r--   0        0        0     6926 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/new_annotation_dialog.py
+-rw-r--r--   0        0        0    19525 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/dialogs/settings_dialog.py
+-rw-r--r--   0        0        0      149 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/file_cache/__init__.py
+-rw-r--r--   0        0        0     8255 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/file_cache/_file_cache.py
+-rw-r--r--   0        0        0     8848 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/gui.py
+-rw-r--r--   0        0        0    13437 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/main_controller.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media/backend/__init__.py
+-rw-r--r--   0        0        0    10038 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media/backend/controller.py
+-rw-r--r--   0        0        0     4360 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media/backend/player.py
+-rw-r--r--   0        0        0     5385 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media/backend/timer.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media/backend/type_specific_player/__init__.py
+-rw-r--r--   0        0        0     7546 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media/backend/type_specific_player/mocap.py
+-rw-r--r--   0        0        0     7115 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media/backend/type_specific_player/video.py
+-rw-r--r--   0        0        0     2427 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media/media.py
+-rw-r--r--   0        0        0      279 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/__init__.py
+-rw-r--r--   0        0        0     9583 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/base.py
+-rw-r--r--   0        0        0     1694 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/mocap.py
+-rw-r--r--   0        0        0      121 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/mocap_readers/__init__.py
+-rw-r--r--   0        0        0     2816 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/mocap_readers/base.py
+-rw-r--r--   0        0        0     3839 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/mocap_readers/cache.py
+-rw-r--r--   0        0        0     5018 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/mocap_readers/lara_reader.py
+-rw-r--r--   0        0        0     1579 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/video.py
+-rw-r--r--   0        0        0      160 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/video_readers/__init__.py
+-rw-r--r--   0        0        0     2718 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/video_readers/base.py
+-rw-r--r--   0        0        0     2602 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/video_readers/decord_reader.py
+-rw-r--r--   0        0        0     4171 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/media_reader/video_readers/opencv_reader.py
+-rw-r--r--   0        0        0     4170 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/mediator.py
+-rw-r--r--   0        0        0       64 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/network/__init__.py
+-rw-r--r--   0        0        0     5956 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/network/controller.py
+-rw-r--r--   0        0        0     8622 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/network_video.py
+-rw-r--r--   0        0        0     7556 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/playback.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/__init__.py
+-rw-r--r--   0        0        0     1546 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py
+-rw-r--r--   0        0        0     4401 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/checkable_combobox.py
+-rw-r--r--   0        0        0     2170 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/display_scheme.py
+-rw-r--r--   0        0        0     1798 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/histogram.py
+-rw-r--r--   0        0        0      535 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/line_edit_adapted.py
+-rw-r--r--   0        0        0      403 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/lines.py
+-rw-r--r--   0        0        0     1122 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/own_slider.py
+-rw-r--r--   0        0        0     1230 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/settings.py
+-rw-r--r--   0        0        0     4124 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/user_actions.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/utility/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/utility/decorators.py
+-rw-r--r--   0        0        0     8454 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/utility/filehandler.py
+-rw-r--r--   0        0        0     2402 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/utility/functions.py
+-rw-r--r--   0        0        0     4469 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/utility/priority_queue.py
+-rw-r--r--   0        0        0    53863 2023-06-06 11:56:57.106593 annotation_tool-0.9.0/annotation_tool/utility/resources.py
+-rw-r--r--   0        0        0      520 2023-06-06 11:56:57.110593 annotation_tool-0.9.0/main.py
+-rw-r--r--   0        0        0     1949 2023-06-06 11:56:57.114594 annotation_tool-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 annotation_tool-0.9.0/PKG-INFO
```

### Comparing `annotation_tool-0.8.3/LICENSE` & `annotation_tool-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/README.md` & `annotation_tool-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/annotation_base.py` & `annotation_tool-0.9.0/annotation_tool/annotation/annotation_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             n_frames: Number of frames in the video/mocap file
         """
         self.samples = samples
         self.scheme = scheme
         self.dependencies = dependencies
         self.n_frames = n_frames
         self.position = 0
+        self.selected_sample_idx = None  # reset selected sample
         self.clear_undo_redo()
         self.check_for_selected_sample(force_update=True)
         self.load_subclass()
 
     @qtc.pyqtSlot(int)
     def setPosition(self, x: int) -> None:
         """
@@ -172,46 +173,72 @@
         """
         Annotate the current sample.
         """
         pass
 
     def check_for_selected_sample(self, force_update=False) -> None:
         """
-        Check if the current position is in a sample and if so, select it.
+        Find the selected sample and emit the samples_changed signal if the selected sample changed.
 
         Args:
-            force_update: Force updating the selected sample.
+            force_update: Force the update of the selected sample.
         """
+        _current_sample = self.selected_sample
+
+        if _current_sample is not None:
+            lo, hi = _current_sample.start_position, _current_sample.end_position
+
+            if lo <= self.position <= hi:
+                if force_update:
+                    self.samples_changed.emit(self.samples, _current_sample)
+                return
+
         if len(self.samples) > 0:
-            # binary search
-            lo = 0
-            hi = len(self.samples) - 1
-
-            while lo <= hi:
-                mid = (lo + hi) // 2
-                sample = self.samples[mid]
-                if sample.start_position <= self.position <= sample.end_position:
-                    break
-                elif self.position < sample.start_position:
-                    hi = mid - 1
+            if len(self.samples) > 75:
+                # binary search for large number of samples
+                lo = 0
+                hi = len(self.samples) - 1
+
+                while lo <= hi:
+                    mid = (lo + hi) // 2
+                    sample = self.samples[mid]
+                    if sample.start_position <= self.position <= sample.end_position:
+                        break
+                    elif self.position < sample.start_position:
+                        hi = mid - 1
+                    else:
+                        lo = mid + 1
                 else:
-                    lo = mid + 1
+                    raise RuntimeError(
+                        f"Could not find sample at position {self.position}"
+                    )
+                sample_idx = mid
             else:
-                raise RuntimeError(f"Could not find sample at position {self.position}")
+                # linear search for small number of samples
+                for sample_idx, sample in enumerate(self.samples):
+                    if sample.start_position <= self.position <= sample.end_position:
+                        break
+                else:
+                    raise RuntimeError(
+                        f"Could not find sample at position {self.position}"
+                    )
 
             if force_update or self.selected_sample is not sample:
-                self.selected_sample_idx = mid
+                self.selected_sample_idx = sample_idx
                 self.samples_changed.emit(self.samples, sample)
         else:
             assert self.position == 0
 
     @property
     def selected_sample(self) -> Optional[Sample]:
         if self.selected_sample_idx is not None:
-            return self.samples[self.selected_sample_idx]
+            try:
+                return self.samples[self.selected_sample_idx]
+            except IndexError:
+                return None
         else:
             return None
 
     def copy(self):
         """
         Copy the current annotation.
         """
@@ -304,17 +331,18 @@
         """
         Update the annotation of a sample.
 
         Args:
             sample: Sample to update.
             new_annotation: New annotation.
         """
-        self.add_to_undo_stack()
-        sample.annotation = new_annotation
-        self.samples_changed.emit(self.samples, self.selected_sample)
+        if sample.annotation != new_annotation:
+            self.add_to_undo_stack()
+            sample.annotation = new_annotation
+            self.samples_changed.emit(self.samples, self.selected_sample)
 
     @abstractmethod
     def load_subclass(self) -> None:
         """
         Load the subclass.
         """
         raise NotImplementedError
```

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/controller.py` & `annotation_tool-0.9.0/annotation_tool/annotation/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/manual/controller.py` & `annotation_tool-0.9.0/annotation_tool/annotation/manual/controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from annotation_tool.annotation.annotation_base import AnnotationBaseClass
 from annotation_tool.annotation.manual.main_widget import QDisplaySample
 from annotation_tool.annotation.manual.tool_widget import ManualAnnotationTools
 from annotation_tool.annotation.modes import AnnotationMode
 from annotation_tool.data_model import Sample
 from annotation_tool.dialogs.annotation_dialog import QAnnotationDialog
+from annotation_tool.settings import settings
 
 
 class ManualAnnotation(AnnotationBaseClass):
     def __init__(self):
         super().__init__()
 
         self.mode = AnnotationMode.MANUAL
@@ -56,15 +57,15 @@
 
     def annotate(self):
         if self.enabled:
             dialog = QAnnotationDialog(
                 self.selected_sample, self.scheme, self.dependencies
             )
             self.pause_replay.emit()
-            dialog.finished.connect(lambda _: self.check_for_selected_sample(True))
+            dialog.annotation_changed.connect(self.update_sample_annotation)
             self.open_dialog(dialog)
 
     def cut(self):
         if self.enabled:
             sample = self.selected_sample
 
             start_1, end_1 = sample.start_position, self.position
@@ -101,15 +102,22 @@
 
             other_idx = sample_idx - 1 if left else sample_idx + 1
             if 0 <= other_idx < len(self.samples):
                 other_sample = self.samples[other_idx]
                 start = min(sample.start_position, other_sample.start_position)
                 end = max(sample.end_position, other_sample.end_position)
 
-                merged_sample = Sample(start, end, other_sample.annotation)
+                if settings.merging_mode == "from":
+                    annotation = sample.annotation
+                elif settings.merging_mode == "into":
+                    annotation = other_sample.annotation
+                else:
+                    raise ValueError(f"Invalid merging mode: {settings.merging_mode}")
+
+                merged_sample = Sample(start, end, annotation)
 
                 self.add_to_undo_stack()
 
                 self.samples.remove(sample)
                 self.samples.remove(other_sample)
                 self.samples.insert(min(sample_idx, other_idx), merged_sample)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/manual/main_widget.py` & `annotation_tool-0.9.0/annotation_tool/annotation/manual/main_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/manual/tool_widget.py` & `annotation_tool-0.9.0/annotation_tool/annotation/manual/tool_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/controller.py` & `annotation_tool-0.9.0/annotation_tool/annotation/retrieval/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/main_widget.py` & `annotation_tool-0.9.0/annotation_tool/annotation/retrieval/main_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/element.py` & `annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/element.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/filter.py` & `annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/filter.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py` & `annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/loader.py` & `annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,36 @@
+import logging
 from typing import List, Tuple
 
 import PyQt6.QtCore as qtc
 import numpy as np
 from scipy import spatial
 
 from annotation_tool.annotation.retrieval.retrieval_backend.element import (
     RetrievalElement,
 )
-from annotation_tool.data_model import SingleAnnotation
+from annotation_tool.data_model.single_annotation import create_single_annotation
 import annotation_tool.network.controller as network
 
 
 class RetrievalLoader(qtc.QThread):
     success = qtc.pyqtSignal(list, np.ndarray, list)
     error = qtc.pyqtSignal(Exception)
     progress = qtc.pyqtSignal(int)
 
     def __init__(self, controller, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.controller = controller
 
     def run(self):
-        # intervals, classifications, retrieval_elements = self.load()
-        # self.success.emit(intervals, classifications, retrieval_elements)
-        # return
         try:
             intervals, classifications, retrieval_elements = self.load()
             self.success.emit(intervals, classifications, retrieval_elements)
         except Exception as e:
+            logging.debug(str(e))
             self.error.emit(e)
 
     def load(
         self,
     ) -> Tuple[List[Tuple[int, int]], List[np.ndarray], List[RetrievalElement]]:
         # List of intervals (start, end) given by all not-annotated samples using
         # the user defined step- and interval-sizes (see settings dialog).
@@ -53,44 +52,38 @@
         if attribute_representations is not None and len(classifications) > 0:
             # Default case: We have attribute representations (="dependencies") and classifications.
             attribute_representations = np.array(
                 attribute_representations
             )  # cast to numpy array
 
             # Compute the distance between each attribute-representation and each classification.
-            if attribute_representations.shape[1] == 27:
-                # TODO: LAra specific -> remove later
-                # Attributes begin at the 8th index of the attribute representation
-                dists = spatial.distance.cdist(
-                    classifications, attribute_representations[:, 8:], metric="cosine"
-                )
-            else:
-                dists = spatial.distance.cdist(
-                    classifications, attribute_representations, metric="cosine"
-                )
+
+            dists = spatial.distance.cdist(
+                classifications, attribute_representations, metric="cosine"
+            )
 
             for i, interval in enumerate(intervals):
                 for j, attr_repr in enumerate(attribute_representations):
                     dist = dists[i, j]
-                    annotation = SingleAnnotation(
+                    annotation = create_single_annotation(
                         self.controller.scheme, np.copy(attr_repr)
                     )
 
                     # RetrievalElements are just wrapped tuples more or less (for convenience)
                     # (see annotation_tool/annotation/retrieval/retrieval_backend/element.py)
                     elem = RetrievalElement(annotation, interval, dist, i, j)
                     retrieval_elements.append(elem)
         else:
             # This case applies if the loaded dateset does not have any dependencies.
             # Instead of comparing each network-output to the attribute-representations/dependencies
             # we can only compare it to its rounded binarized version (each attribute is rounded to 0 or 1).
             for i, interval in enumerate(intervals):
                 attr_repr = np.round(classifications[i])
                 dist = spatial.distance.cosine(classifications[i], attr_repr)
-                annotation = SingleAnnotation(
+                annotation = create_single_annotation(
                     self.controller.scheme, np.copy(attr_repr)
                 )
                 elem = RetrievalElement(
                     annotation, interval, dist, i, None
                 )  # j is None here, because there are no dependencies.
                 retrieval_elements.append(elem)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/query.py` & `annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,15 @@
     def similarity_distribution(self) -> np.ndarray:
         """
         Returns the distance distribution of the query.
 
         Returns:
             The distance distribution of the query.
         """
-        start = time.perf_counter()
+        start = time.perf_counter()  # noqa
 
         accepted_similarities = np.array(
             [elem._similarity for elem in self.accepted_elements]
         )
 
         open_similarities = [
             self._retrieval_queue.peek_into_interval(i)._similarity
@@ -280,18 +280,18 @@
         ]
 
         # get similarity distribution
         similarity_distribution = np.concatenate(
             (accepted_similarities, open_similarities)
         )
 
-        end = time.perf_counter()
-        logging.debug(
-            f"Computing the similarity_distribution took {(end - start):.3f} seconds in total."
-        )
+        end = time.perf_counter()  # noqa
+        # logging.debug(
+        #    f"Computing the similarity_distribution took {(end - start):.3f} seconds in total."
+        # )
 
         return similarity_distribution
 
     def set_filter(self, new_filter: FilterCriterion = None) -> None:
         """
         Sets the filter set.
         If the filter is set to None, the filter is removed.
```

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/queue.py` & `annotation_tool-0.9.0/annotation_tool/annotation/retrieval/retrieval_backend/queue.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/tool_widget.py` & `annotation_tool-0.9.0/annotation_tool/annotation/retrieval/tool_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/annotation/timeline.py` & `annotation_tool-0.9.0/annotation_tool/annotation/timeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 from collections import namedtuple
+import time
 from typing import Tuple
 
 import PyQt6.QtCore as qtc
 import PyQt6.QtGui as qtg
 import PyQt6.QtWidgets as qtw
 
 from annotation_tool.data_model.sample import Sample
 from annotation_tool.settings import settings
 from annotation_tool.utility import functions
-from annotation_tool.utility.functions import FrameTimeMapper, ms_to_time_string
 
 ScalingRatio = namedtuple("ScalingRatio", ["Frames", "Pixels"])
 
+# set some constants
+HEIGHT_SAMPLE = 70
+MARGIN_SAMPLE = 10
+WIDTH_TEXT = 100
+HEIGHT_TEXT = 25
+HEIGHT_LINE = 40
+HEIGHT_DASHED_LINE = 20
+MARGIN_HORIZONTAL_LINES = 40
+
 
 class Scaling:
     def __init__(self, parent: qtw.QWidget):
         self.idx = 0
         self.parent = parent
         self.negative_scales = [
             ScalingRatio(1, 2),
@@ -111,20 +120,20 @@
 
     def __init__(self):
         super(qtw.QWidget, self).__init__()
         self.frame_idx = 0
         self.pos = None  # Don't remove
         self.scaler = Scaling(self)
         self.n_frames = self.width()
+        self.fps = 30
         self.lower = 0
 
         self.samples = []
         self.current_sample = None
 
-        # Set variables
         self.backgroundColor = qtg.QColor(60, 63, 65)
         self.textColor = qtg.QColor(187, 187, 187)
         self.clicking = False  # Check if mouse left button is being pressed
         self.is_in = False  # check if user is in the widget
 
         self.setMouseTracking(True)  # Mouse events
         self.setAutoFillBackground(True)  # background
@@ -132,18 +141,19 @@
         # Constants
         self.setMinimumSize(600, 200)
 
     @property
     def font(self):
         return qtg.QFont("Decorative", settings.font_size)
 
-    @qtc.pyqtSlot(int)
-    def set_range(self, n):
-        assert 0 < n
+    @qtc.pyqtSlot(int, float)
+    def set_range(self, n: int, fps: float):
+        assert 0 < n and 0 < fps
         self.n_frames = n
+        self.fps = fps
         self.update()
 
     def update_visible_range(self):
         if self.frame_idx <= self.scroll_left_interval[1]:
             too_less = self.scroll_left_interval[1] - self.frame_idx
             self.lower = max(self.lower - (too_less + 1), 0)
         elif self.frame_idx >= self.scroll_right_interval[0]:
@@ -260,40 +270,22 @@
         super().resizeEvent(event)
         self.update()
 
     def update(self) -> None:
         self.update_visible_range()
         super().update()
 
-    def paintEvent(self, event):
-        # set some constants
-        HEIGHT_SAMPLE = 70
-        MARGIN_SAMPLE = 10
-        WIDTH_TEXT = 100
-        HEIGHT_TEXT = 25
-        HEIGHT_LINE = 40
-        HEIGHT_DASHED_LINE = 20
-        MARGIN_HORIZONTAL_LINES = 40
-
-        # step_size between ticks
-        dist = 100
-
-        qp = qtg.QPainter()
-        qp.begin(self)
-        qp.setPen(self.textColor)
-        qp.setFont(self.font)
-        qp.setRenderHint(qtg.QPainter.RenderHint.Antialiasing)
-
+    def _draw_time(self, qp, dist):
         # Draw time
         pos = dist
         while pos < self.width():
             frame_idx = self.scaler.pixel_to_frame(int(pos)) + self.lower
 
-            time_stamp = FrameTimeMapper.instance().frame_to_ms(frame_idx)
-            time_stamp = ms_to_time_string(time_stamp)
+            time_stamp = int(frame_idx * 1000 / self.fps)
+            time_stamp = functions.ms_to_time_string(time_stamp)
             time_stamp = time_stamp.split(":")
             time_stamp = ":".join(time_stamp[:-1])
 
             start_pos = int(pos) - WIDTH_TEXT // 2
 
             # Draw time_stamps and frame_numbers
             qp.drawText(
@@ -317,16 +309,18 @@
                 HEIGHT_TEXT,
                 qtc.Qt.AlignmentFlag.AlignHCenter,
                 time_stamp,
             )
 
             pos += dist
 
+    def _draw_lines(self, qp, dist):
         # Draw horizontal lines
         qp.setPen(qtg.QPen(qtc.Qt.GlobalColor.darkCyan, 5, qtc.Qt.PenStyle.SolidLine))
+
         qp.drawLine(0, MARGIN_HORIZONTAL_LINES, self.width(), 40)
         lower_horizontal_line_y = (
             MARGIN_HORIZONTAL_LINES + 2 * MARGIN_SAMPLE + HEIGHT_SAMPLE
         )
         qp.drawLine(0, lower_horizontal_line_y, self.width(), lower_horizontal_line_y)
 
         # Draw dash lines
@@ -341,20 +335,27 @@
                 int(pos),
                 lower_dashed_line_y,
                 int(pos),
                 lower_dashed_line_y + HEIGHT_DASHED_LINE,
             )
             pos += dist
 
+    def _draw_mouse_pos(self, qp):
+        qp.setPen(qtc.Qt.GlobalColor.darkCyan)
+        qp.setBrush(qtg.QBrush(qtc.Qt.GlobalColor.darkCyan))
         # Draw line of current mouse-position
         if self.pos is not None and self.is_in:
             # qp.drawLine(self.pos.x(), 0, self.pos.x(), HEIGHT_LINE)
             line_height = MARGIN_HORIZONTAL_LINES + 2 * MARGIN_SAMPLE + HEIGHT_SAMPLE
             qp.drawLine(self.pos.x(), 0, self.pos.x(), line_height + HEIGHT_LINE)
 
+    def _draw_pointer(self, qp):
+        qp.setPen(qtc.Qt.GlobalColor.darkCyan)
+        qp.setBrush(qtg.QBrush(qtc.Qt.GlobalColor.darkCyan))
+
         # Draw pos
         if self.frame_idx is not None:
             pos = self.scaler.frame_to_pixel(self.frame_idx - self.lower)
 
             line_height = 2 * MARGIN_SAMPLE + HEIGHT_SAMPLE
             line = qtc.QLine(
                 qtc.QPoint(pos, MARGIN_HORIZONTAL_LINES),
@@ -374,59 +375,80 @@
                 [
                     qtc.QPoint(pos - 10, 20),
                     qtc.QPoint(pos + 10, 20),
                     qtc.QPoint(pos, 40),
                 ]
             )
 
-        # Draw samples
-        for sample in self.samples:
-            if sample.start_position > self.upper or sample.end_position < self.lower:
-                continue
+        qp.drawPolygon(poly)
+        qp.drawLine(line)
+
+    def _draw_samples(self, qp):
+        qp.setPen(qtc.Qt.GlobalColor.white)
+        qp.setBrush(qtc.Qt.BrushStyle.NoBrush)
 
+        # Clear clip path
+        height = MARGIN_HORIZONTAL_LINES + MARGIN_SAMPLE
+
+        # Draw samples
+        for sample in self.samples_in_view:
             sample_start = self.scaler.frame_to_pixel(
                 sample.start_position - self.lower
             )
             sample_end = self.scaler.frame_to_pixel(sample.end_position - self.lower)
             sample_length = sample_end - sample_start + 1
 
             r, g, b = sample.color
             alpha = 255 if sample == self.current_sample else 127
             color = qtg.QColor(r, g, b, alpha)
 
-            # Clear clip path
-            height = MARGIN_HORIZONTAL_LINES + MARGIN_SAMPLE
+            if settings.timeline_design == "rounded":
+                path = qtg.QPainterPath()
+                path.addRoundedRect(
+                    sample_start, height, sample_length, HEIGHT_SAMPLE, 10, 10
+                )
+                qp.setClipPath(path)
+                qp.setPen(color)
+                qp.fillPath(path, color)
+                qp.drawPath(path)
+            elif settings.timeline_design == "rectangular":
+                qp.fillRect(sample_start, height, sample_length, HEIGHT_SAMPLE, color)
+            else:
+                raise ValueError(f"Unknown timeline design: {settings.timeline_design}")
 
-            path = qtg.QPainterPath()
-            path.addRoundedRect(
-                qtc.QRectF(sample_start, height, sample_length, HEIGHT_SAMPLE), 10, 10
-            )
-            qp.setClipPath(path)
+    def paintEvent(self, event):
+        # step_size between ticks
+        dist = 100
 
-            path = qtg.QPainterPath()
-            qp.setPen(color)
-            path.addRoundedRect(
-                qtc.QRectF(sample_start, height, sample_length, HEIGHT_SAMPLE), 10, 10
-            )
-            qp.fillPath(path, color)
-            qp.drawPath(path)
+        # init painter
+        qp = qtg.QPainter()
+        qp.begin(self)
+        qp.setPen(self.textColor)
+        qp.setFont(self.font)
+        qp.setRenderHint(qtg.QPainter.RenderHint.Antialiasing)
+
+        self._draw_time(qp, dist)
+        self._draw_lines(qp, dist)
+        self._draw_mouse_pos(qp)
+
+        # This is the bottleneck for drawing the timeline
+        _s_draw = time.perf_counter()  # noqa
+        self._draw_samples(qp)
+        _e_draw = time.perf_counter()  # noqa
+        # print(f"Drawing samples took {_e_draw - _s_draw: .4f} seconds")
 
         # Clear clip path
         path = qtg.QPainterPath()
         path.addRect(
             self.rect().x(), self.rect().y(), self.rect().width(), self.rect().height()
         )
         qp.setClipPath(path)
 
-        # Draw pointer
-        qp.setPen(qtc.Qt.GlobalColor.darkCyan)
-        qp.setBrush(qtg.QBrush(qtc.Qt.GlobalColor.darkCyan))
+        self._draw_pointer(qp)
 
-        qp.drawPolygon(poly)
-        qp.drawLine(line)
         qp.end()
 
     @property
     def upper(self):
         return self.lower + self.scaler.pixel_to_frame(self.width()) - 1
 
     @property
@@ -440,7 +462,15 @@
     @property
     def scroll_left_interval(self):
         return self.lower, self.lower + self.n_inner_frames // 10
 
     @property
     def scroll_right_interval(self):
         return self.upper - self.n_inner_frames // 10, self.upper
+
+    @property
+    def samples_in_view(self):
+        return (
+            sample
+            for sample in self.samples
+            if sample.start_position <= self.upper and sample.end_position >= self.lower
+        )
```

### Comparing `annotation_tool-0.8.3/annotation_tool/data_model/annotation.py` & `annotation_tool-0.9.0/annotation_tool/data_model/annotation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,48 @@
-import copy
 from dataclasses import dataclass, field
-import json
 import logging
-import math
-import os
+from pathlib import Path
 import time
-from typing import List
+from typing import List, Tuple
 
 import numpy as np
 
 from annotation_tool.file_cache import cached
-from annotation_tool.utility.decorators import accepts
-from annotation_tool.utility.filehandler import footprint_of_file
+from annotation_tool.media_reader import meta_data as get_meta_data
+from annotation_tool.utility.decorators import accepts, returns
+from annotation_tool.utility.filehandler import checksum, is_non_zero_file
 
 from .dataset import Dataset
 from .sample import Sample
 from .single_annotation import empty_annotation
 
 
 @cached
 @dataclass
 class Annotation:
     annotator_id: int
     _dataset: Dataset
     name: str
-    _media_path: os.PathLike
-    _footprint: str = field(init=False)
+    _annotated_file: Path
+    _checksum: str = field(init=False)
     _samples: list = field(init=False, default_factory=list)
-    _timestamp: time.struct_time = field(init=False, default_factory=time.localtime)
-    _additional_media_paths: List[os.PathLike] = field(init=False, default_factory=list)
+    _creation_time: time.time = field(init=False, default_factory=time.time)
+    _additional_media_paths: List[Tuple[Path, int]] = field(
+        init=False, default_factory=list
+    )
+    _last_save: float = field(init=False, default_factory=time.time)
 
     def __post_init__(self):
-        # finish initialization
-        from annotation_tool.utility.filehandler import footprint_of_file
-
-        self.__init_valid__()
-        self._footprint = footprint_of_file(self.path)
+        self._checksum = checksum(self.path)
         self.__init_samples__()
 
-    def __init_valid__(self):
-        assert self.dataset is not None, "Dataset must not be None."
-        assert isinstance(self.dataset, Dataset), "Dataset must be of type Dataset."
-        assert self.name is not None, "Name must not be None."
-        assert isinstance(self.name, str), "Name must be of type str."
-        assert len(self.name) > 0, "Name must not be empty."
-        assert self.annotator_id is not None, "Annotator ID must not be None."
-        assert isinstance(self.annotator_id, int), "Annotator ID must be of type int."
-        assert (
-            self.annotator_id >= 0
-        ), "Annotator ID must be greater than or equal to 0."
-        assert self.path is not None, "Path must not be None."
-        assert isinstance(
-            self.path, (str, os.PathLike)
-        ), "Path must be of type os.PathLike."
-        assert os.path.isfile(self.path), "Path must be a file."
-        assert os.path.getsize(self.path) > 0, "Path must not be empty."
-
     def __init_samples__(self):
-        from annotation_tool.media_reader import MediaReader, media_reader
-
-        media: MediaReader = media_reader(self.path)
-
+        n_frames = get_meta_data(self.path)["n_frames"]
         a = empty_annotation(self.dataset.scheme)
-        s = Sample(0, len(media) - 1, a)
+        s = Sample(0, n_frames - 1, a)
         self._samples.append(s)
 
     @property
     def samples(self) -> List[Sample]:
         # assert len(self._samples) > 0, "Samples must not be empty."
         return self._samples
 
@@ -84,14 +60,15 @@
                     raise ValueError("Elements must be from type Sample.")
                 if sample.start_position != last + 1:
                     logging.error("Last = {} | sample = {}".format(last, sample))
                     raise ValueError("Gaps between Samples are not allowed!")
                 last = sample.end_position
 
             self._samples = list_of_samples
+            self._last_save = time.time()
 
     def to_numpy(self) -> np.ndarray:
         """
         Converts the samples to a numpy array.
 
         Returns:
             np.ndarray: The samples as a numpy array.
@@ -108,28 +85,28 @@
         return x
 
     @property
     def dataset(self) -> Dataset:
         return self._dataset
 
     @property
-    def path(self) -> os.PathLike:
-        return self._media_path
+    def path(self) -> Path:
+        return self._annotated_file
 
     @path.setter
-    def path(self, path: os.PathLike):
-        if not os.path.isfile(path):
+    def path(self, path: Path):
+        if not path.is_file():
             raise FileNotFoundError(path)
-        if footprint_of_file(path) != self.footprint:
+        if checksum(path) != self.checksum:
             raise ValueError("File has changed.")
-        self._media_path = path
+        self._annotated_file = path
 
     @property
     def creation_time(self) -> time.struct_time:
-        return self._timestamp
+        return time.localtime(self._creation_time)
 
     @property
     def timestamp(self) -> str:
         return time.strftime("%Y-%m-%d_%H-%M-%S", self.creation_time)
 
     @property
     def progress(self) -> int:
@@ -141,103 +118,63 @@
         n_annotations = sum(
             [
                 s.end_position - s.start_position + 1
                 for s in self.samples
                 if not s.annotation.is_empty()
             ]
         )
-        return math.ceil(n_annotations / n_frames * 100)
+        return int(n_annotations / n_frames * 100)
 
     @property
     def meta_data(self) -> dict:
         return {
             "annotator_id": self.annotator_id,
             "dataset": self.dataset.name,
-            "file": self.path,
+            "file": self.path.as_posix(),
             "name": self.name,
             "creation_time": self.timestamp,
             "progress": self.progress,
         }
 
     @property
-    def footprint(self) -> str:
-        return self._footprint
+    def checksum(self) -> str:
+        return self._checksum
+
+    @property
+    def last_save(self) -> float:
+        return self._last_save
 
-    def set_additional_media_paths(self, paths: List[os.PathLike]):
+    def set_additional_media_paths(self, paths_with_offsets: List[Tuple[Path, int]]):
         additional_paths = []
-        for x in paths:
-            if not os.path.isfile(x):
-                raise FileNotFoundError(x)
-            additional_paths.append(x)
+        for p, o in paths_with_offsets:
+            if not p.is_file():
+                raise FileNotFoundError(p)
+            additional_paths.append((p, o))
         self._additional_media_paths = additional_paths
 
-    def get_additional_media_paths(self) -> List[os.PathLike]:
+    def get_additional_media_paths(self) -> List[Tuple[Path, int]]:
         return self._additional_media_paths
 
-    # TODO: update copy functions (additional media paths)
-    def __copy__(self):
-        return Annotation(
-            self.annotator_id,
-            self.dataset,
-            self.name,
-            self.path,
-        )
-
-    def __deepcopy__(self, memodict={}):
-        return Annotation(
-            self.annotator_id,
-            copy.deepcopy(self.dataset),
-            self.name,
-            self.path,
-        )
-
-    def to_dict(self) -> dict:
-        _annotations = []
-        for sample in self.samples:
-            _tmp = {
-                "start": sample.start_position,
-                "end": sample.end_position,
-                "annotation": sample.annotation.annotation_dict,
-            }
-            _annotations.append(_tmp)
-
-        _dataset = self.dataset.to_dict()
-
-        _additional_media_paths = self._additional_media_paths
-
-        _d = {
-            "annotator_id": self.annotator_id,
-            "dataset": _dataset,
-            "annotations": _annotations,
-            "name": self.name,
-            "path": self.path,
-            "footprint": self.footprint,
-            "timestamp": self.timestamp,
-            "additional_media_paths": _additional_media_paths,
-        }
-        return _d
-
-    def to_json(self) -> str:
-        return json.dumps(self.to_dict(), indent=4, sort_keys=True, ensure_ascii=False)
-
 
-def create_global_state(
-    annotator_id: int, dataset: Dataset, name: str, path: os.PathLike
+@returns(Annotation)
+@accepts(int, Dataset, str, Path)
+def create_annotation(
+    annotator_id: int, dataset: Dataset, name: str, file_path: Path
 ) -> Annotation:
     """
     Creates a new GlobalState object.
 
     Args:
         annotator_id (int): The id of the annotator.
         dataset (Dataset): The dataset.
         name (str): The name of the annotation.
-        path (os.PathLike): The path to the media file.
+        file_path (Path): The path to the file to be annotated.
 
     Returns:
         Annotation: The new GlobalState object.
     Raises:
         ValueError If parameters are invalid.
     """
-    try:
-        return Annotation(annotator_id, dataset, name, path)
-    except AssertionError as e:
-        raise ValueError(e)
+    if is_non_zero_file(file_path):
+        return Annotation(annotator_id, dataset, name, file_path)
+    else:
+        raise ValueError(f"File {file_path} does not exist or is empty.")
```

### Comparing `annotation_tool-0.8.3/annotation_tool/data_model/annotation_scheme.py` & `annotation_tool-0.9.0/annotation_tool/data_model/annotation_scheme.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from collections import namedtuple
 from copy import deepcopy
 from dataclasses import dataclass, field
 import logging
+from typing import List
 
+from annotation_tool.utility.decorators import accepts, returns
 
-def scheme_is_valid(scheme):
+
+@returns(bool)
+@accepts(List)
+def _scheme_is_valid(scheme: List) -> bool:
     try:
         valid = True
         valid &= scheme is not None
         valid &= isinstance(scheme, list)
         valid &= len(scheme) > 0
         for x in scheme:
             valid &= isinstance(x, (list, tuple))
@@ -38,34 +43,35 @@
             ["group_name", "element_name", "row", "column"],
         )
         for row, (group_name, group_elements) in enumerate(self.scheme):
             for col, elem in enumerate(group_elements):
                 yield scheme_element(group_name, elem, row, col)
 
     def __copy__(self):
-
         return AnnotationScheme(self.scheme, self._scheme_str, self._n)
 
     def __deepcopy__(self, memo):
         return AnnotationScheme(deepcopy(self.scheme), self._scheme_str, self._n)
 
 
+@returns(AnnotationScheme)
+@accepts(list)
 def create_annotation_scheme(scheme: list) -> AnnotationScheme:
     """
     Creates a new annotation scheme from the given scheme.
 
     Args:
         scheme: The scheme to create the annotation scheme from.
 
     Returns:
         The created annotation scheme.
 
     Raises:
         ValueError: If the scheme is invalid.
     """
-    if scheme_is_valid(scheme):
+    if _scheme_is_valid(scheme):
         n = 0
         for _, gr in scheme:
             n += len(gr)
         return AnnotationScheme(scheme, str(scheme), n)
     else:
         raise ValueError(f"{scheme} is not valid")
```

### Comparing `annotation_tool-0.8.3/annotation_tool/data_model/media_type.py` & `annotation_tool-0.9.0/annotation_tool/data_model/media_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import enum
 
+from annotation_tool.utility.decorators import accepts, returns
+
 
 class MediaType(enum.Enum):
     UNKNOWN = 0
     VIDEO = 1
     MOCAP = 2
     IMU = 3
 
 
 __str_map__ = {x.name: x for x in MediaType}
 
 
+@returns(str)
+@accepts(MediaType)
 def to_str(media_type: MediaType) -> str:
     """
     Returns the string representation of a media type.
 
     Args:
         media_type: The media type.
     Returns:
         The string representation of the media type.
     """
     return media_type.name
 
 
+@returns(MediaType)
+@accepts(str)
 def from_str(media_type: str) -> MediaType:
     """
     Returns the media type from a string.
 
     Args:
         media_type: The string representation of the media type.
```

### Comparing `annotation_tool-0.8.3/annotation_tool/data_model/sample.py` & `annotation_tool-0.9.0/annotation_tool/data_model/sample.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from dataclasses import dataclass, field
 import random
 from typing import Tuple
 
 from distinctipy import distinctipy
 
 from annotation_tool.data_model.single_annotation import SingleAnnotation
-from annotation_tool.utility.decorators import accepts_m, returns
+from annotation_tool.utility.decorators import accepts, accepts_m, returns
 
 random.seed(42)
 __color_map__ = distinctipy.get_colors(50, n_attempts=250)
 __default_color__ = 105, 105, 105
 
 
-def __annotation_to_color__(annotation: SingleAnnotation) -> Tuple[int, int, int, int]:
+@returns(tuple)
+@accepts(SingleAnnotation)
+def __annotation_to_color__(annotation: SingleAnnotation) -> Tuple[int, int, int]:
     """
     Converts an annotation to a color.
 
      Args:
         annotation: The annotation to convert.
 
     Returns:
@@ -39,27 +41,21 @@
     r, g, b = int(r * 255), int(g * 255), int(b * 255)
 
     return r, g, b
 
 
 @dataclass(order=True, unsafe_hash=True)
 class Sample:
-    _sort_index: int = field(init=False, repr=False, hash=False, compare=False)
     _start_pos: int = field(init=True, hash=True, compare=True)
     _end_pos: int = field(init=True, hash=True, compare=True)
     _annotation: SingleAnnotation = field(init=True, hash=False, compare=False)
+    _color: Tuple[int, int, int] = field(init=False, hash=False, compare=False)
 
     def __post_init__(self):
-        assert isinstance(self._start_pos, int)
-        assert isinstance(self._end_pos, int)
-        assert isinstance(self._annotation, SingleAnnotation)
-        assert self._start_pos <= self._end_pos
-        assert self._start_pos >= 0
-
-        self._sort_index = self._start_pos
+        self._color = __annotation_to_color__(self._annotation)
 
     def __len__(self):
         return (self._end_pos - self._start_pos) + 1
 
     @property
     @returns(int)
     def start_position(self):
@@ -96,26 +92,31 @@
     def annotation(self, value):
         if value is None:
             raise ValueError("None not allowed")
         # check compatibility
         if self.annotation.scheme != value.scheme:
             raise ValueError("Incompatible schemes")
         self._annotation = value
+        self._color = __annotation_to_color__(
+            value
+        )  # update color, computing it is expensive
 
     @property
     def color(self):
-        return __annotation_to_color__(self._annotation)
+        return self._color
 
     def __copy__(self):
         return Sample(self._start_pos, self._end_pos, self._annotation)
 
     def __deepcopy__(self, memo):
         return Sample(self._start_pos, self._end_pos, deepcopy(self._annotation))
 
 
+@returns(Sample)
+@accepts(int, int, SingleAnnotation)
 def create_sample(start_pos: int, end_pos: int, annotation: SingleAnnotation) -> Sample:
     """
     Creates a new sample.
 
     Args:
         start_pos: The start position of the sample.
         end_pos: The end position of the sample.
@@ -123,11 +124,8 @@
 
     Returns:
         The created sample.
 
     Raises:
         ValueError: If the parameters are invalid.
     """
-    try:
-        return Sample(start_pos, end_pos, annotation)
-    except AssertionError:
-        raise ValueError("Invalid sample.")
+    return Sample(start_pos, end_pos, annotation)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/data_model/single_annotation.py` & `annotation_tool-0.9.0/annotation_tool/data_model/single_annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from collections import namedtuple
 from copy import deepcopy
 from typing import Union
 
 import numpy as np
 
-from annotation_tool.utility.decorators import returns
+from annotation_tool.utility.decorators import accepts, returns
 
 from .annotation_scheme import AnnotationScheme
 
 
+@returns(type(True))
+@accepts((np.ndarray, dict), AnnotationScheme)
 def is_compatible(raw_annotation: Union[np.ndarray, dict], scheme: AnnotationScheme):
     if len(scheme) <= 0:
         return False
     if isinstance(raw_annotation, dict):
         for elem in scheme:
             val = raw_annotation.get(elem.row)(elem.column)
             if val is None:
@@ -23,23 +25,19 @@
                 return False
         return True
     if isinstance(raw_annotation, np.ndarray):
         if len(scheme) != raw_annotation.shape[0]:
             return False
         if len(raw_annotation.shape) > 1:
             return False
-        return np.all((raw_annotation == 0) | (raw_annotation == 1))
+        return bool(np.all((raw_annotation == 0) | (raw_annotation == 1)))
 
     return False
 
 
-def empty_annotation(scheme: AnnotationScheme):
-    return SingleAnnotation(scheme)
-
-
 class SingleAnnotation:
     def __init__(
         self, scheme: AnnotationScheme, annotation: Union[np.ndarray, dict, None] = None
     ):
         assert isinstance(scheme, AnnotationScheme)
 
         if annotation is None:
@@ -74,15 +72,15 @@
         if isinstance(a, dict):
             return a
         else:
             raise RuntimeError
 
     def _make_vector(self, a):
         if isinstance(a, np.ndarray):
-            a = a.astype(dtype=np.int8)
+            a = np.array(a, copy=True, dtype=np.int8)
             return a
         if isinstance(a, dict):
             ls = []
             for scheme_element in self.scheme:
                 group_name, elem = (
                     scheme_element.group_name,
                     scheme_element.element_name,
@@ -148,20 +146,20 @@
             scheme_equal = self.scheme == other.scheme
             vec_equal = np.array_equal(self.annotation_vector, other.annotation_vector)
             return scheme_equal and vec_equal
         else:
             return False
 
     def __copy__(self):
-        new_anno = SingleAnnotation(self.scheme, self.annotation_vector)
+        new_anno = create_single_annotation(self.scheme, self.annotation_vector)
         assert self == new_anno and new_anno is not self
         return new_anno
 
     def __deepcopy__(self, memo):
-        new_anno = SingleAnnotation(
+        new_anno = create_single_annotation(
             deepcopy(self.scheme), deepcopy(self.annotation_vector)
         )
         assert self == new_anno
         assert new_anno is not self
         return new_anno
 
     def __iter__(self):
@@ -179,15 +177,17 @@
             yield annotation_element(group_name, element_name, value, row, col)
 
     def __hash__(self):
         # logging.warning("Hash of annotation is deprecated")
         return hash((self.scheme, self.binary_str))
 
 
-def create_annotation(
+@returns(SingleAnnotation)
+@accepts(AnnotationScheme, (np.ndarray, dict, type(None)))
+def create_single_annotation(
     scheme: AnnotationScheme, annotation: Union[np.ndarray, dict, None] = None
 ) -> SingleAnnotation:
     """
     Create an annotation from a scheme and a vector or a dict.
 
     Args:
         scheme: The scheme of the annotation.
@@ -197,11 +197,17 @@
         The annotation.
 
     Raises:
         ValueError: If the parameters are not valid.
     """
     try:
         return SingleAnnotation(scheme, annotation)
-    except AssertionError:
+    except AssertionError as e:
+        print(str(e))
         raise ValueError(
             "Cannot create annotation from {} and {}".format(scheme, annotation)
         )
+
+
+@returns(SingleAnnotation)
+def empty_annotation(scheme: AnnotationScheme):
+    return SingleAnnotation(scheme)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/dialogs/annotation_dialog.py` & `annotation_tool-0.9.0/annotation_tool/dialogs/annotation_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import PyQt6.QtCore as qtc
 import PyQt6.QtWidgets as qtw
 import numpy as np
 
 from annotation_tool.data_model import AnnotationScheme, Sample
-from annotation_tool.data_model.single_annotation import SingleAnnotation
+from annotation_tool.data_model.single_annotation import (
+    SingleAnnotation,
+    create_single_annotation,
+    empty_annotation,
+)
 
 preferred_size = None
 
 
 class QAnnotationDialog(qtw.QDialog):
+    annotation_changed = qtc.pyqtSignal(Sample, SingleAnnotation)
+
     def __init__(
         self,
         sample: Sample,
         scheme: AnnotationScheme,
         dependencies: np.ndarray = None,
         *args,
         **kwargs
@@ -206,33 +212,32 @@
             self.accept_button.setEnabled(True)
         else:
             attr_vec = self.get_current_vector()
             x = np.equal(attr_vec, arr).all(axis=1).any()
             self.accept_button.setEnabled(x)
 
     def __reset_annotation__(self):
-        self.sample.annotation = SingleAnnotation(self.scheme)
+        self.annotation_changed.emit(self.sample, empty_annotation(self.scheme))
         self.close()
 
     def __save_annotation__(self):
         # Empty Annotation -> Reset Sample
         if not np.any(self.current_selection):
             self.__reset_annotation__()
             return
         # Default Case
         else:
             if self.dependencies is None:
                 attr_vec = self.current_selection
             else:
                 attr_vec = self.get_current_vector()
 
-        anno = self.sample.annotation
-        anno.annotation = attr_vec
+        new_annotation = create_single_annotation(self.scheme, attr_vec)
+        self.annotation_changed.emit(self.sample, new_annotation)
 
-        self.sample.annotation = anno
         self.close()
 
     def __cancel_annotation__(self):
         self.close()
 
     def resizeEvent(self, a0) -> None:
         global preferred_size
```

### Comparing `annotation_tool-0.8.3/annotation_tool/dialogs/annotation_list.py` & `annotation_tool-0.9.0/annotation_tool/dialogs/annotation_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,79 @@
 import os
+from pathlib import Path
 import shutil
 
 import PyQt6.QtCore as qtc
+from PyQt6.QtGui import QIntValidator
 import PyQt6.QtWidgets as qtw
 
 from annotation_tool.data_model.annotation import Annotation
 from annotation_tool.utility import filehandler
 
 
-class GlobalStateWidget(qtw.QWidget):
+class AnnotationManagerWidget(qtw.QWidget):
     deleted = qtc.pyqtSignal()
 
     def __init__(self, global_state: Annotation, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.global_state = global_state
+        self.current_annotation = global_state
         self.init_ui()
         self._delete = False
 
     def init_ui(self):
         self.grid = qtw.QGridLayout(self)
 
         # name
         self.name_label = qtw.QLabel("Name")
-        self.name_edit = qtw.QLineEdit(self.global_state.name)
+        self.name_edit = qtw.QLineEdit(self.current_annotation.name)
         self.name_edit.textChanged.connect(self.name_changed)
         self.grid.addWidget(self.name_label, 0, 0)
         self.grid.addWidget(self.name_edit, 0, 1)
 
         # file
         self.file_label = qtw.QLabel("File")
-        file_name = os.path.basename(self.global_state.path)
+        file_name = os.path.basename(self.current_annotation.path)
         self.file_edit = qtw.QLineEdit(file_name)
         self.file_edit.setReadOnly(True)
-        self.file_edit.setToolTip(self.global_state.path)
+        self.file_edit.setToolTip(self.current_annotation.path.as_posix())
         self.grid.addWidget(self.file_label, 1, 0)
         self.grid.addWidget(self.file_edit, 1, 1)
 
         # annotator id
         self.annotator_id_label = qtw.QLabel("Annotator ID")
-        self.annotator_id_edit = qtw.QLineEdit(str(self.global_state.annotator_id))
+        self.annotator_id_edit = qtw.QLineEdit(
+            str(self.current_annotation.annotator_id)
+        )
+        onlyInt = QIntValidator()
+        onlyInt.setRange(0, 1000)
+        self.annotator_id_edit.setValidator(onlyInt)
+        self.annotator_id_edit.setMaxLength(3)
         self.annotator_id_edit.textChanged.connect(self.annotator_id_changed)
         self.grid.addWidget(self.annotator_id_label, 2, 0)
         self.grid.addWidget(self.annotator_id_edit, 2, 1)
 
         # timestamp
         self.timestamp_label = qtw.QLabel("Created")
-        self.timestamp_edit = qtw.QLineEdit(self.global_state.timestamp)
+        self.timestamp_edit = qtw.QLineEdit(self.current_annotation.timestamp)
         self.timestamp_edit.setReadOnly(True)
         self.grid.addWidget(self.timestamp_label, 3, 0)
         self.grid.addWidget(self.timestamp_edit, 3, 1)
 
         # dataset
         self.dataset_label = qtw.QLabel("Dataset")
-        self.dataset_edit = qtw.QLineEdit(self.global_state.dataset.name)
+        self.dataset_edit = qtw.QLineEdit(self.current_annotation.dataset.name)
         self.dataset_edit.setReadOnly(True)
         self.grid.addWidget(self.dataset_label, 4, 0)
         self.grid.addWidget(self.dataset_edit, 4, 1)
 
         # show progress as a colored bar
         self.progress_label = qtw.QLabel("Progress")
         self.progress_bar = qtw.QProgressBar()
         self.progress_bar.setRange(0, 100)
-        self.progress_bar.setValue(self.global_state.progress)
+        self.progress_bar.setValue(self.current_annotation.progress)
         self.progress_bar.setTextVisible(True)
         self.progress_bar.setFormat("%p%")
         self.grid.addWidget(self.progress_label, 5, 0)
         self.grid.addWidget(self.progress_bar, 5, 1)
 
         # Export button and Delete button in a horizontal layout
         self.button_layout = qtw.QHBoxLayout()
@@ -73,23 +81,31 @@
         self.export_button.clicked.connect(self.export)
         self.button_layout.addWidget(self.export_button)
         self.delete_button = qtw.QPushButton("Delete")
         self.delete_button.clicked.connect(self.delete)
         self.button_layout.addWidget(self.delete_button)
         self.grid.addLayout(self.button_layout, 6, 0, 1, 2)
 
+        # set layout
+        self.setLayout(self.grid)
+
+        # use minimal height
+        height = self.minimumSizeHint().height()
+        self.setFixedHeight(height)
+
     def name_changed(self):
-        self.global_state.name = self.name_edit.text()
+        self.current_annotation.name = self.name_edit.text()
 
     def annotator_id_changed(self):
-        self.global_state.annotator_id = self.annotator_id_edit.text()
+        if self.annotator_id_edit.text() != "":
+            self.current_annotation.annotator_id = int(self.annotator_id_edit.text())
 
     def export(self):
         # open export dialog
-        dlg = ExportAnnotationDialog(self.global_state, self)
+        dlg = ExportAnnotationDialog(self.current_annotation, self)
         dlg.exec()
         dlg.deleteLater()
 
     def delete(self):
         # ask for confirmation
         msg = qtw.QMessageBox(self)
         msg.setIcon(qtw.QMessageBox.Icon.Warning)
@@ -97,15 +113,15 @@
         msg.setInformativeText("This action cannot be undone.")
         msg.setWindowTitle("Delete Annotation-Object")
         msg.setStandardButtons(
             qtw.QMessageBox.StandardButton.Yes | qtw.QMessageBox.StandardButton.No
         )
         msg.setDefaultButton(qtw.QMessageBox.StandardButton.No)
         if msg.exec() == qtw.QMessageBox.StandardButton.Yes:
-            self.global_state.delete()
+            self.current_annotation.delete()
             self.deleted.emit()
 
 
 class GlobalStateList(qtw.QWidget):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.init_ui()
@@ -126,26 +142,26 @@
 
     def update(self) -> None:
         # clear layout
         for i in reversed(range(self.scroll_layout.count())):
             self.scroll_layout.itemAt(i).widget().setParent(None)
 
         # add global states
-        global_states = Annotation.get_all()
-        # global_states.sort(key=lambda x: x.creation_time, reverse=True)
-        for global_state in global_states:
-            widget = GlobalStateWidget(global_state)
+        annotations = Annotation.get_all()
+        for annotation in annotations:
+            widget = AnnotationManagerWidget(annotation)
             widget.deleted.connect(self.update)
 
             # make frame around the widget
             frame = qtw.QFrame()
             frame.setFrameShape(qtw.QFrame.Shape.StyledPanel)
             frame.setFrameShadow(qtw.QFrame.Shadow.Raised)
             frame_layout = qtw.QVBoxLayout(frame)
             frame_layout.addWidget(widget)
+            frame.setFixedHeight(widget.size().height())
 
             self.scroll_layout.addWidget(frame)
 
 
 class GlobalStatesDialog(qtw.QDialog):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -155,30 +171,26 @@
         self.setWindowTitle("Annotations")
         self.setMinimumSize(500, 500)
         self.grid = qtw.QGridLayout(self)
 
         self.scroll_global_states = GlobalStateList()
         self.grid.addWidget(self.scroll_global_states)
 
-        self.button_box = qtw.QDialogButtonBox(qtw.QDialogButtonBox.StandardButton.Ok)
-        self.button_box.accepted.connect(self.accept)
-        self.grid.addWidget(self.button_box)
-
     def update(self):
         self.scroll_global_states.update()
 
 
 class ExportAnnotationDialog(qtw.QDialog):
-    def __init__(self, global_state: Annotation, *args, **kwargs):
+    def __init__(self, annotation: Annotation, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.global_state = global_state
+        self.current_annotation = annotation
         self.init_ui()
 
     def init_ui(self):
-        self.setWindowTitle("Export Annotation {}".format(self.global_state.name))
+        self.setWindowTitle("Export Annotation {}".format(self.current_annotation.name))
         self.setMinimumSize(500, 500)
         self.grid = qtw.QGridLayout(self)
 
         # Give the user some options and group them visual box with a title
         self.export_options = qtw.QGroupBox("Export Options")
         self.export_options_layout = qtw.QGridLayout(self.export_options)
 
@@ -228,43 +240,45 @@
         # ask for export path
         export_path = qtw.QFileDialog.getExistingDirectory(self, "Select Directory")
         if not export_path:
             return
 
         # annotation name
         annotation_name = "annotation_{}_by_{}".format(
-            self.global_state.name, self.global_state.annotator_id
+            self.current_annotation.name, self.current_annotation.annotator_id
         )
 
         # create export directory
         export_dir = os.path.join(export_path, annotation_name)
         os.makedirs(export_dir, exist_ok=True)
 
         # Export main annotation-file
-        array = self.global_state.to_numpy()
-        scheme = self.global_state.dataset.scheme
+        array = self.current_annotation.to_numpy()
+        scheme = self.current_annotation.dataset.scheme
         header = [x.element_name for x in scheme]
-        filehandler.write_csv(os.path.join(export_dir, "annotation.csv"), array, header)
+        filehandler.write_csv(
+            Path(os.path.join(export_dir, "annotation.csv")), array, header
+        )
 
         # add copy of annotated file
         if self.add_copy_checkbox.isChecked():
-            shutil.copy2(self.global_state.path, export_dir)
+            shutil.copy2(self.current_annotation.path, export_dir)
 
         # export dataset-scheme
         if self.export_dataset_scheme_checkbox.isChecked():
             filehandler.write_json(
-                os.path.join(export_dir, "dataset_scheme.json"),
-                self.global_state.dataset.scheme.scheme,
+                Path(os.path.join(export_dir, "dataset_scheme.json")),
+                self.current_annotation.dataset.scheme.scheme,
             )
 
         # export meta informations
         if self.export_meta_informations_checkbox.isChecked():
             filehandler.write_json(
-                os.path.join(export_dir, "meta_informations.json"),
-                self.global_state.meta_data,
+                Path(os.path.join(export_dir, "meta_informations.json")),
+                self.current_annotation.meta_data,
             )
 
         # compress to zip file
         if self.compress_checkbox.isChecked():
             shutil.make_archive(export_dir, "zip", export_dir)
             shutil.rmtree(export_dir)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/dialogs/dialog_manager.py` & `annotation_tool-0.9.0/annotation_tool/dialogs/dialog_manager.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/dialogs/edit_datasets.py` & `annotation_tool-0.9.0/annotation_tool/dialogs/edit_datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from functools import partial
 import logging
+from pathlib import Path
 
 import PyQt6.QtCore as qtc
 import PyQt6.QtWidgets as qtw
 import numpy as np
 
 from annotation_tool.data_model import Dataset, create_dataset
 from annotation_tool.data_model.annotation_scheme import create_annotation_scheme
@@ -42,45 +43,46 @@
 
         self._dependencies = QLineEditAdapted()
         self._dependencies.setPlaceholderText("Path to dataset dependencies.")
         self._dependencies.setReadOnly(True)
         self._dependencies.mousePressed.connect(self.get_dependencies_path)
         self.bottom_widget.layout().addRow("Dependencies:", self._dependencies)
 
-        self.add_button = qtw.QPushButton("Add")
-        self.add_button.setFixedWidth(100)
-        self.add_button.setEnabled(False)
-        self.add_button.clicked.connect(lambda _: self.add_pressed())
-        self.bottom_widget.layout().addRow(self.add_button)
+        self.create_button = qtw.QPushButton("Create")
+        self.create_button.setFixedWidth(100)
+        self.create_button.setEnabled(False)
+        self.create_button.clicked.connect(lambda _: self.add_pressed())
+        self.bottom_widget.layout().addRow(self.create_button)
 
         vbox.addWidget(self.bottom_widget)
 
         self.setLayout(vbox)
         self.setMinimumSize(600, 400)
 
         self._reload()
 
     def get_scheme_path(self):
         file_path, _ = qtw.QFileDialog.getOpenFileName(
             parent=self, directory="", filter="(*.json)"
         )
-        if filehandler.is_non_zero_file(file_path):
+
+        if filehandler.is_non_zero_file(Path(file_path)):
             # TODO check scheme valid
 
-            self.add_button.setEnabled(True)
+            self.create_button.setEnabled(True)
             self._scheme.setText(file_path)
         else:
-            self.add_button.setEnabled(False)
+            self.create_button.setEnabled(False)
             self._scheme.setText("")
 
     def get_dependencies_path(self):
         file_path, _ = qtw.QFileDialog.getOpenFileName(
             parent=self, directory="", filter="(*.csv)"
         )
-        if filehandler.is_non_zero_file(file_path):
+        if filehandler.is_non_zero_file(Path(file_path)):
             # TODO check dependencies valid
             self._dependencies.setText(file_path)
         else:
             self._dependencies.setText("")
 
     def make_header(self):
         row_widget = qtw.QWidget(self)
@@ -147,15 +149,15 @@
             self.scroll_widget.addItem(row)
 
     def add_pressed(self):
         name = self._name.text()
         if name == "":
             name = "nameless"
 
-        scheme = filehandler.read_json(self._scheme.text())
+        scheme = filehandler.read_json(Path(self._scheme.text()))
         try:
             scheme = create_annotation_scheme(scheme)
         except ValueError:
             logging.error(f"{scheme}")
             self._scheme.setText("Could not load scheme.")
             return
 
@@ -164,15 +166,15 @@
 
         dependencies = None
 
         if len(dependency_txt) > 0:
             if dependency_txt != dependency_error_str:
                 try:
                     dependencies = filehandler.read_csv(
-                        self._dependencies.text(), data_type=np.int8
+                        Path(self._dependencies.text()), data_type=np.int8
                     )
                 except FileNotFoundError:
                     self._dependencies.setText(dependency_error_str)
                     return
                 if dependencies.shape[0] < 0 or dependencies.shape[1] != len(scheme):
                     self._dependencies.setText(dependency_error_str)
                     return
@@ -180,15 +182,15 @@
         create_dataset(name, scheme, dependencies)
 
         self._reload()
 
         self._name.setText("")
         self._scheme.setText("")
         self._dependencies.setText("")
-        self.add_button.setEnabled(False)
+        self.create_button.setEnabled(False)
 
     def remove_pressed(self, idx):
         dataset = Dataset.get_all()[idx]
         dataset_name = dataset.name
 
         msg = qtw.QMessageBox(self)
         msg.setIcon(qtw.QMessageBox.Icon.Question)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/dialogs/import_annotation_dialog.py` & `annotation_tool-0.9.0/annotation_tool/dialogs/import_annotation_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
+from pathlib import Path
 
 import PyQt6.QtCore as qtc
 import PyQt6.QtWidgets as qtw
 import numpy as np
 
-from annotation_tool.data_model import Annotation, Dataset, create_global_state
+from annotation_tool.data_model import Annotation, Dataset
 from annotation_tool.media_reader import media_reader as mr
 from annotation_tool.qt_helper_widgets.line_edit_adapted import QLineEditAdapted
 from annotation_tool.settings import settings
 
 
 class ImportAnnotationDialog(qtw.QDialog):
     load_annotation = qtc.pyqtSignal(Annotation)
@@ -25,15 +26,15 @@
         self._name_error_msg = "Please insert a valid name."
         self._dataset_error_msg = "Please select a valid dataset."
 
         # UI components
         self.combobox = None
         self.input_path_edit = None
         self.annotation_name_edit = None
-        self.open_button = None
+        self.import_button = None
         self.cancel_button = None
         self.button_widget = None
 
         self.init_ui()
 
     def init_ui(self):
         self.setWindowTitle("Import Annotation")
@@ -62,26 +63,26 @@
 
         self.combobox = qtw.QComboBox()
         for data_description in self._datasets:
             self.combobox.addItem(data_description.name)
         self.combobox.currentIndexChanged.connect(self.dataset_changed)
         form.addRow("Dataset:", self.combobox)
 
-        self.open_button = qtw.QPushButton()
-        self.open_button.setText("Create")
-        self.open_button.setEnabled(False)
-        self.open_button.clicked.connect(lambda _: self.open_pressed())
+        self.import_button = qtw.QPushButton()
+        self.import_button.setText("Import")
+        self.import_button.setEnabled(False)
+        self.import_button.clicked.connect(lambda _: self.open_pressed())
 
         self.cancel_button = qtw.QPushButton()
         self.cancel_button.setText("Cancel")
         self.cancel_button.clicked.connect(lambda _: self.cancel_pressed())
 
         self.button_widget = qtw.QWidget()
         self.button_widget.setLayout(qtw.QHBoxLayout())
-        self.button_widget.layout().addWidget(self.open_button)
+        self.button_widget.layout().addWidget(self.import_button)
         self.button_widget.layout().addWidget(self.cancel_button)
 
         form.addRow(self.button_widget)
         self.setLayout(form)
 
         self.dataset_changed(self.combobox.currentIndex())  # initialize dataset
 
@@ -143,23 +144,27 @@
     def check_enabled(self):
         enabled = (
             self.annotation_path is not None
             and self.input_path is not None
             and self.annotation_name is not None
             and self.dataset is not None
         )
-        self.open_button.setEnabled(enabled)
+        self.import_button.setEnabled(enabled)
 
     def cancel_pressed(self):
         self.close()
 
     def open_pressed(self):
         self.check_enabled()
-        if self.open_button.isEnabled():
-            from ..data_model import create_annotation, create_sample
+        if self.import_button.isEnabled():
+            from ..data_model import (
+                create_annotation,
+                create_sample,
+                create_single_annotation,
+            )
             from ..utility.filehandler import read_csv
 
             try:
                 annotation = read_csv(self.annotation_path)
             except ValueError:
                 msg = qtw.QMessageBox(self)
                 msg.setIcon(qtw.QMessageBox.Icon.Critical)
@@ -186,15 +191,16 @@
                 self.annotation_path_edit.setText("")
                 self.annotation_path_edit.setPlaceholderText(self._file_error_msg)
                 self.annotation_path = None
                 self.check_enabled()
                 return
 
             try:
-                media_reader = mr(self.input_path)
+                input_path = Path(self.input_path)
+                media_reader = mr(input_path)
             except ValueError:
                 msg = qtw.QMessageBox(self)
                 msg.setIcon(qtw.QMessageBox.Icon.Critical)
                 msg.setText("Unknown media type.")
                 msg.setInformativeText("The selected media type is not supported.")
                 msg.setWindowTitle("Error")
                 msg.exec()
@@ -241,15 +247,15 @@
             samples = []
             start_idx = 0
             for idx in range(annotation.shape[0]):
                 if idx == annotation.shape[0] - 1 or not np.array_equal(
                     annotation[idx], annotation[idx + 1]
                 ):
                     try:
-                        _anno = create_annotation(scheme, annotation[idx])
+                        _anno = create_single_annotation(scheme, annotation[idx])
                     except ValueError:
                         msg = qtw.QMessageBox(self)
                         msg.setIcon(qtw.QMessageBox.Icon.Critical)
                         msg.setText("Invalid annotation.")
                         msg.setInformativeText(
                             "The selected annotation file contains invalid annotations."
                         )
@@ -263,15 +269,15 @@
                         self.check_enabled()
                         return
 
                     samples.append(create_sample(start_idx, idx, _anno))
                     start_idx = idx + 1
 
             annotator_id = settings.annotator_id
-            annotation = create_global_state(
+            annotation = create_annotation(
                 annotator_id,
                 dataset,
                 self.annotation_name_edit.text(),
                 media_reader.path,
             )
 
             annotation.samples = samples
```

### Comparing `annotation_tool-0.8.3/annotation_tool/dialogs/load_annotation_dialog.py` & `annotation_tool-0.9.0/annotation_tool/dialogs/load_annotation_dialog.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 
 import PyQt6.QtCore as qtc
 import PyQt6.QtWidgets as qtw
 
 from ..data_model import Dataset
 from ..data_model.annotation import Annotation
 from ..qt_helper_widgets.line_edit_adapted import QLineEditAdapted
@@ -11,16 +12,16 @@
 
 class LoadAnnotationDialog(qtw.QDialog):
     load_annotation = qtc.pyqtSignal(Annotation)
 
     def __init__(self, *args, **kwargs):
         super(LoadAnnotationDialog, self).__init__(*args, **kwargs)
 
-        self.global_states = Annotation.get_all()
-        self.global_states.sort(key=lambda x: x.timestamp, reverse=True)
+        self.annotations = Annotation.get_all()
+        self.annotations.sort(key=lambda x: x.last_save, reverse=True)
 
         self.name_changed_msg = (
             "The name of the annotation has changed, please insert the new name."
         )
         self.path_changed_msg = (
             "The path of the annotation has changed, please select the new file."
         )
@@ -32,15 +33,15 @@
     def init_ui(self):
         self.setWindowTitle("Load Annotation")
         self.setModal(True)
 
         form = qtw.QFormLayout()
         self.combobox = qtw.QComboBox()
 
-        for global_state in self.global_states:
+        for global_state in self.annotations:
             self.combobox.addItem(global_state.name)
 
         self.combobox.currentIndexChanged.connect(
             lambda x: self.process_combobox_value(x)
         )
         form.addRow("Name:", self.combobox)
 
@@ -76,56 +77,57 @@
         self.button_widget.layout().addWidget(self.cancel_button)
 
         form.addRow(self.button_widget)
         self.setLayout(form)
         self.setMinimumWidth(500)
 
     def process_combobox_value(self, idx):
-        if idx >= 0 and idx < len(self.global_states):
-            global_state = self.global_states[idx]
+        if 0 <= idx < len(self.annotations):
+            global_state = self.annotations[idx]
 
             dataset = global_state.dataset
 
             self.dataset_line_edit.setText(dataset.name)
 
             if dataset not in self.datasets:
                 depr_str = self.dataset_line_edit.text() + " [Deleted]"
                 self.dataset_line_edit.setText(depr_str)
                 self.dataset_line_edit.setStatusTip(
                     "The original Dataset was deleted via the Edit-Dataset Menu."
                 )
 
             if os.path.isfile(global_state.path):
-                self.line_edit.setText(global_state.path)
+                self.line_edit.setText(global_state.path.as_posix())
             else:
                 self.line_edit.setText(
                     "The path of the input has changed, please select the new path."
                 )
 
             self.progress_bar.setValue(global_state.progress)
 
         self.check_enabled()
 
     def select_input_source(self):
         file_path, _ = qtw.QFileDialog.getOpenFileName(
             parent=self, directory="", filter="Video MoCap (*.mp4 *.avi *.csv)"
         )
+        file_path = Path(file_path)
         if filehandler.is_non_zero_file(file_path):
-            hash = filehandler.footprint_of_file(file_path)
+            hash = filehandler.checksum(file_path)
             idx = self.combobox.currentIndex()
 
             if idx < 0:
                 self.line_edit.setText("")
                 return
 
-            global_state: Annotation = self.global_states[idx]
-            other_hash = global_state.footprint
+            global_state: Annotation = self.annotations[idx]
+            other_hash = global_state.checksum
 
             if hash == other_hash:
-                self.line_edit.setText(file_path)
+                self.line_edit.setText(file_path.as_posix())
             else:
                 self.line_edit.setText(
                     "The input_file is not compatible with the selected global_state, please select the correct file."  # noqa E501
                 )
         self.check_enabled()
 
     def check_enabled(self):
@@ -139,22 +141,22 @@
             self.open_button.setEnabled(True)
 
     def cancel_pressed(self):
         self.close()
 
     def open_pressed(self):
         idx = self.combobox.currentIndex()
-        global_state = self.global_states[idx]
-        path = self.line_edit.text()
-        file_hash = filehandler.footprint_of_file(path)
+        annotation = self.annotations[idx]
+        path = Path(self.line_edit.text())
+        file_hash = filehandler.checksum(path)
 
-        if file_hash == global_state.footprint:
-            global_state.path = self.line_edit.text()
+        if file_hash == annotation.checksum:
+            annotation.path = path
             self.close()
-            self.load_annotation.emit(global_state)
+            self.load_annotation.emit(annotation)
         else:
             self.line_edit.setText(
                 "The input_file is not compatible with the selected global_state, please select the correct file."  # noqa E501
             )
 
     @property
     def datasets(self):
```

### Comparing `annotation_tool-0.8.3/annotation_tool/dialogs/local_files.py` & `annotation_tool-0.9.0/annotation_tool/dialogs/local_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from annotation_tool.file_cache._file_cache import (
     get_all,
     get_dir,
     get_size_in_bytes,
     path_of,
 )
-from annotation_tool.qt_helper_widgets.lines import QHLine
 
 
 class LocalFilesDialog(qtw.QDialog):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.setWindowTitle("Local Files")
         self.setLayout(qtw.QGridLayout(self))
@@ -42,15 +41,14 @@
         )
         self.layout().addWidget(self.size_label, 2, 0)
         self.layout().addWidget(self.size_label_value, 2, 1)
 
         # show directory path and button to copy it
         self.path_label = qtw.QLabel("Path to local files:")
         self.path_value_label = qtw.QLabel(f"{get_dir()}")
-        self.path_value_label.setWordWrap(True)
         self.path_value_label.setTextInteractionFlags(
             qtc.Qt.TextInteractionFlag.TextSelectableByMouse
         )
         self.layout().addWidget(self.path_label, 3, 0)
         self.layout().addWidget(self.path_value_label, 3, 1)
 
         # make button box with copy path and open dir buttons
@@ -61,22 +59,14 @@
 
         # add buttons to own layout and add layout to dialog
         self.button_box_layout = qtw.QHBoxLayout()
         self.button_box_layout.addWidget(self.copy_path_button)
         self.button_box_layout.addWidget(self.open_dir_button)
         self.layout().addLayout(self.button_box_layout, 4, 0, 1, 2)
 
-        # add horizontal line
-        self.layout().addWidget(QHLine(), 5, 0, 1, 2)
-
-        # add close button
-        self.close_button = qtw.QPushButton("Close")
-        self.close_button.clicked.connect(self.accept)
-        self.layout().addWidget(self.close_button, 6, 0, 1, 2)
-
     def copy_path(self):
         qtw.QApplication.clipboard().setText(get_dir())
 
     def open_dir(self):
         path = get_dir()
         if platform.system() == "Windows":
             os.startfile(path)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/dialogs/new_annotation_dialog.py` & `annotation_tool-0.9.0/annotation_tool/dialogs/new_annotation_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
+from pathlib import Path
 
 import PyQt6.QtCore as qtc
 import PyQt6.QtWidgets as qtw
 
-from annotation_tool.data_model import Annotation, Dataset, create_global_state
+from annotation_tool.data_model import Annotation, Dataset, create_annotation
 from annotation_tool.media_reader import media_reader as mr
 from annotation_tool.qt_helper_widgets.line_edit_adapted import QLineEditAdapted
 from annotation_tool.settings import settings
 
 
 class NewAnnotationDialog(qtw.QDialog):
     load_annotation = qtc.pyqtSignal(Annotation)
@@ -136,15 +137,15 @@
     def cancel_pressed(self):
         self.close()
 
     def open_pressed(self):
         self.check_enabled()
         if self.open_button.isEnabled():
             try:
-                media_reader = mr(self.input_path)
+                media_reader = mr(Path(self.input_path))
                 if len(media_reader) < 1000:
                     msg = qtw.QMessageBox(self)
                     msg.setIcon(qtw.QMessageBox.Icon.Critical)
                     msg.setText("Media too short.")
                     msg.setInformativeText(
                         "The selected media's length [={}] is too small.\nIt should at least consist of 1000 frames!".format(
                             len(media_reader)
@@ -170,15 +171,15 @@
                 self.check_enabled()
                 return
 
             idx = self.combobox.currentIndex()
             dataset = self._datasets[idx]
 
             annotator_id = settings.annotator_id
-            annotation = create_global_state(
+            annotation = create_annotation(
                 annotator_id,
                 dataset,
                 self.annotation_name_edit.text(),
                 media_reader.path,
             )
             self.close()
             self.load_annotation.emit(annotation)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/dialogs/settings_dialog.py` & `annotation_tool-0.9.0/annotation_tool/dialogs/settings_dialog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 import PyQt6.QtCore as qtc
+import PyQt6.QtGui as qtg
 import PyQt6.QtWidgets as qtw
 
 from annotation_tool.settings import settings
 
 
 class SettingsDialog(qtw.QDialog):
     window_size_changed = qtc.pyqtSignal(int, int)
@@ -21,37 +22,32 @@
 
         self.layout = qtw.QVBoxLayout()
 
         # annotator ID
         self.annotator_id_layout = qtw.QHBoxLayout()
         self.annotator_id_label = qtw.QLabel("Annotator ID:")
         self.annotator_id_edit = qtw.QLineEdit()
+        only_int = qtg.QIntValidator()
         self.annotator_id_edit.setText(str(self.settings.annotator_id))
+        self.annotator_id_edit.setValidator(only_int)
+        self.annotator_id_edit.setMaxLength(3)
+        self.annotator_id_edit.textChanged.connect(self.annotator_id_changed)
         self.annotator_id_layout.addWidget(self.annotator_id_label)
         self.annotator_id_layout.addWidget(self.annotator_id_edit)
         self.layout.addLayout(self.annotator_id_layout)
 
         # appearance sub-menu
         self.appearance_layout = qtw.QHBoxLayout()
         self.appearance_label = qtw.QLabel("Appearance:")
         self.appearance_button = qtw.QPushButton("Change")
         self.appearance_button.clicked.connect(self.change_appearance)
         self.appearance_layout.addWidget(self.appearance_label)
         self.appearance_layout.addWidget(self.appearance_button)
         self.layout.addLayout(self.appearance_layout)
 
-        # media sub-menu
-        self.media_layout = qtw.QHBoxLayout()
-        self.media_label = qtw.QLabel("Media:")
-        self.media_button = qtw.QPushButton("Change")
-        self.media_button.clicked.connect(self.change_media)
-        self.media_layout.addWidget(self.media_label)
-        self.media_layout.addWidget(self.media_button)
-        self.layout.addLayout(self.media_layout)
-
         # navigation sub-menu
         self.navigation_layout = qtw.QHBoxLayout()
         self.navigation_label = qtw.QLabel("Navigation:")
         self.navigation_button = qtw.QPushButton("Change")
         self.navigation_button.clicked.connect(self.change_navigation)
         self.navigation_layout.addWidget(self.navigation_label)
         self.navigation_layout.addWidget(self.navigation_button)
@@ -102,33 +98,31 @@
 
     def change_developer_settings(self):
         dlg = DeveloperSettingsDialog(self)
         dlg.settings_changed.connect(self.settings_changed.emit)
         dlg.exec()
         dlg.deleteLater()
 
-    def change_media(self):
-        dlg = MediaSettingsDialog(self)
-        dlg.settings_changed.connect(self.settings_changed.emit)
-        dlg.exec()
-        dlg.deleteLater()
-
     def change_navigation(self):
         dlg = NavigationSettingsDialog(self)
         dlg.exec()
         dlg.deleteLater()
 
     def change_retrieval_mode(self):
         dlg = RetrievalSettingsDialog(self)
         dlg.exec()
         dlg.deleteLater()
 
     def reset_settings(self):
         self.annotator_id_edit.setText(str(self.settings.get_default("annotator_id")))
 
+    def annotator_id_changed(self):
+        if self.annotator_id_edit.text() != "":
+            self.settings.annotator_id = int(self.annotator_id_edit.text())
+
     def accept(self):
         # only allow numbers in annotator ID field
         if self.annotator_id_edit.text().isnumeric():
             self.settings.annotator_id = int(self.annotator_id_edit.text())
         else:
             self.annotator_id_edit.setText(str(self.settings.annotator_id))
         super().accept()
@@ -148,16 +142,17 @@
 
         self.layout = qtw.QVBoxLayout()
 
         # theme
         self.theme_layout = qtw.QHBoxLayout()
         self.theme_label = qtw.QLabel("Theme:")
         self.theme_combobox = qtw.QComboBox()
-        self.theme_combobox.addItems(["Light", "Dark"])
-        self.theme_combobox.setCurrentIndex(1 if settings.darkmode else 0)
+        self.theme_combobox.addItems(["Light", "Dark"])  # for now disable System theme
+        idx = self.theme_combobox.findText(settings.color_theme.capitalize())
+        self.theme_combobox.setCurrentIndex(idx)
         self.theme_combobox.currentIndexChanged.connect(self.change_theme)
         self.theme_layout.addWidget(self.theme_label)
         self.theme_layout.addWidget(self.theme_combobox)
         self.layout.addLayout(self.theme_layout)
 
         # font size
         self.font_size_layout = qtw.QHBoxLayout()
@@ -170,27 +165,27 @@
         self.font_size_layout.addWidget(self.font_size_spinbox)
         self.layout.addLayout(self.font_size_layout)
 
         # preferred width
         self.preferred_width_layout = qtw.QHBoxLayout()
         self.preferred_width_label = qtw.QLabel("Preferred Width:")
         self.preferred_width_spinbox = qtw.QSpinBox()
-        self.preferred_width_spinbox.setRange(600, 4000)
+        self.preferred_width_spinbox.setRange(1200, 4000)
         self.preferred_width_spinbox.setSingleStep(100)
         self.preferred_width_spinbox.setValue(settings.preferred_width)
         self.preferred_width_spinbox.valueChanged.connect(self.preferred_width_changed)
         self.preferred_width_layout.addWidget(self.preferred_width_label)
         self.preferred_width_layout.addWidget(self.preferred_width_spinbox)
         self.layout.addLayout(self.preferred_width_layout)
 
         # preferred height
         self.preferred_height_layout = qtw.QHBoxLayout()
         self.preferred_height_label = qtw.QLabel("Preferred Height:")
         self.preferred_height_spinbox = qtw.QSpinBox()
-        self.preferred_height_spinbox.setRange(400, 2000)
+        self.preferred_height_spinbox.setRange(700, 2000)
         self.preferred_height_spinbox.setSingleStep(100)
         self.preferred_height_spinbox.setValue(settings.preferred_height)
         self.preferred_height_spinbox.valueChanged.connect(
             self.preferred_height_changed
         )
         self.preferred_height_layout.addWidget(self.preferred_height_label)
         self.preferred_height_layout.addWidget(self.preferred_height_spinbox)
@@ -199,37 +194,58 @@
         # high DPI scaling
         self.high_dpi_scaling_layout = qtw.QHBoxLayout()
         self.high_dpi_scaling_label = qtw.QLabel("High DPI Scaling:")
         self.high_dpi_scaling_label.setToolTip(
             "Changing this will only take effect after a restart."
         )
 
+        # timeline design
+        self.timeline_design_layout = qtw.QHBoxLayout()
+        self.timeline_design_label = qtw.QLabel("Timeline Design:")
+        self.timeline_design_combobox = qtw.QComboBox()
+        self.timeline_design_combobox.addItems(["Rounded", "Rectangular"])
+        idx = self.timeline_design_combobox.findText(
+            settings.timeline_design.capitalize()
+        )
+        self.timeline_design_combobox.setCurrentIndex(idx)
+        self.timeline_design_combobox.currentTextChanged.connect(
+            self.change_timeline_design
+        )
+        self.timeline_design_layout.addWidget(self.timeline_design_label)
+        self.timeline_design_layout.addWidget(self.timeline_design_combobox)
+        self.layout.addLayout(self.timeline_design_layout)
+
         # Accept, Reset buttons
         self.button_layout = qtw.QHBoxLayout()
         self.accept_button = qtw.QPushButton("Accept")
         self.accept_button.clicked.connect(self.accept)
         self.reset_button = qtw.QPushButton("Reset")
         self.reset_button.clicked.connect(self.reset_settings)
         self.button_layout.addWidget(self.accept_button)
         self.button_layout.addWidget(self.reset_button)
         self.layout.addLayout(self.button_layout)
 
         self.setLayout(self.layout)
 
     def reset_settings(self):
-        self.theme_combobox.setCurrentIndex(
-            1 if settings.get_default("darkmode") else 0
-        )
+        default_color_scheme = settings.get_default("color_theme")
+        _idx = self.theme_combobox.findText(default_color_scheme.capitalize())
+        self.theme_combobox.setCurrentIndex(_idx)
         self.font_size_spinbox.setValue(settings.get_default("font_size"))
         self.preferred_width_spinbox.setValue(settings.get_default("preferred_width"))
         self.preferred_height_spinbox.setValue(settings.get_default("preferred_height"))
+        self.timeline_design_combobox.setCurrentIndex(
+            self.timeline_design_combobox.findText(
+                settings.get_default("timeline_design").capitalize()
+            )
+        )
 
     def change_theme(self):
-        is_darkmode = bool(self.theme_combobox.currentIndex())
-        settings.darkmode = is_darkmode
+        mode = self.theme_combobox.currentText().lower()
+        settings.color_theme = mode
         qtw.QApplication.instance().update_theme()
 
     def preferred_width_changed(self, value):
         # grab the main window
         settings.preferred_width = value
         self.window_size_changed.emit(value, settings.preferred_height)
 
@@ -237,65 +253,17 @@
         settings.preferred_height = value
         self.window_size_changed.emit(settings.preferred_width, value)
 
     def change_font_size(self, value):
         settings.font_size = value
         qtw.QApplication.instance().update_theme()
 
-
-class MediaSettingsDialog(qtw.QDialog):
-    settings_changed = qtc.pyqtSignal()
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.init_ui()
-
-    def init_ui(self):
-        # set window title
-        self.setWindowTitle("Media Settings")
-        self.setFixedSize(400, 300)
-
-        # layout
-        self.layout = qtw.QVBoxLayout()
-
-        # fallback FPS if no FPS is detected
-        self.fallback_fps_layout = qtw.QHBoxLayout()
-        self.fallback_fps_label = qtw.QLabel("Fallback FPS:")
-        # slider for fallback FPS
-        self.fallback_fps_slider = qtw.QSlider(qtc.Qt.Orientation.Horizontal)
-        self.fallback_fps_slider.setRange(1, 250)
-        # display the current value of the slider
-        self.fallback_fps_edit = qtw.QLabel(str(settings.refresh_rate))
-        self.fallback_fps_slider.valueChanged.connect(self.change_fallback_fps)
-
-        self.fallback_fps_layout.addWidget(self.fallback_fps_label)
-        self.fallback_fps_slider.setValue(settings.refresh_rate)
-        self.fallback_fps_layout.addWidget(self.fallback_fps_slider)
-        self.fallback_fps_layout.addWidget(self.fallback_fps_edit)
-        self.layout.addLayout(self.fallback_fps_layout)
-
-        # Accept, Reset buttons
-        self.button_layout = qtw.QHBoxLayout()
-        self.accept_button = qtw.QPushButton("Accept")
-        self.accept_button.clicked.connect(self.accept)
-        self.reset_button = qtw.QPushButton("Reset")
-        self.reset_button.clicked.connect(self.reset_settings)
-        self.button_layout.addWidget(self.accept_button)
-        self.button_layout.addWidget(self.reset_button)
-        self.layout.addLayout(self.button_layout)
-
-        self.setLayout(self.layout)
-
-    def change_fallback_fps(self, value) -> None:
-        self.fallback_fps_edit.setText(str(value))
-        settings.refresh_rate = value
-        self.settings_changed.emit()
-
-    def reset_settings(self):
-        self.fallback_fps_slider.setValue(settings.get_default("refresh_rate"))
+    def change_timeline_design(self, value):
+        settings.timeline_design = value.lower()
+        qtw.QApplication.instance().timeline.update()
 
 
 class NavigationSettingsDialog(qtw.QDialog):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.init_ui()
 
@@ -303,14 +271,28 @@
         # set window title
         self.setWindowTitle("Navigation Settings")
         self.setFixedSize(400, 300)
 
         # layout
         self.layout = qtw.QVBoxLayout()
 
+        # Merging mode
+        self.merge_mode_layout = qtw.QHBoxLayout()
+        self.merge_mode_label = qtw.QLabel("Merging behavior:")
+        self.merge_mode_combobox = qtw.QComboBox()
+        self.merge_mode_combobox.addItems(
+            ["Use own annotation", "Use annotation from neighbor"]
+        )
+        idx = 1 if settings.merging_mode == "into" else 0
+        self.merge_mode_combobox.setCurrentIndex(idx)
+        self.merge_mode_combobox.currentIndexChanged.connect(self.change_merge_mode)
+        self.merge_mode_layout.addWidget(self.merge_mode_label)
+        self.merge_mode_layout.addWidget(self.merge_mode_combobox)
+        self.layout.addLayout(self.merge_mode_layout)
+
         # Small skip
         self.small_skip_layout = qtw.QHBoxLayout()
         self.small_skip_label = qtw.QLabel("Skip:")
         self.small_skip_spinbox = qtw.QSpinBox()
         self.small_skip_spinbox.setRange(1, 100)
         self.small_skip_spinbox.setValue(settings.small_skip)
         self.small_skip_spinbox.valueChanged.connect(self.change_small_skip)
@@ -344,17 +326,23 @@
 
     def change_small_skip(self, value: int) -> None:
         settings.small_skip = value
 
     def change_big_skip(self, value: int) -> None:
         settings.big_skip = value
 
+    def change_merge_mode(self, idx: int) -> None:
+        settings.merging_mode = "into" if idx == 1 else "from"
+
     def reset_settings(self):
         self.small_skip_spinbox.setValue(settings.get_default("small_skip"))
         self.big_skip_spinbox.setValue(settings.get_default("big_skip"))
+        self.merge_mode_combobox.setCurrentIndex(
+            1 if settings.get_default("merging_mode") == "into" else 0
+        )
 
 
 class RetrievalSettingsDialog(qtw.QDialog):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.init_ui()
```

### Comparing `annotation_tool-0.8.3/annotation_tool/file_cache/_file_cache.py` & `annotation_tool-0.9.0/annotation_tool/file_cache/_file_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import abc
 import functools
 import logging
 import os
 from pickle import UnpicklingError
 from typing import List, Optional, Type, Union
 
 import appdirs
@@ -13,15 +12,15 @@
 except ImportError:
     # default values
     __version__ = "0.1.0"
     __application_name__ = "annotation-tool"
 
 
 __application_path__ = appdirs.user_data_dir(
-    __application_name__, False, "{}.x.x".format(__version__.split(".")[0])
+    __application_name__, False, "{}.{}.x".format(*__version__.split(".")[:2])
 )
 
 __file_cache__ = FileCache(
     __application_name__, flag="c", app_cache_dir=__application_path__
 )
 __cache_directory__ = __file_cache__.cache_dir
 
@@ -275,16 +274,15 @@
         raise FileNotFoundError(f"Could not find file for object {obj}")
 
 
 def wrap_setattr(func):
     @functools.wraps(func)
     def wrapper(self, key, value):
         func(self, key, value)
-        if key != "_id":  # TODO check if this is necessary, _id is not used anymore
-            write(self)
+        write(self)
 
     return wrapper
 
 
 def cached(cls):
     """
     Decorator for classes that should be cached.
@@ -307,62 +305,7 @@
     cls.delete = delete
     cls.sync = write
     cls.synchronize = write
     cls.get_all = functools.partial(get_all_of_class, cls.__name__)
     cls.del_all = functools.partial(del_all_of_class, cls.__name__)
 
     return cls
-
-
-class Cachable(abc.ABC):
-    """
-    Abstract base class for cachable objects.
-    """
-
-    __cache_id__: str
-
-    def __init__(self):
-        self.__cache_id__ = get_next_id()  # init cache_id
-
-    def delete(self) -> None:
-        """
-        Deletes the object from the cache.
-        """
-        delete(self)
-
-    def sync(self) -> None:
-        """
-        Writes the object to the cache.
-        """
-        write(self)
-
-    def synchronize(self) -> None:
-        """
-        Writes the object to the cache. (alias for sync)
-        """
-        write(self)
-
-    @classmethod
-    def get_all(cls) -> List[object]:
-        """
-        Returns a list of all objects of type cls in the cache.
-        The elements are sorted by their cache_id.
-        """
-        return get_all_of_class(cls)
-
-    @classmethod
-    def del_all(cls) -> None:
-        """
-        Deletes all objects of type cls from the cache.
-        """
-        del_all_of_class(cls)
-
-    @property
-    def cache_id(self) -> str:
-        return self.__cache_id__
-
-    def __setattr__(self, key, value):
-        super().__setattr__(key, value)
-        if self.cache_id:
-            write(self)
-        else:
-            logging.warning("cache_id is not set yet.")
```

### Comparing `annotation_tool-0.8.3/annotation_tool/gui.py` & `annotation_tool-0.9.0/annotation_tool/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import PyQt6.QtGui as qtg
 import PyQt6.QtWidgets as qtw
 
 from annotation_tool.annotation.modes import AnnotationMode
 from annotation_tool.dialogs.annotation_list import GlobalStatesDialog
 from annotation_tool.settings import settings
 from annotation_tool.user_actions import (
+    get_action,
     get_annotation_actions,
     get_edit_actions,
     get_replay_actions,
     get_shortcut,
 )
 
 from . import __application_name__, __version__
@@ -45,14 +46,15 @@
     user_action = qtc.pyqtSignal(enum.Enum)
 
     def __init__(self, *args, **kwargs):
         super(GUI, self).__init__(*args, **kwargs)
 
         self.current_mode = AnnotationMode.MANUAL
 
+        self.setMinimumSize(1200, 700)
         self.resize(settings.preferred_width, settings.preferred_height)
         self.setWindowTitle(
             "{} v{}".format(__application_name__.replace("_", " "), __version__)
         )
         self.setWindowIcon(qtg.QIcon(qtg.QPixmap(":/icon.png")))
 
         self.main_widget = qtw.QWidget()
@@ -261,10 +263,20 @@
         old_widget.setParent(None)
         old_widget.deleteLater()
 
     @qtc.pyqtSlot(qtg.QCloseEvent)
     def closeEvent(self, a0: qtg.QCloseEvent) -> None:
         self._exit()
 
+    @qtc.pyqtSlot(qtg.QKeyEvent)
+    def keyPressEvent(self, a0: qtg.QKeyEvent) -> None:
+        # print("GUI", a0.key())
+        action = get_action(a0.key())
+
+        if action is not None:
+            self.user_action.emit(action)
+        else:
+            super().keyPressEvent(a0)
+
     def _exit(self):
         self.close_dialog()
         self.exit_pressed.emit()
```

### Comparing `annotation_tool-0.8.3/annotation_tool/main_controller.py` & `annotation_tool-0.9.0/annotation_tool/main_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 import logging
 import logging.config
+from pathlib import Path
 import sys
 import time
 
 import PyQt6.QtCore as qtc
 from PyQt6.QtCore import Qt
 from PyQt6.QtGui import QColor, QPalette
 import PyQt6.QtWidgets as qtw
 
 from annotation_tool.annotation.timeline import QTimeLine
-from annotation_tool.media_reader import media_reader, set_fallback_fps
+from annotation_tool.media_reader import meta_data
 import annotation_tool.network.controller as network
 from annotation_tool.settings import settings
 
 from . import __version__
 from .annotation.controller import AnnotationController
 from .data_model.annotation import Annotation
 from .gui import GUI, LayoutPosition
 from .media.media import QMediaWidget  # This raises all the debug-messages on startup
 from .mediator import Mediator
 from .playback import QPlaybackWidget
 from .utility import filehandler
-from .utility.functions import FrameTimeMapper
-
-# init media_reader
-set_fallback_fps(settings.refresh_rate)
 
 
 class MainApplication(qtw.QApplication):
     update_media_pos = qtc.pyqtSignal(int)
     update_annotation_pos = qtc.pyqtSignal(int)
-    load_media = qtc.pyqtSignal(str, list)
+    load_media = qtc.pyqtSignal(Path, list)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        # Controll-Attributes
+        # Control-Attributes
         self.current_annotation = None
         self.n_frames = 0
         self.mediator = Mediator()
 
         # timer for automatic saving
         self.save_timer = qtc.QTimer()
         self.save_timer.timeout.connect(self.autosave)
-        self.save_interval = 5  # 1 minute
+        self.save_interval = 120  # 2 minutes
         self.last_save = time.time()
-        self.save_timer.start(30 * 1000)  # check every 10 seconds
+        self.save_timer.start(30 * 1000)  # check every 30 seconds
 
         # Widgets
         self.gui = GUI()
         self.annotation_controller = AnnotationController()
         self.playback = QPlaybackWidget()
         self.media_player = QMediaWidget()
         self.timeline = QTimeLine()
@@ -93,15 +90,14 @@
 
         # from GUI
         self.gui.user_action.connect(self.playback.on_user_action)
         self.gui.user_action.connect(self.annotation_controller.on_user_action)
         self.gui.save_pressed.connect(self.save_annotation)
         self.gui.load_annotation.connect(self.load_state)
         self.gui.settings_changed.connect(self.settings_changed)
-        self.gui.settings_changed.connect(self.media_player.settings_changed)
         self.gui.exit_pressed.connect(self.shutdown)
         self.gui.annotation_mode_changed.connect(self.annotation_controller.change_mode)
 
         # Init mediator
         self.mediator.add_receiver(self.timeline)
         self.mediator.add_receiver(self.annotation_controller)
         self.mediator.add_receiver(self.media_player)
@@ -109,80 +105,79 @@
         self.mediator.add_emitter(self.timeline)
         self.mediator.add_emitter(self.annotation_controller)
         self.mediator.add_emitter(self.media_player)
         self.mediator.add_emitter(self.playback)
 
     @qtc.pyqtSlot(Annotation)
     def load_state(self, annotation: Annotation):
+        """
+        Core function to update the application state.
+        """
         if annotation is not None:
-            # store annotation
             self.current_annotation = annotation
 
-            media = media_reader(path=annotation.path)
-            duration = media.duration
-            n_frames = len(media)
-
-            FrameTimeMapper.instance().update(n_frames=n_frames, millis=duration)
+            meta_data_dict = meta_data(annotation.path)
+            n_frames = meta_data_dict["n_frames"]
+            fps = meta_data_dict["fps"]
 
             # load media
-            # self.media_player.additional_media_changed.disconnect()  # disconnect to filter out outdated signals
-            # self.media_player.load(media.path)
             self.load_media.emit(
                 annotation.path, annotation.get_additional_media_paths()
-            )  # noqa TODO: Make get_additional_media_paths() a property
+            )
 
             # update network module
-            network.update_file(media.path)
+            network.update_state(
+                file=annotation.path, num_labels=len(annotation.dataset.scheme)
+            )
 
             # save for later reuse
             self.n_frames = n_frames
 
             # reset playback
             self.playback.reset()
 
             # update mediator
             self.mediator.n_frames = n_frames
 
             # update playback
             self.playback.n_frames = n_frames
 
             # adjust timeline
-            self.timeline.set_range(n_frames)
+            self.timeline.set_range(n_frames, fps)
 
             # update annotation controller
             self.annotation_controller.load(
                 annotation.samples,
                 annotation.dataset.scheme,
                 annotation.dataset.dependencies,
                 n_frames,
             )
 
-            # self.mediator.set_position(0, force_update=True)
             self.mediator.reset_position()
 
             self.save_annotation()
 
         else:
             raise RuntimeError("State must not be None")
 
     @qtc.pyqtSlot(list)
     def set_additional_media_paths(self, paths: list):
-        assert self.current_annotation is not None
-        self.current_annotation.set_additional_media_paths(paths)
+        if self.current_annotation is not None:
+            self.current_annotation.set_additional_media_paths(paths)
+        else:
+            raise RuntimeError("No current annotation set")
 
     @qtc.pyqtSlot()
     def media_player_loaded(self):
-        assert self.current_annotation is not None
-        self.media_player.additional_media_changed.connect(
-            self.set_additional_media_paths
-        )  # reconnect after loading
-
-        # additional_media = self.current_annotation.get_additional_media_paths()
-        # self.media_player.set_additional_media(additional_media)
-        logging.debug("media_player_loaded")
+        if self.current_annotation is not None:
+            self.media_player.additional_media_changed.connect(
+                self.set_additional_media_paths
+            )
+        else:
+            raise RuntimeError("No current annotation set")
 
     def save_annotation(self):
         if self.current_annotation is not None:
             samples = self.annotation_controller.controller.samples
 
             if len(samples) > 0:
                 assert samples[-1].end_position + 1 == self.n_frames
@@ -203,29 +198,18 @@
         if time.time() - self.last_save > self.save_interval:
             self.save_annotation()
 
     @qtc.pyqtSlot()
     def settings_changed(self):
         filehandler.set_logging_level(settings.logging_level)
 
-        set_fallback_fps(settings.refresh_rate)
-
-        if self.current_annotation is not None:
-            media = media_reader(path=self.current_annotation.path)
-            duration = media.duration
-            n_frames = len(media)
-
-            FrameTimeMapper.instance().update(n_frames=n_frames, millis=duration)
-
-        self.timeline.update()
-
     def update_theme(self):
         self.setStyle("Fusion")
 
-        if settings.darkmode:
+        if settings.color_theme == "dark":
             # # Now use a palette to switch to dark colors:
             dark_palette = QPalette(self.style().standardPalette())
             dark_palette.setColor(QPalette.ColorRole.Window, QColor(53, 53, 53))
             dark_palette.setColor(QPalette.ColorRole.WindowText, Qt.GlobalColor.white)
             dark_palette.setColor(QPalette.ColorRole.Base, QColor(35, 35, 35))
             dark_palette.setColor(QPalette.ColorRole.AlternateBase, QColor(53, 53, 53))
             dark_palette.setColor(QPalette.ColorRole.ToolTipBase, QColor(25, 25, 25))
@@ -261,42 +245,80 @@
             )
             dark_palette.setColor(
                 QPalette.ColorGroup.Disabled,
                 QPalette.ColorRole.Light,
                 QColor(53, 53, 53),
             )
             self.setPalette(dark_palette)
+        elif settings.color_theme == "light":
+            light_palette = QPalette(self.style().standardPalette())
+            light_palette.setColor(QPalette.ColorRole.Window, Qt.GlobalColor.white)
+            light_palette.setColor(QPalette.ColorRole.WindowText, Qt.GlobalColor.black)
+            light_palette.setColor(QPalette.ColorRole.Base, Qt.GlobalColor.white)
+            light_palette.setColor(
+                QPalette.ColorRole.AlternateBase, Qt.GlobalColor.white
+            )
+            light_palette.setColor(QPalette.ColorRole.ToolTipBase, Qt.GlobalColor.white)
+            light_palette.setColor(QPalette.ColorRole.ToolTipText, Qt.GlobalColor.black)
+            light_palette.setColor(QPalette.ColorRole.Text, Qt.GlobalColor.black)
+            light_palette.setColor(QPalette.ColorRole.Button, Qt.GlobalColor.white)
+            light_palette.setColor(QPalette.ColorRole.ButtonText, Qt.GlobalColor.black)
+            light_palette.setColor(QPalette.ColorRole.BrightText, Qt.GlobalColor.red)
+            light_palette.setColor(QPalette.ColorRole.Link, QColor(42, 130, 218))
+            light_palette.setColor(QPalette.ColorRole.Highlight, QColor(42, 130, 218))
+            light_palette.setColor(
+                QPalette.ColorRole.HighlightedText, QColor(35, 35, 35)
+            )
+            light_palette.setColor(
+                QPalette.ColorGroup.Active,
+                QPalette.ColorRole.Button,
+                Qt.GlobalColor.white,
+            )
+            light_palette.setColor(
+                QPalette.ColorGroup.Disabled,
+                QPalette.ColorRole.ButtonText,
+                Qt.GlobalColor.darkGray,
+            )
+
+            self.setPalette(light_palette)
+
+        elif settings.color_theme == "system":
+            # This is disabled for now, since icons might not be visible
+            raise NotImplementedError(
+                "System theme is not implemented yet, please use light or dark theme"
+            )
+            # self.setPalette(QPalette())
+            # get background color from system
+            # background_color = self.palette().color(QPalette.ColorRole.Window)
+
         else:
-            self.setPalette(QPalette())
-            # self.setPalette(self.style().standardPalette())  # reset to system default
+            raise ValueError(f"Unknown color theme {settings.color_theme}")
 
         font = self.font()
         font.setPointSize(settings.font_size)
         self.setFont(font)
 
         # hack for updating color of histogram in retrieval-widget
         from annotation_tool.annotation.retrieval.controller import RetrievalAnnotation
 
         if self.annotation_controller is not None and isinstance(
             self.annotation_controller.controller, RetrievalAnnotation
         ):
             self.annotation_controller.controller.main_widget.histogram.plot_data()
 
     def closeEvent(self, event):
-        logging.info("Closing application via closeEvent")
         self.shutdown()
         event.accept()
 
     @qtc.pyqtSlot()
     def shutdown(self):
         """
         This method is called when the application is closed.
         It saves the current annotation and closes the main window.
         """
-        logging.info("Closing application")
         self.save_timer.stop()
         self.save_annotation()
         self.media_player.shutdown()
         self.gui.close()  # close main window
         logging.info("Successfully stopped application!")
 
 
@@ -312,15 +334,14 @@
     app = MainApplication(sys.argv)
 
     # set font for app
     font = app.font()
     font.setPointSize(settings.font_size)
     app.setFont(font)
 
-    # styles: 'Breeze', 'Oxygen', 'QtCurve', 'Windows', 'Fusion'
     app.setStyle("Fusion")
 
     app.update_theme()
 
     logging.info(f"PyQt-Version: {qtc.PYQT_VERSION_STR}")
     logging.info(f"Python-Version: {sys.version}")
     logging.info(f"Platform: {sys.platform}")
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media/backend/controller.py` & `annotation_tool-0.9.0/annotation_tool/media/backend/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,38 +110,38 @@
         assert (
             self.STATE == MediaState.LOADING
         ), f"State must be LOADING but is {self.STATE}"
 
         self._open_loading_tasks = 1 + len(additional_media)
 
         self.add_replay_widget(file, is_main_widget=True, from_load=True)
-        for path in additional_media:
-            self.add_replay_widget(path, from_load=True)
+        for path, offset in additional_media:
+            self.add_replay_widget(path, from_load=True, offset=offset)
 
     def clear(self, notify=True):
         while self.replay_widgets:
             self.remove_replay_source(self.replay_widgets[0], notify)
 
-    def add_replay_widget(self, path, is_main_widget=False, from_load=False):
+    def add_replay_widget(self, path, is_main_widget=False, from_load=False, offset=0):
         if self.STATE == MediaState.LOADING and not from_load:
             logging.warning("Media is loading -> ignoring new replay widget")
             return
         if len(self.replay_widgets) < self.MAX_WIDGETS:
-            # is_main_widget = len(self.replay_widgets) == 0
-
             # select correct media_player
 
             media_type = media_type_of(path)
             if media_type == "video":
                 widget = VideoPlayer(is_main_widget, self)
             elif media_type == "mocap":
                 widget = MocapPlayer(is_main_widget, self)
             else:
                 raise NotImplementedError(f"Media type {media_type} is not supported")
 
+            widget.offset = offset
+
             if widget.is_main_replay_widget:
                 self.grid.addWidget(widget, 0, 0)
             else:
                 widget.remove_wanted.connect(self.remove_replay_source)
                 self.vbox.addWidget(widget)
 
             if not widget.is_main_replay_widget:
@@ -161,27 +161,34 @@
                 self._open_loading_tasks >= 0
             ), f"Open loading tasks must be >= 0 but is {self._open_loading_tasks}"
         else:
             assert (
                 self._open_loading_tasks == 0
             ), f"Open loading tasks must be 0 but is {self._open_loading_tasks}"
 
+    @qtc.pyqtSlot()
+    def _update_additional_media(self):
+        widgets = [w for w in self.replay_widgets if not w.is_main_replay_widget]
+        additional_media = [(self._widget_2_path[id(w)], w.offset) for w in widgets]
+        self.additional_media_changed.emit(additional_media)
+
     @qtc.pyqtSlot(AbstractMediaPlayer)
     def widget_loaded(self, widget: AbstractMediaPlayer):
         # check if widget belongs to current loading process
 
         widget.new_input_wanted.connect(self.add_replay_widget)
         widget.finished.connect(self.widget_terminated)
+        widget.offset_changed.connect(lambda _: self._update_additional_media())
         self.replay_widgets.append(widget)
         proxy = MediaProxy(widget)
 
         self.subscribe.emit(proxy)
 
         if not widget.is_main_replay_widget and self.STATE != MediaState.LOADING:
-            self.additional_media_changed.emit(self._widget_2_path.values())
+            self._update_additional_media()
 
         self._check_loading_finished()  # check if loading is finished
 
     @qtc.pyqtSlot(AbstractMediaPlayer)
     def widget_failed(self, widget):
         self.remove_replay_source(widget, ignore_errors=True)
         logging.error(f"COULD NOT LOAD {widget = }")
@@ -211,15 +218,15 @@
             self._dead_widgets.append(
                 widget
             )  # keep reference to widget until it is terminated
 
         if not widget.is_main_replay_widget:
             del self._widget_2_path[id(widget)]
             if notify:
-                self.additional_media_changed.emit(self._widget_2_path.values())
+                self._update_additional_media()
             logging.debug(f"self._widget_2_path {self._widget_2_path}")
 
     def widget_terminated(self, widget):
         if widget in self._dead_widgets:
             self._dead_widgets.remove(widget)
         assert widget not in self.replay_widgets
         assert widget not in self._dead_widgets
@@ -279,18 +286,7 @@
         logging.debug("Waiting for dead widgets to terminate")
         # wait for all widgets to be deleted
 
         for w in self._dead_widgets:
             w.kill()
 
         logging.info("Shut down MediaController successfully")
-
-    @qtc.pyqtSlot()
-    def settings_changed(self):
-        for widget in self.replay_widgets:
-            proxy = media_proxy_map.get(id(widget))
-            if proxy is None:
-                raise RuntimeError(f"Could not find proxy for widget {widget}")
-            if proxy.fps != widget.fps:
-                proxy.fps = widget.fps
-                self.unsubscribe.emit(proxy)
-                self.subscribe.emit(proxy)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media/backend/player.py` & `annotation_tool-0.9.0/annotation_tool/media/backend/player.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from abc import abstractmethod
+from pathlib import Path
 
 import PyQt6.QtCore as qtc
 import PyQt6.QtGui as qtg
 import PyQt6.QtWidgets as qtw
 
 from annotation_tool.utility import filehandler
 
 
 class AbstractMediaPlayer(qtw.QWidget):
     remove_wanted = qtc.pyqtSignal(qtw.QWidget)  # Emit self to be removed
-    new_input_wanted = qtc.pyqtSignal(str)  # Path to new input-file
+    new_input_wanted = qtc.pyqtSignal(Path)  # Path to new input-file
     loaded = qtc.pyqtSignal(
         qtw.QWidget
     )  # Emit self to notify controller about successfully loading
     failed = qtc.pyqtSignal(
         qtw.QWidget
     )  # Emit self to notify controller about failed loading
     cleaned_up = qtc.pyqtSignal(qtw.QWidget)
     finished = qtc.pyqtSignal(qtw.QWidget)
+    offset_changed = qtc.pyqtSignal(int)
 
     def __init__(self, is_main, *args, **kwargs):
         super(AbstractMediaPlayer, self).__init__(*args, **kwargs)
 
         self._terminated = False
 
         # media controll attributes
@@ -50,24 +52,26 @@
         menu.popup(qtg.QCursor.pos())
 
     @qtc.pyqtSlot()
     def add_input(self):
         filename, _ = qtw.QFileDialog.getOpenFileName(
             directory="", filter="Video MoCap (*.mp4 *.avi *.csv)"
         )
+        filename = Path(filename)
         if filehandler.is_non_zero_file(filename):
             self.new_input_wanted.emit(filename)
 
     @qtc.pyqtSlot()
     def remove_input(self):
         self.remove_wanted.emit(self)
 
     def change_offset(self, offs):
         self.offset = offs
         self.update_media_position()
+        self.offset_changed.emit(offs)
 
     @qtc.pyqtSlot()
     def adjust_offset(self):
         old_offset = self.offset
         input_dialog = qtw.QInputDialog(self)
 
         input_dialog.setInputMode(qtw.QInputDialog.InputMode.IntInput)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media/backend/timer.py` & `annotation_tool-0.9.0/annotation_tool/media/backend/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,9 +168,9 @@
 
     @qtc.pyqtSlot(qtc.QObject)
     def unsubscribe(self, subscriber):
         self._subscribers = [x for x in self._subscribers if x != subscriber]
         self.position_changed.disconnect(subscriber.set_position_)
 
     def sync_time(self, new_pos: int = None):
-        self._start_pos = new_pos if new_pos else self.frame_position
+        self._start_pos = new_pos if new_pos is not None else self.frame_position
         self._start_time = time_in_millis() if not self._paused else None
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media/backend/type_specific_player/video.py` & `annotation_tool-0.9.0/annotation_tool/media/backend/type_specific_player/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from pathlib import Path
 from threading import Thread
 from time import sleep
 
 import PyQt6.QtCore as qtc
 import PyQt6.QtGui as qtg
 import PyQt6.QtWidgets as qtw
 
@@ -24,15 +25,15 @@
             w, h = vp.lblVid.width(), vp.lblVid.height()
         sleep(0.1)
 
 
 class VideoPlayer(AbstractMediaPlayer):
     get_update = qtc.pyqtSignal()
     media_loaded = qtc.pyqtSignal(object)
-    load_worker = qtc.pyqtSignal(str)
+    load_worker = qtc.pyqtSignal(Path)
     stop_worker = qtc.pyqtSignal()
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         self.lblVid = qtw.QLabel(self)
         self.lblVid.setSizePolicy(
@@ -137,16 +138,16 @@
         self._last_img = None
         self._finished = False
 
         self._last_pos = -9999999
         self._last_w = -1
         self._last_h = -1
 
-    @qtc.pyqtSlot(str)
-    def load(self, path):
+    @qtc.pyqtSlot(Path)
+    def load(self, path: Path):
         self.media = mr(path)
         self.loaded.emit(self.fps, self.n_frames)
 
     @property
     def n_frames(self):
         if self.media:
             return len(self.media)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media/media.py` & `annotation_tool-0.9.0/annotation_tool/media/media.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from pathlib import Path
+from typing import List
+
 import PyQt6.QtCore as qtc
 import PyQt6.QtWidgets as qtw
 
 from .backend.controller import QMediaMainController
 
 
 class QMediaWidget(qtw.QWidget):
@@ -9,28 +12,30 @@
     A simple facade, forwarding all necessary slots and signals
     between the main-application and the media-backend.
 
     Signals:
         position_changed
             Transports the current position of the main replay source
             (always the leftmost on the screen)
+        loaded
+            Emitted when the media is loaded
+        additional_media_changed
+            Emitted when the additional media is changed (added or removed)
 
     Slots:
         load
            Expects an Annotation-instance
         set_position
             Updates the current displayed frame
         play
             Starts running the media
         pause
             Pauses the media
         set_replay_speed
             Updates how fast the media is played
-        settings_changed
-            Needed for updating FPS of Media
         shutdown
             Cleans up all threads and subwidgets
     """
 
     position_changed = qtc.pyqtSignal(int)
     loaded = qtc.pyqtSignal()
     additional_media_changed = qtc.pyqtSignal(list)
@@ -41,39 +46,37 @@
         self.controller.timeout.connect(self.position_changed)
         self.controller.additional_media_changed.connect(self.additional_media_changed)
         self.controller.loaded.connect(self.loaded)
         self._layout = qtw.QHBoxLayout(self)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._layout.addWidget(self.controller)
 
-    @qtc.pyqtSlot(str, list)
-    def load(self, file, additional_media=[]):
+    @qtc.pyqtSlot(Path, list)
+    def load(self, file: Path, additional_media: List = None):
+        if additional_media is None:
+            additional_media = []
         self.controller.load(file, additional_media)
 
     @qtc.pyqtSlot(list)
     def set_additional_media(self, files):
         for f in files:
             self.controller.add_replay_widget(f)
 
     @qtc.pyqtSlot(int)
-    def set_position(self, p):
-        self.controller.set_position(p)
+    def set_position(self, x):
+        self.controller.set_position(x)
 
     @qtc.pyqtSlot()
     def play(self):
         self.controller.play()
 
     @qtc.pyqtSlot()
     def pause(self):
         self.controller.pause()
 
     @qtc.pyqtSlot(float)
     def set_replay_speed(self, x):
         self.controller.set_replay_speed(x)
 
     @qtc.pyqtSlot()
-    def settings_changed(self):
-        self.controller.settings_changed()
-
-    @qtc.pyqtSlot()
     def shutdown(self):
         self.controller.shutdown()
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media_reader/base.py` & `annotation_tool-0.9.0/annotation_tool/media_reader/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,57 @@
 import abc
+import functools
 import logging
 import os
-from typing import Optional, Union
+from pathlib import Path
+import time
+from typing import Optional, Tuple
 
 import numpy as np
 
-__FALLBACK_FPS__ = 30  # fallback framerate if no framerate can be determined
-
-
-def set_fallback_fps(fps: float) -> None:
-    """
-    Sets the fallback framerate.
-
-    Args:
-        fps: The fallback framerate.
-    """
-    if isinstance(fps, (int, float)):
-        logging.debug(f"Setting fallback framerate to {fps}.")
-        global __FALLBACK_FPS__
-        __FALLBACK_FPS__ = fps
-    else:
-        raise TypeError("Framerate must be a number.")
-
-
-def get_fallback_fps() -> Union[int, float]:
-    """
-    Returns the fallback framerate.
-
-    Returns:
-        The fallback framerate.
-    """
-    return __FALLBACK_FPS__
-
 
 class MediaReader(abc.ABC):
     """
     Baseclass for media readers (e.g. video, mocap, etc.)
     """
 
     @abc.abstractmethod
-    def __init__(self, path: os.PathLike, **kwargs) -> None:
+    def __init__(self, path: Path, **kwargs) -> None:
         """
         Initializes a new __MediaReader object.
 
         Args:
             path: The path to the media file.
             kwargs: {fps: The framerate of the media data., n_frames: The number of frames in the media data.}
 
         Raises:
             FileNotFoundError: If the file does not exist.
         """
-        if not os.path.exists(path):
+        if not path.is_file():
             raise FileNotFoundError(f"File {path} does not exist.")
 
     @property
     def duration(self) -> int:
         """
         Returns the duration of the media in milliseconds.
         """
-        try:
-            _duration = self.__get_duration__()
-        except NotImplementedError:
-            _duration = None
-        if _duration:
-            return int(self.__get_duration__()) * 1000
-        else:
-            return int(len(self) / self.fps) * 1000
+        return int(len(self) / self.fps) * 1000
 
     @property
     def fps(self) -> float:
-        _fps = self.__get_fps__()
-        if _fps:
-            return _fps
-        else:
-            return get_fallback_fps()
-
-    @fps.setter
-    def fps(self, fps: Union[int, float]) -> None:
-        self.__set_fps__(fps)
+        return self.__get_fps__()
 
     @property
-    def path(self) -> os.PathLike:
+    def path(self) -> Path:
         return self.__get_path__()
 
+    @property
+    def media_type(self) -> str:
+        return media_type_of(self.path)
+
     def __len__(self):
         return self.__get_frame_count__()
 
     def __getitem__(self, idx):
         """
         Returns the frame at the given index.
         If the index is a slice, returns a list of frames.
@@ -134,49 +99,45 @@
 
         Returns:
             The number of frames in the media file.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __get_duration__(self) -> Optional[float]:
-        """
-        Returns the duration of the media in seconds.
-        """
-        raise NotImplementedError
-
-    @abc.abstractmethod
     def __get_fps__(self) -> Optional[float]:
         """
         Detects the framerate of the media file.
 
         Returns:
             The framerate of the media file if it can be detected, None otherwise.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __get_path__(self) -> os.PathLike:
+    def __get_path__(self) -> Path:
         """
         Returns the path to the media file.
 
         Returns:
             The path to the media file.
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
-    def __set_fps__(self, fps: Union[int, float]) -> None:
+    def numpy(self, lo: int, hi: int, step: int = 1):
         """
-        Sets the framerate of the media file.
+        Returns a numpy array of the frames between lo and hi.
 
         Args:
-            fps: The framerate to set.
+            lo: The lower bound of the frame indices.
+            hi: The upper bound of the frame indices.
+            step: The step size between frames.
+        Returns:
+            A numpy array of the frames between lo and hi with step size step.
         """
-        raise NotImplementedError
+        return np.array([self[i] for i in range(lo, hi, step)])
 
 
 class __MediaSelector:
     def __init__(self):
         self._selector_functions = {}
 
     def register(self, media_type: str, selector_function: callable) -> None:
@@ -193,15 +154,15 @@
         media_type = media_type.lower()
         if not isinstance(media_type, str):
             raise TypeError(f"Invalid argument type {type(media_type) = }")
         if not callable(selector_function):
             raise TypeError(f"Invalid argument type {type(selector_function) = }")
         self._selector_functions[media_type] = selector_function
 
-    def select(self, path: os.PathLike) -> Optional[str]:
+    def select(self, path: Path) -> Optional[str]:
         """
         Selects the media type of the given path.
 
         Args:
             path: The path to the media file.
         Returns:
             The media type of the given path.
@@ -273,38 +234,87 @@
     Raises:
         TypeError: If the media_type is not a string or the selector_function or factory is not a callable.
     """
     __media_selector__.register(media_type, selector_function)
     __media_factory__.register(media_type, factory)
 
 
-def media_reader(path: os.PathLike, **kwargs) -> MediaReader:
+def media_reader(path: Path, **kwargs) -> MediaReader:
     """
     Returns a MediaReader for the given path.
 
     Args:
         path: The path to the media file.
 
     Returns:
         A MediaReader for the given path.
 
     Raises:
         ValueError: If the media type could not be determined.
     """
+    if not isinstance(path, Path):
+        raise TypeError(f"Invalid argument type {type(path) = }")
 
+    start = time.perf_counter()
     media_type = __media_selector__.select(path)
     mr = __media_factory__.create(media_type, path=path, **kwargs)
+    end = time.perf_counter()
+
+    logging.debug(
+        f"Created {media_type} reader for {path} in {end - start:.4f} seconds."
+    )
 
     return mr
 
 
-def media_type_of(path: os.PathLike) -> str:
+def media_type_of(path: Path) -> str:
     """
     Returns the media type of the given path.
 
     Args:
         path: The path to the media file.
 
     Returns:
         The media type of the given path.
     """
     return __media_selector__.select(path)
+
+
+@functools.lru_cache(maxsize=None)
+def _meta_data(file: Path, identifier: Tuple) -> dict:
+    """
+    The identifier-arg is only used for caching.
+    """
+    mr = media_reader(file)
+    return {
+        "fps": mr.fps,
+        "n_frames": len(mr),
+        "duration": mr.duration,
+        "media_type": mr.media_type,
+    }
+
+
+def meta_data(file: Path) -> dict:
+    """
+    Returns the metadata of the media file. The metadata is a dictionary with the following keys:
+        - fps: (float) The framerate of the media.
+        - n_frames: (int) The number of frames in the media.
+        - duration: (int) The duration of the media in milliseconds.
+        - media_type: (str) The type of the media (e.g. video, mocap, etc.).
+
+    The values are cached, so this function can be called multiple times without performance loss.
+    This is the preferred way to get information about the media file.
+    Use this if you don't need the actual media data.
+
+    Args:
+        file: The path to the media file.
+
+    Returns:
+        dict: The metadata. If the file does not exist, an empty dictionary is returned.
+    """
+    try:
+        last_change = int(os.path.getmtime(file))
+        size = os.path.getsize(file)
+        identifier = (last_change, size)
+        return _meta_data(file, identifier)
+    except FileNotFoundError:
+        return {}
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media_reader/mocap.py` & `annotation_tool-0.9.0/annotation_tool/media_reader/mocap.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,57 @@
 import logging
-import os
-from typing import Optional, Union
+from pathlib import Path
+from typing import Optional
 
 import numpy as np
 
 from .base import MediaReader, register_media_reader
 
 
 class MocapReader(MediaReader):
-    def __init__(self, path: os.PathLike, **kwargs) -> None:
+    def __init__(self, path: Path, **kwargs) -> None:
         super().__init__(path, **kwargs)
 
         from .mocap_readers import get_mocap_reader
 
         try:
-            self._mocap_reader = get_mocap_reader(path)
+            self._mocap_reader = get_mocap_reader(path, **kwargs)
         except ValueError as e:
             raise ValueError(f"Could not load mocap data {path}.") from e
 
         self._fps = kwargs.get("fps", None)
         self._duration = kwargs.get("duration", None)
 
     def __get_frame__(self, idx: int) -> np.ndarray:
         return self._mocap_reader.get_frame(idx)
 
     def __get_frame_count__(self) -> int:
         return self._mocap_reader.get_frame_count()
 
-    def __get_duration__(self) -> Optional[float]:
-        if self._duration is None:
-            self._duration = self._mocap_reader.get_duration()
-        return self._duration
-
     def __get_fps__(self) -> Optional[float]:
         if self._fps is None:
             self._fps = self._mocap_reader.get_fps()
         return self._fps
 
-    def __get_path__(self) -> os.PathLike:
+    def __get_path__(self) -> Path:
         return self._mocap_reader.get_path()
 
-    def __set_fps__(self, fps: Union[int, float]) -> None:
-        if not isinstance(fps, (int, float)):
-            raise TypeError("Framerate must be a number.")
-        if fps <= 0:
-            raise ValueError("Framerate must be positive.")
-        self._fps = fps
-
 
-def __is_mocap__(path: os.PathLike) -> bool:
+def __is_mocap__(path: Path) -> bool:
     # TODO improve
     file_extensions = [".c3d", ".bvh", ".csv"]
-    return os.path.splitext(path)[1] in file_extensions
+    return path.suffix.lower() in file_extensions
 
 
-def __mocap_builder__(path: os.PathLike, **kwargs) -> MocapReader:
+def __mocap_builder__(path: Path, **kwargs) -> MocapReader:
     """
     Builds a MocapReader object from the given path.
 
     Args:
-        path (os.PathLike): The path to the mocap file.
+        path (Path): The path to the mocap file.
         fps (float): The framerate of the mocap data.
 
     Returns:
         MocapReader: The MocapReader object.
     """
     return MocapReader(path, **kwargs)
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/base.py` & `annotation_tool-0.9.0/annotation_tool/media_reader/mocap_readers/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import abc
 import dataclasses
-import os
+from pathlib import Path
 from typing import Optional
 
 import numpy as np
 
 
 class MocapReaderBase(abc.ABC):
     """
     Abstract class for video_readers readers.
     """
 
     @abc.abstractmethod
-    def __init__(self, path: os.PathLike, **kwargs):
+    def __init__(self, path: Path, **kwargs):
         """
         Initializes the video_readers reader.
 
         Args:
-            path (os.PathLike): The path to the video_readers file.
+            path (Path): The path to the video_readers file.
         """
         pass
 
     @abc.abstractmethod
     def get_frame(self, frame_idx: int) -> np.ndarray:
         """
         Returns the RGB-frame at the given index.
@@ -54,38 +54,28 @@
 
         Returns:
             Optional[float]: The frames per second. None if the video_readers has no fps.
         """
         pass
 
     @abc.abstractmethod
-    def get_duration(self) -> Optional[float]:
-        """
-        Returns the duration of the video_readers in seconds.
-
-        Returns:
-            float: The duration of the video_readers in seconds. None if the video_readers has no duration.
-        """
-        pass
-
-    @abc.abstractmethod
-    def get_path(self) -> os.PathLike:
+    def get_path(self) -> Path:
         """
         Returns the path to the video_readers.
         """
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def is_supported(path: os.PathLike) -> bool:
+    def is_supported(path: Path) -> bool:
         """
         Returns whether the video_readers format is supported by the reader.
 
         Args:
-            path (os.PathLike): The path to the video_readers file.
+            path (Path): The path to the video_readers file.
 
         Returns:
             bool: Whether the video_readers format is supported by the reader.
         """
         return False
 
 
@@ -110,12 +100,12 @@
         reader (VideoReaderBase): The video_readers reader to register.
         priority (int, optional): The priority of the reader. Defaults to 0.
     """
     __registered_mocap_readers.append(RegisteredMocapReader(reader, priority))
     __registered_mocap_readers.sort(key=lambda x: x.priority, reverse=True)
 
 
-def get_mocap_reader(path: os.PathLike) -> MocapReaderBase:
+def get_mocap_reader(path: Path, **kwargs) -> MocapReaderBase:
     for reader in __registered_mocap_readers:
         if reader.reader.is_supported(path):
-            return reader.reader(path)
-    raise ValueError(f"No video_readers reader found for {path}.")
+            return reader.reader(path, **kwargs)
+    raise ValueError(f"No mocap_reader found for {path}.")
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/lara_reader.py` & `annotation_tool-0.9.0/annotation_tool/media_reader/mocap_readers/lara_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,51 @@
 import logging
-import os
 from pathlib import Path
-from typing import Optional
 
 import numpy as np
 
-try:
-    from .cache import get_cache
-except ImportError:
-    from cache import get_cache
-except Exception:
-    get_cache = None
-
-try:
-    from .base import MocapReaderBase, register_mocap_reader
-except ImportError:
-    from base import MocapReaderBase, register_mocap_reader
+from annotation_tool.utility.filehandler import checksum
 
+from .base import MocapReaderBase, register_mocap_reader
+from .cache import get_cache
 
-def load_lara_mocap(path: Path, data_type: np.dtype = float) -> np.ndarray:
+_mocap_cache = {}
+
+
+def load_lara_mocap(path: Path, normalize: bool) -> np.ndarray:
     """
     Loads the LARa-mocap data from a file.
 
     Args:
-        path (os.PathLike): The path to the LARa-mocap file.
-        data_type (np.dtype): The data type of the returned data.
+        path (Path): The path to the LARa-mocap file.
+        normalize (bool): Whether to normalize the data to the center of the coordinate system.
 
     Returns:
         np.ndarray: The mocap data.
 
     Raises:
         AssertionError: If the data type is not supported.
     """
-    assert data_type in [
-        np.float16,
-        np.float32,
-        np.float64,
-        float,
-    ], f"Invalid dtype {data_type} for mocap data."
-    assert isinstance(path, Path), "Path must be a pathlib.Path object."
+    _hash = checksum(path)
+    _key = (_hash, normalize)
 
     if get_cache is None:
-        logging.warning("Cache not available. Loading mocap from file.")
-        return __load_lara_mocap__(path).astype(data_type)
+        return __load_lara_mocap__(path, normalize)
     else:
-        mocap_cache = get_cache()
+        _cache = get_cache()
 
-        if path in mocap_cache:
-            logging.debug(f"Loaded mocap from cache: {path}")
-            return mocap_cache[path].astype(data_type)
+        if _key in _cache:
+            return _cache[_key]
         else:
-            logging.debug(f"Loaded mocap from file: {path}")
-            mocap = __load_lara_mocap__(path).astype(data_type)
-            mocap_cache[path] = mocap
+            mocap = __load_lara_mocap__(path, normalize)
+            _cache[_key] = mocap
             return mocap
 
 
-def __load_lara_mocap__(path: os.PathLike) -> np.ndarray:
-    """
-    Loads the LARa-mocap data from a file.
-    Right now the LARa-file is expected to contain either 1 or 5 header lines.
-    There should be 132 columns of data + 2 columns for the frame number and the subject.
-
-
-    Args:
-        path (os.PathLike): Path to motion-capture data.
-
-    Raises:
-        TypeError: If the path could not be parsed as a Motion-capture file.
-    """
-
+def __load_lara_mocap__(path: Path, normalize: bool) -> np.ndarray:
     def is_data_row(line2check: str) -> bool:
         """
         Checks if a line is a data row.
         Specific checking for the LARa dataset.
 
         Args:
             line2check (str): Line to check.
@@ -96,20 +68,24 @@
                     break
                 else:
                     header_lines += 1
                 if header_lines > 5:
                     raise TypeError("Too many header lines in mocap file.")
 
         if header_lines in [1, 5]:
-            array = np.loadtxt(path, delimiter=",", skiprows=header_lines)
+            array = np.loadtxt(
+                path, delimiter=",", skiprows=header_lines, dtype=np.float64
+            )
 
             if array.shape[1] == 134:
                 array = array[:, 2:]
 
-            array = __normalize_lara_mocap__(array)
+            if normalize:
+                array = __normalize_lara_mocap__(array)
+
             return array
         else:
             raise TypeError("The number of header lines is not supported.")
     except Exception:
         raise TypeError("Loading mocap failed.")
 
 
@@ -149,24 +125,22 @@
     """Class for reading mocap data."""
 
     def __init__(self, path, **kwargs) -> None:
         """
         Initializes a new MocapReader object.
 
         Args:
-            path (os.PathLike): The path to the mocap file.
-            fps (float): The framerate of the mocap data.
+            path (Path): The path to the mocap file.
 
         Raises:
             FileNotFoundError: If the file does not exist.
         """
-
         self.path = path
-        self._dtype = kwargs.get("dtype", float)
-        self.mocap = load_lara_mocap(Path(self.path), self._dtype)
+        _normalize = kwargs.get("normalize", True)
+        self.mocap = load_lara_mocap(self.path, _normalize)
 
     def get_frame(self, frame_idx: int) -> np.ndarray:
         """
         Returns the skeleton at the given frame index.
 
         Args:
             frame_idx (int): Frame index.
@@ -181,28 +155,25 @@
             raise IndexError("Index out of range.")
 
         return self.mocap[frame_idx]
 
     def get_frame_count(self) -> int:
         return self.mocap.shape[0]
 
-    def get_fps(self) -> Optional[float]:
-        return None
-
-    def get_duration(self) -> float:
-        return None
+    def get_fps(self) -> float:
+        return 200.0
 
-    def get_path(self) -> os.PathLike:
+    def get_path(self) -> Path:
         return self.path
 
     @staticmethod
-    def is_supported(path: os.PathLike) -> bool:
+    def is_supported(path: Path) -> bool:
         # TODO: improve this
         try:
-            load_lara_mocap(Path(path))
+            load_lara_mocap(Path(path), True)
             return True
         except:  # noqa E722
             return False
 
 
 register_mocap_reader(LARaMocapReader, 0)
 logging.info("Registered LARa mocap reader.")
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media_reader/video.py` & `annotation_tool-0.9.0/annotation_tool/media_reader/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
-import os
-from typing import Optional, Union
+from pathlib import Path
+from typing import Optional
 
 import filetype
 import numpy as np
 
 from .base import MediaReader, register_media_reader
 
 
 class VideoReader(MediaReader):
     """
     Adapter class for video_readers for loading and reading videos frame by frame.
     """
 
-    def __init__(self, path: os.PathLike, **kwargs) -> None:
+    def __init__(self, path: Path, **kwargs) -> None:
         super().__init__(path, **kwargs)
 
         from .video_readers import get_video_reader
 
         try:
             self._video_reader = get_video_reader(path)
         except ValueError as e:
@@ -25,37 +25,32 @@
 
     def __get_frame__(self, idx: int) -> np.ndarray:
         return self._video_reader.get_frame(idx)
 
     def __get_frame_count__(self) -> int:
         return self._video_reader.get_frame_count()
 
-    def __get_duration__(self) -> Optional[float]:
-        return self._video_reader.get_duration()
-
     def __get_fps__(self) -> Optional[float]:
         return self._video_reader.get_fps()
 
-    def __get_path__(self) -> os.PathLike:
+    def __get_path__(self) -> Path:
         return self._video_reader.get_path()
 
-    def __set_fps__(self, fps: Union[int, float]) -> None:
-        raise NotImplementedError("Setting the framerate of a video is not supported.")
-
 
-def __is_video__(path: os.PathLike) -> bool:
-    if not os.path.isfile(path):
-        return False
-    try:
-        return filetype.is_video(path)
-    except TypeError:
-        return False
+def __is_video__(path: Path) -> bool:
+    if path.is_file():
+        try:
+            return filetype.is_video(path)
+        except TypeError:
+            return False
+    else:
+        raise FileNotFoundError(f"File {path} does not exist.")
 
 
-def __video_builder__(path=None, **kwargs) -> VideoReader:
+def __video_builder__(path, **kwargs) -> VideoReader:
     if __is_video__(path):
         return VideoReader(path, **kwargs)
     else:
         raise ValueError(f"Path {path} is not a video.")
 
 
 register_media_reader(
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/base.py` & `annotation_tool-0.9.0/annotation_tool/media_reader/video_readers/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import abc
 import dataclasses
-import os
-from typing import Tuple
+from pathlib import Path
 
 import numpy as np
 
 
 class VideoReaderBase(abc.ABC):
     """
     Abstract class for video_readers readers.
     """
 
     @abc.abstractmethod
-    def __init__(self, path: os.PathLike, **kwargs):
+    def __init__(self, path: Path, **kwargs):
         """
         Initializes the video_readers reader.
 
         Args:
-            path (os.PathLike): The path to the video_readers file.
+            path (Path): The path to the video_readers file.
         """
         pass
 
     @abc.abstractmethod
     def get_frame(self, frame_idx: int) -> np.ndarray:
         """
         Returns the RGB-frame at the given index.
@@ -54,88 +53,28 @@
 
         Returns:
             float: The frames per second.
         """
         pass
 
     @abc.abstractmethod
-    def get_height(self) -> int:
-        """
-        Returns the height of the video_readers.
-
-        Returns:
-            int: The height of the video_readers.
-        """
-        pass
-
-    @abc.abstractmethod
-    def get_width(self) -> int:
-        """
-        Returns the width of the video_readers.
-
-        Returns:
-            int: The width of the video_readers.
-        """
-        pass
-
-    @abc.abstractmethod
-    def get_size(self) -> Tuple[int, int]:
-        """
-        Returns the size of the video_readers.
-
-        Returns:
-            Tuple[int, int]: The size of the video_readers.
-        """
-        pass
-
-    @abc.abstractmethod
-    def get_duration(self) -> float:
-        """
-        Returns the duration of the video_readers in seconds.
-
-        Returns:
-            float: The duration of the video_readers in seconds.
-        """
-        pass
-
-    @abc.abstractmethod
-    def get_fourcc(self) -> str:
-        """
-        Returns the fourcc code of the video_readers.
-
-        Returns:
-            str: The fourcc code of the video_readers.
-        """
-        pass
-
-    @abc.abstractmethod
-    def get_codec(self) -> str:
-        """
-        Returns the codec of the video_readers.
-
-        Returns:
-            str: The codec of the video_readers.
-        """
-        pass
-
-    @abc.abstractmethod
-    def get_path(self) -> os.PathLike:
+    def get_path(self) -> Path:
         """
         Returns the path to the video_readers.
         """
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def is_supported(path: os.PathLike) -> bool:
+    def is_supported(path: Path) -> bool:
         """
         Returns whether the video_readers format is supported by the reader.
 
         Args:
-            path (os.PathLike): The path to the video_readers file.
+            path (Path): The path to the video_readers file.
 
         Returns:
             bool: Whether the video_readers format is supported by the reader.
         """
         return False
 
 
@@ -160,12 +99,12 @@
         reader (VideoReaderBase): The video_readers reader to register.
         priority (int, optional): The priority of the reader. Defaults to 0.
     """
     __registered_video_readers.append(RegisteredVideoReader(reader, priority))
     __registered_video_readers.sort(key=lambda x: x.priority, reverse=True)
 
 
-def get_video_reader(path: os.PathLike) -> VideoReaderBase:
+def get_video_reader(path: Path) -> VideoReaderBase:
     for reader in __registered_video_readers:
         if reader.reader.is_supported(path):
             return reader.reader(path)
     raise ValueError(f"No video_readers reader found for {path}.")
```

### Comparing `annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/decord_reader.py` & `annotation_tool-0.9.0/annotation_tool/media_reader/video_readers/decord_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 import logging
 import os
-from typing import Tuple
+from pathlib import Path
 
 try:
     import decord
 
-    # use decord only for windows
-    _use_decord = os.name == "nt"
+    _use_decord = os.name == "nt"  # use decord only for windows
 except ImportError:
     logging.debug("Decord not available, falling back to OpenCV")
     decord = None
     _use_decord = False
 
 import numpy as np
 
-try:
-    from .base import VideoReaderBase, register_video_reader
-except ImportError:
-    from base import VideoReaderBase, register_video_reader
+from .base import VideoReaderBase, register_video_reader
 
 
 class DecordReader(VideoReaderBase):
     """
     Video reader using decord.
     """
 
-    def __init__(self, path: os.PathLike, **kwargs):
+    def __init__(self, path: Path, **kwargs):
         """
         Initializes the video reader.
 
         Args:
-            path (os.PathLike): The path to the video file.
+            path (Path): The path to the video file.
         """
         self.path = path
-        self.video = decord.VideoReader(path, ctx=decord.cpu(0))
+        self.video = decord.VideoReader(path.as_posix(), ctx=decord.cpu(0))
 
         logging.info(f"Using decord for video {path}.")
 
     def get_frame(self, frame_idx: int) -> np.ndarray:
         """
         Returns the RGB-frame at the given index.
 
@@ -66,84 +62,42 @@
         Returns the frames per second of the video.
 
         Returns:
             float: The frames per second.
         """
         return self.video.get_avg_fps()
 
-    def get_height(self) -> int:
-        """
-        Returns the height of the video.
-
-        Returns:
-            int: The height of the video.
-        """
-        return self.video[0].shape[0]
-
-    def get_width(self) -> int:
-        """
-        Returns the width of the video.
-
-        Returns:
-            int: The width of the video.
-        """
-        return self.video[0].shape[1]
-
-    def get_size(self) -> Tuple[int, int]:
-        return self.get_width(), self.get_height()
-
-    def get_duration(self) -> float:
-        """
-        Returns the duration of the video in seconds.
-
-        Returns:
-            float: The duration of the video in seconds.
-        """
-        return self.get_frame_count() / self.get_fps()
-
-    def get_codec(self) -> str:
-        """
-        Returns the codec of the video.
-
-        Returns:
-            str: The codec of the video.
-        """
-        raise NotImplementedError
-
-    def get_fourcc(self) -> str:
-        raise NotImplementedError
-
-    def get_path(self) -> os.PathLike:
+    def get_path(self) -> Path:
         return self.path
 
     @staticmethod
-    def is_supported(path: str) -> bool:
+    def is_supported(path: Path) -> bool:
         """
         Returns whether the video format is supported by the reader.
 
         Args:
-            path (os.PathLike): The path to the video file.
+            path (Path): The path to the video file.
 
         Returns:
             bool: True if the video format is supported, False otherwise.
         """
         # dont accept .avi
-        if path.endswith(".avi"):
+        if path.suffix == ".avi":
             return False
         try:
-            decord_reader = decord.VideoReader(path)
+            decord_reader = decord.VideoReader(path.as_posix())
             if len(decord_reader) <= 10:
                 return False
             _ = [decord_reader[i] for i in range(10)]
 
             if decord_reader.get_avg_fps() < 1:
                 return False
 
             return True
         except Exception:  # noqa
             return False
 
 
 if _use_decord:
-    register_video_reader(DecordReader, 1)
+    register_video_reader(DecordReader, -1)  # too heavy on RAM
 
 logging.info("Registered DecordReader.")
```

### Comparing `annotation_tool-0.8.3/annotation_tool/mediator.py` & `annotation_tool-0.9.0/annotation_tool/mediator.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/playback.py` & `annotation_tool-0.9.0/annotation_tool/playback.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py` & `annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/checkable_combobox.py` & `annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/checkable_combobox.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/display_scheme.py` & `annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/display_scheme.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/histogram.py` & `annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/histogram.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/own_slider.py` & `annotation_tool-0.9.0/annotation_tool/qt_helper_widgets/own_slider.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 
 
 class OwnSlider(qtw.QSlider):
     def __init__(self):
         super(OwnSlider, self).__init__(qtc.Qt.Orientation.Horizontal)
 
     def keyPressEvent(self, event) -> None:
-        if event.key() == qtc.Qt.Key.Key_Right:
+        if event.key() == qtc.Qt.Key.Key_Plus:
             self.plus_step()
-        elif event.key() == qtc.Qt.Key.Key_Left:
+            event.accept()
+        elif event.key() == qtc.Qt.Key.Key_Minus:
             self.minus_step()
+            event.accept()
         else:
-            super(OwnSlider, self).keyPressEvent(event)
+            self.parent().keyPressEvent(event)
 
     def plus_step(self):
         """Increase slider to next multiple of single step."""
         rest = self.value() % self.singleStep()
         self.setValue(self.value() + self.singleStep() - rest)
 
     def minus_step(self):
```

### Comparing `annotation_tool-0.8.3/annotation_tool/settings.py` & `annotation_tool-0.9.0/annotation_tool/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,41 +5,33 @@
 
 
 @cached
 @dataclass
 class Settings:
     annotator_id: int = field(init=False, default=0)
     big_skip: int = field(init=False, default=100)
-    darkmode: bool = field(init=False, default=False)
+    color_theme: str = field(init=False, default="light")
     font_size: int = field(init=False, default=10)
     logging_level: int = field(init=False, default=logging.WARNING)
+    merging_mode: str = field(init=False, default="into")
     preferred_width: int = field(init=False, default=1200)
     preferred_height: int = field(init=False, default=700)
-    refresh_rate: int = field(init=False, default=200)
+    timeline_design: str = field(init=False, default="rounded")
     retrieval_segment_overlap: float = field(init=False, default=0)
     retrieval_segment_size: int = field(init=False, default=200)
     small_skip: int = field(init=False, default=1)
 
     def reset(self):
         for fld in fields(self):
             setattr(self, fld.name, fld.default)
 
     def get_default(self, name):
         for fld in fields(self):
             if fld.name == name:
                 return fld.default
 
-    def as_dict(self):
-        return {fld.name: getattr(self, fld.name) for fld in fields(self)}
 
-    def from_dict(self, dct):
-        for fld in fields(self):
-            setattr(self, fld.name, dct.get(fld.name, fld.default))
-
-
-settings = Settings.get_all()
-if len(settings) == 0:
+_cached_settings = Settings.get_all()
+if len(_cached_settings) == 0:
     settings = Settings()
 else:
-    if len(settings) > 1:
-        logging.warning("Found multiple cached settings-objects. Using the first one.")
-    settings = settings[0]
+    settings = _cached_settings[0]
```

### Comparing `annotation_tool-0.8.3/annotation_tool/user_actions.py` & `annotation_tool-0.9.0/annotation_tool/user_actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,21 @@
 }
 
 
 def get_shortcut(action):
     return ActionToShortcut[action] if action in ActionToShortcut else None
 
 
+def get_action(shortcut):
+    for action, shortcut_ in ActionToShortcut.items():
+        if shortcut == shortcut_:
+            return action
+    return None
+
+
 def get_annotation_actions(mode: AnnotationMode):
     if mode == AnnotationMode.MANUAL:
         return [
             AnnotationActions.ANNOTATE,
             AnnotationActions.CUT,
             AnnotationActions.CUT_AND_ANNOTATE,
             AnnotationActions.MERGE_LEFT,
@@ -105,15 +112,14 @@
         return []
 
 
 def get_replay_actions(mode: AnnotationMode):
     if mode == AnnotationMode.MANUAL:
         return [
             ReplayActions.PLAY_OR_PAUSE,
-            # ReplayActions.TOGGLE_FORWARD_BACKWARD,  # TODO: implement
             ReplayActions.SKIP_FRAMES,
             ReplayActions.SKIP_FRAMES_BACK,
             ReplayActions.SKIP_FRAMES_FAR,
             ReplayActions.SKIP_FRAMES_BACK_FAR,
             AnnotationActions.JUMP_PREVIOUS,
             AnnotationActions.JUMP_NEXT,
         ]
```

### Comparing `annotation_tool-0.8.3/annotation_tool/utility/priority_queue.py` & `annotation_tool-0.9.0/annotation_tool/utility/priority_queue.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/annotation_tool/utility/resources.py` & `annotation_tool-0.9.0/annotation_tool/utility/resources.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.3/pyproject.toml` & `annotation_tool-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "annotation-tool"
-version = "0.8.3"
+version = "0.9.0"
 description = "Tool for annotating time series data from sources such as IMUs, MoCap, Videos and more."
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/TUD-Patrec/annotation-tool"
 authors = [
     "Fernando Moya Rueda <fernando.moya@cs.tu-dortmund.de>",
     "Erik Altermann <erik.altermann@tu-dortmund.de>",
@@ -19,60 +19,60 @@
 maintainers = []
 packages = [
     { include = "annotation_tool" },
     { include = "main.py" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.11"
+python = "^3.8,<3.12"
 distinctipy = "^1.2.2"
 filetype = "^1.2.0"
 numpy = "~1.23.5"
 opencv-python = "~4.5.3.56"
 PyOpenGL = "^3.1.6"
 PyOpenGL-accelerate = "^3.1.6"
 PyQt6 = "^6.4.0"
 pyqtgraph = "^0.12.4"
 scipy = "^1.10.0"
 torch = "^2.0.0"
 sortedcontainers = "^2.4.0"
-fcache = "^0.4.7"
+fcache = "^0.5.0"
 appdirs = "^1.4.4"
 decord = { version = "^0.6.0", platform = "win32"}
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 flake8 = "^5.0.4"
 isort = "^5.11.4"
-pyinstaller = "~5.4"
+pyinstaller = "^5.4"
 toml = "^0.10.2"
 commitizen = "^2.37.0"
 pylint = "^2.15.5"
 
 [tool.poetry.group.build]
 optional = true
 
 [tool.poetry.group.build.dependencies]
-pyinstaller = "~5.4"
+pyinstaller = "^5.4"
 
 [tool.poetry.scripts]
 annotation-tool = 'main:start'
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 line_length = 88
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.8.3"
+version = "0.9.0"
 tag_format = "v$version"
 major_version_zero = true
 version_files = [
     "annotation_tool/__init__.py:^__version__",
     "pyproject.toml:^version"
 ]
 update_changelog_on_bump = false
```

### Comparing `annotation_tool-0.8.3/PKG-INFO` & `annotation_tool-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: annotation-tool
-Version: 0.8.3
+Version: 0.9.0
 Summary: Tool for annotating time series data from sources such as IMUs, MoCap, Videos and more.
 Home-page: https://github.com/TUD-Patrec/annotation-tool
 License: MIT
 Author: Fernando Moya Rueda
 Author-email: fernando.moya@cs.tu-dortmund.de
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyOpenGL (>=3.1.6,<4.0.0)
 Requires-Dist: PyOpenGL-accelerate (>=3.1.6,<4.0.0)
 Requires-Dist: PyQt6 (>=6.4.0,<7.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: decord (>=0.6.0,<0.7.0) ; sys_platform == "win32"
 Requires-Dist: distinctipy (>=1.2.2,<2.0.0)
-Requires-Dist: fcache (>=0.4.7,<0.5.0)
+Requires-Dist: fcache (>=0.5.0,<0.6.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: opencv-python (>=4.5.3.56,<4.6.0.0)
 Requires-Dist: pyqtgraph (>=0.12.4,<0.13.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
```

