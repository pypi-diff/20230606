# Comparing `tmp/sd-parsers-0.2.2.tar.gz` & `tmp/sd-parsers-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd-parsers-0.2.2.tar", last modified: Sun Apr 23 14:51:29 2023, max compression
+gzip compressed data, was "sd-parsers-0.2.3.tar", last modified: Tue Jun  6 02:10:25 2023, max compression
```

## Comparing `sd-parsers-0.2.2.tar` & `sd-parsers-0.2.3.tar`

### file list

```diff
@@ -1,65 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.102538 sd-parsers-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.102538 sd-parsers-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/.github/workflows/publish-to.pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.102538 sd-parsers-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/examples/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/examples/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.102538 sd-parsers-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/src/sd_parsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-23 14:51:29.000000 sd-parsers-0.2.2/src/sd_parsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-23 14:51:29.000000 sd-parsers-0.2.2/src/sd_parsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:51:29.000000 sd-parsers-0.2.2/src/sd_parsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 14:51:29.000000 sd-parsers-0.2.2/src/sd_parsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 14:51:29.000000 sd-parsers-0.2.2/src/sd_parsers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/src/sdparsers/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parser_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/src/sdparsers/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/automatic1111.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/automatic1111_stealth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/invokeai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/novelai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/prompt_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.102538 sd-parsers-0.2.2/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/tests/resources/automatic1111/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/automatic1111/automatic1111_cropped.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/automatic1111/automatic1111_cropped.png
--rw-r--r--   0 runner    (1001) docker     (123)   382368 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/automatic1111/automatic1111_stealth.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/tests/resources/bad_images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/bad_images/empty_file.png
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/bad_images/text_after_idat.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/tests/resources/comfyui/
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/comfyui/img2img_cropped.png
--rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/comfyui/night_evening_day_morning_cropped.png
--rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/comfyui/noisy_latents_3_subjects_cropped.png
--rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/comfyui/unclip_2pass_cropped.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/tests/resources/invokeai/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/invokeai/invokeai1_cropped.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/tests/resources/novelai/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/novelai/novelai1_cropped.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/tests/resources/parser_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/parser_manager/test_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/test_automatic1111.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/test_comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/test_invokeai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/test_novelai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/test_parser_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/tools/crop_image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/tools/crop_image.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.058603 sd-parsers-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.046602 sd-parsers-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.050603 sd-parsers-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/.github/workflows/publish-to.pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-06 02:10:25.058603 sd-parsers-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.050603 sd-parsers-0.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/examples/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/examples/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 02:10:25.058603 sd-parsers-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.046602 sd-parsers-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.050603 sd-parsers-0.2.3/src/sd_parsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-06 02:10:25.000000 sd-parsers-0.2.3/src/sd_parsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-06 02:10:25.000000 sd-parsers-0.2.3/src/sd_parsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:10:25.000000 sd-parsers-0.2.3/src/sd_parsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 02:10:25.000000 sd-parsers-0.2.3/src/sd_parsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 02:10:25.000000 sd-parsers-0.2.3/src/sd_parsers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.054602 sd-parsers-0.2.3/src/sdparsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/src/sdparsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/src/sdparsers/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/src/sdparsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/src/sdparsers/parser_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.054602 sd-parsers-0.2.3/src/sdparsers/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/src/sdparsers/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/src/sdparsers/parsers/automatic1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/src/sdparsers/parsers/comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/src/sdparsers/parsers/invokeai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/src/sdparsers/parsers/novelai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/src/sdparsers/prompt_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.054602 sd-parsers-0.2.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.046602 sd-parsers-0.2.3/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.054602 sd-parsers-0.2.3/tests/resources/automatic1111/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/automatic1111/automatic1111_cropped.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/automatic1111/automatic1111_cropped.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.054602 sd-parsers-0.2.3/tests/resources/bad_images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/bad_images/empty_file.png
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/bad_images/text_after_idat.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.058603 sd-parsers-0.2.3/tests/resources/comfyui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/comfyui/img2img_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/comfyui/night_evening_day_morning_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/comfyui/noisy_latents_3_subjects_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/comfyui/unclip_2pass_cropped.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.058603 sd-parsers-0.2.3/tests/resources/invokeai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/invokeai/invokeai1_cropped.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.058603 sd-parsers-0.2.3/tests/resources/novelai/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/novelai/novelai1_cropped.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.058603 sd-parsers-0.2.3/tests/resources/parser_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/resources/parser_manager/test_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/test_automatic1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/test_comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/test_invokeai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/test_novelai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/test_parser_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:10:25.058603 sd-parsers-0.2.3/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/tools/crop_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-06 02:10:10.000000 sd-parsers-0.2.3/tests/tools/crop_image.sh
```

### Comparing `sd-parsers-0.2.2/.github/workflows/publish-to.pypi.yml` & `sd-parsers-0.2.3/.github/workflows/publish-to.pypi.yml`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/.github/workflows/test.yml` & `sd-parsers-0.2.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/LICENSE.txt` & `sd-parsers-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/PKG-INFO` & `sd-parsers-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-parsers
-Version: 0.2.2
+Version: 0.2.3
 Summary: SD Parsers - read metadata from images created by Stable Diffusion
 License: MIT License
         
         Copyright (c) 2023 d3x-at
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -29,20 +29,22 @@
 License-File: LICENSE.txt
 
 
 ## Features
 
 Supports reading metadata from images generated with:
 * Automatic1111's Stable Diffusion web UI
-* ComfyUI
-* Invoke AI
+* ComfyUI *
+* InvokeAI
 * NovelAI
 
 Provides a list of prompts used in the generation of the image, as well as generator-specific metadata.
 
+\* Custom ComfyUI nodes might parse incorrectly / with incomplete data.
+
 ## Installation
 ```
 pip install sd-parsers
 ```
 
 ## Usage
 For a simple query, import ```ParserManager``` from ```sdparsers``` and use its ```parse()``` method to parse an image. (see [examples](https://github.com/d3x-at/sd-parsers/tree/master/examples))
```

### Comparing `sd-parsers-0.2.2/README.md` & `sd-parsers-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 
 ## Features
 
 Supports reading metadata from images generated with:
 * Automatic1111's Stable Diffusion web UI
-* ComfyUI
-* Invoke AI
+* ComfyUI *
+* InvokeAI
 * NovelAI
 
 Provides a list of prompts used in the generation of the image, as well as generator-specific metadata.
 
+\* Custom ComfyUI nodes might parse incorrectly / with incomplete data.
+
 ## Installation
 ```
 pip install sd-parsers
 ```
 
 ## Usage
 For a simple query, import ```ParserManager``` from ```sdparsers``` and use its ```parse()``` method to parse an image. (see [examples](https://github.com/d3x-at/sd-parsers/tree/master/examples))
```

### Comparing `sd-parsers-0.2.2/examples/cmdline.py` & `sd-parsers-0.2.3/examples/cmdline.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/examples/fast_api.py` & `sd-parsers-0.2.3/examples/fast_api.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/src/sd_parsers.egg-info/PKG-INFO` & `sd-parsers-0.2.3/src/sd_parsers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-parsers
-Version: 0.2.2
+Version: 0.2.3
 Summary: SD Parsers - read metadata from images created by Stable Diffusion
 License: MIT License
         
         Copyright (c) 2023 d3x-at
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -29,20 +29,22 @@
 License-File: LICENSE.txt
 
 
 ## Features
 
 Supports reading metadata from images generated with:
 * Automatic1111's Stable Diffusion web UI
-* ComfyUI
-* Invoke AI
+* ComfyUI *
+* InvokeAI
 * NovelAI
 
 Provides a list of prompts used in the generation of the image, as well as generator-specific metadata.
 
+\* Custom ComfyUI nodes might parse incorrectly / with incomplete data.
+
 ## Installation
 ```
 pip install sd-parsers
 ```
 
 ## Usage
 For a simple query, import ```ParserManager``` from ```sdparsers``` and use its ```parse()``` method to parse an image. (see [examples](https://github.com/d3x-at/sd-parsers/tree/master/examples))
```

### Comparing `sd-parsers-0.2.2/src/sd_parsers.egg-info/SOURCES.txt` & `sd-parsers-0.2.3/src/sd_parsers.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,26 +16,24 @@
 src/sdparsers/__init__.py
 src/sdparsers/config.json
 src/sdparsers/parser.py
 src/sdparsers/parser_manager.py
 src/sdparsers/prompt_info.py
 src/sdparsers/parsers/__init__.py
 src/sdparsers/parsers/automatic1111.py
-src/sdparsers/parsers/automatic1111_stealth.py
 src/sdparsers/parsers/comfyui.py
 src/sdparsers/parsers/invokeai.py
 src/sdparsers/parsers/novelai.py
 tests/test_automatic1111.py
 tests/test_comfyui.py
 tests/test_invokeai.py
 tests/test_novelai.py
 tests/test_parser_manager.py
 tests/resources/automatic1111/automatic1111_cropped.jpg
 tests/resources/automatic1111/automatic1111_cropped.png
-tests/resources/automatic1111/automatic1111_stealth.png
 tests/resources/bad_images/empty_file.png
 tests/resources/bad_images/text_after_idat.png
 tests/resources/comfyui/img2img_cropped.png
 tests/resources/comfyui/night_evening_day_morning_cropped.png
 tests/resources/comfyui/noisy_latents_3_subjects_cropped.png
 tests/resources/comfyui/unclip_2pass_cropped.png
 tests/resources/invokeai/invokeai1_cropped.png
```

### Comparing `sd-parsers-0.2.2/src/sdparsers/config.json` & `sd-parsers-0.2.3/src/sdparsers/config.json`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/src/sdparsers/parser.py` & `sd-parsers-0.2.3/src/sdparsers/parser.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/src/sdparsers/parser_manager.py` & `sd-parsers-0.2.3/src/sdparsers/parser_manager.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/src/sdparsers/parsers/automatic1111.py` & `sd-parsers-0.2.3/src/sdparsers/parsers/automatic1111.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,45 +72,48 @@
 
 
 def split_parameters(parameters: str) -> Tuple[str, str, dict]:
     '''
     split an A1111 parameters string into prompt, negative prompt and metadata
     :exception ValueError: If the metadata does not conform to the expected format.
     '''
-    def split_meta(last_line: str) -> Iterable[Tuple[str, str]]:
-        for item in last_line.split(','):
-            try:
-                key, value = map(str.strip, item.split(':'))
-                yield key, value
-            except ValueError:
-                pass
-
     last_newline = parameters.rfind("\n")
     if last_newline == -1:
         raise ValueError("malformed parameters")
 
-    last_line, hashes = get_civitai_hashes(parameters[last_newline:])
-    metadata = dict(split_meta(last_line))
+    metadata = dict(split_meta(parameters[last_newline:]))
     if len(metadata) < 3:
         # actually a bit stricter than in the webui itself
         # grants some protection against "non-a1111" parameters
         raise ValueError("metadata too short")
 
     prompts = parameters[:last_newline].split('Negative prompt:')
     prompt, negative_prompt = prompts + ['']*(2-len(prompts))
-    if hashes:
-        metadata["hashes"] = hashes
 
     return (
         prompt.strip("\n "),
         negative_prompt.strip("\n "),
         metadata
     )
 
 
+def split_meta(last_line: str) -> Iterable[Tuple[str, str]]:
+    # extract civitai hashes
+    last_line, hashes = get_civitai_hashes(last_line)
+    if hashes:
+        yield 'hashes', hashes
+
+    for item in last_line.split(','):
+        try:
+            key, value = map(str.strip, item.split(':'))
+            yield key, value
+        except ValueError:
+            pass
+
+
 def get_civitai_hashes(line: str) -> Tuple[str, Optional[dict]]:
     hashes = None
     match = _RE_CIVITAI_HASHES.search(line)
     if match:
         hashes = json.loads(match.group(1))
         start, end = match.span(0)
         line = line[:start] + line[end:]
```

### Comparing `sd-parsers-0.2.2/src/sdparsers/parsers/comfyui.py` & `sd-parsers-0.2.3/src/sdparsers/parsers/comfyui.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,16 @@
         if self.traverse_limit != -1 and depth >= self.traverse_limit:
             return
         try:
             # test if the current node has prompt text
             node = image_data['prompt'][node_id]
             if not self.text_types or node['class_type'] in self.text_types:
                 for text_key in text_tags & set(node['inputs'].keys()):
-                    yield node['inputs'][text_key].strip()
+                    item = node['inputs'][text_key]
+                    if isinstance(item, str):
+                        yield item.strip()
         except KeyError:
             pass
 
         # explore other inputs fed into this node
         for output_id in image_data['links'].get(node_id, []):
             yield from self._get_parts(output_id, text_tags, depth + 1)
```

### Comparing `sd-parsers-0.2.2/src/sdparsers/parsers/invokeai.py` & `sd-parsers-0.2.3/src/sdparsers/parsers/invokeai.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/src/sdparsers/parsers/novelai.py` & `sd-parsers-0.2.3/src/sdparsers/parsers/novelai.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/src/sdparsers/prompt_info.py` & `sd-parsers-0.2.3/src/sdparsers/prompt_info.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/resources/automatic1111/automatic1111_cropped.jpg` & `sd-parsers-0.2.3/tests/resources/automatic1111/automatic1111_cropped.jpg`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/resources/bad_images/text_after_idat.png` & `sd-parsers-0.2.3/tests/resources/bad_images/text_after_idat.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/resources/comfyui/img2img_cropped.png` & `sd-parsers-0.2.3/tests/resources/comfyui/img2img_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/resources/comfyui/night_evening_day_morning_cropped.png` & `sd-parsers-0.2.3/tests/resources/comfyui/night_evening_day_morning_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/resources/comfyui/noisy_latents_3_subjects_cropped.png` & `sd-parsers-0.2.3/tests/resources/comfyui/noisy_latents_3_subjects_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/resources/comfyui/unclip_2pass_cropped.png` & `sd-parsers-0.2.3/tests/resources/comfyui/unclip_2pass_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/resources/invokeai/invokeai1_cropped.png` & `sd-parsers-0.2.3/tests/resources/invokeai/invokeai1_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/resources/novelai/novelai1_cropped.png` & `sd-parsers-0.2.3/tests/resources/novelai/novelai1_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/test_automatic1111.py` & `sd-parsers-0.2.3/tests/test_automatic1111.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import unittest
 
 from PIL import Image
 from tools import RESOURCE_PATH
 
 from sdparsers import Model, Prompt, PromptInfo, Sampler
-from sdparsers.parsers import (AUTOMATIC1111Parser, AUTOMATICStealthParser,
-                               automatic1111)
+from sdparsers.parsers import AUTOMATIC1111Parser, automatic1111
 
 IMAGES_FOLDER = RESOURCE_PATH / "automatic1111"
 OUTPUT = PromptInfo(
     generator='AUTOMATIC1111',
     prompts=[(
         Prompt(value='photo of a duck',
                parts=['photo of a duck'],
@@ -37,31 +36,22 @@
 class Automatic1111Tester(unittest.TestCase):
 
     def parse_image(self, filename: str, config=None):
         parser = AUTOMATIC1111Parser(config)
         with Image.open(IMAGES_FOLDER / filename) as image:
             return parser.parse(image)
 
-    def parse_stealth_image(self, filename: str, config=None):
-        parser = AUTOMATICStealthParser(config)
-        with Image.open(IMAGES_FOLDER / filename) as image:
-            return parser.parse(image)
-
     def test_parse_png(self):
         prompt_info = self.parse_image("automatic1111_cropped.png")
         self.assertEqual(prompt_info, OUTPUT)
 
     def test_parse_jpg(self):
         prompt_info = self.parse_image("automatic1111_cropped.jpg")
         self.assertEqual(prompt_info, OUTPUT)
 
-    def test_parse_stealth(self):
-        prompt_info = self.parse_stealth_image("automatic1111_stealth.png")
-        self.assertEqual(prompt_info, OUTPUT)
-
     def test_civitai_hashes(self):
         parameters = OUTPUT.raw_params['parameters'] \
             + ', Hashes: {"vae": "c6a580b13a", "model": "c0d1994c73"}'
 
         prompt, negative_prompt, metadata = automatic1111.split_parameters(parameters)
         self.assertEqual(prompt, "photo of a duck")
         self.assertEqual(negative_prompt, "monochrome")
```

### Comparing `sd-parsers-0.2.2/tests/test_comfyui.py` & `sd-parsers-0.2.3/tests/test_comfyui.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/test_invokeai.py` & `sd-parsers-0.2.3/tests/test_invokeai.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/test_novelai.py` & `sd-parsers-0.2.3/tests/test_novelai.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/test_parser_manager.py` & `sd-parsers-0.2.3/tests/test_parser_manager.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.2/tests/tools/crop_image.py` & `sd-parsers-0.2.3/tests/tools/crop_image.py`

 * *Files identical despite different names*

