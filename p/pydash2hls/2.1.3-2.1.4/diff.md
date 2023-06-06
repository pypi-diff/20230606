# Comparing `tmp/pydash2hls-2.1.3.tar.gz` & `tmp/pydash2hls-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash2hls-2.1.3.tar", last modified: Mon Jun  5 17:21:50 2023, max compression
+gzip compressed data, was "pydash2hls-2.1.4.tar", last modified: Tue Jun  6 18:37:39 2023, max compression
```

## Comparing `pydash2hls-2.1.3.tar` & `pydash2hls-2.1.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:21:50.440164 pydash2hls-2.1.3/
--rw-rw-rw-   0        0        0    35823 2023-06-05 16:27:43.000000 pydash2hls-2.1.3/LICENSE
--rw-rw-rw-   0        0        0     3385 2023-06-05 17:21:50.439171 pydash2hls-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2459 2023-06-05 16:27:43.000000 pydash2hls-2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 17:21:50.421283 pydash2hls-2.1.3/pydash2hls/
--rw-rw-rw-   0        0        0       51 2023-06-05 17:18:03.000000 pydash2hls-2.1.3/pydash2hls/__init__.py
--rw-rw-rw-   0        0        0     7397 2023-06-05 17:16:44.000000 pydash2hls-2.1.3/pydash2hls/converter.py
--rw-rw-rw-   0        0        0      469 2023-06-05 16:27:43.000000 pydash2hls-2.1.3/pydash2hls/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:21:50.439171 pydash2hls-2.1.3/pydash2hls.egg-info/
--rw-rw-rw-   0        0        0     3385 2023-06-05 17:21:50.000000 pydash2hls-2.1.3/pydash2hls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-05 17:21:50.000000 pydash2hls-2.1.3/pydash2hls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:21:50.000000 pydash2hls-2.1.3/pydash2hls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-05 17:21:50.000000 pydash2hls-2.1.3/pydash2hls.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 17:21:50.000000 pydash2hls-2.1.3/pydash2hls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 17:21:50.440164 pydash2hls-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-06-05 17:18:03.000000 pydash2hls-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:37:39.335865 pydash2hls-2.1.4/
+-rw-rw-rw-   0        0        0    35823 2023-06-06 11:16:08.000000 pydash2hls-2.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3389 2023-06-06 18:37:39.335865 pydash2hls-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2463 2023-06-06 11:16:08.000000 pydash2hls-2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 18:37:39.303737 pydash2hls-2.1.4/pydash2hls/
+-rw-rw-rw-   0        0        0       59 2023-06-06 18:22:52.000000 pydash2hls-2.1.4/pydash2hls/__init__.py
+-rw-rw-rw-   0        0        0    11315 2023-06-06 18:21:39.000000 pydash2hls-2.1.4/pydash2hls/converter.py
+-rw-rw-rw-   0        0        0      469 2023-06-06 11:16:08.000000 pydash2hls-2.1.4/pydash2hls/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:37:39.335865 pydash2hls-2.1.4/pydash2hls.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-06-06 18:37:39.000000 pydash2hls-2.1.4/pydash2hls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-06 18:37:39.000000 pydash2hls-2.1.4/pydash2hls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 18:37:39.000000 pydash2hls-2.1.4/pydash2hls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-06 18:37:39.000000 pydash2hls-2.1.4/pydash2hls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 18:37:39.000000 pydash2hls-2.1.4/pydash2hls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 18:37:39.335865 pydash2hls-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-06-06 17:59:10.000000 pydash2hls-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:37:39.335865 pydash2hls-2.1.4/test/
+-rw-rw-rw-   0        0        0      865 2023-06-06 18:20:13.000000 pydash2hls-2.1.4/test/test.py
```

### Comparing `pydash2hls-2.1.3/LICENSE` & `pydash2hls-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydash2hls-2.1.3/PKG-INFO` & `pydash2hls-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash2hls
-Version: 2.1.3
+Version: 2.1.4
 Summary: Python library for converting DASH manifest files to HLS format.
 Home-page: https://github.com/hyugogirubato/pydash2hls
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: manifest,hls,m3u8,dash
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,18 +29,18 @@
 [![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls/)
 
 PyDash2HLS is a Python library for converting DASH (Dynamic Adaptive Streaming over HTTP) manifest files to HLS (HTTP
 Live Streaming) format.
 
 ## Features
 
-- Convert MPD files to HLS format
-- Support for remote and local MPD files
-- Retrieve media URLs for a specific profile
-- Handle DRM (Digital Rights Management) information in MPD files
+- Convert MPD files to HLS format.
+- Support for remote and local MPD files.
+- Retrieve media URLs for a specific profile.
+- Handle DRM (Digital Rights Management) information in MPD files.
 
 ## Installation
 
 You can install PyDash2HLS using pip:
 
 ````shell
 pip install pydash2hls
```

### Comparing `pydash2hls-2.1.3/README.md` & `pydash2hls-2.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 [![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls/)
 
 PyDash2HLS is a Python library for converting DASH (Dynamic Adaptive Streaming over HTTP) manifest files to HLS (HTTP
 Live Streaming) format.
 
 ## Features
 
-- Convert MPD files to HLS format
-- Support for remote and local MPD files
-- Retrieve media URLs for a specific profile
-- Handle DRM (Digital Rights Management) information in MPD files
+- Convert MPD files to HLS format.
+- Support for remote and local MPD files.
+- Retrieve media URLs for a specific profile.
+- Handle DRM (Digital Rights Management) information in MPD files.
 
 ## Installation
 
 You can install PyDash2HLS using pip:
 
 ````shell
 pip install pydash2hls
```

### Comparing `pydash2hls-2.1.3/pydash2hls/converter.py` & `pydash2hls-2.1.4/pydash2hls/converter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import base64
 from pathlib import Path
+from typing import Optional
 
 import requests
 import xmltodict
 
 from pydash2hls.exceptions import InvalidFileContent, InvalidPath, InvalidProfile, MissingRemoteUrl
 
 
@@ -27,15 +29,16 @@
 
 class Converter:
 
     def __init__(self, mdp_srt: str, mdp_dict: dict, url: str = None):
         self.mdp_srt = mdp_srt
         self.mdp_dict = mdp_dict
         self.mdp_url = url
-        self.profiles = self._manifest_profiles()
+        self.profiles = []
+        self._manifest_profiles()
 
     @classmethod
     def from_remote(cls, url: str, **kwargs) -> Converter:
         r = requests.request(method=kwargs.get("method", "GET"), url=url, **kwargs)
         r.raise_for_status()
         mdp_srt = r.text
         try:
@@ -61,23 +64,40 @@
 
     def _get_profile(self, profile_id: str) -> dict:
         for profile in self.profiles:
             if profile["id"] == profile_id:
                 return profile
         raise InvalidProfile(f"Profile does not exist: {profile_id}")
 
-    def _manifest_profiles(self) -> list:
+    def _existing_profile(self, profile_id: str) -> Optional[int]:
+        for i, profile in enumerate(self.profiles):
+            if profile["id"] == profile_id:
+                return i
+        return None
+
+    def _manifest_profiles(self) -> None:
         source = None if self.mdp_url is None else "/".join(self.mdp_url.split("/")[:-1])
-        profiles = []
 
-        for adaptation in self.mdp_dict["MPD"]["Period"]["AdaptationSet"]:
-            if isinstance(adaptation["Representation"], list):
-                for representation in adaptation["Representation"]:
+        # Period
+        periods = self.mdp_dict["MPD"]["Period"]
+        periods = periods if isinstance(periods, list) else [periods]
+
+        for i, period in enumerate(periods):
+            for adaptation in period["AdaptationSet"]:
+
+                # Representations
+                representations = adaptation["Representation"]
+                representations = representations if isinstance(representations, list) else [representations]
+
+                for representation in representations:
                     mime_type = self._get_key(adaptation, representation, "@mimeType") or ("video/mp4" if "avc" in representation["@codecs"] else "audio/m4a")
                     start_with_sap = self._get_key(adaptation, representation, "@startWithSAP") or "1"
+                    if "video" not in mime_type and "audio" not in mime_type:
+                        continue
+
                     profile = {
                         "id": representation["@id"],
                         "mimeType": mime_type,
                         "codecs": representation["@codecs"],
                         "bandwidth": int(representation["@bandwidth"]),
                         "startWithSAP": start_with_sap
                     }
@@ -87,73 +107,134 @@
                         profile["width"] = int(representation["@width"])
                         profile["height"] = int(representation["@height"])
                         frame_rate = representation.get("@frameRate") or adaptation.get("@maxFrameRate") or "1/1"
                         frame_rate = frame_rate if "/" in frame_rate else f"{frame_rate}/1"
                         profile["frameRate"] = round(int(frame_rate.split("/")[0]) / int(frame_rate.split("/")[1]), 3)
                         profile["sar"] = representation.get("@sar", "1:1")
 
+                    # DRM
                     drm = _get_drm(adaptation)
                     item = adaptation.get("SegmentTemplate")
                     if not item:
                         item = representation.get("SegmentTemplate")
                         drm = _get_drm(representation)
 
-                    fragments = []
+                    index = self._existing_profile(profile["id"])
+                    fragments = [] if index is None else self.profiles[index]["fragments"]
                     if item:
                         position = 0
                         number = int(item.get("@startNumber", 1)) - 1
                         timescale = int(item["@timescale"])
+
+                        # Initialization
+                        if len(fragments) == 0 and "@initialization" in item:
+                            media = item["@initialization"]
+                            media = media.replace("$RepresentationID$", profile["id"])
+                            media = media.replace("$Bandwidth$", str(profile["bandwidth"]))
+                            if not media.startswith("http"):
+                                if "BaseURL" in representation:
+                                    base_url = representation["BaseURL"]
+                                    base_url = base_url if isinstance(base_url, list) else [base_url]
+                                    source = base_url[0]
+
+                                if source is None:
+                                    raise MissingRemoteUrl("Remote manifest URL required.")
+
+                                if source.endswith("/"):
+                                    source = source[:-1]
+                                media = f"{source}/{media}"
+                            fragments.append({
+                                "range": "0-",
+                                "extinf": f"{timescale / 1000:.3f}",
+                                "media": media
+                            })
+
+                        # Timelines
                         timelines = item["SegmentTimeline"]["S"]
+                        timelines = timelines if type(timelines) is list else [timelines]
+
                         for timeline in timelines:
-                            for _ in range(int(timeline.get("@r", 1))):
+                            for _ in range(int(timeline.get("@r", 0)) + 1):
                                 number += 1
                                 extinf = int(timelines[position]["@d"]) / timescale
                                 media = item["@media"]
+
                                 if not media.startswith("http"):
+                                    if "BaseURL" in representation:
+                                        base_url = representation["BaseURL"]
+                                        base_url = base_url if isinstance(base_url, list) else [base_url]
+                                        source = base_url[0]
+
                                     if source is None:
                                         raise MissingRemoteUrl("Remote manifest URL required.")
+
+                                    if source.endswith("/"):
+                                        source = source[:-1]
                                     media = f"{source}/{media}"
 
                                 media = media.replace("$Number$", str(number))
                                 time = int(timelines[position].get("@t", 0)) + int(timelines[position]["@d"])
                                 media = media.replace("$Time$", str(time))
                                 media = media.replace("$RepresentationID$", profile["id"])
                                 media = media.replace("$Bandwidth$", str(profile["bandwidth"]))
-
                                 fragments.append({
                                     "range": "0-",
                                     "extinf": f"{extinf:.3f}",
                                     "media": media
                                 })
                             position += 1
                     else:
                         drm = _get_drm(adaptation)
-                        segment = representation["SegmentBase"]["@indexRange"]
-                        start, end = map(int, segment.split("-"))
+                        segment = representation["SegmentBase"]
+                        start, end = map(int, segment["@indexRange"].split("-"))
+                        if "Initialization" in segment:
+                            start, _ = map(int, segment["Initialization"]["@range"].split("-"))
+
                         extinf = (end - start) / 1000
                         fragments.append({
-                            "range": segment,
+                            "range": f"{start}-{end}",
                             "extinf": f"{extinf:.3f}",
                             "media": f"{source}/{representation['BaseURL']}"
                         })
 
                     profile["fragments"] = fragments
                     profile["drm"] = drm
-                    profiles.append(profile)
-            else:
-                pass
-        return profiles
 
-    def build_hls(self, profile_id: str) -> str:
+                    index = self._existing_profile(profile["id"])
+                    if index is None:
+                        self.profiles.append(profile)
+                    else:
+                        if not self.profiles[index]["drm"]:
+                            self.profiles[index]["drm"] = profile["drm"]
+                        self.profiles[index]["fragments"] = profile["fragments"]
+
+    def build_hls(self, profile_id: str, licence: str = None) -> str:
         profile = self._get_profile(profile_id)
-        hls = ["#EXTM3U", "#EXT-X-TARGETDURATION:4", "#EXT-X-ALLOW-CACHE:YES", "#EXT-X-PLAYLIST-TYPE:VOD"]
-        licence = profile["drm"].get("license")
+        sequence = 0 if len(profile["fragments"]) == 1 else 1
+        duration = int(max([float(f["extinf"]) for f in profile["fragments"]]))
+        hls = [
+            "#EXTM3U",
+            "#EXT-X-VERSION:6",
+            f"#EXT-X-MEDIA-SEQUENCE:{sequence}",
+            f"#EXT-X-TARGETDURATION:{duration}",
+            "#EXT-X-PLAYLIST-TYPE:VOD",
+            "#EXT-X-ALLOW-CACHE:YES",
+        ]
+
         if licence:
-            hls.append(f'#EXT-X-KEY:METHOD=SAMPLE-AES,URI="{licence}"')
-        hls += ["#EXT-X-VERSION:5", "#EXT-X-MEDIA-SEQUENCE:1"]
+            kid, key = licence.split(":")
+            key_uri = "data:text/plain;base64," + base64.b64encode(bytes.fromhex(key)).decode("utf-8")
+            key_id = "0x" + bytes.fromhex(kid).hex().upper()
+            key_iv = "0x00000000000000000000000000000000"
+            hls.append(f'#EXT-X-KEY:METHOD=SAMPLE-AES-CTR,URI="{key_uri}",KEYID={key_id},IV={key_iv},KEYFORMATVERSIONS="1",KEYFORMAT="urn:uuid:edef8ba9-79d6-4ace-a3c8-27dcd51d21ed"')
+        else:
+            licence = profile["drm"].get("license")
+            if licence:
+                hls.append(f'#EXT-X-KEY:METHOD=SAMPLE-AES,URI="{licence}"')
+
         hls.extend(f"#EXTINF:{fragment['extinf']},\n{fragment['media']}" for fragment in profile["fragments"])
         hls.append("#EXT-X-ENDLIST")
         return "\n".join(hls)
 
     def media_urls(self, profile_id: str) -> list:
         profile = self._get_profile(profile_id)
         return [fragment["media"] for fragment in profile["fragments"]]
```

### Comparing `pydash2hls-2.1.3/pydash2hls.egg-info/PKG-INFO` & `pydash2hls-2.1.4/pydash2hls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash2hls
-Version: 2.1.3
+Version: 2.1.4
 Summary: Python library for converting DASH manifest files to HLS format.
 Home-page: https://github.com/hyugogirubato/pydash2hls
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: manifest,hls,m3u8,dash
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,18 +29,18 @@
 [![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls/)
 
 PyDash2HLS is a Python library for converting DASH (Dynamic Adaptive Streaming over HTTP) manifest files to HLS (HTTP
 Live Streaming) format.
 
 ## Features
 
-- Convert MPD files to HLS format
-- Support for remote and local MPD files
-- Retrieve media URLs for a specific profile
-- Handle DRM (Digital Rights Management) information in MPD files
+- Convert MPD files to HLS format.
+- Support for remote and local MPD files.
+- Retrieve media URLs for a specific profile.
+- Handle DRM (Digital Rights Management) information in MPD files.
 
 ## Installation
 
 You can install PyDash2HLS using pip:
 
 ````shell
 pip install pydash2hls
```

### Comparing `pydash2hls-2.1.3/setup.py` & `pydash2hls-2.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pydash2hls",
-    version="2.1.3",
+    version="2.1.4",
     author="hyugogirubato",
     author_email="hyugogirubato@gmail.com",
     description="Python library for converting DASH manifest files to HLS format.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hyugogirubato/pydash2hls",
     packages=find_packages(),
```

