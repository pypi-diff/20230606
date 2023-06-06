# Comparing `tmp/blue-engine-0.0.3.5.tar.gz` & `tmp/blue-engine-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue-engine-0.0.3.5.tar", last modified: Fri May 26 07:47:14 2023, max compression
+gzip compressed data, was "blue-engine-0.0.4.tar", last modified: Tue Jun  6 12:30:52 2023, max compression
```

## Comparing `blue-engine-0.0.3.5.tar` & `blue-engine-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 07:47:13.977826 blue-engine-0.0.3.5/
--rw-rw-rw-   0        0        0       68 2023-05-21 04:57:53.000000 blue-engine-0.0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0      482 2023-05-26 07:47:13.974825 blue-engine-0.0.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 07:47:12.617485 blue-engine-0.0.3.5/blueEngine/
--rw-rw-rw-   0        0        0      207 2023-05-26 06:36:53.000000 blue-engine-0.0.3.5/blueEngine/BETime.py
--rw-rw-rw-   0        0        0        0 2023-05-07 14:20:14.000000 blue-engine-0.0.3.5/blueEngine/__init__.py
--rw-rw-rw-   0        0        0     2374 2023-05-25 03:43:59.000000 blue-engine-0.0.3.5/blueEngine/app.py
--rw-rw-rw-   0        0        0     2272 2023-05-20 07:28:36.000000 blue-engine-0.0.3.5/blueEngine/camera.py
--rw-rw-rw-   0        0        0      145 2023-05-26 06:26:49.000000 blue-engine-0.0.3.5/blueEngine/canvas.py
--rw-rw-rw-   0        0        0       89 2023-05-26 05:14:05.000000 blue-engine-0.0.3.5/blueEngine/component.py
--rw-rw-rw-   0        0        0      236 2023-05-22 13:59:34.000000 blue-engine-0.0.3.5/blueEngine/errors.py
--rw-rw-rw-   0        0        0      352 2023-05-26 05:04:34.000000 blue-engine-0.0.3.5/blueEngine/font_component.py
--rw-rw-rw-   0        0        0      361 2023-05-26 06:24:16.000000 blue-engine-0.0.3.5/blueEngine/gobject.py
--rw-rw-rw-   0        0        0     2262 2023-05-25 04:22:31.000000 blue-engine-0.0.3.5/blueEngine/input.py
--rw-rw-rw-   0        0        0      359 2023-05-11 07:14:39.000000 blue-engine-0.0.3.5/blueEngine/light.py
--rw-rw-rw-   0        0        0      287 2023-05-11 12:59:41.000000 blue-engine-0.0.3.5/blueEngine/mesh.py
--rw-rw-rw-   0        0        0     2558 2023-05-26 06:26:29.000000 blue-engine-0.0.3.5/blueEngine/model.py
--rw-rw-rw-   0        0        0      869 2023-05-25 19:13:25.000000 blue-engine-0.0.3.5/blueEngine/scene.py
--rw-rw-rw-   0        0        0      634 2023-05-11 07:33:57.000000 blue-engine-0.0.3.5/blueEngine/shader_program.py
--rw-rw-rw-   0        0        0        0 2023-05-26 06:22:27.000000 blue-engine-0.0.3.5/blueEngine/textobject.py
--rw-rw-rw-   0        0        0     1034 2023-05-11 14:19:28.000000 blue-engine-0.0.3.5/blueEngine/texture.py
--rw-rw-rw-   0        0        0      493 2023-05-20 05:10:43.000000 blue-engine-0.0.3.5/blueEngine/transfrom.py
--rw-rw-rw-   0        0        0       86 2023-05-23 05:53:48.000000 blue-engine-0.0.3.5/blueEngine/utils.py
--rw-rw-rw-   0        0        0      612 2023-05-11 07:41:36.000000 blue-engine-0.0.3.5/blueEngine/vao.py
--rw-rw-rw-   0        0        0     2407 2023-05-25 03:44:26.000000 blue-engine-0.0.3.5/blueEngine/vbo.py
-drwxrwxrwx   0        0        0        0 2023-05-26 07:47:13.884803 blue-engine-0.0.3.5/blue_engine.egg-info/
--rw-rw-rw-   0        0        0      482 2023-05-26 07:47:08.000000 blue-engine-0.0.3.5/blue_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-05-26 07:47:09.000000 blue-engine-0.0.3.5/blue_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 07:47:08.000000 blue-engine-0.0.3.5/blue_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 06:47:43.000000 blue-engine-0.0.3.5/blue_engine.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2023-05-26 07:47:08.000000 blue-engine-0.0.3.5/blue_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 07:47:08.000000 blue-engine-0.0.3.5/blue_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1070 2023-05-21 05:17:33.000000 blue-engine-0.0.3.5/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 07:47:13.978826 blue-engine-0.0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-05-26 07:31:52.000000 blue-engine-0.0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:30:52.521242 blue-engine-0.0.4/
+-rw-rw-rw-   0        0        0       32 2023-05-30 16:51:11.000000 blue-engine-0.0.4/.projdata
+-rw-rw-rw-   0        0        0      116 2023-06-06 12:27:37.000000 blue-engine-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      479 2023-06-06 12:30:52.505238 blue-engine-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 12:30:51.976111 blue-engine-0.0.4/blueEngine/
+-rw-rw-rw-   0        0        0      764 2023-05-30 17:36:47.000000 blue-engine-0.0.4/blueEngine/__init__.py
+-rw-rw-rw-   0        0        0     2414 2023-05-28 15:29:19.000000 blue-engine-0.0.4/blueEngine/app.py
+-rw-rw-rw-   0        0        0       25 2023-05-27 07:43:01.000000 blue-engine-0.0.4/blueEngine/blue_object.py
+-rw-rw-rw-   0        0        0     2272 2023-05-20 07:28:36.000000 blue-engine-0.0.4/blueEngine/camera.py
+-rw-rw-rw-   0        0        0      149 2023-05-27 07:40:32.000000 blue-engine-0.0.4/blueEngine/canvas.py
+-rw-rw-rw-   0        0        0       89 2023-05-26 05:14:05.000000 blue-engine-0.0.4/blueEngine/component.py
+-rw-rw-rw-   0        0        0      236 2023-05-22 13:59:34.000000 blue-engine-0.0.4/blueEngine/errors.py
+-rw-rw-rw-   0        0        0      352 2023-05-26 05:04:34.000000 blue-engine-0.0.4/blueEngine/font_component.py
+-rw-rw-rw-   0        0        0      672 2023-05-28 15:35:31.000000 blue-engine-0.0.4/blueEngine/game_object.py
+-rw-rw-rw-   0        0        0     2310 2023-05-28 11:58:48.000000 blue-engine-0.0.4/blueEngine/input.py
+-rw-rw-rw-   0        0        0      359 2023-05-11 07:14:39.000000 blue-engine-0.0.4/blueEngine/light.py
+-rw-rw-rw-   0        0        0      287 2023-05-11 12:59:41.000000 blue-engine-0.0.4/blueEngine/mesh.py
+-rw-rw-rw-   0        0        0     2615 2023-05-29 03:21:59.000000 blue-engine-0.0.4/blueEngine/model.py
+-rw-rw-rw-   0        0        0      905 2023-05-28 08:53:27.000000 blue-engine-0.0.4/blueEngine/scene.py
+-rw-rw-rw-   0        0        0      634 2023-05-11 07:33:57.000000 blue-engine-0.0.4/blueEngine/shader_program.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 06:22:27.000000 blue-engine-0.0.4/blueEngine/textobject.py
+-rw-rw-rw-   0        0        0     1034 2023-05-11 14:19:28.000000 blue-engine-0.0.4/blueEngine/texture.py
+-rw-rw-rw-   0        0        0      493 2023-05-20 05:10:43.000000 blue-engine-0.0.4/blueEngine/transfrom.py
+-rw-rw-rw-   0        0        0       86 2023-05-23 05:53:48.000000 blue-engine-0.0.4/blueEngine/utils.py
+-rw-rw-rw-   0        0        0      612 2023-05-11 07:41:36.000000 blue-engine-0.0.4/blueEngine/vao.py
+-rw-rw-rw-   0        0        0     2407 2023-05-25 03:44:26.000000 blue-engine-0.0.4/blueEngine/vbo.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:30:52.159151 blue-engine-0.0.4/blue_engine.egg-info/
+-rw-rw-rw-   0        0        0      479 2023-06-06 12:30:49.000000 blue-engine-0.0.4/blue_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      896 2023-06-06 12:30:50.000000 blue-engine-0.0.4/blue_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 12:30:49.000000 blue-engine-0.0.4/blue_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 06:47:43.000000 blue-engine-0.0.4/blue_engine.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-06-06 12:30:50.000000 blue-engine-0.0.4/blue_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 12:30:50.000000 blue-engine-0.0.4/blue_engine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 12:30:52.247178 blue-engine-0.0.4/images/
+-rw-rw-rw-   0        0        0     2280 2023-04-17 14:01:00.000000 blue-engine-0.0.4/images/BlueEngineLogo.png
+-rw-rw-rw-   0        0        0     1070 2023-05-21 05:17:33.000000 blue-engine-0.0.4/license.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 12:30:52.274182 blue-engine-0.0.4/meshes/
+-rw-rw-rw-   0        0        0      237 2023-06-06 11:19:08.000000 blue-engine-0.0.4/meshes/grey_cube.mtl
+-rw-rw-rw-   0        0        0      952 2023-06-06 11:19:08.000000 blue-engine-0.0.4/meshes/grey_cube.obj
+-rw-rw-rw-   0        0        0       42 2023-06-06 12:30:52.522244 blue-engine-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-05-30 16:46:35.000000 blue-engine-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:30:52.373208 blue-engine-0.0.4/shaders/
+-rw-rw-rw-   0        0        0     1100 2023-05-29 03:18:30.000000 blue-engine-0.0.4/shaders/default.frag
+-rw-rw-rw-   0        0        0      521 2023-05-28 17:27:40.000000 blue-engine-0.0.4/shaders/default.vert
+drwxrwxrwx   0        0        0        0 2023-06-06 12:30:52.479234 blue-engine-0.0.4/textures/
+-rw-rw-rw-   0        0        0      135 2023-05-11 13:15:48.000000 blue-engine-0.0.4/textures/img1.png
+-rw-rw-rw-   0        0        0      135 2023-05-11 13:16:16.000000 blue-engine-0.0.4/textures/img2.png
+-rw-rw-rw-   0        0        0      135 2023-05-11 13:16:49.000000 blue-engine-0.0.4/textures/img3.png
+-rw-rw-rw-   0        0        0     2918 2023-03-18 16:09:32.000000 blue-engine-0.0.4/textures/test.png
```

### Comparing `blue-engine-0.0.3.5/blueEngine/app.py` & `blue-engine-0.0.4/blueEngine/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.ctx.enable(flags=moderngl.DEPTH_TEST|moderngl.CULL_FACE)
         
         self.light = Light()
         self.camera = Camera(self)
         self.mesh = Mesh(self)
         self.scene = Scene(self)
   
-
+        print(self.scene.get_children())
         self.loop()
         
 
     def loop(self):
         while True:
             self.get_time()
             pygame.display.set_caption(f'{self.title} @ {int(self.clock.get_fps())} fps')
```

### Comparing `blue-engine-0.0.3.5/blueEngine/camera.py` & `blue-engine-0.0.4/blueEngine/camera.py`

 * *Files identical despite different names*

### Comparing `blue-engine-0.0.3.5/blueEngine/input.py` & `blue-engine-0.0.4/blueEngine/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pygame
+from game_object import GameObject
 from utils import clamp
 import json
 
 keymap={
     'a':pygame.K_a,
     'b':pygame.K_b,
     'c':pygame.K_c,
@@ -71,15 +72,15 @@
             if self.event.key in self.positives:
                 self.value += 0.1
             if self.event.key in self.negatives:
                 self.value -= 0.1
 
             self.value = clamp(self.value, 0, 1)
 
-class Input:
+class Input(GameObject):
     def __init__(self) -> None:
         self.axes = {}
 
     def update(self):
         for i in self.axes:
             self.axes[i].update()
```

### Comparing `blue-engine-0.0.3.5/blueEngine/model.py` & `blue-engine-0.0.4/blueEngine/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import glm
+import moderngl
 
 from errors import *
 from transfrom import Transfrom
-from gobject import GameObject
+from game_object import GameObject
 
 class BaseModel(GameObject):
     def __init__(self, app, vao_name, tex_id, parent = None, position=(0, 0, 0), rotation = (0, 0, 0), scale = (1, 1, 1)) -> None:
         super().__init__(parent)
         self.app = app
         self.components = {'transform':Transfrom(self, scale, rotation, position)}
         self.m_model = self.get_model_matrix()
         self.tex_id = tex_id
         self.vao = app.mesh.vao.vaos[vao_name]
-        self.program = self.vao.program
+        self.program:moderngl.Program = self.vao.program
         self.camera = self.app.camera
+        self.lighting = 0
 
     def update(self): ...
 
     def get_model_matrix(self):
         m_model = glm.mat4()
         m_model = glm.translate(m_model, self.components['transform'].position)
         m_model = glm.rotate(m_model, self.components['transform'].rotation.x, glm.vec3(1, 0, 0))
@@ -25,14 +27,15 @@
         m_model = glm.rotate(m_model, self.components['transform'].rotation.z, glm.vec3(0, 0, 1))
         m_model = glm.scale(m_model, self.components['transform'].scale)
         return m_model
     
     def render(self):
         self.update()
         self.vao.render()
+
     def get_component(self, component:str):
         try:
             return self.components[component]
         except KeyError:
             raise ChildComponentNotExistsException(component)
 
 class Cube(BaseModel):
@@ -50,12 +53,11 @@
         self.texture = self.app.mesh.texture.textures[self.tex_id]
         self.program['u_texture_0'] = 0
         self.texture.use()
         
         self.program['m_proj'].write(self.camera.m_proj)
         self.program['m_view'].write(self.camera.m_view)
         self.program['m_model'].write(self.m_model)
-        
         self.program['light.position'].write(self.app.light.position)
         self.program['light.Ia'].write(self.app.light.Ia)
         self.program['light.Id'].write(self.app.light.Id)
         self.program['light.Is'].write(self.app.light.Is)
```

### Comparing `blue-engine-0.0.3.5/blueEngine/scene.py` & `blue-engine-0.0.4/blueEngine/scene.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from model import *
 import threading
 from input import Input, InputAxis
 
-class Scene:
+class Scene(GameObject):
     def __init__(self, app) -> None:
+        super().__init__()
         self.app = app
         self.objects = []
-        self.input_axes = Input() 
         self.load()
 
     def add_object(self, object):
         self.objects.append(object)
+        self.add_child(object)
 
     def load(self):
         app = self.app
         add = self.add_object
 
         n, s = 10 ,2
```

### Comparing `blue-engine-0.0.3.5/blueEngine/shader_program.py` & `blue-engine-0.0.4/blueEngine/shader_program.py`

 * *Files identical despite different names*

### Comparing `blue-engine-0.0.3.5/blueEngine/texture.py` & `blue-engine-0.0.4/blueEngine/texture.py`

 * *Files identical despite different names*

### Comparing `blue-engine-0.0.3.5/blueEngine/vao.py` & `blue-engine-0.0.4/blueEngine/vao.py`

 * *Files identical despite different names*

### Comparing `blue-engine-0.0.3.5/blueEngine/vbo.py` & `blue-engine-0.0.4/blueEngine/vbo.py`

 * *Files identical despite different names*

### Comparing `blue-engine-0.0.3.5/license.txt` & `blue-engine-0.0.4/license.txt`

 * *Files identical despite different names*

### Comparing `blue-engine-0.0.3.5/setup.py` & `blue-engine-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     with open('readme.md') as f:
         README = f.read()
     return README
 
 
 setup(
     name='blue-engine',
-    version='0.0.3.5',
+    version='0.0.4',
     description='',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/MrBlueBlobGuy/Blue-Engine',
     author='Debojyoti Ganguly',
     author_email='debojyotiganguly70@gmail.com',
-    license='Zlib',
+    license='MIT',
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
     ],
     packages=['blueEngine'],
     include_package_data=True,
```

