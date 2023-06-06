# Comparing `tmp/gtfs_kit-5.2.6.tar.gz` & `tmp/gtfs_kit-5.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtfs_kit-5.2.6.tar", max compression
+gzip compressed data, was "gtfs_kit-5.2.7.tar", max compression
```

## Comparing `gtfs_kit-5.2.6.tar` & `gtfs_kit-5.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2020-01-09 20:55:35.590106 gtfs_kit-5.2.6/LICENSE.txt
--rw-r--r--   0        0        0     1937 2023-04-27 00:05:00.839952 gtfs_kit-5.2.6/README.rst
--rw-r--r--   0        0        0      304 2023-05-30 02:41:39.895479 gtfs_kit-5.2.6/gtfs_kit/__init__.py
--rw-r--r--   0        0        0     3426 2021-04-28 23:42:59.436692 gtfs_kit-5.2.6/gtfs_kit/calendar.py
--rw-r--r--   0        0        0    10692 2022-04-12 04:10:10.474482 gtfs_kit-5.2.6/gtfs_kit/cleaners.py
--rw-r--r--   0        0        0     6971 2022-01-17 03:01:47.667252 gtfs_kit-5.2.6/gtfs_kit/constants.py
--rw-r--r--   0        0        0    16515 2022-04-13 02:04:39.526021 gtfs_kit-5.2.6/gtfs_kit/feed.py
--rw-r--r--   0        0        0    19581 2021-11-25 21:52:10.388179 gtfs_kit-5.2.6/gtfs_kit/helpers.py
--rw-r--r--   0        0        0    35644 2023-04-27 00:05:00.843952 gtfs_kit-5.2.6/gtfs_kit/miscellany.py
--rw-r--r--   0        0        0    30517 2023-05-30 02:41:39.895479 gtfs_kit-5.2.6/gtfs_kit/routes.py
--rw-r--r--   0        0        0     6648 2022-07-05 02:59:12.080231 gtfs_kit-5.2.6/gtfs_kit/shapes.py
--rw-r--r--   0        0        0     6231 2022-04-13 02:04:39.526021 gtfs_kit-5.2.6/gtfs_kit/stop_times.py
--rw-r--r--   0        0        0    24935 2022-04-26 01:06:51.650776 gtfs_kit-5.2.6/gtfs_kit/stops.py
--rw-r--r--   0        0        0    21337 2021-11-25 21:52:10.392179 gtfs_kit-5.2.6/gtfs_kit/trips.py
--rw-r--r--   0        0        0    49077 2022-04-26 21:35:43.321257 gtfs_kit-5.2.6/gtfs_kit/validators.py
--rw-r--r--   0        0        0     1097 2023-05-30 02:41:39.899479 gtfs_kit-5.2.6/pyproject.toml
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 gtfs_kit-5.2.6/setup.py
--rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 gtfs_kit-5.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-22 02:01:30.167750 gtfs_kit-5.2.7/LICENSE.txt
+-rw-r--r--   0        0        0     1937 2023-03-22 02:57:07.660723 gtfs_kit-5.2.7/README.rst
+-rw-r--r--   0        0        0      304 2023-06-06 00:32:33.259560 gtfs_kit-5.2.7/gtfs_kit/__init__.py
+-rw-r--r--   0        0        0     3426 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/calendar.py
+-rw-r--r--   0        0        0    10692 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/cleaners.py
+-rw-r--r--   0        0        0     6971 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/constants.py
+-rw-r--r--   0        0        0    16515 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/feed.py
+-rw-r--r--   0        0        0    20051 2023-06-06 00:32:33.259560 gtfs_kit-5.2.7/gtfs_kit/helpers.py
+-rw-r--r--   0        0        0    35644 2023-04-26 03:24:57.537534 gtfs_kit-5.2.7/gtfs_kit/miscellany.py
+-rw-r--r--   0        0        0    30517 2023-06-05 22:22:06.252172 gtfs_kit-5.2.7/gtfs_kit/routes.py
+-rw-r--r--   0        0        0     6648 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/shapes.py
+-rw-r--r--   0        0        0     6231 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/stop_times.py
+-rw-r--r--   0        0        0    24935 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/stops.py
+-rw-r--r--   0        0        0    21337 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/trips.py
+-rw-r--r--   0        0        0    49077 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/validators.py
+-rw-r--r--   0        0        0     1097 2023-06-06 00:32:33.259560 gtfs_kit-5.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 gtfs_kit-5.2.7/setup.py
+-rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 gtfs_kit-5.2.7/PKG-INFO
```

### Comparing `gtfs_kit-5.2.6/LICENSE.txt` & `gtfs_kit-5.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/README.rst` & `gtfs_kit-5.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/calendar.py` & `gtfs_kit-5.2.7/gtfs_kit/calendar.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/cleaners.py` & `gtfs_kit-5.2.7/gtfs_kit/cleaners.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/constants.py` & `gtfs_kit-5.2.7/gtfs_kit/constants.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/feed.py` & `gtfs_kit-5.2.7/gtfs_kit/feed.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/helpers.py` & `gtfs_kit-5.2.7/gtfs_kit/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,39 +52,39 @@
     """
     if not inverse:
         try:
             hours, mins, seconds = x.split(":")
             result = int(hours) * 3600 + int(mins) * 60 + int(seconds)
             if mod24:
                 result %= 24 * 3600
-        except:
+        except Exception:
             result = np.nan
     else:
         try:
             seconds = int(x)
             if mod24:
                 seconds %= 24 * 3600
             hours, remainder = divmod(seconds, 3600)
             mins, secs = divmod(remainder, 60)
             result = f"{hours:02d}:{mins:02d}:{secs:02d}"
-        except:
+        except Exception:
             result = np.nan
     return result
 
 
 def timestr_mod24(timestr: str) -> int:
     """
     Given a GTFS HH:MM:SS time string, return a timestring in the same
     format but with the hours taken modulo 24.
     """
     try:
         hours, mins, secs = [int(x) for x in timestr.split(":")]
         hours %= 24
         result = f"{hours:02d}:{mins:02d}:{secs:02d}"
-    except:
+    except Exception:
         result = None
     return result
 
 
 def weekday_to_str(
     weekday: Union[int, str], *, inverse: bool = False
 ) -> Union[int, str]:
@@ -94,20 +94,20 @@
     Here 0 -> 'monday', 1 -> 'tuesday', and so on.
     If ``inverse``, then perform the inverse operation.
     """
     s = ["monday", "tuesday", "wednesday", "thursday", "friday", "saturday", "sunday"]
     if not inverse:
         try:
             return s[weekday]
-        except:
+        except Exception:
             return
     else:
         try:
             return s.index(weekday)
-        except:
+        except Exception:
             return
 
 
 def get_segment_length(
     linestring: sg.LineString, p: sg.Point, q: Optional[sg.Point] = None
 ) -> float:
     """
@@ -163,22 +163,40 @@
     """
     Given an increasing list of times as seconds past midnight and a
     list of trip counts at those respective times,
     return a pair of indices i, j such that times[i] to times[j] is
     the first longest time period such that for all i <= x < j,
     counts[x] is the max of counts.
     Assume times and counts have the same nonzero length.
+
+    Examples::
+
+        >>> times = [0, 10, 20, 30, 31, 32, 40]
+        >>> counts = [7, 1, 2, 7, 7, 1, 2]
+        >>> get_peak_indices(times, counts)
+        array([0, 1])
+
+        >>> counts = [0, 0, 0]
+        >>> times = [18000, 21600, 28800]
+        >>> get_peak_indices(times, counts)
+        array([0, 3])
+
     """
     max_runs = get_max_runs(counts)
 
     def get_duration(a):
         return times[a[1]] - times[a[0]]
 
-    index = np.argmax(np.apply_along_axis(get_duration, 1, max_runs))
-    return max_runs[index]
+    if len(max_runs) == 1:
+        result = max_runs[0]
+    else:
+        index = np.argmax(np.apply_along_axis(get_duration, 1, max_runs))
+        result = max_runs[index]
+
+    return result
 
 
 def is_metric(dist_units: str) -> bool:
     """
     Return True if the given distance units equals 'm' or 'km';
     otherwise return False.
     """
@@ -573,15 +591,15 @@
 
     for i in range(1, len(seq)):
         # seq[i] can extend a subsequence that ends with a lesser (or equal) element
         j = bisect([rank[k] for k in lastoflength], rank[i])
         # update existing subsequence of length j or extend the longest
         try:
             lastoflength[j] = i
-        except:
+        except Exception:
             lastoflength.append(i)
         # remember element before seq[i] in the subsequence
         predecessor.append(lastoflength[j - 1] if j > 0 else None)
 
     # trace indices [p^n(i), ..., p(p(i)), p(i), i], where n=len(lastoflength)-1
     def trace(i):
         if i is not None:
```

### Comparing `gtfs_kit-5.2.6/gtfs_kit/miscellany.py` & `gtfs_kit-5.2.7/gtfs_kit/miscellany.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/routes.py` & `gtfs_kit-5.2.7/gtfs_kit/routes.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/shapes.py` & `gtfs_kit-5.2.7/gtfs_kit/shapes.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/stop_times.py` & `gtfs_kit-5.2.7/gtfs_kit/stop_times.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/stops.py` & `gtfs_kit-5.2.7/gtfs_kit/stops.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/trips.py` & `gtfs_kit-5.2.7/gtfs_kit/trips.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/gtfs_kit/validators.py` & `gtfs_kit-5.2.7/gtfs_kit/validators.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.6/pyproject.toml` & `gtfs_kit-5.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gtfs_kit"
-version = "5.2.6"
+version = "5.2.7"
 description = "A Python 3.8+ library for analyzing GTFS feeds."
 authors = ["Alex Raichev <araichev@mrcagney.com>"]
 readme = "README.rst"
 license = "MIT"
 repository = "https://github.com/mrcagney/gtfs_kit"
 documentation = "https://mrcagney.github.io/gtfs_kit_docs"
 exclude = ["tests", "docs"]
```

### Comparing `gtfs_kit-5.2.6/setup.py` & `gtfs_kit-5.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'requests>=2',
  'rtree>=0',
  'shapely>=1.8',
  'utm>=0.6']
 
 setup_kwargs = {
     'name': 'gtfs-kit',
-    'version': '5.2.6',
+    'version': '5.2.7',
     'description': 'A Python 3.8+ library for analyzing GTFS feeds.',
     'long_description': "GTFS Kit\n********\n.. image:: https://github.com/mrcagney/gtfs_kit/actions/workflows/test.yml/badge.svg\n\nGTFS Kit is a Python 3.8+ library for analyzing `General Transit Feed Specification (GTFS) <https://en.wikipedia.org/wiki/GTFS>`_ data in memory without a database.\nIt uses Pandas and Shapely to do the heavy lifting.\n\n\nInstallation\n=============\n``poetry add gtfs_kit``.\n\n\nExamples\n========\nYou can find examples in the Jupyter notebook ``notebooks/examples.ipynb``.\n\n\nAuthors\n=========\n- Alex Raichev (2019-09), maintainer\n\n\nDocumentation\n=============\nDocumentation is built via Sphinx from the source code in the ``docs`` directory then published to Github Pages at `mrcagney.github.io/gtfs_kit_docs <https://mrcagney.github.io/gtfs_kit_docs>`_.\n\n\nNotes\n=====\n- This project's development status is Alpha.\n  I use GTFS Kit for work and change it breakingly to suit my needs.\n- This project uses semantic versioning.\n- I aim for GTFS Kit to handle `the current GTFS <https://developers.google.com/transit/gtfs/reference>`_.\n  In particular, i avoid handling `GTFS extensions <https://developers.google.com/transit/gtfs/reference/gtfs-extensions>`_.\n  That is the most reasonable scope boundary i can draw at present, given this project's tiny budget.\n  If you would like to fund me to expand that scope, feel free to email me.\n- Thanks to `MRCagney <http://www.mrcagney.com/>`_ for periodically donating to this project.\n- Constructive feedback and contributions are welcome.\n  Please issue pull requests from a feature branch into the ``develop`` branch and include tests.\n- GTFS time is measured relative noon minus 12 hours, which can mess things up when crossing into daylight savings time.\n  I don't think this issue causes any bugs in GTFS Kit, but you and i have been warned.\n  Thanks to user derhuerst for bringing this to my attention in `closed Issue 8 <https://github.com/mrcagney/gtfs_kit/issues/8#issue-1063633457>`_.\n",
     'author': 'Alex Raichev',
     'author_email': 'araichev@mrcagney.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mrcagney/gtfs_kit',
```

### Comparing `gtfs_kit-5.2.6/PKG-INFO` & `gtfs_kit-5.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtfs-kit
-Version: 5.2.6
+Version: 5.2.7
 Summary: A Python 3.8+ library for analyzing GTFS feeds.
 Home-page: https://github.com/mrcagney/gtfs_kit
 License: MIT
 Author: Alex Raichev
 Author-email: araichev@mrcagney.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
```

