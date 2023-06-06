# Comparing `tmp/FindSystemFontsFilename-0.0.3.tar.gz` & `tmp/FindSystemFontsFilename-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindSystemFontsFilename-0.0.3.tar", last modified: Sat Apr 29 13:33:34 2023, max compression
+gzip compressed data, was "FindSystemFontsFilename-0.0.4.tar", last modified: Tue Jun  6 00:57:55 2023, max compression
```

## Comparing `FindSystemFontsFilename-0.0.3.tar` & `FindSystemFontsFilename-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 13:33:34.023905 FindSystemFontsFilename-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-04-29 13:33:33.980882 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/
--rw-rw-rw-   0        0        0     1984 2023-04-29 13:33:33.000000 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-04-29 13:33:33.000000 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 13:33:33.000000 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 13:33:33.000000 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-29 13:33:33.000000 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-04-28 01:55:06.000000 FindSystemFontsFilename-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1984 2023-04-29 13:33:34.022929 FindSystemFontsFilename-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-04-29 02:43:05.000000 FindSystemFontsFilename-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 13:33:34.020002 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/
--rw-rw-rw-   0        0        0      140 2023-04-29 13:26:27.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/__init__.py
--rw-rw-rw-   0        0        0      190 2023-04-28 16:03:29.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/exceptions.py
--rw-rw-rw-   0        0        0      652 2023-04-29 01:59:59.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/fonts_filename.py
--rw-rw-rw-   0        0        0     4441 2023-04-28 16:05:18.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/linux_fonts.py
--rw-rw-rw-   0        0        0     4681 2023-04-29 13:26:53.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/mac_fonts.py
--rw-rw-rw-   0        0        0      280 2023-04-28 01:38:49.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/system_fonts.py
--rw-rw-rw-   0        0        0    20206 2023-04-28 16:04:31.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/windows_fonts.py
--rw-rw-rw-   0        0        0       42 2023-04-29 13:33:34.023905 FindSystemFontsFilename-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1698 2023-04-29 02:21:21.000000 FindSystemFontsFilename-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 00:57:55.919253 FindSystemFontsFilename-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-06 00:57:55.910468 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/
+-rw-rw-rw-   0        0        0     1984 2023-06-06 00:57:55.000000 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-06-06 00:57:55.000000 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 00:57:55.000000 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 00:57:55.000000 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-06 00:57:55.000000 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-04-28 01:55:06.000000 FindSystemFontsFilename-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1984 2023-06-06 00:57:55.919253 FindSystemFontsFilename-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-04-29 02:43:05.000000 FindSystemFontsFilename-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 00:57:55.917299 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/
+-rw-rw-rw-   0        0        0      140 2023-06-06 00:45:05.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-04-28 16:03:29.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/exceptions.py
+-rw-rw-rw-   0        0        0      652 2023-04-29 01:59:59.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/fonts_filename.py
+-rw-rw-rw-   0        0        0     4931 2023-06-06 00:44:37.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/linux_fonts.py
+-rw-rw-rw-   0        0        0     5326 2023-06-06 00:55:47.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/mac_fonts.py
+-rw-rw-rw-   0        0        0      280 2023-04-28 01:38:49.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/system_fonts.py
+-rw-rw-rw-   0        0        0    20240 2023-06-06 00:44:41.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/windows_fonts.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 00:57:55.920240 FindSystemFontsFilename-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1698 2023-04-29 02:21:21.000000 FindSystemFontsFilename-0.0.4/setup.py
```

### Comparing `FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/PKG-INFO` & `FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindSystemFontsFilename
-Version: 0.0.3
+Version: 0.0.4
 Summary: Find the system fonts filename.
 Home-page: https://github.com/moi15moi/FindSystemFontsFilename/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FindSystemFontsFilename/
 Project-URL: Tracker, https://github.com/moi15moi/FindSystemFontsFilename/issues/
```

### Comparing `FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/SOURCES.txt` & `FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.3/LICENSE` & `FindSystemFontsFilename-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.3/PKG-INFO` & `FindSystemFontsFilename-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindSystemFontsFilename
-Version: 0.0.3
+Version: 0.0.4
 Summary: Find the system fonts filename.
 Home-page: https://github.com/moi15moi/FindSystemFontsFilename/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FindSystemFontsFilename/
 Project-URL: Tracker, https://github.com/moi15moi/FindSystemFontsFilename/issues/
```

### Comparing `FindSystemFontsFilename-0.0.3/README.md` & `FindSystemFontsFilename-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.3/find_system_fonts_filename/fonts_filename.py` & `FindSystemFontsFilename-0.0.4/find_system_fonts_filename/fonts_filename.py`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.3/find_system_fonts_filename/linux_fonts.py` & `FindSystemFontsFilename-0.0.4/find_system_fonts_filename/linux_fonts.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,31 +78,35 @@
         LinuxFonts._font_config.FcConfigDestroy(config)
         LinuxFonts._font_config.FcPatternDestroy(pat)
         LinuxFonts._font_config.FcObjectSetDestroy(os)
         LinuxFonts._font_config.FcFontSetDestroy(fs)
 
         return fonts_filename
 
-
     @staticmethod
     def _load_font_config_library():
         font_config_library_name = util.find_library("fontconfig")
 
         if font_config_library_name is None:
             raise FontConfigNotFound("You need to install FontConfig to get the fonts filename")
 
         LinuxFonts._font_config = cdll.LoadLibrary(font_config_library_name)
 
+        # https://www.freedesktop.org/software/fontconfig/fontconfig-devel/fcinitloadconfigandfonts.html
         LinuxFonts._font_config.FcInitLoadConfigAndFonts.restype = c_void_p
         LinuxFonts._font_config.FcInitLoadConfigAndFonts.argtypes = []
 
+        # https://www.freedesktop.org/software/fontconfig/fontconfig-devel/fcpatterncreate.html
         LinuxFonts._font_config.FcPatternCreate.restype = c_void_p
         LinuxFonts._font_config.FcPatternCreate.argtypes = []
 
+        # https://www.freedesktop.org/software/fontconfig/fontconfig-devel/fcobjectsetbuild.html
         LinuxFonts._font_config.FcObjectSetBuild.restype = c_void_p
         LinuxFonts._font_config.FcObjectSetBuild.argtypes = [c_char_p, c_void_p]
 
+        # https://www.freedesktop.org/software/fontconfig/fontconfig-devel/fcfontlist.html
         LinuxFonts._font_config.FcFontList.restype = POINTER(FcFontSet)
         LinuxFonts._font_config.FcFontList.argtypes = [c_void_p, c_void_p, c_void_p]
 
+        # https://www.freedesktop.org/software/fontconfig/fontconfig-devel/fcpatternget-type.html
         LinuxFonts._font_config.FcPatternGetString.restype = FC_RESULT
         LinuxFonts._font_config.FcPatternGetString.argtypes = [c_void_p, c_char_p, c_int, POINTER(c_char_p)]
```

### Comparing `FindSystemFontsFilename-0.0.3/find_system_fonts_filename/mac_fonts.py` & `FindSystemFontsFilename-0.0.4/find_system_fonts_filename/mac_fonts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,105 @@
-from ctypes import c_bool, c_char_p, c_long, c_void_p, cdll, create_string_buffer, util
-from os import pathconf
-from pathlib import Path
-from platform import mac_ver
-from typing import Set
-from .exceptions import OSNotSupported
-from .system_fonts import SystemFonts
-
-
-class MacFonts(SystemFonts):
-    _core_foundation = None
-    _core_text = None
-    # CoreText has an API to get the format of the font: https://developer.apple.com/documentation/coretext/ctfontformat
-    # But, the API is "semi-broken" since it says .dfont are TrueType. This is kinda true, but it is not a behaviour that we want.
-    # So, we only check the file extension and see if it is valid.
-    VALID_FONT_FORMATS = ["ttf", "otf", "ttc"]
-
-    def get_system_fonts_filename() -> Set[str]:
-        if MacVersionHelpers.is_mac_version_or_greater(10, 6):
-            if MacFonts._core_foundation is None or MacFonts._core_text is None:
-                MacFonts._load_core_library()
-
-            fonts_filename = set()
-
-            font_urls = MacFonts._core_text.CTFontManagerCopyAvailableFontURLs()
-            font_count = MacFonts._core_foundation.CFArrayGetCount(font_urls)
-
-            max_length = pathconf("/", "PC_PATH_MAX")
-
-            for i in range(font_count):
-                url = MacFonts._core_foundation.CFArrayGetValueAtIndex(font_urls, i)
-
-                file_name_ptr = create_string_buffer(max_length)
-                no_error = MacFonts._core_foundation.CFURLGetFileSystemRepresentation(url, True, file_name_ptr, max_length)
-
-                if no_error:
-                    filename = file_name_ptr.value.decode()
-
-                    if Path(filename).suffix.lstrip(".").strip().lower() in MacFonts.VALID_FONT_FORMATS:
-                        fonts_filename.add(filename)
-                else:
-                    raise Exception("An unexpected error has occurred while decoded the CFURL.")
-
-            MacFonts._core_foundation.CFRelease(font_urls)
-        else:
-            raise OSNotSupported("FindSystemFontsFilename only works on Mac 10.6 or more")
-
-        return fonts_filename
-
-    @staticmethod
-    def _load_core_library():
-        core_foundation_library_name = util.find_library("CoreFoundation")
-        # Hack for compatibility with macOS greater or equals to 11.0.
-        # From: https://github.com/pyglet/pyglet/blob/a44e83a265e7df8ece793de865bcf3690f66adbd/pyglet/libs/darwin/cocoapy/cocoalibs.py#L10-L14
-        if core_foundation_library_name is None:
-            core_foundation_library_name = "/System/Library/Frameworks/CoreFoundation.framework/CoreFoundation"
-        MacFonts._core_foundation = cdll.LoadLibrary(core_foundation_library_name)
-
-        core_text_library_name = util.find_library("CoreText")
-        # Hack for compatibility with macOS greater or equals to 11.0.
-        # From: https://github.com/pyglet/pyglet/blob/a44e83a265e7df8ece793de865bcf3690f66adbd/pyglet/libs/darwin/cocoapy/cocoalibs.py#L520-L524
-        if core_text_library_name is None:
-            core_text_library_name = "/System/Library/Frameworks/CoreText.framework/CoreText"
-        MacFonts._core_text = cdll.LoadLibrary(core_text_library_name)
-
-        CFIndex = c_long
-
-        MacFonts._core_foundation.CFRelease.restype = c_void_p
-        MacFonts._core_foundation.CFRelease.argtypes = [c_void_p]
-
-        MacFonts._core_foundation.CFArrayGetCount.restype = CFIndex
-        MacFonts._core_foundation.CFArrayGetCount.argtypes = [c_void_p]
-
-        MacFonts._core_foundation.CFArrayGetValueAtIndex.restype = c_void_p
-        MacFonts._core_foundation.CFArrayGetValueAtIndex.argtypes = [c_void_p, CFIndex]
-
-        MacFonts._core_foundation.CFURLGetFileSystemRepresentation.restype = c_bool
-        MacFonts._core_foundation.CFURLGetFileSystemRepresentation.argtypes = [c_void_p, c_bool, c_char_p, CFIndex]
-
-        MacFonts._core_text.CTFontManagerCopyAvailableFontURLs.restype = c_void_p
-        MacFonts._core_text.CTFontManagerCopyAvailableFontURLs.argtypes = []
-
-
-class MacVersionHelpers:
-    @staticmethod
-    def is_mac_version_or_greater(minimum_major: int, minimum_minor: int) -> bool:
-        """
-        Parameters:
-            major (int): The minimum major OS version number.
-            minor (int): The minimum minor OS version number.
-        Returns:
-            True if the specified version matches or if it is greater than the version of the current Mac OS. Otherwise, False.
-        """
-
-        system_major, system_minor = mac_ver()[0].split(".")[:2]
-
-        system_major = int(system_major)
-        system_minor = int(system_minor)
-
-        return minimum_major > system_major or (system_major == minimum_major and system_minor >= minimum_minor)
+from ctypes import c_bool, c_char_p, c_long, c_void_p, cdll, create_string_buffer, util
+from os import pathconf
+from pathlib import Path
+from platform import mac_ver
+from typing import Set
+from .exceptions import OSNotSupported
+from .system_fonts import SystemFonts
+
+
+class MacFonts(SystemFonts):
+    _core_foundation = None
+    _core_text = None
+    # CoreText has an API to get the format of the font: https://developer.apple.com/documentation/coretext/ctfontformat
+    # But, the API is "semi-broken" since it says .dfont are TrueType. This is kinda true, but it is not a behaviour that we want.
+    # So, we only check the file extension and see if it is valid.
+    VALID_FONT_FORMATS = ["ttf", "otf", "ttc"]
+
+    def get_system_fonts_filename() -> Set[str]:
+        if MacVersionHelpers.is_mac_version_or_greater(10, 6):
+            if MacFonts._core_foundation is None or MacFonts._core_text is None:
+                MacFonts._load_core_library()
+
+            fonts_filename = set()
+
+            font_urls = MacFonts._core_text.CTFontManagerCopyAvailableFontURLs()
+            font_count = MacFonts._core_foundation.CFArrayGetCount(font_urls)
+
+            max_length = pathconf("/", "PC_PATH_MAX")
+
+            for i in range(font_count):
+                url = MacFonts._core_foundation.CFArrayGetValueAtIndex(font_urls, i)
+
+                file_name_ptr = create_string_buffer(max_length)
+                no_error = MacFonts._core_foundation.CFURLGetFileSystemRepresentation(url, True, file_name_ptr, max_length)
+
+                if no_error:
+                    filename = file_name_ptr.value.decode()
+
+                    if Path(filename).suffix.lstrip(".").strip().lower() in MacFonts.VALID_FONT_FORMATS:
+                        fonts_filename.add(filename)
+                else:
+                    raise Exception("An unexpected error has occurred while decoded the CFURL.")
+
+            MacFonts._core_foundation.CFRelease(font_urls)
+        else:
+            raise OSNotSupported("FindSystemFontsFilename only works on Mac 10.6 or more")
+
+        return fonts_filename
+
+    @staticmethod
+    def _load_core_library():
+        core_foundation_library_name = util.find_library("CoreFoundation")
+        # Hack for compatibility with macOS greater or equals to 11.0.
+        # From: https://github.com/pyglet/pyglet/blob/a44e83a265e7df8ece793de865bcf3690f66adbd/pyglet/libs/darwin/cocoapy/cocoalibs.py#L10-L14
+        if core_foundation_library_name is None:
+            core_foundation_library_name = "/System/Library/Frameworks/CoreFoundation.framework/CoreFoundation"
+        MacFonts._core_foundation = cdll.LoadLibrary(core_foundation_library_name)
+
+        core_text_library_name = util.find_library("CoreText")
+        # Hack for compatibility with macOS greater or equals to 11.0.
+        # From: https://github.com/pyglet/pyglet/blob/a44e83a265e7df8ece793de865bcf3690f66adbd/pyglet/libs/darwin/cocoapy/cocoalibs.py#L520-L524
+        if core_text_library_name is None:
+            core_text_library_name = "/System/Library/Frameworks/CoreText.framework/CoreText"
+        MacFonts._core_text = cdll.LoadLibrary(core_text_library_name)
+
+        CFIndex = c_long
+
+        # https://developer.apple.com/documentation/corefoundation/1521153-cfrelease
+        MacFonts._core_foundation.CFRelease.restype = c_void_p
+        MacFonts._core_foundation.CFRelease.argtypes = [c_void_p]
+
+        # https://developer.apple.com/documentation/corefoundation/1388772-cfarraygetcount?language=objc
+        MacFonts._core_foundation.CFArrayGetCount.restype = CFIndex
+        MacFonts._core_foundation.CFArrayGetCount.argtypes = [c_void_p]
+
+        # https://developer.apple.com/documentation/corefoundation/1388767-cfarraygetvalueatindex?language=objc
+        MacFonts._core_foundation.CFArrayGetValueAtIndex.restype = c_void_p
+        MacFonts._core_foundation.CFArrayGetValueAtIndex.argtypes = [c_void_p, CFIndex]
+
+        # https://developer.apple.com/documentation/corefoundation/1541515-cfurlgetfilesystemrepresentation?language=objc
+        MacFonts._core_foundation.CFURLGetFileSystemRepresentation.restype = c_bool
+        MacFonts._core_foundation.CFURLGetFileSystemRepresentation.argtypes = [c_void_p, c_bool, c_char_p, CFIndex]
+
+        # https://developer.apple.com/documentation/coretext/1499478-ctfontmanagercopyavailablefontur?language=objc
+        MacFonts._core_text.CTFontManagerCopyAvailableFontURLs.restype = c_void_p
+        MacFonts._core_text.CTFontManagerCopyAvailableFontURLs.argtypes = []
+
+
+class MacVersionHelpers:
+    @staticmethod
+    def is_mac_version_or_greater(minimum_major: int, minimum_minor: int) -> bool:
+        """
+        Parameters:
+            major (int): The minimum major OS version number.
+            minor (int): The minimum minor OS version number.
+        Returns:
+            True if the specified version matches or if it is greater than the version of the current Mac OS. Otherwise, False.
+        """
+
+        system_major, system_minor = mac_ver()[0].split(".")[:2]
+
+        system_major = int(system_major)
+        system_minor = int(system_minor)
+
+        return system_major > minimum_major or (system_major == minimum_major and system_minor >= minimum_minor)
```

### Comparing `FindSystemFontsFilename-0.0.3/find_system_fonts_filename/windows_fonts.py` & `FindSystemFontsFilename-0.0.4/find_system_fonts_filename/windows_fonts.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     DWRITE_FONT_FILE_TYPE_CFF = 1
     DWRITE_FONT_FILE_TYPE_TRUETYPE = 2
     DWRITE_FONT_FILE_TYPE_OPENTYPE_COLLECTION = 3
     DWRITE_FONT_FILE_TYPE_TYPE1_PFM = 4
     DWRITE_FONT_FILE_TYPE_TYPE1_PFB = 5
     DWRITE_FONT_FILE_TYPE_VECTOR = 6
     DWRITE_FONT_FILE_TYPE_BITMAP = 7
-    DWRITE_FONT_FILE_TYPE_TRUETYPE_COLLECTION = 8
+    DWRITE_FONT_FILE_TYPE_TRUETYPE_COLLECTION = DWRITE_FONT_FILE_TYPE_OPENTYPE_COLLECTION
 
 
 class IDWriteFontFileLoader(IUnknown):
     # https://learn.microsoft.com/en-us/windows/win32/api/dwrite/nn-dwrite-idwritefontfileloader
     _iid_ = GUID("{727cad4e-d6af-4c9e-8a08-d695b11caa49}")
     _methods_ = [
         STDMETHOD(None, "CreateStreamFromKey"),  # Need to be implemented
@@ -363,15 +363,14 @@
 
                     buffer = create_unicode_buffer(path_len.value + 1)
                     local_loader.GetFilePathFromKey(font_file_reference_key, font_file_reference_key_size, buffer, len(buffer))
 
                     fonts_filename.add(buffer.value)
 
         return fonts_filename
-    
 
     @staticmethod
     def _load_DWriteCreateFactory():
         WindowsFonts._DWriteCreateFactory = windll.dwrite.DWriteCreateFactory
         WindowsFonts._DWriteCreateFactory.restype = HRESULT
         WindowsFonts._DWriteCreateFactory.argtypes = [wintypes.UINT, GUID, POINTER(POINTER(IUnknown))]
```

### Comparing `FindSystemFontsFilename-0.0.3/setup.py` & `FindSystemFontsFilename-0.0.4/setup.py`

 * *Files identical despite different names*

