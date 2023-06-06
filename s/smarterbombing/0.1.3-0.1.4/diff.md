# Comparing `tmp/smarterbombing-0.1.3.tar.gz` & `tmp/smarterbombing-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarterbombing-0.1.3.tar", max compression
+gzip compressed data, was "smarterbombing-0.1.4.tar", max compression
```

## Comparing `smarterbombing-0.1.3.tar` & `smarterbombing-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/LICENSE
--rw-r--r--   0        0        0      684 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/README.md
--rw-r--r--   0        0        0      860 2023-06-06 15:42:53.154736 smarterbombing-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      116 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/__init__.py
--rw-r--r--   0        0        0      769 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/__main__.py
--rw-r--r--   0        0        0    10681 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/analysis.py
--rw-r--r--   0        0        0     5497 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/app_live.py
--rw-r--r--   0        0        0     2979 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/app_offline.py
--rw-r--r--   0        0        0      817 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/configuration.py
--rw-r--r--   0        0        0     3698 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/log_reader.py
--rw-r--r--   0        0        0     3533 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/logs.py
--rw-r--r--   0        0        0        0 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/webui/__init__.py
--rw-r--r--   0        0        0     1104 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/webui/ui.py
--rw-r--r--   0        0        0     1837 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/webui/ui_configuration.py
--rw-r--r--   0        0        0     5546 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/webui/ui_live.py
--rw-r--r--   0        0        0     4199 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/webui/ui_offline_analysis.py
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 smarterbombing-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/LICENSE
+-rw-r--r--   0        0        0      684 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/README.md
+-rw-r--r--   0        0        0      860 2023-06-06 15:53:37.348858 smarterbombing-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/__init__.py
+-rw-r--r--   0        0        0      769 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/__main__.py
+-rw-r--r--   0        0        0    10637 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/analysis.py
+-rw-r--r--   0        0        0     5473 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/app_live.py
+-rw-r--r--   0        0        0     2979 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/app_offline.py
+-rw-r--r--   0        0        0      817 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/configuration.py
+-rw-r--r--   0        0        0     3648 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/log_reader.py
+-rw-r--r--   0        0        0     3533 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/logs.py
+-rw-r--r--   0        0        0        0 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/webui/__init__.py
+-rw-r--r--   0        0        0     1104 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/webui/ui.py
+-rw-r--r--   0        0        0     1837 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/webui/ui_configuration.py
+-rw-r--r--   0        0        0     5546 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/webui/ui_live.py
+-rw-r--r--   0        0        0     4199 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/webui/ui_offline_analysis.py
+-rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 smarterbombing-0.1.4/PKG-INFO
```

### Comparing `smarterbombing-0.1.3/LICENSE` & `smarterbombing-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.3/README.md` & `smarterbombing-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.3/pyproject.toml` & `smarterbombing-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smarterbombing"
-version = "0.1.3"
+version = "0.1.4"
 description = "A tool which reads combat logs from Eve Online and displays statistics."
 repository = "https://github.com/agelito/eve-smarterbombing"
 authors = ["Axel Wettervik <axel.wettervik@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `smarterbombing-0.1.3/src/smarterbombing/__main__.py` & `smarterbombing-0.1.4/src/smarterbombing/__main__.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.3/src/smarterbombing/analysis.py` & `smarterbombing-0.1.4/src/smarterbombing/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 EVENT_GROUP_INCOMING_HOSTILE_DAMAGE='incoming_hostile_damage'
 EVENT_GROUP_INCOMING_FRIENDLY_DAMAGE='incoming_friendly_damage'
 
 def _filter_by_direction(events: pd.DataFrame, direction: str):
     filter_outgoing = events['direction'].isin([direction])
     return events[filter_outgoing]
 
-def _filter_unfriendly_damage(events: pd.DataFrame, characters: list[str]):
+def _filter_unfriendly_damage(events: pd.DataFrame, characters):
     filter_friendly = events['subject'].isin(characters)
     return events[~filter_friendly]
 
-def _filter_friendly_damage(events: pd.DataFrame, characters: list[str]):
+def _filter_friendly_damage(events: pd.DataFrame, characters):
     filter_friendly = events['subject'].isin(characters)
     return events[filter_friendly]
 
 def _group_by_delta_time(events: pd.DataFrame, max_gap_seconds: float):
     events['delta'] = events['timestamp'].diff() > timedelta(seconds=max_gap_seconds)
 
     groups = []
     for _, group in events.groupby([events['delta'].cumsum()]):
         groups.append(group)
 
     return groups
 
-def group_damage_events(events: pd.DataFrame, characters: list[str]):
+def group_damage_events(events: pd.DataFrame, characters):
     """Sort combat events by type and direction"""
     outgoing_damage = _filter_by_direction(events, 'to')
     outgoing_damage_to_friendly = _filter_friendly_damage(outgoing_damage, characters)
     outgoing_damage_to_hostile = _filter_unfriendly_damage(outgoing_damage, characters)
 
     incoming_damage = _filter_by_direction(events, 'from')
     incoming_damage_from_friendly = _filter_friendly_damage(incoming_damage, characters)
@@ -129,15 +129,15 @@
     data = data.resample('1S').asfreq(fill_value=0.0)
 
     if average_seconds > 0:
         data = data.rolling(timedelta(seconds=average_seconds)).mean()
 
     return data
 
-def site_statistics(data: pd.DataFrame, characters: list[str], minimum_gap_seconds: int = 30) -> pd.DataFrame:
+def site_statistics(data: pd.DataFrame, characters, minimum_gap_seconds: int = 30) -> pd.DataFrame:
     """Calculate site based time statistics"""
     data = _filter_by_direction(data, 'to')
     data = data.sort_values(by='timestamp')
     data = data.reset_index()
 
     # Calculate event deltas
     data['delta_time'] = data['timestamp'].diff()
```

### Comparing `smarterbombing-0.1.3/src/smarterbombing/app_live.py` & `smarterbombing-0.1.4/src/smarterbombing/app_live.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class AppLive:
     """Live application"""
     def __init__(self, configuration):
         self.configuration = configuration
         self.current_time = datetime.now(timezone.utc)
 
-        self.logs: list[CharacterLogFile] = []
+        self.logs = []
 
         self.data = pd.DataFrame([])
         self.outgoing_hostile_damage = create_empty_damage_dataframe()
         self.outgoing_friendly_damage = create_empty_damage_dataframe()
         self.incoming_hostile_damage = create_empty_damage_dataframe()
         self.incoming_friendly_damage = create_empty_damage_dataframe()
```

### Comparing `smarterbombing-0.1.3/src/smarterbombing/app_offline.py` & `smarterbombing-0.1.4/src/smarterbombing/app_offline.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.3/src/smarterbombing/configuration.py` & `smarterbombing-0.1.4/src/smarterbombing/configuration.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.3/src/smarterbombing/log_reader.py` & `smarterbombing-0.1.4/src/smarterbombing/log_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,28 +84,28 @@
             parsed_lines.append(parsed)
 
     return parsed_lines
 
 def _flatten(in_list):
     return [item for ll in in_list for item in ll]
 
-def read_all_combat_log_entries(character_files: list[CharacterLogFile]):
+def read_all_combat_log_entries(character_files):
     """Read all combat log entries from character log files"""
     if len(character_files) == 0:
         return []
 
     character_log_entries = map(_read_and_parse_combat_log_lines, character_files)
 
     return _flatten(character_log_entries)
 
 def open_log_files(
         character_logs,
         filter_characters,
         seek_to_end: bool = False
-    ) -> list[CharacterLogFile]:
+    ):
     """Open character log files"""
     character_files = []
     for character_log in character_logs:
         name = character_log['character_name']
         path = character_log['path']
 
         if name not in filter_characters:
```

### Comparing `smarterbombing-0.1.3/src/smarterbombing/logs.py` & `smarterbombing-0.1.4/src/smarterbombing/logs.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.3/src/smarterbombing/webui/ui.py` & `smarterbombing-0.1.4/src/smarterbombing/webui/ui.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.3/src/smarterbombing/webui/ui_configuration.py` & `smarterbombing-0.1.4/src/smarterbombing/webui/ui_configuration.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.3/src/smarterbombing/webui/ui_live.py` & `smarterbombing-0.1.4/src/smarterbombing/webui/ui_live.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.3/src/smarterbombing/webui/ui_offline_analysis.py` & `smarterbombing-0.1.4/src/smarterbombing/webui/ui_offline_analysis.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.3/PKG-INFO` & `smarterbombing-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarterbombing
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool which reads combat logs from Eve Online and displays statistics.
 Home-page: https://github.com/agelito/eve-smarterbombing
 License: MIT
 Author: Axel Wettervik
 Author-email: axel.wettervik@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

