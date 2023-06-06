# Comparing `tmp/tator-1.0.3.tar.gz` & `tmp/tator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tator-1.0.3.tar", last modified: Tue May 23 02:58:06 2023, max compression
+gzip compressed data, was "tator-1.0.4.tar", last modified: Tue Jun  6 02:58:53 2023, max compression
```

## Comparing `tator-1.0.3.tar` & `tator-1.0.4.tar`

### file list

```diff
@@ -1,292 +1,292 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.804189 tator-1.0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-05-23 02:46:03.000000 tator-1.0.3/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-05-23 02:58:06.804189 tator-1.0.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      667 2023-05-23 02:46:03.000000 tator-1.0.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-05-23 02:46:03.000000 tator-1.0.3/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-23 02:58:06.804189 tator-1.0.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3663 2023-05-23 02:46:03.000000 tator-1.0.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.768189 tator-1.0.3/tator/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-05-23 02:46:03.000000 tator-1.0.3/tator/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.768189 tator-1.0.3/tator/extractor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:46:03.000000 tator-1.0.3/tator/extractor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2023-05-23 02:46:03.000000 tator-1.0.3/tator/extractor/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1562 2023-05-23 02:46:03.000000 tator-1.0.3/tator/extractor/env_launcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12295 2023-05-23 02:46:03.000000 tator-1.0.3/tator/extractor/extractor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.768189 tator-1.0.3/tator/openapi/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-05-23 02:46:03.000000 tator-1.0.3/tator/openapi/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.768189 tator-1.0.3/tator/openapi/tator_openapi/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12710 2023-05-23 02:58:04.000000 tator-1.0.3/tator/openapi/tator_openapi/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.768189 tator-1.0.3/tator/openapi/tator_openapi/api/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-23 02:58:04.000000 tator-1.0.3/tator/openapi/tator_openapi/api/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1854040 2023-05-23 02:58:04.000000 tator-1.0.3/tator/openapi/tator_openapi/api/tator_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26204 2023-05-23 02:58:04.000000 tator-1.0.3/tator/openapi/tator_openapi/api_client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13489 2023-05-23 02:58:04.000000 tator-1.0.3/tator/openapi/tator_openapi/configuration.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2023-05-23 02:58:04.000000 tator-1.0.3/tator/openapi/tator_openapi/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.792189 tator-1.0.3/tator/openapi/tator_openapi/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12120 2023-05-23 02:58:04.000000 tator-1.0.3/tator/openapi/tator_openapi/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8163 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/affiliation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4305 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/affiliation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/affiliation_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8842 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/algorithm.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3019 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/algorithm_manifest.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3697 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/algorithm_parameter.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8339 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/algorithm_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4152 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/analysis.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/analysis_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5083 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/announcement.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6017 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/applet.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4903 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/applet_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/archive_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4121 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/attribute_combinator_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11001 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/attribute_filter_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12663 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/attribute_operation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14079 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/attribute_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/attribute_type_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3763 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/attribute_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5270 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/attribute_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14933 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/audio_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4042 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/autocomplete_service.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6295 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/auxiliary_file_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3705 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bad_request_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5353 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bookmark.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3479 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bookmark_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3495 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bookmark_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8573 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bucket.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10945 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bucket_gcp_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bucket_oci_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6268 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bucket_oci_native_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6022 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bucket_s3_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7814 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bucket_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/bucket_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5847 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/change_log.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/change_log_description_of_change.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5302 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/clone_media_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6715 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/color_map.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3762 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/concat_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/create_list_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4228 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/create_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4548 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/credentials.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/download_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3223 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/download_info_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/email_attachment_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5904 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/email_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6900 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/encode_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7681 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/favorite.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6659 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/favorite_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/favorite_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/feed_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9920 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6208 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6170 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/file_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/file_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/file_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7650 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/file_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/fill.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5778 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/float_array_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4789 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/generic_file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/generic_file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3741 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/get_cloned_media_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/image_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9423 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/invitation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4364 2023-05-23 02:58:02.000000 tator-1.0.3/tator/openapi/tator_openapi/models/invitation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4424 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/invitation_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7272 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/job.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6531 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/job_cluster.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/job_cluster_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5756 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/job_node.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4849 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/job_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6316 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/leaf.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/leaf_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/leaf_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5040 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/leaf_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/leaf_suggestion.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6760 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/leaf_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/leaf_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4306 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/leaf_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/leaf_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/live_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/live_update_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20648 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/localization.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9814 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/localization_bulk_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9386 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/localization_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/localization_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6826 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/localization_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15764 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/localization_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11602 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/localization_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/localization_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8114 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/localization_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15159 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/localization_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18245 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10699 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10188 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_files.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5974 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_next.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_prev.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14774 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5697 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_stats.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14738 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14015 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11297 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16079 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/media_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8877 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/membership.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5693 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/membership_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4593 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/membership_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3057 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/message_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/multi_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/not_found_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3904 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/notify_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6630 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/organization.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5620 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/organization_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5486 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/organization_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3234 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/password_reset_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13571 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/project.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9161 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/project_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/project_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6157 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/resolution_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4639 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/s3_storage_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7613 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/section.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6657 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/section_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6535 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/section_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12378 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_bulk_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10960 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6810 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3465 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_merge_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8846 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_trim_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13336 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12260 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6953 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9375 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/state_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7383 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/temporary_file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5689 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/temporary_file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/token.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3363 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/transcode.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10545 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/transcode_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4532 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/upload_completion_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4597 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/upload_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3883 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/upload_part.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7129 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/user.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8946 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/user_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7852 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/user_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7988 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/version.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5820 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/version_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5694 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/version_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4827 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/video_clip.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9722 2023-05-23 02:58:03.000000 tator-1.0.3/tator/openapi/tator_openapi/models/video_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13486 2023-05-23 02:58:04.000000 tator-1.0.3/tator/openapi/tator_openapi/rest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.792189 tator-1.0.3/tator/transcode/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:46:03.000000 tator-1.0.3/tator/transcode/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6547 2023-05-23 02:46:03.000000 tator-1.0.3/tator/transcode/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2105 2023-05-23 02:46:03.000000 tator-1.0.3/tator/transcode/black.mp4
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-05-23 02:46:03.000000 tator-1.0.3/tator/transcode/create_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2023-05-23 02:46:03.000000 tator-1.0.3/tator/transcode/delete_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8534 2023-05-23 02:46:03.000000 tator-1.0.3/tator/transcode/determine_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2023-05-23 02:46:03.000000 tator-1.0.3/tator/transcode/make_fragment_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6071 2023-05-23 02:46:03.000000 tator-1.0.3/tator/transcode/make_thumbnails.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2023-05-23 02:46:03.000000 tator-1.0.3/tator/transcode/prepare.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16774 2023-05-23 02:46:03.000000 tator-1.0.3/tator/transcode/transcode.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.796189 tator-1.0.3/tator/util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/_download_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6959 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/_upload_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/chunked_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      955 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/chunked_file_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4470 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_leaf_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7441 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_localization_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2510 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11100 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_media_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_membership.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_section.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6560 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_state_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2140 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/clone_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4489 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/concat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/download_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4887 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/download_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/download_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/find_single_change.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/full_state_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/get_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2448 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/get_images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2219 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/get_paginator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      508 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/get_parser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/import_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1729 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/live_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/md5sum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/media_manipulation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17897 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/media_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7283 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/multi_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2322 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/register_algorithm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/register_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5653 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/tator-symbol.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/to_dataframe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/update_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/upload_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3315 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/upload_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1813 2023-05-23 02:46:03.000000 tator-1.0.3/tator/util/upload_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-05-23 02:46:03.000000 tator-1.0.3/tator/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.768189 tator-1.0.3/tator.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-05-23 02:58:06.000000 tator-1.0.3/tator.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11773 2023-05-23 02:58:06.000000 tator-1.0.3/tator.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-23 02:58:06.000000 tator-1.0.3/tator.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       90 2023-05-23 02:58:06.000000 tator-1.0.3/tator.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-23 02:58:06.000000 tator-1.0.3/tator.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 02:58:06.804189 tator-1.0.3/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4863 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_a_float_array.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13689 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_algorithm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9519 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_algorithm_launch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6577 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_archive_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8615 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_attribute_type_addition.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2760 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_attribute_type_deletion.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12411 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_attribute_type_mutation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_attributes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23749 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_change_log.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_clone_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1517 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_clone_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7204 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_clone_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_clone_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1209 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_clone_membership.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_clone_section.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_clone_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_clone_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_collection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6149 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_download_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2123 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12346 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_file_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      585 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_get_clip.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_getframe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1770 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_import_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2558 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_job_cancel.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1772 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_job_cluster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3364 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_leaf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_local_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9199 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_localization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17733 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_localization_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6973 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1423 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3773 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_poly.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      397 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_project_thumbnail.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9638 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_search.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9393 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1854 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_state_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1597 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_stategraphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3884 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_tracks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5487 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1923 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_util_media_manipulation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_util_media_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      912 2023-05-23 02:46:03.000000 tator-1.0.3/test/test_version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.215602 tator-1.0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-06-06 02:47:33.000000 tator-1.0.4/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-06-06 02:58:53.215602 tator-1.0.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      667 2023-06-06 02:47:33.000000 tator-1.0.4/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-06-06 02:47:33.000000 tator-1.0.4/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-06 02:58:53.215602 tator-1.0.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3673 2023-06-06 02:47:33.000000 tator-1.0.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-06-06 02:47:33.000000 tator-1.0.4/tator/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator/extractor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:47:33.000000 tator-1.0.4/tator/extractor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2023-06-06 02:47:33.000000 tator-1.0.4/tator/extractor/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1562 2023-06-06 02:47:33.000000 tator-1.0.4/tator/extractor/env_launcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12295 2023-06-06 02:47:33.000000 tator-1.0.4/tator/extractor/extractor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator/openapi/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-06-06 02:47:33.000000 tator-1.0.4/tator/openapi/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator/openapi/tator_openapi/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12710 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator/openapi/tator_openapi/api/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/api/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1854040 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/api/tator_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26204 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/api_client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13489 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/configuration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.199602 tator-1.0.4/tator/openapi/tator_openapi/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12120 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8163 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/affiliation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4305 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/affiliation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/affiliation_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8842 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/algorithm.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3019 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_manifest.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3697 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_parameter.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8339 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4152 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/analysis.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/analysis_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5083 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/announcement.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6017 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/applet.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4903 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/applet_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/archive_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4121 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_combinator_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11001 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_filter_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12663 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_operation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14079 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3763 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5270 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14933 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/audio_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4042 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/autocomplete_service.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6295 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/auxiliary_file_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3705 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bad_request_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5353 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bookmark.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3479 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bookmark_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3495 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bookmark_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8573 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10945 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_gcp_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_oci_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6268 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_oci_native_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6022 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_s3_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7814 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5847 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/change_log.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/change_log_description_of_change.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5302 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/clone_media_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6715 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/color_map.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3762 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/concat_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/create_list_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4228 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/create_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4548 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/credentials.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/download_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3223 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/download_info_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/email_attachment_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5904 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/email_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9514 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/encode_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7681 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/favorite.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6659 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/favorite_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/favorite_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/feed_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9920 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6208 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6170 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7650 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/fill.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5778 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/float_array_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4789 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/generic_file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/generic_file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3741 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/get_cloned_media_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/image_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9423 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/invitation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4364 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/invitation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4424 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/invitation_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7272 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/job.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6531 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/job_cluster.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/job_cluster_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5756 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/job_node.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4849 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/job_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6316 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5040 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_suggestion.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6760 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4306 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/live_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/live_update_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20648 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9814 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_bulk_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9386 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6826 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15764 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11602 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8114 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15159 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18245 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10699 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10188 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_files.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5974 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_next.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_prev.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14774 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5697 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_stats.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14738 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14015 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11297 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16079 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8877 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/membership.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5693 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/membership_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4593 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/membership_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3057 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/message_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/multi_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/not_found_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3904 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/notify_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6630 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/organization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5620 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/organization_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5486 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/organization_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3234 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/password_reset_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13571 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/project.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9161 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/project_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/project_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/resolution_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4639 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/s3_storage_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7613 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/section.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6657 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/section_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6535 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/section_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12378 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_bulk_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10960 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6810 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3465 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_merge_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8846 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_trim_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13336 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12260 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6953 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9375 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7383 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/temporary_file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5689 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/temporary_file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/token.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3363 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/transcode.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10545 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/transcode_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4532 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/upload_completion_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4597 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/upload_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3883 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/upload_part.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7129 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/user.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8946 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/user_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7852 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/user_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7988 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5820 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/version_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5694 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/version_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4827 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/video_clip.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9722 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/video_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13486 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/rest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.203601 tator-1.0.4/tator/transcode/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6547 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2105 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/black.mp4
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/create_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/delete_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9425 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/determine_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/make_fragment_info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5938 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/make_thumbnails.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/prepare.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19001 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/transcode.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.207602 tator-1.0.4/tator/util/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/_download_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7168 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/_upload_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/chunked_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      955 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/chunked_file_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4470 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_leaf_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7441 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_localization_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2510 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11100 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_media_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_membership.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_section.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6560 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_state_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2140 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4489 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/concat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/download_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4887 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/download_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/download_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/find_single_change.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/full_state_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/get_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2448 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/get_images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2219 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/get_paginator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      508 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/get_parser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/import_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1729 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/live_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/md5sum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/media_manipulation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17897 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/media_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7283 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/multi_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2322 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/register_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/register_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5653 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/tator-symbol.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/to_dataframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/update_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/upload_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3315 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/upload_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1813 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/upload_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-06-06 02:47:33.000000 tator-1.0.4/tator/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-06-06 02:58:53.000000 tator-1.0.4/tator.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11773 2023-06-06 02:58:53.000000 tator-1.0.4/tator.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-06 02:58:53.000000 tator-1.0.4/tator.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       97 2023-06-06 02:58:53.000000 tator-1.0.4/tator.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-06-06 02:58:53.000000 tator-1.0.4/tator.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.215602 tator-1.0.4/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4863 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_a_float_array.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13689 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9519 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_algorithm_launch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6577 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_archive_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8615 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_attribute_type_addition.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2760 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_attribute_type_deletion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12411 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_attribute_type_mutation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_attributes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23749 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_change_log.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1517 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7204 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1209 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_membership.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_section.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_collection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6149 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_download_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2123 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12346 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_file_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      585 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_get_clip.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_getframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1770 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_import_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2558 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_job_cancel.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1772 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_job_cluster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3364 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_leaf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2996 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_local_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9199 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_localization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17733 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_localization_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6973 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1423 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3773 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_poly.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      397 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_project_thumbnail.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9638 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_search.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9393 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1854 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_state_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1597 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_stategraphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3884 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_tracks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5487 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1923 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_util_media_manipulation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_util_media_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      912 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_version.py
```

### Comparing `tator-1.0.3/README.md` & `tator-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/setup.py` & `tator-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup, find_packages  # noqa: H301
 from setuptools.command.dist_info import dist_info
 import requests
 import yaml
 import json
 
 REQUIRES = ["urllib3 >= 1.26", "six >= 1.10", "certifi", "python-dateutil",
-            "requests >= 2.25", "pyyaml", "progressbar2", "pillow"]
+            "requests >= 2.25", "pyyaml", "progressbar2", "pillow", "psutil"]
 
 SCHEMA_FILENAME = 'schema.yaml'
 CONFIG_FILENAME = 'config.json'
 
 def get_version():
     with open(CONFIG_FILENAME, 'r') as f:
         config = json.load(f)
```

### Comparing `tator-1.0.3/tator/__init__.py` & `tator-1.0.4/tator/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/extractor/__main__.py` & `tator-1.0.4/tator/extractor/__main__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/extractor/env_launcher.py` & `tator-1.0.4/tator/extractor/env_launcher.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/extractor/extractor.py` & `tator-1.0.4/tator/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/__init__.py` & `tator-1.0.4/tator/openapi/tator_openapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v1
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 # import apis into sdk package
 from tator.openapi.tator_openapi.api.tator_api import TatorApi
 
 # import ApiClient
 from tator.openapi.tator_openapi.api_client import ApiClient
 from tator.openapi.tator_openapi.configuration import Configuration
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/api/tator_api.py` & `tator-1.0.4/tator/openapi/tator_openapi/api/tator_api.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/api_client.py` & `tator-1.0.4/tator/openapi/tator_openapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.3/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.4/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/configuration.py` & `tator-1.0.4/tator/openapi/tator_openapi/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 1.0.3".\
+               "SDK Package Version: 1.0.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/exceptions.py` & `tator-1.0.4/tator/openapi/tator_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/__init__.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/affiliation.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/affiliation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/affiliation_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/affiliation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/affiliation_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/affiliation_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/algorithm.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/algorithm_manifest.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_manifest.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/algorithm_parameter.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_parameter.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/algorithm_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/analysis.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/analysis.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/analysis_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/analysis_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/announcement.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/announcement.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/applet.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/applet_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/applet_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/archive_config.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/archive_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/attribute_combinator_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_combinator_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/attribute_filter_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_filter_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/attribute_operation_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_operation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/attribute_type.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/attribute_type_delete.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/attribute_type_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/attribute_type_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/audio_definition.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/audio_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/autocomplete_service.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/autocomplete_service.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/auxiliary_file_definition.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/auxiliary_file_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bad_request_response.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bad_request_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bookmark.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bookmark.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bookmark_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bookmark_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bookmark_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bookmark_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bucket.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bucket.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bucket_gcp_config.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_gcp_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bucket_oci_config.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_oci_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bucket_oci_native_config.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_oci_native_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bucket_s3_config.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_s3_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bucket_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/bucket_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/change_log.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/change_log.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/change_log_description_of_change.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/change_log_description_of_change.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/clone_media_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/clone_media_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/color_map.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/color_map.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/concat_definition.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/concat_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/create_list_response.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/create_list_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/create_response.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/create_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/credentials.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/credentials.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/download_info.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/download_info.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/download_info_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/download_info_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/email_attachment_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/email_attachment_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/email_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/email_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/encode_config.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/favorite.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,193 +14,236 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class EncodeConfig(object):
+class Favorite(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'crf': 'int',
-        'movflags': 'str',
-        'preset': 'str',
-        'tune': 'str',
-        'vcodec': 'str'
+        'entity_type_name': 'str',
+        'id': 'int',
+        'name': 'str',
+        'page': 'int',
+        'type': 'int',
+        'user': 'int',
+        'values': 'dict(str, object)'
     }
 
     attribute_map = {
-        'crf': 'crf',
-        'movflags': 'movflags',
-        'preset': 'preset',
-        'tune': 'tune',
-        'vcodec': 'vcodec'
+        'entity_type_name': 'entity_type_name',
+        'id': 'id',
+        'name': 'name',
+        'page': 'page',
+        'type': 'type',
+        'user': 'user',
+        'values': 'values'
     }
 
-    def __init__(self, crf=23, movflags='', preset='fast', tune='fastdecode', vcodec='hevc', local_vars_configuration=None):  # noqa: E501
-        """EncodeConfig - a model defined in OpenAPI"""
+    def __init__(self, entity_type_name=None, id=None, name=None, page=1, type=None, user=None, values=None, local_vars_configuration=None):  # noqa: E501
+        """Favorite - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._crf = None
-        self._movflags = None
-        self._preset = None
-        self._tune = None
-        self._vcodec = None
+        self._entity_type_name = None
+        self._id = None
+        self._name = None
+        self._page = None
+        self._type = None
+        self._user = None
+        self._values = None
         self.discriminator = None
 
-        if crf is not None:
-            self.crf = crf
-        if movflags is not None:
-            self.movflags = movflags
-        if preset is not None:
-            self.preset = preset
-        if tune is not None:
-            self.tune = tune
-        if vcodec is not None:
-            self.vcodec = vcodec
+        if entity_type_name is not None:
+            self.entity_type_name = entity_type_name
+        if id is not None:
+            self.id = id
+        if name is not None:
+            self.name = name
+        if page is not None:
+            self.page = page
+        if type is not None:
+            self.type = type
+        if user is not None:
+            self.user = user
+        if values is not None:
+            self.values = values
 
     @property
-    def crf(self):
+    def entity_type_name(self):
         """
-        Constant rate factor.
+        Name of entity type associated with the favorite
 
-        :return: The crf of this EncodeConfig. 
+        :return: The entity_type_name of this Favorite. 
+        :rtype: str
+        """
+        return self._entity_type_name
+
+    @entity_type_name.setter
+    def entity_type_name(self, entity_type_name):
+        """
+        Name of entity type associated with the favorite
+
+        :param entity_type_name: The entity_type_name of this Favorite.
+        :type: str
+        """
+        allowed_values = ["Localization", "State"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and entity_type_name not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `entity_type_name` ({0}), must be one of {1}"  # noqa: E501
+                .format(entity_type_name, allowed_values)
+            )
+
+        self._entity_type_name = entity_type_name
+
+    @property
+    def id(self):
+        """
+        Unique integer identifying a favorite.
+
+        :return: The id of this Favorite. 
         :rtype: int
         """
-        return self._crf
+        return self._id
 
-    @crf.setter
-    def crf(self, crf):
+    @id.setter
+    def id(self, id):
         """
-        Constant rate factor.
+        Unique integer identifying a favorite.
 
-        :param crf: The crf of this EncodeConfig.
+        :param id: The id of this Favorite.
         :type: int
         """
-        if (self.local_vars_configuration.client_side_validation and
-                crf is not None and crf > 51):  # noqa: E501
-            raise ValueError("Invalid value for `crf`, must be a value less than or equal to `51`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                crf is not None and crf < 0):  # noqa: E501
-            raise ValueError("Invalid value for `crf`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self._crf = crf
+        self._id = id
 
     @property
-    def movflags(self):
+    def name(self):
         """
-        Movflags to specify to packager
+        Name of the favorite.
 
-        :return: The movflags of this EncodeConfig. 
+        :return: The name of this Favorite. 
         :rtype: str
         """
-        return self._movflags
+        return self._name
 
-    @movflags.setter
-    def movflags(self, movflags):
+    @name.setter
+    def name(self, name):
         """
-        Movflags to specify to packager
+        Name of the favorite.
 
-        :param movflags: The movflags of this EncodeConfig.
+        :param name: The name of this Favorite.
         :type: str
         """
 
-        self._movflags = movflags
+        self._name = name
 
     @property
-    def preset(self):
+    def page(self):
         """
-        Preset for ffmpeg encoding.
+        Integer specifying page to display on. Should be 1-10.
 
-        :return: The preset of this EncodeConfig. 
-        :rtype: str
+        :return: The page of this Favorite. 
+        :rtype: int
         """
-        return self._preset
+        return self._page
 
-    @preset.setter
-    def preset(self, preset):
+    @page.setter
+    def page(self, page):
         """
-        Preset for ffmpeg encoding.
+        Integer specifying page to display on. Should be 1-10.
 
-        :param preset: The preset of this EncodeConfig.
-        :type: str
+        :param page: The page of this Favorite.
+        :type: int
         """
-        allowed_values = ["ultrafast", "superfast", "veryfast", "faster", "fast", "medium", "slow", "slower", "veryslow"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and preset not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `preset` ({0}), must be one of {1}"  # noqa: E501
-                .format(preset, allowed_values)
-            )
+        if (self.local_vars_configuration.client_side_validation and
+                page is not None and page > 10):  # noqa: E501
+            raise ValueError("Invalid value for `page`, must be a value less than or equal to `10`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                page is not None and page < 1):  # noqa: E501
+            raise ValueError("Invalid value for `page`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._preset = preset
+        self._page = page
 
     @property
-    def tune(self):
+    def type(self):
         """
-        Tune setting for ffmpeg.
+        Unique integer identifying entity type of this entry.
 
-        :return: The tune of this EncodeConfig. 
-        :rtype: str
+        :return: The type of this Favorite. 
+        :rtype: int
         """
-        return self._tune
+        return self._type
 
-    @tune.setter
-    def tune(self, tune):
+    @type.setter
+    def type(self, type):
         """
-        Tune setting for ffmpeg.
+        Unique integer identifying entity type of this entry.
 
-        :param tune: The tune of this EncodeConfig.
-        :type: str
+        :param type: The type of this Favorite.
+        :type: int
         """
-        allowed_values = ["film", "animation", "grain", "stillimage", "fastdecode", "zerolatency", "psnr", "ssim"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and tune not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `tune` ({0}), must be one of {1}"  # noqa: E501
-                .format(tune, allowed_values)
-            )
 
-        self._tune = tune
+        self._type = type
 
     @property
-    def vcodec(self):
+    def user(self):
         """
-        Video codec.
+        Unique integer identifying a user.
 
-        :return: The vcodec of this EncodeConfig. 
-        :rtype: str
+        :return: The user of this Favorite. 
+        :rtype: int
         """
-        return self._vcodec
+        return self._user
 
-    @vcodec.setter
-    def vcodec(self, vcodec):
+    @user.setter
+    def user(self, user):
         """
-        Video codec.
+        Unique integer identifying a user.
 
-        :param vcodec: The vcodec of this EncodeConfig.
-        :type: str
+        :param user: The user of this Favorite.
+        :type: int
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                user is not None and user < 1):  # noqa: E501
+            raise ValueError("Invalid value for `user`, must be a value greater than or equal to `1`")  # noqa: E501
+
+        self._user = user
+
+    @property
+    def values(self):
+        """
+        Attribute name/value pairs.
+
+        :return: The values of this Favorite. 
+        :rtype: dict(str, object)
+        """
+        return self._values
+
+    @values.setter
+    def values(self, values):
+        """
+        Attribute name/value pairs.
+
+        :param values: The values of this Favorite.
+        :type: dict(str, object)
         """
-        allowed_values = ["copy", "h264", "hevc"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and vcodec not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `vcodec` ({0}), must be one of {1}"  # noqa: E501
-                .format(vcodec, allowed_values)
-            )
 
-        self._vcodec = vcodec
+        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -228,18 +271,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, EncodeConfig):
+        if not isinstance(other, Favorite):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, EncodeConfig):
+        if not isinstance(other, Favorite):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/favorite.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/favorite_spec.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,232 +14,180 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Favorite(object):
+class FavoriteSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'entity_type_name': 'str',
-        'id': 'int',
         'name': 'str',
         'page': 'int',
         'type': 'int',
-        'user': 'int',
         'values': 'dict(str, object)'
     }
 
     attribute_map = {
         'entity_type_name': 'entity_type_name',
-        'id': 'id',
         'name': 'name',
         'page': 'page',
         'type': 'type',
-        'user': 'user',
         'values': 'values'
     }
 
-    def __init__(self, entity_type_name=None, id=None, name=None, page=1, type=None, user=None, values=None, local_vars_configuration=None):  # noqa: E501
-        """Favorite - a model defined in OpenAPI"""
+    def __init__(self, entity_type_name=None, name=None, page=1, type=None, values=None, local_vars_configuration=None):  # noqa: E501
+        """FavoriteSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._entity_type_name = None
-        self._id = None
         self._name = None
         self._page = None
         self._type = None
-        self._user = None
         self._values = None
         self.discriminator = None
 
         if entity_type_name is not None:
             self.entity_type_name = entity_type_name
-        if id is not None:
-            self.id = id
         if name is not None:
             self.name = name
         if page is not None:
             self.page = page
         if type is not None:
             self.type = type
-        if user is not None:
-            self.user = user
         if values is not None:
             self.values = values
 
     @property
     def entity_type_name(self):
         """
         Name of entity type associated with the favorite
 
-        :return: The entity_type_name of this Favorite. 
+        :return: The entity_type_name of this FavoriteSpec. 
         :rtype: str
         """
         return self._entity_type_name
 
     @entity_type_name.setter
     def entity_type_name(self, entity_type_name):
         """
         Name of entity type associated with the favorite
 
-        :param entity_type_name: The entity_type_name of this Favorite.
+        :param entity_type_name: The entity_type_name of this FavoriteSpec.
         :type: str
         """
         allowed_values = ["Localization", "State"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and entity_type_name not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `entity_type_name` ({0}), must be one of {1}"  # noqa: E501
                 .format(entity_type_name, allowed_values)
             )
 
         self._entity_type_name = entity_type_name
 
     @property
-    def id(self):
-        """
-        Unique integer identifying a favorite.
-
-        :return: The id of this Favorite. 
-        :rtype: int
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """
-        Unique integer identifying a favorite.
-
-        :param id: The id of this Favorite.
-        :type: int
-        """
-
-        self._id = id
-
-    @property
     def name(self):
         """
         Name of the favorite.
 
-        :return: The name of this Favorite. 
+        :return: The name of this FavoriteSpec. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
         Name of the favorite.
 
-        :param name: The name of this Favorite.
+        :param name: The name of this FavoriteSpec.
         :type: str
         """
 
         self._name = name
 
     @property
     def page(self):
         """
         Integer specifying page to display on. Should be 1-10.
 
-        :return: The page of this Favorite. 
+        :return: The page of this FavoriteSpec. 
         :rtype: int
         """
         return self._page
 
     @page.setter
     def page(self, page):
         """
         Integer specifying page to display on. Should be 1-10.
 
-        :param page: The page of this Favorite.
+        :param page: The page of this FavoriteSpec.
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
                 page is not None and page > 10):  # noqa: E501
             raise ValueError("Invalid value for `page`, must be a value less than or equal to `10`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 page is not None and page < 1):  # noqa: E501
             raise ValueError("Invalid value for `page`, must be a value greater than or equal to `1`")  # noqa: E501
 
         self._page = page
 
     @property
     def type(self):
         """
-        Unique integer identifying entity type of this entry.
+        Unique integer identifying an entity type.
 
-        :return: The type of this Favorite. 
+        :return: The type of this FavoriteSpec. 
         :rtype: int
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """
-        Unique integer identifying entity type of this entry.
-
-        :param type: The type of this Favorite.
-        :type: int
-        """
-
-        self._type = type
-
-    @property
-    def user(self):
-        """
-        Unique integer identifying a user.
+        Unique integer identifying an entity type.
 
-        :return: The user of this Favorite. 
-        :rtype: int
-        """
-        return self._user
-
-    @user.setter
-    def user(self, user):
-        """
-        Unique integer identifying a user.
-
-        :param user: The user of this Favorite.
+        :param type: The type of this FavoriteSpec.
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
-                user is not None and user < 1):  # noqa: E501
-            raise ValueError("Invalid value for `user`, must be a value greater than or equal to `1`")  # noqa: E501
+                type is not None and type < 1):  # noqa: E501
+            raise ValueError("Invalid value for `type`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._user = user
+        self._type = type
 
     @property
     def values(self):
         """
         Attribute name/value pairs.
 
-        :return: The values of this Favorite. 
+        :return: The values of this FavoriteSpec. 
         :rtype: dict(str, object)
         """
         return self._values
 
     @values.setter
     def values(self, values):
         """
         Attribute name/value pairs.
 
-        :param values: The values of this Favorite.
+        :param values: The values of this FavoriteSpec.
         :type: dict(str, object)
         """
 
         self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -271,18 +219,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Favorite):
+        if not isinstance(other, FavoriteSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Favorite):
+        if not isinstance(other, FavoriteSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/favorite_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/job_cluster.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,184 +14,221 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class FavoriteSpec(object):
+class JobCluster(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'entity_type_name': 'str',
+        'cert': 'str',
+        'host': 'str',
+        'id': 'int',
         'name': 'str',
-        'page': 'int',
-        'type': 'int',
-        'values': 'dict(str, object)'
+        'organization': 'int',
+        'port': 'int',
+        'token': 'str'
     }
 
     attribute_map = {
-        'entity_type_name': 'entity_type_name',
+        'cert': 'cert',
+        'host': 'host',
+        'id': 'id',
         'name': 'name',
-        'page': 'page',
-        'type': 'type',
-        'values': 'values'
+        'organization': 'organization',
+        'port': 'port',
+        'token': 'token'
     }
 
-    def __init__(self, entity_type_name=None, name=None, page=1, type=None, values=None, local_vars_configuration=None):  # noqa: E501
-        """FavoriteSpec - a model defined in OpenAPI"""
+    def __init__(self, cert=None, host=None, id=None, name=None, organization=None, port=None, token=None, local_vars_configuration=None):  # noqa: E501
+        """JobCluster - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._entity_type_name = None
+        self._cert = None
+        self._host = None
+        self._id = None
         self._name = None
-        self._page = None
-        self._type = None
-        self._values = None
+        self._organization = None
+        self._port = None
+        self._token = None
         self.discriminator = None
 
-        if entity_type_name is not None:
-            self.entity_type_name = entity_type_name
+        if cert is not None:
+            self.cert = cert
+        if host is not None:
+            self.host = host
+        if id is not None:
+            self.id = id
         if name is not None:
             self.name = name
-        if page is not None:
-            self.page = page
-        if type is not None:
-            self.type = type
-        if values is not None:
-            self.values = values
+        if organization is not None:
+            self.organization = organization
+        if port is not None:
+            self.port = port
+        if token is not None:
+            self.token = token
 
     @property
-    def entity_type_name(self):
+    def cert(self):
         """
-        Name of entity type associated with the favorite
+        Certificate for accessing the job cluster.
 
-        :return: The entity_type_name of this FavoriteSpec. 
+        :return: The cert of this JobCluster. 
         :rtype: str
         """
-        return self._entity_type_name
+        return self._cert
 
-    @entity_type_name.setter
-    def entity_type_name(self, entity_type_name):
+    @cert.setter
+    def cert(self, cert):
         """
-        Name of entity type associated with the favorite
+        Certificate for accessing the job cluster.
 
-        :param entity_type_name: The entity_type_name of this FavoriteSpec.
+        :param cert: The cert of this JobCluster.
         :type: str
         """
-        allowed_values = ["Localization", "State"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and entity_type_name not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `entity_type_name` ({0}), must be one of {1}"  # noqa: E501
-                .format(entity_type_name, allowed_values)
-            )
 
-        self._entity_type_name = entity_type_name
+        self._cert = cert
+
+    @property
+    def host(self):
+        """
+        Hostname where the cluster can be accessed.
+
+        :return: The host of this JobCluster. 
+        :rtype: str
+        """
+        return self._host
+
+    @host.setter
+    def host(self, host):
+        """
+        Hostname where the cluster can be accessed.
+
+        :param host: The host of this JobCluster.
+        :type: str
+        """
+
+        self._host = host
+
+    @property
+    def id(self):
+        """
+        Unique integer identifying the job cluster.
+
+        :return: The id of this JobCluster. 
+        :rtype: int
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """
+        Unique integer identifying the job cluster.
+
+        :param id: The id of this JobCluster.
+        :type: int
+        """
+
+        self._id = id
 
     @property
     def name(self):
         """
-        Name of the favorite.
+        Unique name of the job cluster.
 
-        :return: The name of this FavoriteSpec. 
+        :return: The name of this JobCluster. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Name of the favorite.
+        Unique name of the job cluster.
 
-        :param name: The name of this FavoriteSpec.
+        :param name: The name of this JobCluster.
         :type: str
         """
 
         self._name = name
 
     @property
-    def page(self):
+    def organization(self):
         """
-        Integer specifying page to display on. Should be 1-10.
+        Unique integer identifying the organization associated with the job cluster.
 
-        :return: The page of this FavoriteSpec. 
+        :return: The organization of this JobCluster. 
         :rtype: int
         """
-        return self._page
+        return self._organization
 
-    @page.setter
-    def page(self, page):
+    @organization.setter
+    def organization(self, organization):
         """
-        Integer specifying page to display on. Should be 1-10.
+        Unique integer identifying the organization associated with the job cluster.
 
-        :param page: The page of this FavoriteSpec.
+        :param organization: The organization of this JobCluster.
         :type: int
         """
-        if (self.local_vars_configuration.client_side_validation and
-                page is not None and page > 10):  # noqa: E501
-            raise ValueError("Invalid value for `page`, must be a value less than or equal to `10`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                page is not None and page < 1):  # noqa: E501
-            raise ValueError("Invalid value for `page`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._page = page
+        self._organization = organization
 
     @property
-    def type(self):
+    def port(self):
         """
-        Unique integer identifying an entity type.
+        Port where the cluster can be accessed.
 
-        :return: The type of this FavoriteSpec. 
+        :return: The port of this JobCluster. 
         :rtype: int
         """
-        return self._type
+        return self._port
 
-    @type.setter
-    def type(self, type):
+    @port.setter
+    def port(self, port):
         """
-        Unique integer identifying an entity type.
+        Port where the cluster can be accessed.
 
-        :param type: The type of this FavoriteSpec.
+        :param port: The port of this JobCluster.
         :type: int
         """
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and type < 1):  # noqa: E501
-            raise ValueError("Invalid value for `type`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._type = type
+        self._port = port
 
     @property
-    def values(self):
+    def token(self):
         """
-        Attribute name/value pairs.
+        Token for accessing the job cluster.
 
-        :return: The values of this FavoriteSpec. 
-        :rtype: dict(str, object)
+        :return: The token of this JobCluster. 
+        :rtype: str
         """
-        return self._values
+        return self._token
 
-    @values.setter
-    def values(self, values):
+    @token.setter
+    def token(self, token):
         """
-        Attribute name/value pairs.
+        Token for accessing the job cluster.
 
-        :param values: The values of this FavoriteSpec.
-        :type: dict(str, object)
+        :param token: The token of this JobCluster.
+        :type: str
         """
 
-        self._values = values
+        self._token = token
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -219,18 +256,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FavoriteSpec):
+        if not isinstance(other, JobCluster):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, FavoriteSpec):
+        if not isinstance(other, JobCluster):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/favorite_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/favorite_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/feed_definition.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/feed_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/file.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/file_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/file_type.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/file_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/file_type_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/file_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/file_type_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/file_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/file_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/file_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/fill.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/fill.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/float_array_query.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/float_array_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/generic_file.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/generic_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/generic_file_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/generic_file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/get_cloned_media_response.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/get_cloned_media_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/image_definition.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/image_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/invitation.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/invitation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/invitation_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/invitation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/invitation_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/invitation_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/job.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/job.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/job_cluster.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/job_cluster_spec.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,219 +14,172 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class JobCluster(object):
+class JobClusterSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'cert': 'str',
         'host': 'str',
-        'id': 'int',
         'name': 'str',
-        'organization': 'int',
         'port': 'int',
         'token': 'str'
     }
 
     attribute_map = {
         'cert': 'cert',
         'host': 'host',
-        'id': 'id',
         'name': 'name',
-        'organization': 'organization',
         'port': 'port',
         'token': 'token'
     }
 
-    def __init__(self, cert=None, host=None, id=None, name=None, organization=None, port=None, token=None, local_vars_configuration=None):  # noqa: E501
-        """JobCluster - a model defined in OpenAPI"""
+    def __init__(self, cert=None, host=None, name=None, port=None, token=None, local_vars_configuration=None):  # noqa: E501
+        """JobClusterSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._cert = None
         self._host = None
-        self._id = None
         self._name = None
-        self._organization = None
         self._port = None
         self._token = None
         self.discriminator = None
 
-        if cert is not None:
-            self.cert = cert
-        if host is not None:
-            self.host = host
-        if id is not None:
-            self.id = id
-        if name is not None:
-            self.name = name
-        if organization is not None:
-            self.organization = organization
-        if port is not None:
-            self.port = port
-        if token is not None:
-            self.token = token
+        self.cert = cert
+        self.host = host
+        self.name = name
+        self.port = port
+        self.token = token
 
     @property
     def cert(self):
         """
         Certificate for accessing the job cluster.
 
-        :return: The cert of this JobCluster. 
+        :return: The cert of this JobClusterSpec. 
         :rtype: str
         """
         return self._cert
 
     @cert.setter
     def cert(self, cert):
         """
         Certificate for accessing the job cluster.
 
-        :param cert: The cert of this JobCluster.
+        :param cert: The cert of this JobClusterSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and cert is None:  # noqa: E501
+            raise ValueError("Invalid value for `cert`, must not be `None`")  # noqa: E501
 
         self._cert = cert
 
     @property
     def host(self):
         """
         Hostname where the cluster can be accessed.
 
-        :return: The host of this JobCluster. 
+        :return: The host of this JobClusterSpec. 
         :rtype: str
         """
         return self._host
 
     @host.setter
     def host(self, host):
         """
         Hostname where the cluster can be accessed.
 
-        :param host: The host of this JobCluster.
+        :param host: The host of this JobClusterSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and host is None:  # noqa: E501
+            raise ValueError("Invalid value for `host`, must not be `None`")  # noqa: E501
 
         self._host = host
 
     @property
-    def id(self):
-        """
-        Unique integer identifying the job cluster.
-
-        :return: The id of this JobCluster. 
-        :rtype: int
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """
-        Unique integer identifying the job cluster.
-
-        :param id: The id of this JobCluster.
-        :type: int
-        """
-
-        self._id = id
-
-    @property
     def name(self):
         """
         Unique name of the job cluster.
 
-        :return: The name of this JobCluster. 
+        :return: The name of this JobClusterSpec. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
         Unique name of the job cluster.
 
-        :param name: The name of this JobCluster.
+        :param name: The name of this JobClusterSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
-    def organization(self):
-        """
-        Unique integer identifying the organization associated with the job cluster.
-
-        :return: The organization of this JobCluster. 
-        :rtype: int
-        """
-        return self._organization
-
-    @organization.setter
-    def organization(self, organization):
-        """
-        Unique integer identifying the organization associated with the job cluster.
-
-        :param organization: The organization of this JobCluster.
-        :type: int
-        """
-
-        self._organization = organization
-
-    @property
     def port(self):
         """
         Port where the cluster can be accessed.
 
-        :return: The port of this JobCluster. 
+        :return: The port of this JobClusterSpec. 
         :rtype: int
         """
         return self._port
 
     @port.setter
     def port(self, port):
         """
         Port where the cluster can be accessed.
 
-        :param port: The port of this JobCluster.
+        :param port: The port of this JobClusterSpec.
         :type: int
         """
+        if self.local_vars_configuration.client_side_validation and port is None:  # noqa: E501
+            raise ValueError("Invalid value for `port`, must not be `None`")  # noqa: E501
 
         self._port = port
 
     @property
     def token(self):
         """
         Token for accessing the job cluster.
 
-        :return: The token of this JobCluster. 
+        :return: The token of this JobClusterSpec. 
         :rtype: str
         """
         return self._token
 
     @token.setter
     def token(self, token):
         """
         Token for accessing the job cluster.
 
-        :param token: The token of this JobCluster.
+        :param token: The token of this JobClusterSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and token is None:  # noqa: E501
+            raise ValueError("Invalid value for `token`, must not be `None`")  # noqa: E501
 
         self._token = token
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -256,18 +209,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, JobCluster):
+        if not isinstance(other, JobClusterSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, JobCluster):
+        if not isinstance(other, JobClusterSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/job_cluster_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/organization_spec.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,174 +14,124 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class JobClusterSpec(object):
+class OrganizationSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'cert': 'str',
-        'host': 'str',
+        'default_membership_permission': 'str',
         'name': 'str',
-        'port': 'int',
-        'token': 'str'
+        'thumb': 'str'
     }
 
     attribute_map = {
-        'cert': 'cert',
-        'host': 'host',
+        'default_membership_permission': 'default_membership_permission',
         'name': 'name',
-        'port': 'port',
-        'token': 'token'
+        'thumb': 'thumb'
     }
 
-    def __init__(self, cert=None, host=None, name=None, port=None, token=None, local_vars_configuration=None):  # noqa: E501
-        """JobClusterSpec - a model defined in OpenAPI"""
+    def __init__(self, default_membership_permission=None, name=None, thumb=None, local_vars_configuration=None):  # noqa: E501
+        """OrganizationSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._cert = None
-        self._host = None
+        self._default_membership_permission = None
         self._name = None
-        self._port = None
-        self._token = None
+        self._thumb = None
         self.discriminator = None
 
-        self.cert = cert
-        self.host = host
+        if default_membership_permission is not None:
+            self.default_membership_permission = default_membership_permission
         self.name = name
-        self.port = port
-        self.token = token
+        if thumb is not None:
+            self.thumb = thumb
 
     @property
-    def cert(self):
+    def default_membership_permission(self):
         """
-        Certificate for accessing the job cluster.
+        Default user permission level for all projects in this organization. If specified, users in this organizaiton will be automatically added to all projects in this organization with at least this permission level.
 
-        :return: The cert of this JobClusterSpec. 
+        :return: The default_membership_permission of this OrganizationSpec. 
         :rtype: str
         """
-        return self._cert
+        return self._default_membership_permission
 
-    @cert.setter
-    def cert(self, cert):
+    @default_membership_permission.setter
+    def default_membership_permission(self, default_membership_permission):
         """
-        Certificate for accessing the job cluster.
+        Default user permission level for all projects in this organization. If specified, users in this organizaiton will be automatically added to all projects in this organization with at least this permission level.
 
-        :param cert: The cert of this JobClusterSpec.
+        :param default_membership_permission: The default_membership_permission of this OrganizationSpec.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and cert is None:  # noqa: E501
-            raise ValueError("Invalid value for `cert`, must not be `None`")  # noqa: E501
+        allowed_values = ["No Access", "View Only", "Can Edit", "Can Transfer", "Can Execute", "Full Control"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and default_membership_permission not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `default_membership_permission` ({0}), must be one of {1}"  # noqa: E501
+                .format(default_membership_permission, allowed_values)
+            )
 
-        self._cert = cert
-
-    @property
-    def host(self):
-        """
-        Hostname where the cluster can be accessed.
-
-        :return: The host of this JobClusterSpec. 
-        :rtype: str
-        """
-        return self._host
-
-    @host.setter
-    def host(self, host):
-        """
-        Hostname where the cluster can be accessed.
-
-        :param host: The host of this JobClusterSpec.
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and host is None:  # noqa: E501
-            raise ValueError("Invalid value for `host`, must not be `None`")  # noqa: E501
-
-        self._host = host
+        self._default_membership_permission = default_membership_permission
 
     @property
     def name(self):
         """
-        Unique name of the job cluster.
+        Name of the organization.
 
-        :return: The name of this JobClusterSpec. 
+        :return: The name of this OrganizationSpec. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Unique name of the job cluster.
+        Name of the organization.
 
-        :param name: The name of this JobClusterSpec.
+        :param name: The name of this OrganizationSpec.
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
-    def port(self):
-        """
-        Port where the cluster can be accessed.
-
-        :return: The port of this JobClusterSpec. 
-        :rtype: int
-        """
-        return self._port
-
-    @port.setter
-    def port(self, port):
-        """
-        Port where the cluster can be accessed.
-
-        :param port: The port of this JobClusterSpec.
-        :type: int
-        """
-        if self.local_vars_configuration.client_side_validation and port is None:  # noqa: E501
-            raise ValueError("Invalid value for `port`, must not be `None`")  # noqa: E501
-
-        self._port = port
-
-    @property
-    def token(self):
+    def thumb(self):
         """
-        Token for accessing the job cluster.
+        S3 key of thumbnail used to represent the organization.
 
-        :return: The token of this JobClusterSpec. 
+        :return: The thumb of this OrganizationSpec. 
         :rtype: str
         """
-        return self._token
+        return self._thumb
 
-    @token.setter
-    def token(self, token):
+    @thumb.setter
+    def thumb(self, thumb):
         """
-        Token for accessing the job cluster.
+        S3 key of thumbnail used to represent the organization.
 
-        :param token: The token of this JobClusterSpec.
+        :param thumb: The thumb of this OrganizationSpec.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and token is None:  # noqa: E501
-            raise ValueError("Invalid value for `token`, must not be `None`")  # noqa: E501
 
-        self._token = token
+        self._thumb = thumb
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -209,18 +159,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, JobClusterSpec):
+        if not isinstance(other, OrganizationSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, JobClusterSpec):
+        if not isinstance(other, OrganizationSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/job_node.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/job_node.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/job_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/job_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/leaf.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/leaf.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/leaf_bulk_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/leaf_id_query.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/leaf_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/leaf_suggestion.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_suggestion.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/leaf_type.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/leaf_type_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/leaf_type_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/leaf_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/live_definition.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/live_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/live_update_definition.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/live_update_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/localization.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/localization.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/localization_bulk_delete.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/localization_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/localization_bulk_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/localization_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/localization_delete.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/localization_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/localization_id_query.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/localization_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/localization_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/localization_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/localization_type.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/localization_type_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/localization_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/localization_type_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/localization_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/localization_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/localization_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_bulk_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_files.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_files.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_id_query.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_next.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_next.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_prev.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_prev.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_stats.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_stats.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_type.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_type_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_type_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/media_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/media_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/membership.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/membership_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/membership_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/membership_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/membership_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/message_response.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/message_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/multi_definition.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/multi_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/not_found_response.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/not_found_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/notify_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/notify_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/organization.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/organization.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/organization_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/organization_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class OrganizationSpec(object):
+class OrganizationUpdate(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
@@ -38,46 +38,47 @@
     attribute_map = {
         'default_membership_permission': 'default_membership_permission',
         'name': 'name',
         'thumb': 'thumb'
     }
 
     def __init__(self, default_membership_permission=None, name=None, thumb=None, local_vars_configuration=None):  # noqa: E501
-        """OrganizationSpec - a model defined in OpenAPI"""
+        """OrganizationUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._default_membership_permission = None
         self._name = None
         self._thumb = None
         self.discriminator = None
 
         if default_membership_permission is not None:
             self.default_membership_permission = default_membership_permission
-        self.name = name
+        if name is not None:
+            self.name = name
         if thumb is not None:
             self.thumb = thumb
 
     @property
     def default_membership_permission(self):
         """
         Default user permission level for all projects in this organization. If specified, users in this organizaiton will be automatically added to all projects in this organization with at least this permission level.
 
-        :return: The default_membership_permission of this OrganizationSpec. 
+        :return: The default_membership_permission of this OrganizationUpdate. 
         :rtype: str
         """
         return self._default_membership_permission
 
     @default_membership_permission.setter
     def default_membership_permission(self, default_membership_permission):
         """
         Default user permission level for all projects in this organization. If specified, users in this organizaiton will be automatically added to all projects in this organization with at least this permission level.
 
-        :param default_membership_permission: The default_membership_permission of this OrganizationSpec.
+        :param default_membership_permission: The default_membership_permission of this OrganizationUpdate.
         :type: str
         """
         allowed_values = ["No Access", "View Only", "Can Edit", "Can Transfer", "Can Execute", "Full Control"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and default_membership_permission not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `default_membership_permission` ({0}), must be one of {1}"  # noqa: E501
                 .format(default_membership_permission, allowed_values)
@@ -86,48 +87,46 @@
         self._default_membership_permission = default_membership_permission
 
     @property
     def name(self):
         """
         Name of the organization.
 
-        :return: The name of this OrganizationSpec. 
+        :return: The name of this OrganizationUpdate. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
         Name of the organization.
 
-        :param name: The name of this OrganizationSpec.
+        :param name: The name of this OrganizationUpdate.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def thumb(self):
         """
         S3 key of thumbnail used to represent the organization.
 
-        :return: The thumb of this OrganizationSpec. 
+        :return: The thumb of this OrganizationUpdate. 
         :rtype: str
         """
         return self._thumb
 
     @thumb.setter
     def thumb(self, thumb):
         """
         S3 key of thumbnail used to represent the organization.
 
-        :param thumb: The thumb of this OrganizationSpec.
+        :param thumb: The thumb of this OrganizationUpdate.
         :type: str
         """
 
         self._thumb = thumb
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -159,18 +158,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, OrganizationSpec):
+        if not isinstance(other, OrganizationUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, OrganizationSpec):
+        if not isinstance(other, OrganizationUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/organization_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/version_spec.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,123 +14,170 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class OrganizationUpdate(object):
+class VersionSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'default_membership_permission': 'str',
+        'bases': 'list[int]',
+        'description': 'str',
+        'elemental_id': 'str',
         'name': 'str',
-        'thumb': 'str'
+        'show_empty': 'bool'
     }
 
     attribute_map = {
-        'default_membership_permission': 'default_membership_permission',
+        'bases': 'bases',
+        'description': 'description',
+        'elemental_id': 'elemental_id',
         'name': 'name',
-        'thumb': 'thumb'
+        'show_empty': 'show_empty'
     }
 
-    def __init__(self, default_membership_permission=None, name=None, thumb=None, local_vars_configuration=None):  # noqa: E501
-        """OrganizationUpdate - a model defined in OpenAPI"""
+    def __init__(self, bases=None, description='', elemental_id=None, name=None, show_empty=True, local_vars_configuration=None):  # noqa: E501
+        """VersionSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._default_membership_permission = None
+        self._bases = None
+        self._description = None
+        self._elemental_id = None
         self._name = None
-        self._thumb = None
+        self._show_empty = None
         self.discriminator = None
 
-        if default_membership_permission is not None:
-            self.default_membership_permission = default_membership_permission
-        if name is not None:
-            self.name = name
-        if thumb is not None:
-            self.thumb = thumb
+        if bases is not None:
+            self.bases = bases
+        if description is not None:
+            self.description = description
+        if elemental_id is not None:
+            self.elemental_id = elemental_id
+        self.name = name
+        if show_empty is not None:
+            self.show_empty = show_empty
 
     @property
-    def default_membership_permission(self):
+    def bases(self):
         """
-        Default user permission level for all projects in this organization. If specified, users in this organizaiton will be automatically added to all projects in this organization with at least this permission level.
+        Array of other version IDs that are dependencies of this version.
 
-        :return: The default_membership_permission of this OrganizationUpdate. 
+        :return: The bases of this VersionSpec. 
+        :rtype: list[int]
+        """
+        return self._bases
+
+    @bases.setter
+    def bases(self, bases):
+        """
+        Array of other version IDs that are dependencies of this version.
+
+        :param bases: The bases of this VersionSpec.
+        :type: list[int]
+        """
+
+        self._bases = bases
+
+    @property
+    def description(self):
+        """
+        Description of the version.
+
+        :return: The description of this VersionSpec. 
+        :rtype: str
+        """
+        return self._description
+
+    @description.setter
+    def description(self, description):
+        """
+        Description of the version.
+
+        :param description: The description of this VersionSpec.
+        :type: str
+        """
+
+        self._description = description
+
+    @property
+    def elemental_id(self):
+        """
+        Unique ID of an element
+
+        :return: The elemental_id of this VersionSpec. 
         :rtype: str
         """
-        return self._default_membership_permission
+        return self._elemental_id
 
-    @default_membership_permission.setter
-    def default_membership_permission(self, default_membership_permission):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
-        Default user permission level for all projects in this organization. If specified, users in this organizaiton will be automatically added to all projects in this organization with at least this permission level.
+        Unique ID of an element
 
-        :param default_membership_permission: The default_membership_permission of this OrganizationUpdate.
+        :param elemental_id: The elemental_id of this VersionSpec.
         :type: str
         """
-        allowed_values = ["No Access", "View Only", "Can Edit", "Can Transfer", "Can Execute", "Full Control"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and default_membership_permission not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `default_membership_permission` ({0}), must be one of {1}"  # noqa: E501
-                .format(default_membership_permission, allowed_values)
-            )
 
-        self._default_membership_permission = default_membership_permission
+        self._elemental_id = elemental_id
 
     @property
     def name(self):
         """
-        Name of the organization.
+        Name of the version.
 
-        :return: The name of this OrganizationUpdate. 
+        :return: The name of this VersionSpec. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Name of the organization.
+        Name of the version.
 
-        :param name: The name of this OrganizationUpdate.
+        :param name: The name of this VersionSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
-    def thumb(self):
+    def show_empty(self):
         """
-        S3 key of thumbnail used to represent the organization.
+        Whether to show this version on media for which no annotations exist.
 
-        :return: The thumb of this OrganizationUpdate. 
-        :rtype: str
+        :return: The show_empty of this VersionSpec. 
+        :rtype: bool
         """
-        return self._thumb
+        return self._show_empty
 
-    @thumb.setter
-    def thumb(self, thumb):
+    @show_empty.setter
+    def show_empty(self, show_empty):
         """
-        S3 key of thumbnail used to represent the organization.
+        Whether to show this version on media for which no annotations exist.
 
-        :param thumb: The thumb of this OrganizationUpdate.
-        :type: str
+        :param show_empty: The show_empty of this VersionSpec.
+        :type: bool
         """
 
-        self._thumb = thumb
+        self._show_empty = show_empty
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -158,18 +205,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, OrganizationUpdate):
+        if not isinstance(other, VersionSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, OrganizationUpdate):
+        if not isinstance(other, VersionSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/password_reset_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/password_reset_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/project.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/project.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/project_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/project_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/project_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/project_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/resolution_config.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/temporary_file_spec.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,161 +14,152 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class ResolutionConfig(object):
+class TemporaryFileSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'crf': 'int',
-        'preset': 'str',
-        'resolution': 'int',
-        'vcodec': 'str'
+        'hours': 'int',
+        'lookup': 'str',
+        'name': 'str',
+        'url': 'str'
     }
 
     attribute_map = {
-        'crf': 'crf',
-        'preset': 'preset',
-        'resolution': 'resolution',
-        'vcodec': 'vcodec'
+        'hours': 'hours',
+        'lookup': 'lookup',
+        'name': 'name',
+        'url': 'url'
     }
 
-    def __init__(self, crf=23, preset='', resolution=None, vcodec='h264', local_vars_configuration=None):  # noqa: E501
-        """ResolutionConfig - a model defined in OpenAPI"""
+    def __init__(self, hours=24, lookup=None, name=None, url=None, local_vars_configuration=None):  # noqa: E501
+        """TemporaryFileSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._crf = None
-        self._preset = None
-        self._resolution = None
-        self._vcodec = None
+        self._hours = None
+        self._lookup = None
+        self._name = None
+        self._url = None
         self.discriminator = None
 
-        if crf is not None:
-            self.crf = crf
-        if preset is not None:
-            self.preset = preset
-        if resolution is not None:
-            self.resolution = resolution
-        if vcodec is not None:
-            self.vcodec = vcodec
+        if hours is not None:
+            self.hours = hours
+        self.lookup = lookup
+        self.name = name
+        self.url = url
 
     @property
-    def crf(self):
+    def hours(self):
         """
-        Constant rate factor.
+        Number of hours file is to be kept alive
 
-        :return: The crf of this ResolutionConfig. 
+        :return: The hours of this TemporaryFileSpec. 
         :rtype: int
         """
-        return self._crf
+        return self._hours
 
-    @crf.setter
-    def crf(self, crf):
+    @hours.setter
+    def hours(self, hours):
         """
-        Constant rate factor.
+        Number of hours file is to be kept alive
 
-        :param crf: The crf of this ResolutionConfig.
+        :param hours: The hours of this TemporaryFileSpec.
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
-                crf is not None and crf > 63):  # noqa: E501
-            raise ValueError("Invalid value for `crf`, must be a value less than or equal to `63`")  # noqa: E501
+                hours is not None and hours > 24):  # noqa: E501
+            raise ValueError("Invalid value for `hours`, must be a value less than or equal to `24`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                crf is not None and crf < 0):  # noqa: E501
-            raise ValueError("Invalid value for `crf`, must be a value greater than or equal to `0`")  # noqa: E501
+                hours is not None and hours < 1):  # noqa: E501
+            raise ValueError("Invalid value for `hours`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._crf = crf
+        self._hours = hours
 
     @property
-    def preset(self):
+    def lookup(self):
         """
-        Codec Specific Preset (e.g. fast, medium, or 0,1,2)
+        md5hash of lookup parameters
 
-        :return: The preset of this ResolutionConfig. 
+        :return: The lookup of this TemporaryFileSpec. 
         :rtype: str
         """
-        return self._preset
+        return self._lookup
 
-    @preset.setter
-    def preset(self, preset):
+    @lookup.setter
+    def lookup(self, lookup):
         """
-        Codec Specific Preset (e.g. fast, medium, or 0,1,2)
+        md5hash of lookup parameters
 
-        :param preset: The preset of this ResolutionConfig.
+        :param lookup: The lookup of this TemporaryFileSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and lookup is None:  # noqa: E501
+            raise ValueError("Invalid value for `lookup`, must not be `None`")  # noqa: E501
 
-        self._preset = preset
+        self._lookup = lookup
 
     @property
-    def resolution(self):
+    def name(self):
         """
-        Vertical Resolution
+        Unique name for the temporary file
 
-        :return: The resolution of this ResolutionConfig. 
-        :rtype: int
+        :return: The name of this TemporaryFileSpec. 
+        :rtype: str
         """
-        return self._resolution
+        return self._name
 
-    @resolution.setter
-    def resolution(self, resolution):
+    @name.setter
+    def name(self, name):
         """
-        Vertical Resolution
+        Unique name for the temporary file
 
-        :param resolution: The resolution of this ResolutionConfig.
-        :type: int
+        :param name: The name of this TemporaryFileSpec.
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                resolution is not None and resolution > 8192):  # noqa: E501
-            raise ValueError("Invalid value for `resolution`, must be a value less than or equal to `8192`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                resolution is not None and resolution < 0):  # noqa: E501
-            raise ValueError("Invalid value for `resolution`, must be a value greater than or equal to `0`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._resolution = resolution
+        self._name = name
 
     @property
-    def vcodec(self):
+    def url(self):
         """
-        Video codec.
+        URL for the temporary file
 
-        :return: The vcodec of this ResolutionConfig. 
+        :return: The url of this TemporaryFileSpec. 
         :rtype: str
         """
-        return self._vcodec
+        return self._url
 
-    @vcodec.setter
-    def vcodec(self, vcodec):
+    @url.setter
+    def url(self, url):
         """
-        Video codec.
+        URL for the temporary file
 
-        :param vcodec: The vcodec of this ResolutionConfig.
+        :param url: The url of this TemporaryFileSpec.
         :type: str
         """
-        allowed_values = ["h264", "av1"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and vcodec not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `vcodec` ({0}), must be one of {1}"  # noqa: E501
-                .format(vcodec, allowed_values)
-            )
+        if self.local_vars_configuration.client_side_validation and url is None:  # noqa: E501
+            raise ValueError("Invalid value for `url`, must not be `None`")  # noqa: E501
 
-        self._vcodec = vcodec
+        self._url = url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -196,18 +187,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResolutionConfig):
+        if not isinstance(other, TemporaryFileSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ResolutionConfig):
+        if not isinstance(other, TemporaryFileSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/s3_storage_config.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/s3_storage_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/section.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/section.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/section_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/section_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/section_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/section_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_bulk_delete.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_bulk_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_delete.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_id_query.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_merge_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_merge_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_trim_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_trim_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_type.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_type_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_type_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/state_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/state_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/temporary_file.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/token.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/token.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/transcode.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/transcode_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/transcode_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/upload_completion_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/upload_completion_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/upload_info.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/upload_info.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/upload_part.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/upload_part.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/user.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/user.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/user_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/user_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/user_update.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/user_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/version.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/version.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/version_spec.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/version_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class VersionSpec(object):
+class VersionUpdate(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
@@ -42,15 +42,15 @@
         'description': 'description',
         'elemental_id': 'elemental_id',
         'name': 'name',
         'show_empty': 'show_empty'
     }
 
     def __init__(self, bases=None, description='', elemental_id=None, name=None, show_empty=True, local_vars_configuration=None):  # noqa: E501
-        """VersionSpec - a model defined in OpenAPI"""
+        """VersionUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._bases = None
         self._description = None
         self._elemental_id = None
@@ -60,120 +60,119 @@
 
         if bases is not None:
             self.bases = bases
         if description is not None:
             self.description = description
         if elemental_id is not None:
             self.elemental_id = elemental_id
-        self.name = name
+        if name is not None:
+            self.name = name
         if show_empty is not None:
             self.show_empty = show_empty
 
     @property
     def bases(self):
         """
         Array of other version IDs that are dependencies of this version.
 
-        :return: The bases of this VersionSpec. 
+        :return: The bases of this VersionUpdate. 
         :rtype: list[int]
         """
         return self._bases
 
     @bases.setter
     def bases(self, bases):
         """
         Array of other version IDs that are dependencies of this version.
 
-        :param bases: The bases of this VersionSpec.
+        :param bases: The bases of this VersionUpdate.
         :type: list[int]
         """
 
         self._bases = bases
 
     @property
     def description(self):
         """
         Description of the version.
 
-        :return: The description of this VersionSpec. 
+        :return: The description of this VersionUpdate. 
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
         Description of the version.
 
-        :param description: The description of this VersionSpec.
+        :param description: The description of this VersionUpdate.
         :type: str
         """
 
         self._description = description
 
     @property
     def elemental_id(self):
         """
         Unique ID of an element
 
-        :return: The elemental_id of this VersionSpec. 
+        :return: The elemental_id of this VersionUpdate. 
         :rtype: str
         """
         return self._elemental_id
 
     @elemental_id.setter
     def elemental_id(self, elemental_id):
         """
         Unique ID of an element
 
-        :param elemental_id: The elemental_id of this VersionSpec.
+        :param elemental_id: The elemental_id of this VersionUpdate.
         :type: str
         """
 
         self._elemental_id = elemental_id
 
     @property
     def name(self):
         """
         Name of the version.
 
-        :return: The name of this VersionSpec. 
+        :return: The name of this VersionUpdate. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
         Name of the version.
 
-        :param name: The name of this VersionSpec.
+        :param name: The name of this VersionUpdate.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def show_empty(self):
         """
         Whether to show this version on media for which no annotations exist.
 
-        :return: The show_empty of this VersionSpec. 
+        :return: The show_empty of this VersionUpdate. 
         :rtype: bool
         """
         return self._show_empty
 
     @show_empty.setter
     def show_empty(self, show_empty):
         """
         Whether to show this version on media for which no annotations exist.
 
-        :param show_empty: The show_empty of this VersionSpec.
+        :param show_empty: The show_empty of this VersionUpdate.
         :type: bool
         """
 
         self._show_empty = show_empty
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -205,18 +204,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, VersionSpec):
+        if not isinstance(other, VersionUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, VersionSpec):
+        if not isinstance(other, VersionUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/video_clip.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/video_clip.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/models/video_definition.py` & `tator-1.0.4/tator/openapi/tator_openapi/models/video_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/openapi/tator_openapi/rest.py` & `tator-1.0.4/tator/openapi/tator_openapi/rest.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/transcode/__main__.py` & `tator-1.0.4/tator/transcode/__main__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/transcode/black.mp4` & `tator-1.0.4/tator/transcode/black.mp4`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/transcode/create_media.py` & `tator-1.0.4/tator/transcode/create_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/transcode/delete_media.py` & `tator-1.0.4/tator/transcode/delete_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/transcode/determine_transcode.py` & `tator-1.0.4/tator/transcode/determine_transcode.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,25 +36,40 @@
     :param token: API token.
     :param media_type: Unique integer identifying a media type.
     :param media_id: Unique integer identifying the media object for which the transcode workloads
                      need to be determined.
     :param path: Path to original file.
     :param group_to: Resolutions less or equal to this will be grouped into one workload.
     """
-    cmd = [
+    slow_cmd = [
         "ffprobe",
         "-v","error",
         "-show_entries", "stream:format=duration",
         "-print_format", "json",
         "-count_frames",
         "-skip_frame", "nokey",
         path,
     ]
-    output = subprocess.run(cmd, stdout=subprocess.PIPE, check=True).stdout
+    # The magic to reliably getting duration appears to be
+    # the 'format=duration'. Out of an abundance of caution
+    # we will leave the slow command in there in the event duration
+    # slips by this faster method.
+    fast_cmd = [
+        "ffprobe",
+        "-v","error",
+        "-show_entries", "stream:format=duration",
+        "-print_format", "json",
+        path,
+    ]
+    output = subprocess.run(fast_cmd, stdout=subprocess.PIPE, check=True).stdout
     video_info = json.loads(output)
+    if video_info['streams'][0].get('duration', None) is None:
+        logger.info("NOTICE: Duration was null have to resort to slow method.")
+        output = subprocess.run(slow_cmd, stdout=subprocess.PIPE, check=True).stdout
+        video_info = json.loads(output)
     stream_idx=0
     audio=False
     for idx, stream in enumerate(video_info["streams"]):
         if stream["codec_type"] == "video":
             stream_idx=idx
         if stream["codec_type"] == "audio":
             logger.info("Found Audio Track")
@@ -125,22 +140,24 @@
         existing_streaming_resolutions = set()
         existing_archival_resolutions = set()
 
     available_resolutions = STREAMING_RESOLUTIONS
     crf_map = defaultdict(lambda: 23)
     codec_map = defaultdict(lambda: 'libx264')
     preset_map = defaultdict(lambda: '')
+    pixel_format_map = defaultdict(lambda: 'yuv420p')
     try:
         if media_type_obj.streaming_config:
             available_resolutions = []
             for config in media_type_obj.streaming_config:
                 available_resolutions.append(config.resolution)
                 crf_map[config.resolution] = config.crf
                 codec_map[config.resolution] = config.vcodec
                 preset_map[config.resolution] = config.preset
+                pixel_format_map[config.resolution] = config.pixel_format
     except Exception as e:
         # Likely an old version of the server
         # TODO: Remove me someday
         print(e)
         print("Defaulting to STREAMING_RESOLUTIONS")
     print(f"Selected Resolutions {available_resolutions}")
 
@@ -159,26 +176,27 @@
         smallest_higher_res = min(r for r in available_resolutions if r > height)
 
         if not (height, codec_map[smallest_higher_res]) in existing_streaming_resolutions:
             # copy personality form the nearest higher resolution
             crf_map[height] = crf_map[smallest_higher_res]
             codec_map[height] = codec_map[smallest_higher_res]
             preset_map[height] = preset_map[smallest_higher_res]
+            pixel_format_map[height] = pixel_format_map[smallest_higher_res]
             resolutions.append(height)
 
     # Streaming workloads (lower res)
     if any(res <= group_to for res in resolutions):
         workloads = [
             {
                 "category": "streaming",
                 "path": path,
                 "raw_height": height,
                 "raw_width": width,
                 "configs": [
-                    f"{res}:{crf_map[res]}:{codec_map[res]}:{preset_map[res]}"
+                    f"{res}:{crf_map[res]}:{codec_map[res]}:{preset_map[res]}:{pixel_format_map[res]}"
                     for res in resolutions
                     if res <= group_to
                 ],
             }
         ]
     else:
         workloads = []
```

### Comparing `tator-1.0.3/tator/transcode/make_fragment_info.py` & `tator-1.0.4/tator/transcode/make_fragment_info.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/transcode/make_thumbnails.py` & `tator-1.0.4/tator/transcode/make_thumbnails.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from PIL import Image
 
 from ..util import get_api
 from ..util._upload_file import _upload_file
 
 from .transcode import get_length_info
 from ..openapi.tator_openapi.models import MessageResponse
-
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Makes thumbnails for a video.')
     parser.add_argument('--host', type=str, default='https://cloud.tator.io', help='Host URL.')
     parser.add_argument('--token', type=str, help='REST API token.')
@@ -76,48 +75,35 @@
 
     # Create thumbnail.
     if needs_thumb_img:
         cmd = ["ffmpeg", "-y", "-i", video_path, "-vf", "scale=256:-1", "-vframes", "1", thumb_path]
         subprocess.run(cmd, check=True)
 
     if needs_thumb_gif:
-        with tempfile.TemporaryDirectory() as dirname:
-            pts_scale = (fps / 3) * (10 / num_frames)
-
-            # Create gif thumbnail.
-            cmd1 = ["ffmpeg", "-y"]
-            if only_keyframes or num_frames > 10000:
-                cmd2 = ["-skip_frame", "nokey"]
-            else:
-                cmd2 = []
-            cmd3 = [
+        # Create gif thumbnail in a single pass
+        # This logic makes a max(video_length,60) second summary video than speeds it up 4 times and saves as a gif
+        video_duration = num_frames/fps
+
+        # Max thumbnail duration is 60 seconds
+        thumb_duration = min(60, video_duration)
+
+        # We either select every Nth second based on how much longer than 60 seconds we are
+        frame_select = max(fps, (video_duration/thumb_duration)*fps)
+
+        # We play each 1 second sample at 4x
+        speed_up = 4*max(1,round(video_duration/thumb_duration))
+        cmd = ["ffmpeg", "-y",
                 "-i",
                 video_path,
                 "-vf",
-                f"scale=256:-1:flags=lanczos,setpts={pts_scale}*PTS",
-                "-r",
-                "3",
-                os.path.join(dirname, "%09d.jpg"),
-            ]
-            cmd = cmd1 + cmd2 + cmd3
-            subprocess.run(cmd, check=True)
-            cmd = [
-                "ffmpeg",
-                "-y",
-                "-r",
-                "3",
-                "-i",
-                os.path.join(dirname, "%09d.jpg"),
-                "-vf",
-                "split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse",
-                "-r",
-                "3",
+                f"select='not(mod(n\,{round(frame_select)}))',scale=256:-1:flags=lanczos,setpts=PTS/{speed_up},split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse",
                 thumb_gif_path,
-            ]
-            subprocess.run(cmd, check=True)
+        ]
+        logger.info(f"cmd={cmd}")
+        subprocess.run(cmd, check=True)
 
     # Upload thumbnail and thumbnail gif.
     if needs_thumb_img:
         for progress, thumbnail_info in _upload_file(
             api,
             media_obj.project,
             thumb_path,
```

### Comparing `tator-1.0.3/tator/transcode/prepare.py` & `tator-1.0.4/tator/transcode/prepare.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/transcode/transcode.py` & `tator-1.0.4/tator/transcode/transcode.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,61 @@
 import argparse
 import logging
 import subprocess
 import json
 import os
 import sys
 from urllib.parse import urlparse
+import psutil
+import time
 
 from ..util.get_api import get_api
 from ..util._upload_file import _upload_file
 from ..openapi.tator_openapi.models import MessageResponse
 
 from .make_fragment_info import make_fragment_info
 
 logger = logging.getLogger(__name__)
 
 # If HW is available, use this as lookup swap
 encoder_lookup=None
 
+SW_TO_HW_PIXEL_FORMAT_CONVERSION = {
+    'yuv420p': 'nv12', # QSV h264 supports this
+    'yuv420p10le': 'p010le', # QSV h264 supports this
+    'yuv422p': 'nv16', # Not sure if any hw encoders actually support this
+    'yuv444p' : 'nv21' # Not sure if any hw encoders actually support this
+}
+
+def _get_resource_usage():
+    """ Returns an object representing memory + CPU usage """
+    cpu_percentages=psutil.cpu_percent(percpu=True)
+    load_avg = psutil.getloadavg()
+    memory_raw = psutil.virtual_memory()
+    memory_utilization = (memory_raw.used / memory_raw.total) * 100
+    memory_in_gb = memory_raw.used / 1024 / 1024
+    return {'cpu_percentages': cpu_percentages,
+           'load_avg': load_avg,
+           'memory_utilization': memory_utilization,
+           'memory_in_gb': memory_in_gb}
+def _launch_and_monitor_resources(cmd, interval=5):
+    proc = subprocess.Popen(cmd)
+    start = time.time()
+    while proc.returncode == None:
+        try:
+            proc.wait(timeout=interval)
+        except subprocess.TimeoutExpired:
+            pass # we don't care
+        logger.info(f"RESOURCE_INFO = {json.dumps(_get_resource_usage())}")
+    if proc.returncode != 0:
+        raise("Transcode process failed")
+    end = time.time()
+    logger.info(f"cmd={cmd}")
+    logger.info(f"time={end-start}")
+
 def find_best_encoder(codec):
     """ Find the best encoder based on what is available on the system """
     global encoder_lookup
     if encoder_lookup is None:
         # Default codecs
         encoder_lookup={"hevc": "libx265",
                         "h264": "libx264",
@@ -107,20 +142,32 @@
     return video_def
 
 def convert_streaming(host, token, media, path, outpath, raw_width, raw_height, configs):
     print(f"Transcoding {path} to {outpath}...")
     # Get workload parameters.
     os.makedirs(outpath, exist_ok=True)
 
-    # Convert settings into resolution/crf/codec.
+    # Convert settings into resolution/crf/codec/presets/pixel_formats.
     resolutions = [int(config.split(':')[0]) for config in configs]
     crfs = [config.split(':')[1] for config in configs]
     codecs = [config.split(':')[2] for config in configs]
     presets = [config.split(':')[3] for config in configs]
 
+    # Handle pixel format addition as an optional argument
+    # This will maintain backwards API compatibility to folks using
+    # this function
+    # TODO: It'd be nice if we didn't pass in the config so awkwardly.
+    pixel_formats = []
+    for c in configs:
+        split_comps = c.split(':')
+        if len(split_comps) == 5:
+            pixel_formats.append(split_comps[4])
+        else:
+            pixel_formats.append("yuv420p")
+
     # Need to get avg_framerate
     cmd = [
         "ffprobe",
         "-v","error",
         "-show_entries", "stream",
         "-print_format", "json",
         "-select_streams", "v",
@@ -152,20 +199,20 @@
             "-g", "25",
             "-movflags",
             "faststart+frag_keyframe+empty_moov+default_base_moof"]
         logger.info(f"Generating resolution @ {resolution}")
         output_file = os.path.join(outpath, f"{resolution}.mp4")
         codec = find_best_encoder(codecs[ridx])
         quality_flag = "-crf"
-        pixel_format = "yuv420p"
+        pixel_format = pixel_formats[ridx]
         hw_upload = ''
         preset = presets[ridx]
         if codec.find("vaapi") >= 0:
             quality_flag = "-global_quality"
-            pixel_format = "nv12"
+            pixel_format = SW_TO_HW_PIXEL_FORMAT_CONVERSION[pixel_format]
             # add format filter for vaapi + add hwupload to incantation
             hw_upload=f'[uf{ridx}];[uf{ridx}]format={pixel_format}[format{ridx}];[format{ridx}]hwupload'
 
         if codec.find('264') > 0:
             preset = preset if preset else 'fast'
             per_res.extend(["-preset", preset,
                             "-tune", "fastdecode"])
@@ -180,15 +227,15 @@
                     "-filter_complex",
                     # Scale the black mp4 to the input resolution prior to concating and scaling back down.
                     f"[0:v:0]yadif[a{ridx}];[a{ridx}]setsar=1[vid{ridx}];[1:v:0]scale={vid_dims[1]}:{vid_dims[0]},setsar=1[bv{ridx}];[vid{ridx}][bv{ridx}]concat=n=2:v=1:a=0[rv{ridx}];[rv{ridx}]scale=-2:{resolution}[catv{ridx}];[catv{ridx}]pad=ceil(iw/2)*2:ceil(ih/2)*2[norate{ridx}];[norate{ridx}]fps={avg_frame_rate}{hw_upload}[outv{ridx}]",
                     "-map", f"[outv{ridx}]",
                     output_file])
 
     logger.info('ffmpeg cmd = {}'.format(cmd))
-    subprocess.run(cmd, check=True)
+    _launch_and_monitor_resources(cmd)
 
     api = get_api(host, token)
     media_obj = api.get_media(media)
 
     for ridx, resolution in enumerate(resolutions):
         output_file = os.path.join(outpath, f"{resolution}.mp4")
         _, res_length = get_length_of_file(output_file)
@@ -264,44 +311,53 @@
             if archive_config.encode.vcodec == 'copy':
                 # If no encode, just use the original file.
                 output_file = path
             else:
                 # Encode the media to archival format.
                 codec = find_best_encoder(archive_config.encode.vcodec)
                 quality_flag = "-crf"
-                pixel_format = "yuv420p"
+                pixel_format = archive_config.encode.pixel_format
                 tune_settings = ["-preset", archive_config.encode.preset,
                                  "-tune", archive_config.encode.tune]
                 if archive_config.encode.movflags:
                     tune_settings.extend(['-movflags', archive_config.encode.movflags])
                 if codec.find("qsv") >= 0:
                     quality_flag = "-global_quality"
-                    pixel_format = "nv12"
+                    pixel_format = SW_TO_HW_PIXEL_FORMAT_CONVERSION[pixel_format]
                     tune_settings=[] #QSV doesn't do tuning
                 elif codec == "libsvt_hevc":
                     # SVT for HEVC does not do tuning or CRF
                     tune_settings=[]
                     quality_flag = "-global_quality"
+
+                hw_preamble = []
+                vaapi_present = codec.find('vaapi') >= 0
+                if vaapi_present:
+                    hw_preamble = ['-init_hw_device', 'vaapi=hw',
+                                   '-filter_hw_device', 'hw']
                 cmd = [
-                    "ffmpeg", "-y",
+                    "ffmpeg",
+                    *hw_preamble,
+                    "-y",
                     "-i", path,
                     "-vcodec", codec,
                     "-vf", "yadif",
                     quality_flag, str(archive_config.encode.crf),
                     "-pix_fmt", pixel_format,
                     *tune_settings
                 ]
+
                 if archive_config.encode.vcodec == 'hevc':
                     cmd += ["-tag:v", "hvc1"]
                 elif archive_config.encode.vcodec == 'h264':
                     cmd += ["-tag:v", "avc1"]
                 cmd.append(output_file)
                     
                 logger.info('ffmpeg cmd = {}'.format(cmd))
-                subprocess.run(cmd, check=True)
+                _launch_and_monitor_resources(cmd)
 
             if archive_config.s3_storage is None:
                 default_archival_upload(api, host, media, output_file, True, size)
             else:
                 import boto3
                 # Get credentials from config object.
                 aws_access_key = archive_config.s3_storage.aws_access_key
```

### Comparing `tator-1.0.3/tator/util/__init__.py` & `tator-1.0.4/tator/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/_download_file.py` & `tator-1.0.4/tator/util/_download_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/_upload_file.py` & `tator-1.0.4/tator/util/_upload_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -89,30 +89,34 @@
         if path.startswith('https://') or path.startswith('http://'):
             return requests.get(path, stream=True).raw
         else:
             return open(path, 'rb')
     if num_chunks > 1:
         # Upload parts.
         parts = []
-        last_progress = 0
-        yield (last_progress, None)
+        yield (0, None)
         gcp_upload = upload_info.upload_id == upload_info.urls[0]
         with get_data(path) as f:
             with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
-                futures = []
+                def complete_chunk(fs):
+                    parts.append(fs.result())
+                    progress = round((len(parts) / num_chunks) *100,1)
+                    return (progress, None)
+                futures = set()
                 for chunk_count, url in enumerate(upload_info.urls):
                     file_part = f.read(chunk_size)
                     default_etag_val = str(chunk_count) if gcp_upload else None
-                    futures.append(executor.submit(_upload_chunk, file_part, chunk_count, chunk_size, file_size, url, path, gcp_upload, default_etag_val, timeout))
-                for chunk_count, future in enumerate(concurrent.futures.as_completed(futures)):
-                    parts.append(future.result())
-                    this_progress = round((chunk_count / num_chunks) *100,1)
-                    if this_progress != last_progress:
-                        yield (this_progress, None)
-                        last_progress = this_progress
+                    future = executor.submit(_upload_chunk, file_part, chunk_count, chunk_size, file_size, url, path, gcp_upload, default_etag_val, timeout)
+                    futures.add(future)
+                    if len(futures) > max_workers:
+                        done, futures = concurrent.futures.wait(futures, return_when=concurrent.futures.FIRST_COMPLETED)
+                        for future in done:
+                            yield complete_chunk(future)
+                for future in concurrent.futures.as_completed(futures):
+                    yield complete_chunk(future)
 
                 # Complete the upload.
                 completed = False
                 count = 0
                 while completed is False and count < MAX_RETRIES:
                     try:
                         count += 1
```

### Comparing `tator-1.0.3/tator/util/chunked_create.py` & `tator-1.0.4/tator/util/chunked_create.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/chunked_file_list.py` & `tator-1.0.4/tator/util/chunked_file_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_leaf_list.py` & `tator-1.0.4/tator/util/clone_leaf_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_leaf_type.py` & `tator-1.0.4/tator/util/clone_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_localization_list.py` & `tator-1.0.4/tator/util/clone_localization_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_localization_type.py` & `tator-1.0.4/tator/util/clone_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_media_list.py` & `tator-1.0.4/tator/util/clone_media_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_media_type.py` & `tator-1.0.4/tator/util/clone_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_membership.py` & `tator-1.0.4/tator/util/clone_membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_section.py` & `tator-1.0.4/tator/util/clone_section.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_state_list.py` & `tator-1.0.4/tator/util/clone_state_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_state_type.py` & `tator-1.0.4/tator/util/clone_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/clone_version.py` & `tator-1.0.4/tator/util/clone_version.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/concat.py` & `tator-1.0.4/tator/util/concat.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/download_attachment.py` & `tator-1.0.4/tator/util/download_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/download_media.py` & `tator-1.0.4/tator/util/download_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/download_temporary_file.py` & `tator-1.0.4/tator/util/download_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/find_single_change.py` & `tator-1.0.4/tator/util/find_single_change.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/full_state_graphic.py` & `tator-1.0.4/tator/util/full_state_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/get_api.py` & `tator-1.0.4/tator/util/get_api.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/get_images.py` & `tator-1.0.4/tator/util/get_images.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/get_paginator.py` & `tator-1.0.4/tator/util/get_paginator.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/import_media.py` & `tator-1.0.4/tator/util/import_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/live_stream.py` & `tator-1.0.4/tator/util/live_stream.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/md5sum.py` & `tator-1.0.4/tator/util/md5sum.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/media_manipulation.py` & `tator-1.0.4/tator/util/media_manipulation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/media_util.py` & `tator-1.0.4/tator/util/media_util.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/multi_stream.py` & `tator-1.0.4/tator/util/multi_stream.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/register_algorithm.py` & `tator-1.0.4/tator/util/register_algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/register_applet.py` & `tator-1.0.4/tator/util/register_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/tator-symbol.png` & `tator-1.0.4/tator/util/tator-symbol.png`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/to_dataframe.py` & `tator-1.0.4/tator/util/to_dataframe.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/update_applet.py` & `tator-1.0.4/tator/util/update_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/upload_attachment.py` & `tator-1.0.4/tator/util/upload_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/upload_media.py` & `tator-1.0.4/tator/util/upload_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator/util/upload_temporary_file.py` & `tator-1.0.4/tator/util/upload_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/tator.egg-info/SOURCES.txt` & `tator-1.0.4/tator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_a_float_array.py` & `tator-1.0.4/test/test_a_float_array.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_algorithm.py` & `tator-1.0.4/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_algorithm_launch.py` & `tator-1.0.4/test/test_algorithm_launch.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_applet.py` & `tator-1.0.4/test/test_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_archive_date.py` & `tator-1.0.4/test/test_archive_date.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_attachment.py` & `tator-1.0.4/test/test_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_attribute_type_addition.py` & `tator-1.0.4/test/test_attribute_type_addition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_attribute_type_deletion.py` & `tator-1.0.4/test/test_attribute_type_deletion.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_attribute_type_mutation.py` & `tator-1.0.4/test/test_attribute_type_mutation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_attributes.py` & `tator-1.0.4/test/test_attributes.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_change_log.py` & `tator-1.0.4/test/test_change_log.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_clone_leaf_type.py` & `tator-1.0.4/test/test_clone_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_clone_localization_type.py` & `tator-1.0.4/test/test_clone_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_clone_media.py` & `tator-1.0.4/test/test_clone_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_clone_media_type.py` & `tator-1.0.4/test/test_clone_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_clone_membership.py` & `tator-1.0.4/test/test_clone_membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_clone_section.py` & `tator-1.0.4/test/test_clone_section.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_clone_state_type.py` & `tator-1.0.4/test/test_clone_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_clone_version.py` & `tator-1.0.4/test/test_clone_version.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_collection.py` & `tator-1.0.4/test/test_collection.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_download_media.py` & `tator-1.0.4/test/test_download_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_extract.py` & `tator-1.0.4/test/test_extract.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_file.py` & `tator-1.0.4/test/test_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_file_type.py` & `tator-1.0.4/test/test_file_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_get_clip.py` & `tator-1.0.4/test/test_get_clip.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_getframe.py` & `tator-1.0.4/test/test_getframe.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_import_media.py` & `tator-1.0.4/test/test_import_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_job_cancel.py` & `tator-1.0.4/test/test_job_cancel.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_job_cluster.py` & `tator-1.0.4/test/test_job_cluster.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_leaf.py` & `tator-1.0.4/test/test_leaf.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_leaf_type.py` & `tator-1.0.4/test/test_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_localization.py` & `tator-1.0.4/test/test_localization.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_localization_graphic.py` & `tator-1.0.4/test/test_localization_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_localization_type.py` & `tator-1.0.4/test/test_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_media.py` & `tator-1.0.4/test/test_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_media_type.py` & `tator-1.0.4/test/test_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_pagination.py` & `tator-1.0.4/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_poly.py` & `tator-1.0.4/test/test_poly.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_search.py` & `tator-1.0.4/test/test_search.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_state.py` & `tator-1.0.4/test/test_state.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_state_graphic.py` & `tator-1.0.4/test/test_state_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_state_type.py` & `tator-1.0.4/test/test_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_stategraphic.py` & `tator-1.0.4/test/test_stategraphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_temporary_file.py` & `tator-1.0.4/test/test_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_tracks.py` & `tator-1.0.4/test/test_tracks.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_transcode.py` & `tator-1.0.4/test/test_transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_util_media_manipulation.py` & `tator-1.0.4/test/test_util_media_manipulation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_util_media_util.py` & `tator-1.0.4/test/test_util_media_util.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.3/test/test_version.py` & `tator-1.0.4/test/test_version.py`

 * *Files identical despite different names*

