# Comparing `tmp/image_center-1.0.0.tar.gz` & `tmp/image_center-1.0.1.tar.gz`

## Comparing `image_center-1.0.0.tar` & `image_center-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 image_center-1.0.0/image_center/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 image_center-1.0.0/image_center/__version__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 image_center-1.0.0/image_center/conf.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 image_center-1.0.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-1.0.0/LICENSE
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 image_center-1.0.0/README.md
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 image_center-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 image_center-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 image_center-1.0.1/image_center/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 image_center-1.0.1/image_center/__version__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 image_center-1.0.1/image_center/conf.py
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 image_center-1.0.1/image_center/server.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 image_center-1.0.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 image_center-1.0.1/README.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 image_center-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 image_center-1.0.1/PKG-INFO
```

### Comparing `image_center-1.0.0/image_center/__init__.py` & `image_center-1.0.1/image_center/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,25 +71,25 @@
             setting.SCREEN_CACHE = (
                 os.popen("qdbus org.kde.KWin /Screenshot screenshotFullscreen")
                     .read()
                     .strip("\n")
             )
         template_path = f"{image_path}.png"
         if GET_OPENCV_FORM_RPC:
-            server = ServerProxy(setting.OPENCV_SERVER_HOST, allow_none=True)
+            server = ServerProxy(f"http://{setting.SERVER_IP}:{setting.PORT}", allow_none=True)
             source_rb = open(setting.SCREEN_CACHE, "rb")
             template_rb = open(template_path, "rb")
             try:
                 source_path = server.image_put(Binary(source_rb.read()))
                 source_rb.close()
                 tpl_path = server.image_put(Binary(template_rb.read()))
                 template_rb.close()
                 return server.match_image_by_opencv(tpl_path, source_path, rate, multiple)
             except OSError:
-                raise EnvironmentError(f"RPC服务器链接失败. {setting.OPENCV_SERVER_HOST}")
+                raise EnvironmentError(f"RPC服务器链接失败. http://{setting.SERVER_IP}:{setting.PORT}")
         else:
             if not os.path.exists(template_path):
                 raise TemplatePictureNotExist(template_path)
             source = cv.imread(setting.SCREEN_CACHE)
             template = cv.imread(template_path)
             result = cv.matchTemplate(source, template, cv.TM_CCOEFF_NORMED)
             if not multiple:
@@ -282,15 +282,15 @@
             if bdata[_x + point[0], _y + point[1]] == sdata[point[0], point[1]]:
                 same = same + 1
             else:
                 diff = diff + 1
         return same / (same + diff) >= rate
 
     @classmethod
-    def image_center_by_rgb(cls, image_name=None, image_path=None, rate=setting.RATE):
+    def image_center_by_rgb(cls, image_name=None, image_path=None, rate=setting.IMAGE_RATE):
         """
         By comparing the RGB values of the small image with the large
         image on the screen, the coordinates of the small image on
         the screen are returned.
         """
         if not image_path:
             image_path = setting.PIC_PATH
```

### Comparing `image_center-1.0.0/.gitignore` & `image_center-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `image_center-1.0.0/LICENSE` & `image_center-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_center-1.0.0/pyproject.toml` & `image_center-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "image-center"
 authors = [
-  { name="mikigo", email="1964191531@qq.com" },
+    { name = "mikigo", email = "1964191531@qq.com" },
 ]
 description = "image-center"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "allure-pytest",
+    "pyscreenshot",
+    "pillow"
 ]
 
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
-#server = [
-#    "paddlepaddle",
-#    "paddleocr>=2.0.1"
+#all = [
+#    "pyscreenshot",
+#    "pillow"
 #]
 
 test = [
     "pytest",
 ]
 
 doc = ["mkdocs-material"]
```

