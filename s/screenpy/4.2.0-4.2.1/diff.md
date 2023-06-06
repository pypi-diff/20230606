# Comparing `tmp/screenpy-4.2.0.tar.gz` & `tmp/screenpy-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenpy-4.2.0.tar", max compression
+gzip compressed data, was "screenpy-4.2.1.tar", max compression
```

## Comparing `screenpy-4.2.0.tar` & `screenpy-4.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1071 2023-06-02 03:55:36.644684 screenpy-4.2.0/LICENSE
--rw-r--r--   0        0        0     2688 2023-06-02 03:55:36.644684 screenpy-4.2.0/README.md
--rw-r--r--   0        0        0     3625 2023-06-02 03:55:36.644684 screenpy-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     2360 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/__init__.py
--rw-r--r--   0        0        0      955 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/__version__.py
--rw-r--r--   0        0        0     1903 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/__init__.py
--rw-r--r--   0        0        0     1049 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/attach_the_file.py
--rw-r--r--   0        0        0     1442 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/debug.py
--rw-r--r--   0        0        0     5733 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/eventually.py
--rw-r--r--   0        0        0     1353 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/log.py
--rw-r--r--   0        0        0     2597 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/make_note.py
--rw-r--r--   0        0        0     3144 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/pause.py
--rw-r--r--   0        0        0     2337 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/actions/see.py
--rw-r--r--   0        0        0     2246 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/actions/see_all_of.py
--rw-r--r--   0        0        0     2628 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/actions/see_any_of.py
--rw-r--r--   0        0        0     4477 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/actions/silently.py
--rw-r--r--   0        0        0     9622 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/actor.py
--rw-r--r--   0        0        0     3698 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/configuration.py
--rw-r--r--   0        0        0      863 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/directions.py
--rw-r--r--   0        0        0     1011 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/director.py
--rw-r--r--   0        0        0     1401 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/exceptions.py
--rw-r--r--   0        0        0     1415 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/given_when_then.py
--rw-r--r--   0        0        0      369 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/__init__.py
--rw-r--r--   0        0        0      293 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/gravitas.py
--rw-r--r--   0        0        0     9445 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/narrator.py
--rw-r--r--   0        0        0      278 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/stdout_adapter/__init__.py
--rw-r--r--   0        0        0      943 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/stdout_adapter/configuration.py
--rw-r--r--   0        0        0     4732 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/stdout_adapter/stdout_adapter.py
--rw-r--r--   0        0        0     3707 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/pacing.py
--rw-r--r--   0        0        0     4126 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/protocols.py
--rw-r--r--   0        0        0       39 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/py.typed
--rw-r--r--   0        0        0     2657 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/__init__.py
--rw-r--r--   0        0        0     3615 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/base_resolution.py
--rw-r--r--   0        0        0     1061 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_item_matching.py
--rw-r--r--   0        0        0     2375 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_the_entry.py
--rw-r--r--   0        0        0      830 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_the_item.py
--rw-r--r--   0        0        0      868 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_the_key.py
--rw-r--r--   0        0        0      745 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_the_text.py
--rw-r--r--   0        0        0      869 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_the_value.py
--rw-r--r--   0        0        0        0 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/custom_matchers/__init__.py
--rw-r--r--   0        0        0     2911 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/custom_matchers/is_in_bounds.py
--rw-r--r--   0        0        0     1796 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py
--rw-r--r--   0        0        0      777 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/ends_with.py
--rw-r--r--   0        0        0      870 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/has_length.py
--rw-r--r--   0        0        0      897 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_close_to.py
--rw-r--r--   0        0        0      613 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_empty.py
--rw-r--r--   0        0        0      730 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_equal_to.py
--rw-r--r--   0        0        0      772 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_greater_than.py
--rw-r--r--   0        0        0      872 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_greater_than_or_equal_to.py
--rw-r--r--   0        0        0     1677 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_in_range.py
--rw-r--r--   0        0        0      761 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_less_than.py
--rw-r--r--   0        0        0      845 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_less_than_or_equal_to.py
--rw-r--r--   0        0        0      961 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_not.py
--rw-r--r--   0        0        0      866 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/matches.py
--rw-r--r--   0        0        0      733 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/reads_exactly.py
--rw-r--r--   0        0        0      778 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/starts_with.py
--rw-r--r--   0        0        0     1890 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/speech_tools.py
--rw-r--r--   0        0        0     5439 1970-01-01 00:00:00.000000 screenpy-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 18:10:47.822678 screenpy-4.2.1/LICENSE
+-rw-r--r--   0        0        0     2688 2023-06-06 18:10:47.822678 screenpy-4.2.1/README.md
+-rw-r--r--   0        0        0     3625 2023-06-06 18:10:47.822678 screenpy-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2360 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/__init__.py
+-rw-r--r--   0        0        0      955 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/__version__.py
+-rw-r--r--   0        0        0     1903 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/__init__.py
+-rw-r--r--   0        0        0     1049 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/attach_the_file.py
+-rw-r--r--   0        0        0     1442 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/debug.py
+-rw-r--r--   0        0        0     5733 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/eventually.py
+-rw-r--r--   0        0        0     1353 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/log.py
+-rw-r--r--   0        0        0     2597 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/make_note.py
+-rw-r--r--   0        0        0     3144 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/pause.py
+-rw-r--r--   0        0        0     2337 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/see.py
+-rw-r--r--   0        0        0     2246 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/see_all_of.py
+-rw-r--r--   0        0        0     2628 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/see_any_of.py
+-rw-r--r--   0        0        0     4477 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actions/silently.py
+-rw-r--r--   0        0        0     9622 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/actor.py
+-rw-r--r--   0        0        0     3698 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/configuration.py
+-rw-r--r--   0        0        0      863 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/directions.py
+-rw-r--r--   0        0        0     1011 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/director.py
+-rw-r--r--   0        0        0     1401 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/exceptions.py
+-rw-r--r--   0        0        0     1415 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/given_when_then.py
+-rw-r--r--   0        0        0      369 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/narration/__init__.py
+-rw-r--r--   0        0        0      293 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/narration/gravitas.py
+-rw-r--r--   0        0        0     9445 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/narration/narrator.py
+-rw-r--r--   0        0        0      278 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/narration/stdout_adapter/__init__.py
+-rw-r--r--   0        0        0      943 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/narration/stdout_adapter/configuration.py
+-rw-r--r--   0        0        0     4732 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/narration/stdout_adapter/stdout_adapter.py
+-rw-r--r--   0        0        0     3707 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/pacing.py
+-rw-r--r--   0        0        0     4126 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/protocols.py
+-rw-r--r--   0        0        0       39 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/py.typed
+-rw-r--r--   0        0        0     2657 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/resolutions/__init__.py
+-rw-r--r--   0        0        0     3615 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/resolutions/base_resolution.py
+-rw-r--r--   0        0        0     1061 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/resolutions/contains_item_matching.py
+-rw-r--r--   0        0        0     2628 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/resolutions/contains_the_entry.py
+-rw-r--r--   0        0        0      830 2023-06-06 18:10:47.822678 screenpy-4.2.1/screenpy/resolutions/contains_the_item.py
+-rw-r--r--   0        0        0      864 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/contains_the_key.py
+-rw-r--r--   0        0        0      745 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/contains_the_text.py
+-rw-r--r--   0        0        0      869 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/contains_the_value.py
+-rw-r--r--   0        0        0        0 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/custom_matchers/__init__.py
+-rw-r--r--   0        0        0     2911 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/custom_matchers/is_in_bounds.py
+-rw-r--r--   0        0        0     1796 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py
+-rw-r--r--   0        0        0      778 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/ends_with.py
+-rw-r--r--   0        0        0      870 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/has_length.py
+-rw-r--r--   0        0        0      897 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/is_close_to.py
+-rw-r--r--   0        0        0      613 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/is_empty.py
+-rw-r--r--   0        0        0      730 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/is_equal_to.py
+-rw-r--r--   0        0        0      772 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/is_greater_than.py
+-rw-r--r--   0        0        0      872 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/is_greater_than_or_equal_to.py
+-rw-r--r--   0        0        0     1677 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/is_in_range.py
+-rw-r--r--   0        0        0      761 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/is_less_than.py
+-rw-r--r--   0        0        0      845 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/is_less_than_or_equal_to.py
+-rw-r--r--   0        0        0      961 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/is_not.py
+-rw-r--r--   0        0        0      866 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/matches.py
+-rw-r--r--   0        0        0      733 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/reads_exactly.py
+-rw-r--r--   0        0        0      778 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/resolutions/starts_with.py
+-rw-r--r--   0        0        0     1890 2023-06-06 18:10:47.826678 screenpy-4.2.1/screenpy/speech_tools.py
+-rw-r--r--   0        0        0     5439 1970-01-01 00:00:00.000000 screenpy-4.2.1/PKG-INFO
```

### Comparing `screenpy-4.2.0/LICENSE` & `screenpy-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/README.md` & `screenpy-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/pyproject.toml` & `screenpy-4.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Poetry:
 #   poetry install --extras dev
 # PIP:
 #   pip install -e .[dev]
 
 [tool.poetry]
 name = "screenpy"
-version = "4.2.0"
+version = "4.2.1"
 description = "Screenplay pattern base for Python automated test suites."
 authors = ["Perry Goy <perry.goy@gmail.com>"]
 maintainers = ["Gabe Langton", "Marcel Wilson"]
 license = "MIT"
 repository = "https://github.com/ScreenPyHQ/screenpy"
 documentation = "https://screenpy-docs.readthedocs.io"
 readme = "README.md"
```

### Comparing `screenpy-4.2.0/screenpy/__init__.py` & `screenpy-4.2.1/screenpy/__init__.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/__version__.py` & `screenpy-4.2.1/screenpy/__version__.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/__init__.py` & `screenpy-4.2.1/screenpy/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/attach_the_file.py` & `screenpy-4.2.1/screenpy/actions/attach_the_file.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/debug.py` & `screenpy-4.2.1/screenpy/actions/debug.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/eventually.py` & `screenpy-4.2.1/screenpy/actions/eventually.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/log.py` & `screenpy-4.2.1/screenpy/actions/log.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/make_note.py` & `screenpy-4.2.1/screenpy/actions/make_note.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/pause.py` & `screenpy-4.2.1/screenpy/actions/pause.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/see.py` & `screenpy-4.2.1/screenpy/actions/see.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/see_all_of.py` & `screenpy-4.2.1/screenpy/actions/see_all_of.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/see_any_of.py` & `screenpy-4.2.1/screenpy/actions/see_any_of.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actions/silently.py` & `screenpy-4.2.1/screenpy/actions/silently.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/actor.py` & `screenpy-4.2.1/screenpy/actor.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/configuration.py` & `screenpy-4.2.1/screenpy/configuration.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/directions.py` & `screenpy-4.2.1/screenpy/directions.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/director.py` & `screenpy-4.2.1/screenpy/director.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/exceptions.py` & `screenpy-4.2.1/screenpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/given_when_then.py` & `screenpy-4.2.1/screenpy/given_when_then.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/narration/narrator.py` & `screenpy-4.2.1/screenpy/narration/narrator.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/narration/stdout_adapter/configuration.py` & `screenpy-4.2.1/screenpy/narration/stdout_adapter/configuration.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/narration/stdout_adapter/stdout_adapter.py` & `screenpy-4.2.1/screenpy/narration/stdout_adapter/stdout_adapter.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/pacing.py` & `screenpy-4.2.1/screenpy/pacing.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/protocols.py` & `screenpy-4.2.1/screenpy/protocols.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/__init__.py` & `screenpy-4.2.1/screenpy/resolutions/__init__.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/base_resolution.py` & `screenpy-4.2.1/screenpy/resolutions/base_resolution.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/contains_item_matching.py` & `screenpy-4.2.1/screenpy/resolutions/contains_item_matching.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/contains_the_entry.py` & `screenpy-4.2.1/screenpy/resolutions/contains_the_entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,37 +6,43 @@
 
 from hamcrest import has_entries
 from hamcrest.core.matcher import Matcher
 
 from screenpy.exceptions import UnableToFormResolution
 from screenpy.pacing import beat
 
-from .base_resolution import BaseResolution
-
 K = TypeVar("K", bound=Hashable)
 V = TypeVar("V")
 
 
-class ContainsTheEntry(BaseResolution):
+class ContainsTheEntry:
     """Match a dictionary containing the specified key/value pair(s).
 
     Examples::
 
         the_actor.should(
             See.the(
                 HeadersOfTheLastResponse(), ContainTheEntry(Authorization="Bearer 1")
             )
         )
+
+        the_actor.should(
+            See.the(
+                EnglishDictionary(), ContainsTheEntry({"Python": "a large snake."})
+            )
+        )
+
+        the_actor.should(See.the(MathTestAnswers(), ContainsTheEntry("Problem3", 45)))
     """
 
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
-        return f"A mapping with the entries {self.entries_to_log}."
+        return f"A mapping with the {self.entry_plural} {self.entries_to_log}."
 
-    @beat("... hoping it's a mapping with the entries {entries_to_log}")
+    @beat("... hoping it's a mapping with the {entry_plural} {entries_to_log}")
     def resolve(self) -> Matcher[Mapping]:
         """Produce the Matcher to make the assertion."""
         return has_entries(**self.entries)
 
     # Keyword argument form
     @overload
     def __init__(self, **kv_args: V) -> None:
@@ -67,10 +73,9 @@
                 self.entries = dict(kv_args, **kv_kwargs)
             except ValueError:
                 # given a list of implicitly paired arguments
                 pairs: Iterable[Tuple[Any, Any]] = [
                     (kv_args[i], kv_args[i + 1]) for i in range(0, len(kv_args), 2)
                 ]
                 self.entries = dict(pairs, **kv_kwargs)
-        self.entries_to_log = ", ".join(
-            f"{{{k}: {v}}}" for k, v in self.entries.items()
-        )
+        self.entry_plural = "entries" if len(self.entries) != 1 else "entry"
+        self.entries_to_log = ", ".join(f"{k}->{v}" for k, v in self.entries.items())
```

### Comparing `screenpy-4.2.0/screenpy/resolutions/contains_the_item.py` & `screenpy-4.2.1/screenpy/resolutions/contains_the_item.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/contains_the_key.py` & `screenpy-4.2.1/screenpy/resolutions/is_greater_than.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 """
-Matches a dictionary that contains the desired key.
+Matches a value greater than the given number.
 """
 
-from typing import Any, Generic, Hashable, Mapping, TypeVar
+from typing import Any
 
-from hamcrest import has_key
+from hamcrest import greater_than
 from hamcrest.core.matcher import Matcher
 
 from screenpy.pacing import beat
 
-K = TypeVar("K", bound=Hashable)
 
-
-class ContainsTheKey(Generic[K]):
-    """Match a dictionary containing a specific key.
+class IsGreaterThan:
+    """Match on a number that is greater than the given number.
 
     Examples::
 
-        the_actor.should(See.the(LastResponseBody(), ContainsTheKey("skeleton")))
+        the_actor.should(See.the(Number.of(COUPONS), IsGreaterThan(1)))
     """
 
     def describe(self) -> str:
-        """Describe the Resolution in the present tense."""
-        return f'Contain the key "{self.key}".'
+        """Describe the Resolution's expectation."""
+        return f"Greater than {self.number}."
 
-    @beat('... hoping it\'s a dict containing the key "{key}".')
-    def resolve(self) -> Matcher[Mapping[K, Any]]:
+    @beat("... hoping it's greater than {number}.")
+    def resolve(self) -> Matcher[Any]:
         """Produce the Matcher to make the assertion."""
-        return has_key(self.key)
+        return greater_than(self.number)
 
-    def __init__(self, key: K) -> None:
-        self.key = key
+    def __init__(self, number: float) -> None:
+        self.number = number
```

### Comparing `screenpy-4.2.0/screenpy/resolutions/contains_the_text.py` & `screenpy-4.2.1/screenpy/resolutions/contains_the_text.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/contains_the_value.py` & `screenpy-4.2.1/screenpy/resolutions/contains_the_value.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/custom_matchers/is_in_bounds.py` & `screenpy-4.2.1/screenpy/resolutions/custom_matchers/is_in_bounds.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py` & `screenpy-4.2.1/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/ends_with.py` & `screenpy-4.2.1/screenpy/resolutions/ends_with.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         the_actor.should(
             See.the(Text.of_the(LOGIN_ERROR), EndsWith("username or password."))
         )
     """
 
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
-        return f'Ending with {self.postfix}".'
+        return f'Ending with "{self.postfix}".'
 
     @beat('... hoping it ends with "{postfix}".')
     def resolve(self) -> Matcher[str]:
         """Produce the Matcher to make the assertion."""
         return ends_with(self.postfix)
 
     def __init__(self, postfix: str) -> None:
```

### Comparing `screenpy-4.2.0/screenpy/resolutions/has_length.py` & `screenpy-4.2.1/screenpy/resolutions/has_length.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/is_close_to.py` & `screenpy-4.2.1/screenpy/resolutions/is_close_to.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/is_empty.py` & `screenpy-4.2.1/screenpy/resolutions/is_empty.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/is_equal_to.py` & `screenpy-4.2.1/screenpy/resolutions/is_equal_to.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/is_greater_than.py` & `screenpy-4.2.1/screenpy/resolutions/is_less_than_or_equal_to.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
-Matches a value greater than the given number.
+Matches a value less than or equal to the given number.
 """
 
-from typing import Any
-
-from hamcrest import greater_than
+from hamcrest import less_than_or_equal_to
 from hamcrest.core.matcher import Matcher
 
 from screenpy.pacing import beat
 
 
-class IsGreaterThan:
-    """Match on a number that is greater than the given number.
+class IsLessThanOrEqualTo:
+    """Match on a number that is less than or equal to the given number.
 
     Examples::
 
-        the_actor.should(See.the(Number.of(COUPONS), IsGreaterThan(1)))
+        the_actor.should(
+            See.the(Number.of(VOUCHER_INPUTS), IsLessThanOrEqualTo(1))
+        )
     """
 
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
-        return f"Greater than {self.number}."
+        return f"Less than or equal to {self.number}."
 
-    @beat("... hoping it's greater than {number}.")
-    def resolve(self) -> Matcher[Any]:
+    @beat("... hoping it's less than or equal to {number}.")
+    def resolve(self) -> Matcher[float]:
         """Produce the Matcher to make the assertion."""
-        return greater_than(self.number)
+        return less_than_or_equal_to(self.number)
 
     def __init__(self, number: float) -> None:
         self.number = number
```

### Comparing `screenpy-4.2.0/screenpy/resolutions/is_greater_than_or_equal_to.py` & `screenpy-4.2.1/screenpy/resolutions/is_greater_than_or_equal_to.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/is_in_range.py` & `screenpy-4.2.1/screenpy/resolutions/is_in_range.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/is_less_than.py` & `screenpy-4.2.1/screenpy/resolutions/is_less_than.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/is_not.py` & `screenpy-4.2.1/screenpy/resolutions/is_not.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/matches.py` & `screenpy-4.2.1/screenpy/resolutions/matches.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/reads_exactly.py` & `screenpy-4.2.1/screenpy/resolutions/reads_exactly.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/resolutions/starts_with.py` & `screenpy-4.2.1/screenpy/resolutions/starts_with.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/screenpy/speech_tools.py` & `screenpy-4.2.1/screenpy/speech_tools.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.0/PKG-INFO` & `screenpy-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenpy
-Version: 4.2.0
+Version: 4.2.1
 Summary: Screenplay pattern base for Python automated test suites.
 Home-page: https://github.com/ScreenPyHQ/screenpy
 License: MIT
 Author: Perry Goy
 Author-email: perry.goy@gmail.com
 Maintainer: Gabe Langton
 Requires-Python: >=3.8,<4.0
```

