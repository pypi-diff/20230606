# Comparing `tmp/pydraw-2.2a6.tar.gz` & `tmp/pydraw-2.2a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydraw-2.2a6.tar", last modified: Tue Dec 20 05:28:23 2022, max compression
+gzip compressed data, was "pydraw-2.2a7.tar", last modified: Tue Jun  6 18:46:19 2023, max compression
```

## Comparing `pydraw-2.2a6.tar` & `pydraw-2.2a7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 noah       (501) staff       (20)        0 2022-12-20 05:28:23.902559 pydraw-2.2a6/
--rw-r--r--   0 noah       (501) staff       (20)    35148 2022-11-03 15:19:06.000000 pydraw-2.2a6/LICENSE.md
--rw-r--r--   0 noah       (501) staff       (20)    10789 2022-12-20 05:28:23.902325 pydraw-2.2a6/PKG-INFO
--rw-r--r--   0 noah       (501) staff       (20)    10419 2022-11-21 19:27:27.000000 pydraw-2.2a6/README.md
-drwxr-xr-x   0 noah       (501) staff       (20)        0 2022-12-20 05:28:23.899255 pydraw-2.2a6/pydraw/
--rw-r--r--   0 noah       (501) staff       (20)      283 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/__init__.py
--rw-r--r--   0 noah       (501) staff       (20)    16312 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/color.py
--rw-r--r--   0 noah       (501) staff       (20)     5130 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/compound.py
--rw-r--r--   0 noah       (501) staff       (20)      136 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/errors.py
--rw-r--r--   0 noah       (501) staff       (20)     6647 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/location.py
--rw-r--r--   0 noah       (501) staff       (20)   201829 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/objects.py
--rw-r--r--   0 noah       (501) staff       (20)    26065 2022-11-03 15:19:06.000000 pydraw-2.2a6/pydraw/overload.py
--rw-r--r--   0 noah       (501) staff       (20)     2690 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/scene.py
--rw-r--r--   0 noah       (501) staff       (20)    31074 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/screen.py
--rw-r--r--   0 noah       (501) staff       (20)     9368 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/sound.py
--rw-r--r--   0 noah       (501) staff       (20)   143854 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/turtle.py
--rw-r--r--   0 noah       (501) staff       (20)     1447 2022-12-20 05:27:39.000000 pydraw-2.2a6/pydraw/util.py
-drwxr-xr-x   0 noah       (501) staff       (20)        0 2022-12-20 05:28:23.899909 pydraw-2.2a6/pydraw.egg-info/
--rw-r--r--   0 noah       (501) staff       (20)    10789 2022-12-20 05:28:23.000000 pydraw-2.2a6/pydraw.egg-info/PKG-INFO
--rw-r--r--   0 noah       (501) staff       (20)      729 2022-12-20 05:28:23.000000 pydraw-2.2a6/pydraw.egg-info/SOURCES.txt
--rw-r--r--   0 noah       (501) staff       (20)        1 2022-12-20 05:28:23.000000 pydraw-2.2a6/pydraw.egg-info/dependency_links.txt
--rw-r--r--   0 noah       (501) staff       (20)        7 2022-12-20 05:28:23.000000 pydraw-2.2a6/pydraw.egg-info/requires.txt
--rw-r--r--   0 noah       (501) staff       (20)       13 2022-12-20 05:28:23.000000 pydraw-2.2a6/pydraw.egg-info/top_level.txt
--rw-r--r--   0 noah       (501) staff       (20)      103 2022-11-03 15:19:06.000000 pydraw-2.2a6/pyproject.toml
--rw-r--r--   0 noah       (501) staff       (20)       38 2022-12-20 05:28:23.902600 pydraw-2.2a6/setup.cfg
--rw-r--r--   0 noah       (501) staff       (20)      751 2022-12-20 05:28:15.000000 pydraw-2.2a6/setup.py
-drwxr-xr-x   0 noah       (501) staff       (20)        0 2022-12-20 05:28:23.902123 pydraw-2.2a6/tests/
--rw-r--r--   0 noah       (501) staff       (20)       40 2022-12-20 05:27:39.000000 pydraw-2.2a6/tests/__init__.py
--rw-r--r--   0 noah       (501) staff       (20)     2601 2022-12-20 05:27:39.000000 pydraw-2.2a6/tests/algorithms_test.py
--rw-r--r--   0 noah       (501) staff       (20)     1543 2022-12-20 05:27:39.000000 pydraw-2.2a6/tests/blank_test.py
--rw-r--r--   0 noah       (501) staff       (20)      607 2022-12-20 05:27:39.000000 pydraw-2.2a6/tests/color_test.py
--rw-r--r--   0 noah       (501) staff       (20)      675 2022-12-20 05:27:39.000000 pydraw-2.2a6/tests/image_test.py
--rw-r--r--   0 noah       (501) staff       (20)      129 2022-11-03 15:19:06.000000 pydraw-2.2a6/tests/input_test.py
--rw-r--r--   0 noah       (501) staff       (20)     2927 2022-11-03 15:19:06.000000 pydraw-2.2a6/tests/launcher.py
--rw-r--r--   0 noah       (501) staff       (20)       50 2022-11-03 15:19:06.000000 pydraw-2.2a6/tests/line_test.py
--rw-r--r--   0 noah       (501) staff       (20)     1139 2022-12-20 05:27:39.000000 pydraw-2.2a6/tests/location_test.py
--rw-r--r--   0 noah       (501) staff       (20)     2746 2022-12-20 05:27:39.000000 pydraw-2.2a6/tests/objects_test.py
--rw-r--r--   0 noah       (501) staff       (20)      449 2022-11-03 15:19:06.000000 pydraw-2.2a6/tests/overload_test.py
--rw-r--r--   0 noah       (501) staff       (20)     1741 2022-12-20 05:27:39.000000 pydraw-2.2a6/tests/polygon_test.py
--rw-r--r--   0 noah       (501) staff       (20)     1412 2022-11-03 15:19:06.000000 pydraw-2.2a6/tests/scene_test.py
--rw-r--r--   0 noah       (501) staff       (20)     1255 2022-12-20 05:27:39.000000 pydraw-2.2a6/tests/screen_test.py
--rw-r--r--   0 noah       (501) staff       (20)       51 2022-11-03 15:19:06.000000 pydraw-2.2a6/tests/text_test.py
--rw-r--r--   0 noah       (501) staff       (20)     3775 2022-12-20 05:27:39.000000 pydraw-2.2a6/tests/tutorial.py
+drwxr-xr-x   0 noah       (501) staff       (20)        0 2023-06-06 18:46:19.801058 pydraw-2.2a7/
+-rw-r--r--   0 noah       (501) staff       (20)    35148 2022-11-03 15:19:06.000000 pydraw-2.2a7/LICENSE.md
+-rw-r--r--   0 noah       (501) staff       (20)    10789 2023-06-06 18:46:19.800839 pydraw-2.2a7/PKG-INFO
+-rw-r--r--   0 noah       (501) staff       (20)    10419 2022-11-21 19:27:27.000000 pydraw-2.2a7/README.md
+drwxr-xr-x   0 noah       (501) staff       (20)        0 2023-06-06 18:46:19.796018 pydraw-2.2a7/pydraw/
+-rw-r--r--   0 noah       (501) staff       (20)      283 2022-12-20 05:27:39.000000 pydraw-2.2a7/pydraw/__init__.py
+-rw-r--r--   0 noah       (501) staff       (20)    16481 2023-01-02 18:04:34.000000 pydraw-2.2a7/pydraw/color.py
+-rw-r--r--   0 noah       (501) staff       (20)    11292 2023-06-06 18:23:12.000000 pydraw-2.2a7/pydraw/compound.py
+-rw-r--r--   0 noah       (501) staff       (20)      136 2022-12-20 05:27:39.000000 pydraw-2.2a7/pydraw/errors.py
+-rw-r--r--   0 noah       (501) staff       (20)     6647 2022-12-20 05:27:39.000000 pydraw-2.2a7/pydraw/location.py
+-rw-r--r--   0 noah       (501) staff       (20)   205312 2023-06-04 19:34:38.000000 pydraw-2.2a7/pydraw/objects.py
+-rw-r--r--   0 noah       (501) staff       (20)    26065 2022-11-03 15:19:06.000000 pydraw-2.2a7/pydraw/overload.py
+-rw-r--r--   0 noah       (501) staff       (20)     2690 2022-12-20 05:27:39.000000 pydraw-2.2a7/pydraw/scene.py
+-rw-r--r--   0 noah       (501) staff       (20)    31074 2022-12-20 05:27:39.000000 pydraw-2.2a7/pydraw/screen.py
+-rw-r--r--   0 noah       (501) staff       (20)     9368 2022-12-20 05:27:39.000000 pydraw-2.2a7/pydraw/sound.py
+-rw-r--r--   0 noah       (501) staff       (20)   143854 2022-12-20 05:27:39.000000 pydraw-2.2a7/pydraw/turtle.py
+-rw-r--r--   0 noah       (501) staff       (20)     1447 2022-12-20 05:27:39.000000 pydraw-2.2a7/pydraw/util.py
+drwxr-xr-x   0 noah       (501) staff       (20)        0 2023-06-06 18:46:19.796929 pydraw-2.2a7/pydraw.egg-info/
+-rw-r--r--   0 noah       (501) staff       (20)    10789 2023-06-06 18:46:19.000000 pydraw-2.2a7/pydraw.egg-info/PKG-INFO
+-rw-r--r--   0 noah       (501) staff       (20)      729 2023-06-06 18:46:19.000000 pydraw-2.2a7/pydraw.egg-info/SOURCES.txt
+-rw-r--r--   0 noah       (501) staff       (20)        1 2023-06-06 18:46:19.000000 pydraw-2.2a7/pydraw.egg-info/dependency_links.txt
+-rw-r--r--   0 noah       (501) staff       (20)       17 2023-06-06 18:46:19.000000 pydraw-2.2a7/pydraw.egg-info/requires.txt
+-rw-r--r--   0 noah       (501) staff       (20)       13 2023-06-06 18:46:19.000000 pydraw-2.2a7/pydraw.egg-info/top_level.txt
+-rw-r--r--   0 noah       (501) staff       (20)      103 2022-11-03 15:19:06.000000 pydraw-2.2a7/pyproject.toml
+-rw-r--r--   0 noah       (501) staff       (20)       38 2023-06-06 18:46:19.801110 pydraw-2.2a7/setup.cfg
+-rw-r--r--   0 noah       (501) staff       (20)      793 2023-06-03 20:18:47.000000 pydraw-2.2a7/setup.py
+drwxr-xr-x   0 noah       (501) staff       (20)        0 2023-06-06 18:46:19.800496 pydraw-2.2a7/tests/
+-rw-r--r--   0 noah       (501) staff       (20)       40 2022-12-20 05:27:39.000000 pydraw-2.2a7/tests/__init__.py
+-rw-r--r--   0 noah       (501) staff       (20)     2601 2022-12-20 05:27:39.000000 pydraw-2.2a7/tests/algorithms_test.py
+-rw-r--r--   0 noah       (501) staff       (20)     1543 2022-12-20 05:27:39.000000 pydraw-2.2a7/tests/blank_test.py
+-rw-r--r--   0 noah       (501) staff       (20)      607 2022-12-20 05:27:39.000000 pydraw-2.2a7/tests/color_test.py
+-rw-r--r--   0 noah       (501) staff       (20)      675 2022-12-20 05:27:39.000000 pydraw-2.2a7/tests/image_test.py
+-rw-r--r--   0 noah       (501) staff       (20)      129 2022-11-03 15:19:06.000000 pydraw-2.2a7/tests/input_test.py
+-rw-r--r--   0 noah       (501) staff       (20)     2927 2022-11-03 15:19:06.000000 pydraw-2.2a7/tests/launcher.py
+-rw-r--r--   0 noah       (501) staff       (20)     2740 2023-01-03 23:47:36.000000 pydraw-2.2a7/tests/line_test.py
+-rw-r--r--   0 noah       (501) staff       (20)     1139 2022-12-20 05:27:39.000000 pydraw-2.2a7/tests/location_test.py
+-rw-r--r--   0 noah       (501) staff       (20)     2746 2022-12-20 05:27:39.000000 pydraw-2.2a7/tests/objects_test.py
+-rw-r--r--   0 noah       (501) staff       (20)      449 2022-11-03 15:19:06.000000 pydraw-2.2a7/tests/overload_test.py
+-rw-r--r--   0 noah       (501) staff       (20)     1741 2022-12-20 05:27:39.000000 pydraw-2.2a7/tests/polygon_test.py
+-rw-r--r--   0 noah       (501) staff       (20)     1412 2022-11-03 15:19:06.000000 pydraw-2.2a7/tests/scene_test.py
+-rw-r--r--   0 noah       (501) staff       (20)     1255 2022-12-20 05:27:39.000000 pydraw-2.2a7/tests/screen_test.py
+-rw-r--r--   0 noah       (501) staff       (20)       51 2022-11-03 15:19:06.000000 pydraw-2.2a7/tests/text_test.py
+-rw-r--r--   0 noah       (501) staff       (20)     3775 2022-12-20 05:27:39.000000 pydraw-2.2a7/tests/tutorial.py
```

### Comparing `pydraw-2.2a6/LICENSE.md` & `pydraw-2.2a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/PKG-INFO` & `pydraw-2.2a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydraw
-Version: 2.2a6
+Version: 2.2a7
 Summary: A package designed to make graphics with Python simple and easy!
 Home-page: https://github.com/pydraw/pydraw
 Author: Noah Coetsee
 Author-email: noah@noahcoetsee.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydraw-2.2a6/README.md` & `pydraw-2.2a7/README.md`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/pydraw/color.py` & `pydraw-2.2a7/pydraw/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,17 @@
         :param color: the color to convert
         :return: a tuple representing RGB
         """
 
         if color.name() is not None:
             try:
                 rgb = turtle.getcanvas().winfo_rgb(color.name())
-            except tk.TclError:
+            except tk.TclError as e:
+                if hasattr(e, 'message') and e.message == 'can\'t invoke "winfo" command: application has been destroyed':
+                    return 255, 255, 255
                 raise PydrawError('Color-string does not exist: ', color.name())
             except turtle.Terminator:
                 return 255, 255, 255  # Just return black if Program is shutting down.
         elif color.hex() is not None:
             hexval = color.hex().replace('#', '')
 
             if len(hexval) != 6:
```

### Comparing `pydraw-2.2a6/pydraw/location.py` & `pydraw-2.2a7/pydraw/location.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/pydraw/objects.py` & `pydraw-2.2a7/pydraw/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
         self._drawing = False
 
         self._history = []  # stores old line _refs for clearing
         self._ref = None  # currentLine
         self._setup()
 
+    def location(self) -> Location:
+        return self._location
+
     def move(self, *args, **kwargs):
         """
         Adds a new coordinate to the pen line with a passed difference from the previous coordinate.
         Requires coordinates to be len > 0.
 
         Can take two numbers (dx, dy), a tuple, or a Location
         :param dx: the dx to move by
@@ -80,18 +83,18 @@
             if name.lower() == 'dy':
                 diff = (diff[0], value)
 
         if not len(self._coordinates) > 0:
             raise PydrawError('No starting coordinate to move Pen from.')
 
         if self._drawing:
-            location = Location(self._coordinates[-1].x() + diff[0], self._coordinates[-1].y() + diff[1])
+            location = Location(self._coordinates[-1].x() + diff[0], self._coordinates[-1].y() + diff[1]) if len(self._coordinates) > 0 else self._location.move(diff[0], diff[1])
             self._coordinates.append(location)
         else:
-            self._location = Location(self._coordinates[-1].x() + diff[0], self._coordinates[-1].y() + diff[1])
+            self._location = Location(self._coordinates[-1].x() + diff[0], self._coordinates[-1].y() + diff[1]) if len(self._coordinates) > 0 else self._location.move(diff[0], diff[1])
 
         self._update()
 
     def moveto(self, *args, **kwargs):
         """
         Adds a new coordinate to the pen line.
 
@@ -219,15 +222,15 @@
 
     def top(self, top: bool = None) -> bool:
         if top is not None:
             verify(top, bool)
             self._top = top
             self._update()
 
-        return self._top()
+        return self._top
 
     def _setup(self):
         # noinspection PyProtectedMember
         self._ref = self._screen._canvas.create_line(0, 0, 0, 0, fill="", width=2, capstyle=tk.ROUND)
 
     # noinspection PyProtectedMember
     def _update(self):
@@ -265,15 +268,15 @@
                 for line in self._history:
                     self._screen._canvas.tag_raise(line)
 
 
 class Object:
     """
     A base object containing a location and screen. This ensures coordinates are
-    done with the root at the top left corner, and not at the center.
+    done with the root in the top left corner, and not at the center.
     """
 
     def __init__(self, screen: Screen, x: float = 0, y: float = 0, location: Location = None):
         verify(screen, Screen, x, (float, int), y, (float, int), location, Location)
 
         self._screen = screen
         self._location = location if location is not None else Location(x, y)
@@ -316,14 +319,15 @@
         :return: None
         """
 
         self._location.moveto(*args, **kwargs)
         self.update()
 
     def _get_real_location(self):
+        # todo: move this to renderable
         real_x = self.x() + self.width() / 2 - (self._screen.width() / 2)
         real_y = -self.y() + self._screen.height() / 2 - self.height() / 2
 
         return real_x, real_y
 
     def front(self) -> None:
         """
@@ -367,778 +371,780 @@
     # # noinspection PyProtectedMember
     # def add(self) -> None:
     #     """
     #     Should only be used to add an object that has been removed (via .remove() or Screen.clear()
     #     :return: None
     #     """
     #     if self in self._screen.objects():
-    #         raise PydrawError('Error adding object: Object alraedy in Screen.objects()')
+    #         raise PydrawError('Error adding object: Object already in Screen.objects()')
     #
     #     self._setup()
     #     self._screen._add(self)
 
     def _setup(self):
         """
         To be overriden.
         """
         pass
 
     # noinspection PyProtectedMember
     def _check(self) -> None:
         if self._screen is None or Screen._TERMINATING:
-            return  # We don't wanna mess with how stupid tk and turtle are.
+            return  # We don't want to mess with how stupid tk and turtle are.
 
         if not self._screen.contains(self):
             if self in self._screen._gridlines or self in self._screen._helpers:
                 return
 
             raise PydrawError('Cannot update or draw object that is not on the Screen!')
 
     def update(self) -> None:
         """
         To be overriden.
         """
         pass
 
 
-class _Renderable(Object):
-    def __init__(self, screen: Screen, x: float = 0, y: float = 0, width: float = 10, height: float = 10,
-                 color: Color = Color('black'),
-                 border: Color = Color.NONE,
-                 fill: bool = True,
-                 rotation: float = 0,
-                 visible: bool = True,
-                 location: Location = None):
-        super().__init__(screen, x, y, location)
-        self._width = width
-        self._height = height
-        self._color = color
-        self._border = border if border is not None else Color('')
-        self._borderwidth = 1
-        self._fill = fill
-        self._angle = rotation
-        self._last_angle = rotation
-        self._visible = visible
-
-        self._setup()
-
-    def width(self, width: float = None) -> float:
-        """
-        Get or set the width of the object.
-        :param width: the width to set to in pixels, if any
-        :return: the width of the object
-        """
-
-        if width is not None:
-            verify(width, (float, int))
-            self._width = width
-            self.update()
-
-        return self._width
-
-    def height(self, height: float = None) -> float:
-        """
-        Get or set the height of the object
-        :param height: the height to set to in pixels, if any
-        :return: the height of the object
-        """
-
-        if height is not None:
-            verify(height, (float, int))
-            self._height = height
-            self.update()
-
-        return self._height
-
-    def center(self, *args, **kwargs) -> Location:
-        """
-        Returns the location of the center
-        :param move_to: if defined, Move the center to a new Location (Easily center objects!)
-        :param x: if defined, move the center x-coordinate to the specified value
-        :param y: if defined, move the center y-coordinate to the specified value
-        :return: Location object representing center of Renderable
-        """
-
-        centroid = False
-        if len(args) == 0:
-            if len(kwargs) > 0:
-                if 'centroid' in kwargs:
-                    if type(kwargs['centroid']) is bool:
-                        centroid = kwargs['centroid']
-                    else:
-                        raise InvalidArgumentError(
-                            ".center() requires a boolean for centroid (whether to return a bounds "
-                            "center or a calculated centroid).")
-            return self._center(centroid=centroid)
-
-        location = Location(self._center())
-
-        if len(args) != 0:
-            if type(args[0]) is Location or type(args[0]) is tuple:
-                location.moveto(args[0])
-            elif type(args[0]) == float or type(args[0]) is int:
-                if len(args) != 2:
-                    raise InvalidArgumentError(".center() requires both x and y passed unless using keywords.")
-                elif type(args[1]) is not float and type(args[1]) is not int:
-                    raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
-
-                location.moveto(args[0], args[1])
-            else:
-                raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
-
-        if len(kwargs) != 0:
-            if 'move_to' in kwargs:
-                if type(kwargs['move_to']) is Location or type(kwargs['move_to']) is tuple:
-                    location.moveto(kwargs['move_to'])
-                else:
-                    raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
-
-            if 'x' in kwargs:
-                if type(kwargs['x']) is float or type(kwargs['x']) is int:
-                    location.x(kwargs['x'])
-                else:
-                    raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
-            if 'y' in kwargs:
-                if type(kwargs['y']) is float or type(kwargs['y']) is int:
-                    location.y(kwargs['y'])
-                else:
-                    raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
-            if 'centroid' in kwargs:
-                if type(kwargs['centroid']) is bool:
-                    centroid = kwargs['centroid']
-                else:
-                    raise InvalidArgumentError(".center() requires a boolean for centroid (whether to return a bounds "
-                                               "center or a calculated centroid).")
-
-        return self._center(location, centroid)
-
-    def _center(self, move_to: Location = None, centroid: bool = False):
-        if move_to is not None:
-            verify(move_to, Location)
-            self.moveto(move_to.x() - self.width() / 2, move_to.y() - self.height() / 2)
-
-        if centroid:
-            return Location(self.x() + self.width() / 2, self.y() + self.height() / 2)
-
-        # We gonna create a centroid so we can rotate the points around a realistic center
-        # Sorry for those of you that get weird rotations..
-        x_list = []
-        y_list = []
-
-        for vertex in self._vertices:
-            x_list.append(vertex.x())
-            y_list.append(vertex.y())
-
-        # Create a simple centroid (not full centroid)
-        centroid_x = sum(x_list) / len(y_list)
-        centroid_y = sum(y_list) / len(x_list)
-
-        return Location(centroid_x, centroid_y)
-
-    def rotation(self, angle: float = None) -> float:
-        """
-        Get or set the rotation of the object.
-        :param angle: the angle to set the rotation to in degrees, if any
-        :return: the angle of the object's rotation in degrees
-        """
-
-        if angle is not None:
-            verify(angle, (float, int))
-            self._angle = angle
-            self.update()
-
-        return self._angle % 360
-
-    def rotate(self, angle_diff: float = 0) -> None:
-        """
-        Rotate the angle of the object by a difference, in degrees
-        :param angle_diff: the angle difference to rotate by
-        :return: None
-        """
-
-        verify(angle_diff, (float, int))
-        self.rotation(self._angle + angle_diff)
-
-    def angleto(self, obj) -> float:
-        """
-        Retrieve the angle between this object and another (based on 0 degrees at 12 o'clock)
-        :param obj: the Object/Location to get the angle to.
-        :return: the angle in degrees as a float
-        """
-
-        if isinstance(obj, Object):
-            obj = obj.location()
-        elif type(obj) is not Location and type(obj) is not tuple:
-            raise InvalidArgumentError('Renderable#lookat() must be passed either a renderable or a location!')
-
-        location = Location(obj[0], obj[1])
-        # theta = -math.atan2(location.x() - self.x(), location.y() - self.y()) - math.radians(self.rotation())
-        theta = math.atan2(location.y() - self.center().y(), location.x() - self.center().x()) \
-            - math.radians(self.rotation()) + math.pi / 2
-        theta = math.degrees(theta)
-
-        return theta
-
-    def lookat(self, obj) -> None:
-        """
-        Look at another object (Objects or Locations)
-        :param obj: the Object/Location to look at.
-        :return: None
-        """
-
-        theta = self.angleto(obj)
-        self.rotate(theta)
-
-    def forward(self, distance: float) -> None:
-        """
-        Move the Renderable forward by distance at its current heading (rotation/angle)
-        :param distance: the distance to move forward (hypotenuse)
-        :return: None
-        """
-
-        dx = distance * math.sin(math.radians(self._angle))
-        dy = distance * -math.cos(math.radians(self._angle))
-
-        self.move(dx, dy)
-
-    def backward(self, distance: float) -> None:
-        """
-        Move the Renderable backward by distance at its current heading (rotation/angle)
-        :param distance: the distance to move backward (hypotenuse)
-        :return: None
-        """
-
-        self.forward(-distance)
-
-    def color(self, color: Color = None) -> Color:
-        """
-        Get or set the color of the object
-        :param color: the color to set to, if any
-        :return: the color of the object
-        """
-
-        if color is not None:
-            verify(color, Color)
-            self._color = color
-            self.update()
-
-        return self._color
-
-    def border(self, color: Color = None, width: float = None, fill: bool = None) -> Color:
-        """
-        Add or get the border of the object
-        :param color: the color to set the border too, set to Color.NONE to remove border
-        :param width: the width of the border
-        :param fill: whether to fill the polygon.
-        :return: The Color of the border
-        """
-
-        update = False
-
-        if color is not None:
-            verify(color, Color)
-            self._border = color
-            update = True
-        if fill is not None:
-            verify(fill, bool)
-            self._fill = fill
-            update = True
-        if width is not None:
-            verify(width, (float, int))
-            self._borderwidth = width
-            update = True
-
-        if update:
-            self.update()
-
-        return self._border
-
-    def border_width(self, width: float = None) -> float:
-        """
-        Gets or sets the border width
-        :param width: the border width to set to
-        :return: the border width
-        """
-
-        if width is not None:
-            verify(width, (float, int))
-            self._borderwidth = width
-            self.update()
-
-        return self._borderwidth
-
-    def fill(self, fill: bool = None) -> bool:
-        """
-        Returns or sets the current fill boolean
-        :param fill: a new fill value, whether to fill the polygon
-        :return: the fill value
-        """
-
-        if fill is not None:
-            verify(fill, bool)
-            self._fill = fill
-            self.update()
-
-        return self._fill
-
-    def distance(self, obj) -> float:
-        """
-        Returns the distance between two objs or locations in pixels (center to center)
-        :param obj: the Renderable/location to check distance between
-        :return: the distance between this obj and the passed Renderable/Location.
-        """
-
-        if type(obj) is not Location and not isinstance(obj, Renderable):
-            raise InvalidArgumentError(f'.distance() must be passed a Renderable or a Location! '
-                                       f'(Passed: {type(obj)}')
-
-        location = obj if type(obj) is Location else obj.center()
-
-        return math.sqrt((location.x() - self.center().x()) ** 2 + (location.y() - self.center().y()) ** 2)
-
-    def visible(self, visible: bool = None) -> bool:
-        """
-        Get or set the visibility of the renderable.
-        :param visible: the new visibility value, if any
-        :return: the visibility value
-        """
-
-        if visible is not None:
-            verify(visible, bool)
-            self._visible = visible
-            self.update()
-
-        return self._visible
-
-    def transform(self, transform: tuple = None) -> tuple:
-        """
-        Get or set the transform of the Renderable.
-        Transforms represent the width, height, and rotation of Renderables.
-
-        You can retrieve a Transform from a Renderable with this method and set the transform the same way.
-        :param transform: the transform to set to, if any.
-        :return: the transform
-        """
-
-        if transform is not None:
-            verify(transform, tuple)
-            if not len(transform) == 3:
-                raise InvalidArgumentError('Ensure you are passing in a Transform from another object or a '
-                                           'tuple in the following order: (width, height, rotation)')
-            verify(transform[0], (float, int), transform[1], (float, int), transform[2], (float, int))
-            self.width(transform[0])
-            self.height(transform[1])
-            self.rotation(transform[2])
-
-        return self.width(), self.height(), self.rotation()
-
-    def clone(self):
-        """
-        Clone this renderable!
-        :return: a Renderable
-        """
-
-        constructor = type(self)
-
-        return constructor(self._screen, self.x(), self.y(), self.width(), self.height(), self.color(), self.border(),
-                           self.fill(), self.rotation(), self.visible())
-
-    def vertices(self) -> list:
-        """
-        Returns the list of vertices for the Renderable.
-        (The vertices will be returned clockwise, starting from the top-leftmost point)
-        :return: a list of Locations representing the vertices
-        """
-        return self._get_vertices()
-
-    def bounds(self) -> (Location, float, float):
-        """
-        Get the location and dimensions of a bounding box that contains the entire shape
-        :return: a tuple containing the Location, width, and height.
-        """
-
-        x0, y0, x1, y1 = self._screen._screen.cv.bbox(self._ref)
-        location = self._screen.create_location(x0, y0, canvas=True)
-
-        return location, (x1 - x0), (y1 - y0)
-
-    def contains(self, *args) -> bool:
-        """
-        Returns whether or not a Location is contained within the object.
-        :param args: You may pass in either two numbers, a Location, or a tuple containing and x and y point.
-        :return: a boolean value representing whether or not the point is within the vertices of the object.
-        """
-
-        x, y = 0, 0
-        count = 0
-
-        if len(args) == 1:
-            verify(args, (tuple, Location))
-            if type(args[0]) is Location:
-                x = args[0].x()
-                y = args[0].y()
-            elif type(args[0]) is tuple and len(args[0]) == 2:
-                x = args[0][0]
-                y = args[0][1]
-        elif len(args) == 2:
-            verify(args[0], (float, int), args[1], (float, int))
-            if type(args[0]) is not float and type(args[0]) is not int \
-                    and type(args[1]) is not float and type(args[1]) is not int:
-                raise InvalidArgumentError('Passed arguments must be numbers (x, y), '
-                                           'or you may pass a location/tuple.')
-            x = args[0]
-            y = args[1]
-        else:
-            raise InvalidArgumentError('You must pass in a tuple, Location, or two numbers (x, y)!')
-
-        # If the point isn't remotely near us, we don't need to perform any calculations.
-        if not isinstance(self, CustomRenderable) and self._angle == 0:
-            if self.y() > 0 and self.x() > 0:
-                if not (self.x() <= x <= (self.x() + self.width()) and self.y() <= y <= (self.y() + self.height())):
-                    return False
-
-        # the contains algorithm uses the line-intersects algorithm to determine if a point is within a polygon.
-        # we are going to cast a ray from our point to the positive x. (left to right)
-
-        shape = self.vertices()
-        shape = tuple(shape[:]) + (shape[0],)  # Add the first vertex back again to get the last edge.
-
-        point1 = shape[0]
-        for i in range(1, len(shape)):
-            # A cool trick that gets the next index in an array, or the first index if i is the last index.
-            # (since we start at index 1)
-            point2 = shape[i % len(shape)]
-
-            # make sure we're in the ballpark on the y axis (actually able to intersect on the x axis)
-            if y > min(point1.y(), point2.y()):
-
-                # Same thing as above
-                if y <= max(point1.y(), point2.y()):
-
-                    # Make sure our x is at least less than the max x of this line. (since we're travelling right)
-                    if x <= max(point1.x(), point2.x()):
-
-                        # If our y's are equal, that means this line is flat on the x, which makes us tricked until now.
-                        # (We now realize we were never in the ballpark in the first place.
-                        if point1.y() != point2.y():
-
-                            # Now we get a possible intersection point from left to right.
-                            intersects_x = (y - point1.y()) * (point2.x() - point1.x()) / \
-                                           (point2.y() - point1.y()) + point1.x()
-
-                            # if the line was vertical or we actually intersected it
-                            if point1.x() == point2.x() or x <= intersects_x:
-                                count += 1
-
-            # move up the ladder next vertices and edge
-            point1 = point2
-
-        return not (count % 2 == 0)
-
-    def overlaps(self, other: 'Renderable') -> bool:
-        """
-        Returns if this object is overlapping with the passed object.
-        :param other: another Renderable instance.
-        :return: true if they are overlapping, false if not.
-        """
-
-        if not isinstance(other, Renderable):
-            raise TypeError('Passed non-renderable into Renderable#overlaps(), which takes only Renderables!')
-
-        x = self.x()
-        y = self.y()
-        width = self.width()
-        height = self.height()
-
-        other_x = other.x()
-        other_y = other.y()
-        other_width = other.width()
-        other_height = other.height()
-
-        # Only optimize if the angle is not zero.
-        if self._angle % 360 == 0 and other._angle % 360 == 0:
-            min_ax = x
-            max_ax = x + width
-
-            min_bx = other_x
-            max_bx = other_x + other_width
-
-            min_ay = y
-            max_ay = y + height
-
-            min_by = other_y
-            max_by = other_y + other_height
-
-            a_left_b = max_ax < min_bx
-            a_right_b = min_ax > max_bx
-            a_above_b = min_ay > max_by
-            a_below_b = max_ay < min_by
-        else:
-            hypotenuse = math.sqrt(width ** 2 + height ** 2) + 1
-            other_hypotenuse = math.sqrt(other_width ** 2 + other_height ** 2) + 1
-
-            center = Location(x + width / 2, y + height / 2)
-            other_center = Location(other_x + other_width / 2, other_y + other_height / 2)
-
-            min_ax = center.x() - (hypotenuse / 2)
-            max_ax = center.x() + (hypotenuse / 2)
-
-            min_bx = other_center.x() - (other_hypotenuse / 2)
-            max_bx = other_center.x() + (other_hypotenuse / 2)
-
-            min_ay = center.y() - (hypotenuse / 2)
-            max_ay = center.y() + (hypotenuse / 2)
-
-            min_by = other_center.y() - (other_hypotenuse / 2)
-            max_by = other_center.y() + (other_hypotenuse / 2)
-
-            a_left_b = max_ax < min_bx
-            a_right_b = min_ax > max_bx
-            a_above_b = min_ay > max_by
-            a_below_b = max_ay < min_by
-
-        # Do a base check to make sure they are even remotely near each other.
-        # TODO: Re-optimize with rotation in mind.
-        # if other._angle % 360 == 0 and self._angle % 360 == 0:
-        if a_left_b or a_right_b or a_above_b or a_below_b:
-            return False
-
-        # Check if one shape is entirely inside the other shape
-        if (min_ax >= min_bx and max_ax <= max_bx) and (min_ay >= min_by and max_ay <= max_by):
-            return True
-
-        if (min_bx >= min_ax and max_bx <= max_ax) and (min_by >= min_ay and max_by <= max_ay):
-            return True
-
-        # Next we are going to use a sweeping line algorithm.
-        # Essentially we will process the lines on the x axis, one coordinate at a time (imagine a vertical line scan).
-        # Then we will look for their orientations. We will essentially make sure its impossible they do not cross.
-        shape1 = self.vertices()
-
-        # noinspection PyProtectedMember
-        shape2 = other.vertices()
-
-        # Orientation method that will determine if it is a triangle (and in what direction [cc or ccw]) or a line.
-        def orientation(point1: Location, point2: Location, point3: Location) -> str:
-            """
-            Internal method that will determine the orientation of three points. They can be a clockwise triangle,
-            counterclockwise triangle, or a co-linear line segment.
-            :param point1: the first point of the main line segment
-            :param point2: the second point of the main line segment
-            :param point3: the third point to check from another line segment
-            :return: the orientation of the passed points
-            """
-            result = (float(point2.y() - point1.y()) * (point3.x() - point2.x())) - \
-                     (float(point2.x() - point1.x()) * (point3.y() - point2.y()))
-
-            if result > 0:
-                return 'clockwise'
-            elif result < 0:
-                return 'counter-clockwise'
-            else:
-                return 'co-linear'
-
-        def point_on_segment(point1: Location, point2: Location, point3: Location) -> bool:
-            """
-            Returns if point3 lies on the segment formed by point1 and point2.
-            """
-
-            return max(point1.x(), point3.x()) >= point2.x() >= min(point1.x(), point3.x()) \
-                   and max(point1.y(), point3.y()) >= point2.y() >= min(point1.y(), point3.y())
-
-        # Okay to begin actually detecting orientations, we want to loop through some edges. But only ones that are
-        # relevant. In order to do this we will first have to turn the list of vertices into a list of edges.
-        # Then we will look through the lists of edges and find the ones closest to each other.
-
-        shape1_edges = []
-        shape2_edges = []
-
-        shape1 = tuple(shape1[:]) + (shape1[0],)
-        shape2 = tuple(shape2[:]) + (shape2[0],)
-
-        shape1_point1 = shape1[0]
-        for i in range(1, len(shape1)):
-            shape1_point2 = shape1[i % len(shape1)]  # 1, 2, 3, 3 % 5
-            shape1_edges.append((shape1_point1, shape1_point2))
-            shape1_point1 = shape1_point2
-
-        shape2_point1 = shape2[0]
-        for i in range(1, len(shape2)):
-            shape2_point2 = shape2[i % len(shape2)]
-            shape2_edges.append((shape2_point1, shape2_point2))
-            shape2_point1 = shape2_point2
-
-        # Now we are going to test the four orientations that the segments form
-        for edge1 in shape1_edges:
-            for edge2 in shape2_edges:
-                orientation1 = orientation(edge1[0], edge1[1], edge2[0])
-                orientation2 = orientation(edge1[0], edge1[1], edge2[1])
-                orientation3 = orientation(edge2[0], edge2[1], edge1[0])
-                orientation4 = orientation(edge2[0], edge2[1], edge1[1])
-
-                # If orientations 1 and 2 are different as well as 3 and 4 then they intersect!
-                if orientation1 != orientation2 and orientation3 != orientation4:
-                    return True
-
-                # There's some special cases we should check where a point from one segment is on the other segment
-                if orientation1 == 'co-linear' and point_on_segment(edge1[0], edge2[0], edge1[1]):
-                    return True
-
-                if orientation2 == 'co-linear' and point_on_segment(edge1[0], edge2[1], edge1[1]):
-                    return True
-
-                if orientation3 == 'co-linear' and point_on_segment(edge2[0], edge1[0], edge2[1]):
-                    return True
-
-                if orientation4 == 'co-linear' and point_on_segment(edge2[0], edge1[1], edge2[1]):
-                    return True
-
-        # If none of the above conditions were ever met we just return False. Hopefully we are correct xD.
-        return False
-
-    # noinspection PyProtectedMember
-    # noinspection PyUnresolvedReferences
-    def _get_vertices(self):
-        real_shape = self._vertices
-        # real_shape.reverse()
-        #
-        # min_distance = 999999
-        # top_left_index = 0
-        # for i, location in enumerate(real_shape):
-        #     distance = math.sqrt((location.x()) ** 2 + (location.y()) ** 2)
-        #     if distance < min_distance:
-        #         min_distance = distance
-        #         top_left_index = i
-        #
-        # real_shape = real_shape[top_left_index:] + real_shape[:top_left_index]
-
-        return real_shape
-
-    def _setup(self):
-        if not hasattr(self, '_shape'):
-            raise AttributeError('An error occured while initializing a Renderable: '
-                                 'Is _shape set? (Advanced Users Only)')
-
-        shape = self._shape  # List of normal vertices.
-
-        width = self._width
-        height = self._height
-
-        scale_factor = (width / PIXEL_RATIO, height / PIXEL_RATIO)
-
-        cx = 0
-        cy = 0
-
-        vertices = [Location(vertex[0], vertex[1]) for vertex in shape]
-
-        for vertex in vertices:
-            vertex.moveto(scale_factor[0] * (vertex.x() - cx) + cx, -scale_factor[1] * (vertex.y() - cy) + cy)
-
-            vertex.move(self.x() + width / 2, self.y() + height / 2)
-
-        self._vertices = vertices
-
-        self._vertices = self._rotate(self._vertices, self._angle)
-
-        tk_vertices = []  # we need to convert to tk's coordinate system.
-        for vertex in self._vertices:
-            tk_vertices.append((vertex.x() - (self._screen.width() / 2),
-                                (vertex.y() - (self._screen.height() / 2))))
-
-        state = tk.NORMAL if self._visible else tk.HIDDEN
-        color_state = self._color if self._fill else Color.NONE
-
-        # noinspection PyProtectedMember
-        self._ref = self._screen._canvas.create_polygon(
-            tk_vertices,
-            fill=self._screen._colorstr(color_state),
-            outline=self._screen._screen._colorstr(self._border.__value__()),
-            width=self._borderwidth,
-            state=state,
-            joinstyle=tk.MITER
-        )
-        # self.update() # CustomPolygon(self._screen, vertices)
-
-    def _rotate(self, vertices: list, angle: float, pivot: Location = None) -> list:
-        # We have to update here since we cannot remember previous rotations (update method call won't cut it)!
-        # vertices = self._vertices
-
-        # First get some values that we gonna use later
-        theta = math.radians(angle)
-        cosine = math.cos(theta)
-        sine = math.sin(theta)
-
-        if pivot is None:
-            centroid_x = self.center().x()
-            centroid_y = self.center().y()
-        else:
-            centroid_x = pivot.x()
-            centroid_y = pivot.y()
-
-        new_vertices = []
-        for vertex in vertices:
-            # We have to create these separately because they're ironically used in each others calculations xD
-            old_x = vertex.x() - centroid_x
-            old_y = vertex.y() - centroid_y
-
-            new_x = (old_x * cosine - old_y * sine) + centroid_x
-            new_y = (old_x * sine + old_y * cosine) + centroid_y
-            new_vertices.append(Location(new_x, new_y))
-
-        return new_vertices
-
-    def update(self):
-        self._check()
-
-        old_ref = self._ref
-        shape = self._shape  # List of normal vertices.
-
-        width = self._width
-        height = self._height
-
-        scale_factor = (width / PIXEL_RATIO, height / PIXEL_RATIO)
-
-        cx = 0
-        cy = 0
-
-        vertices = [Location(vertex[0], vertex[1]) for vertex in shape]
-        self._vertices = vertices
-
-        for vertex in vertices:
-            vertex.moveto(scale_factor[0] * (vertex.x() - cx) + cx, -scale_factor[1] * (vertex.y() - cy) + cy)
-
-            vertex.move(self.x() + width / 2, self.y() + height / 2)
-
-        self._vertices = self._rotate(self._vertices, self._angle)
-        self._last_angle = self._angle
-
-        tk_vertices = []  # we need to convert to tk's coordinate system.
-        for vertex in self._vertices:
-            tk_vertices.append((vertex.x() - (self._screen.width() / 2),
-                                (vertex.y() - (self._screen.height() / 2))))
-
-        state = tk.NORMAL if self._visible else tk.HIDDEN
-        color_state = self._color if self._fill else Color.NONE
-            
-        try:
-            # noinspection PyProtectedMember
-            self._ref = self._screen._canvas.create_polygon(
-                tk_vertices,
-                fill=self._screen._colorstr(color_state),
-                outline=self._screen._screen._colorstr(self._border.__value__()),
-                width=self._borderwidth,
-                state=state,
-                joinstyle=tk.MITER
-            )
-
-            self._screen._canvas.tag_lower(self._ref, old_ref)
-            self._screen._canvas.delete(old_ref)
-        except:
-            pass
-
+# class _Renderable(Object):
+#     def __init__(self, screen: Screen, x: float = 0, y: float = 0, width: float = 10, height: float = 10,
+#                  color: Color = Color('black'),
+#                  border: Color = Color.NONE,
+#                  fill: bool = True,
+#                  rotation: float = 0,
+#                  visible: bool = True,
+#                  location: Location = None):
+#         super().__init__(screen, x, y, location)
+#         self._width = width
+#         self._height = height
+#         self._color = color
+#         self._border = border if border is not None else Color('')
+#         self._border_width = 1
+#         self._fill = fill
+#         self._angle = rotation
+#         self._last_angle = rotation
+#         self._visible = visible
+#
+#         self._setup()
+#
+#     def width(self, width: float = None) -> float:
+#         """
+#         Get or set the width of the object.
+#         :param width: the width to set to in pixels, if any
+#         :return: the width of the object
+#         """
+#
+#         if width is not None:
+#             verify(width, (float, int))
+#             self._width = width
+#             self.update()
+#
+#         return self._width
+#
+#     def height(self, height: float = None) -> float:
+#         """
+#         Get or set the height of the object
+#         :param height: the height to set to in pixels, if any
+#         :return: the height of the object
+#         """
+#
+#         if height is not None:
+#             verify(height, (float, int))
+#             self._height = height
+#             self.update()
+#
+#         return self._height
+#
+#     def center(self, *args, **kwargs) -> Location:
+#         """
+#         Returns the location of the center
+#         :param move_to: if defined, Move the center to a new Location (Easily center objects!)
+#         :param x: if defined, move the center x-coordinate to the specified value
+#         :param y: if defined, move the center y-coordinate to the specified value
+#         :return: Location object representing center of Renderable
+#         """
+#
+#         centroid = False
+#         if len(args) == 0:
+#             if len(kwargs) > 0:
+#                 if 'centroid' in kwargs:
+#                     if type(kwargs['centroid']) is bool:
+#                         centroid = kwargs['centroid']
+#                     else:
+#                         raise InvalidArgumentError(
+#                             ".center() requires a boolean for centroid (whether to return a bounds "
+#                             "center or a calculated centroid).")
+#             return self._center(centroid=centroid)
+#
+#         location = Location(self._center())
+#
+#         if len(args) != 0:
+#             if type(args[0]) is Location or type(args[0]) is tuple:
+#                 location.moveto(args[0])
+#             elif type(args[0]) == float or type(args[0]) is int:
+#                 if len(args) != 2:
+#                     raise InvalidArgumentError(".center() requires both x and y passed unless using keywords.")
+#                 elif type(args[1]) is not float and type(args[1]) is not int:
+#                     raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
+#
+#                 location.moveto(args[0], args[1])
+#             else:
+#                 raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
+#
+#         if len(kwargs) != 0:
+#             if 'move_to' in kwargs:
+#                 if type(kwargs['move_to']) is Location or type(kwargs['move_to']) is tuple:
+#                     location.moveto(kwargs['move_to'])
+#                 else:
+#                     raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
+#
+#             if 'x' in kwargs:
+#                 if type(kwargs['x']) is float or type(kwargs['x']) is int:
+#                     location.x(kwargs['x'])
+#                 else:
+#                     raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
+#             if 'y' in kwargs:
+#                 if type(kwargs['y']) is float or type(kwargs['y']) is int:
+#                     location.y(kwargs['y'])
+#                 else:
+#                     raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
+#             if 'centroid' in kwargs:
+#                 if type(kwargs['centroid']) is bool:
+#                     centroid = kwargs['centroid']
+#                 else:
+#                     raise InvalidArgumentError(".center() requires a boolean for centroid (whether to return a bounds "
+#                                                "center or a calculated centroid).")
+#
+#         return self._center(location, centroid)
+#
+#     def _center(self, move_to: Location = None, centroid: bool = False):
+#         if move_to is not None:
+#             verify(move_to, Location)
+#             self.moveto(move_to.x() - self.width() / 2, move_to.y() - self.height() / 2)
+#
+#         if centroid:
+#             return Location(self.x() + self.width() / 2, self.y() + self.height() / 2)
+#
+#         # We going to create a centroid so we can rotate the points around a realistic center
+#         # Sorry for those of you that get weird rotations..
+#         x_list = []
+#         y_list = []
+#
+#         for vertex in self._vertices:
+#             x_list.append(vertex.x())
+#             y_list.append(vertex.y())
+#
+#         # Create a simple centroid (not full centroid)
+#         centroid_x = sum(x_list) / len(y_list)
+#         centroid_y = sum(y_list) / len(x_list)
+#
+#         return Location(centroid_x, centroid_y)
+#
+#     def rotation(self, angle: float = None) -> float:
+#         """
+#         Get or set the rotation of the object.
+#         :param angle: the angle to set the rotation to in degrees, if any
+#         :return: the angle of the object's rotation in degrees
+#         """
+#
+#         if angle is not None:
+#             verify(angle, (float, int))
+#             self._angle = angle
+#             self.update()
+#
+#         return self._angle % 360
+#
+#     def rotate(self, angle_diff: float = 0) -> None:
+#         """
+#         Rotate the angle of the object by a difference, in degrees
+#         :param angle_diff: the angle difference to rotate by
+#         :return: None
+#         """
+#
+#         verify(angle_diff, (float, int))
+#         self.rotation(self._angle + angle_diff)
+#
+#     def angleto(self, obj) -> float:
+#         """
+#         Retrieve the angle between this object and another (based on 0 degrees at 12 o'clock)
+#         :param obj: the Object/Location to get the angle to.
+#         :return: the angle in degrees as a float
+#         """
+#
+#         if isinstance(obj, Object):
+#             obj = obj.location()
+#         elif type(obj) is not Location and type(obj) is not tuple:
+#             raise InvalidArgumentError('Renderable#lookat() must be passed either a renderable or a location!')
+#
+#         location = Location(obj[0], obj[1])
+#         # theta = -math.atan2(location.x() - self.x(), location.y() - self.y()) - math.radians(self.rotation())
+#         theta = math.atan2(location.y() - self.center().y(), location.x() - self.center().x()) \
+#             - math.radians(self.rotation()) + math.pi / 2
+#         theta = math.degrees(theta)
+#
+#         return theta
+#
+#     def lookat(self, obj) -> None:
+#         """
+#         Look at another object (Objects or Locations)
+#         :param obj: the Object/Location to look at.
+#         :return: None
+#         """
+#
+#         theta = self.angleto(obj)
+#         self.rotate(theta)
+#
+#     def forward(self, distance: float) -> None:
+#         """
+#         Move the Renderable forward by distance at its current heading (rotation/angle)
+#         :param distance: the distance to move forward (hypotenuse)
+#         :return: None
+#         """
+#
+#         dx = distance * math.sin(math.radians(self._angle))
+#         dy = distance * -math.cos(math.radians(self._angle))
+#
+#         self.move(dx, dy)
+#
+#     def backward(self, distance: float) -> None:
+#         """
+#         Move the Renderable backward by distance at its current heading (rotation/angle)
+#         :param distance: the distance to move backward (hypotenuse)
+#         :return: None
+#         """
+#
+#         self.forward(-distance)
+#
+#     def color(self, color: Color = None) -> Color:
+#         """
+#         Get or set the color of the object
+#         :param color: the color to set to, if any
+#         :return: the color of the object
+#         """
+#
+#         if color is not None:
+#             verify(color, Color)
+#             self._color = color
+#             self.update()
+#
+#         return self._color
+#
+#     def border(self, color: Color = None, width: float = None, fill: bool = None) -> Color:
+#         """
+#         Add or get the border of the object
+#         :param color: the color to set the border too, set to Color.NONE to remove border
+#         :param width: the width of the border
+#         :param fill: whether to fill the polygon.
+#         :return: The Color of the border
+#         """
+#
+#         update = False
+#
+#         if color is not None:
+#             verify(color, Color)
+#             self._border = color
+#             update = True
+#         if fill is not None:
+#             verify(fill, bool)
+#             self._fill = fill
+#             update = True
+#         if width is not None:
+#             verify(width, (float, int))
+#             self._border_width = width
+#             update = True
+#
+#         if update:
+#             self.update()
+#
+#         return self._border
+#
+#     def border_width(self, width: float = None) -> float:
+#         """
+#         Gets or sets the border width
+#         :param width: the border width to set to
+#         :return: the border width
+#         """
+#
+#         if width is not None:
+#             verify(width, (float, int))
+#             self._border_width = width
+#             self.update()
+#
+#         return self._border_width
+#
+#     def fill(self, fill: bool = None) -> bool:
+#         """
+#         Returns or sets the current fill boolean
+#         :param fill: a new fill value, whether to fill the polygon
+#         :return: the fill value
+#         """
+#
+#         if fill is not None:
+#             verify(fill, bool)
+#             self._fill = fill
+#             self.update()
+#
+#         return self._fill
+#
+#     def distance(self, obj) -> float:
+#         """
+#         Returns the distance between two objs or locations in pixels (center to center)
+#         :param obj: the Renderable/location to check distance between
+#         :return: the distance between this obj and the passed Renderable/Location.
+#         """
+#
+#         if type(obj) is not Location and not isinstance(obj, Renderable):
+#             raise InvalidArgumentError(f'.distance() must be passed a Renderable or a Location! '
+#                                        f'(Passed: {type(obj)}')
+#
+#         location = obj if type(obj) is Location else obj.center()
+#
+#         return math.sqrt((location.x() - self.center().x()) ** 2 + (location.y() - self.center().y()) ** 2)
+#
+#     def visible(self, visible: bool = None) -> bool:
+#         """
+#         Get or set the visibility of the renderable.
+#         :param visible: the new visibility value, if any
+#         :return: the visibility value
+#         """
+#
+#         if visible is not None:
+#             verify(visible, bool)
+#             self._visible = visible
+#             self.update()
+#
+#         return self._visible
+#
+#     def transform(self, transform: tuple = None) -> tuple:
+#         """
+#         Get or set the transform of the Renderable.
+#         Transforms represent the width, height, and rotation of Renderables.
+#
+#         You can retrieve a Transform from a Renderable with this method and set the transform the same way.
+#         :param transform: the transform to set to, if any.
+#         :return: the transform
+#         """
+#
+#         if transform is not None:
+#             verify(transform, tuple)
+#             if not len(transform) == 3:
+#                 raise InvalidArgumentError('Ensure you are passing in a Transform from another object or a '
+#                                            'tuple in the following order: (width, height, rotation)')
+#             verify(transform[0], (float, int), transform[1], (float, int), transform[2], (float, int))
+#             self.width(transform[0])
+#             self.height(transform[1])
+#             self.rotation(transform[2])
+#
+#         return self.width(), self.height(), self.rotation()
+#
+#     def clone(self):
+#         """
+#         Clone this renderable!
+#         :return: a Renderable
+#         """
+#
+#         constructor = type(self)
+#
+#         return constructor(self._screen, self.x(), self.y(), self.width(), self.height(), self.color(), self.border(),
+#                            self.fill(), self.rotation(), self.visible())
+#
+#     def vertices(self) -> list:
+#         """
+#         Returns the list of vertices for the Renderable.
+#         (The vertices will be returned clockwise, starting from the top-leftmost point)
+#         :return: a list of Locations representing the vertices
+#         """
+#         return self._get_vertices()
+#
+#     def bounds(self) -> (Location, float, float):
+#         """
+#         Get the location and dimensions of a bounding box that contains the entire shape
+#         :return: a tuple containing the Location, width, and height.
+#         """
+#
+#         x0, y0, x1, y1 = self._screen._screen.cv.bbox(self._ref)
+#         location = self._screen.create_location(x0, y0, canvas=True)
+#
+#         return location, (x1 - x0), (y1 - y0)
+#
+#     def contains(self, *args) -> bool:
+#         """
+#         Returns whether or not a Location is contained within the object.
+#         :param args: You may pass in either two numbers, a Location, or a tuple containing and x and y point.
+#         :return: a boolean value representing whether or not the point is within the vertices of the object.
+#         """
+#
+#         x, y = 0, 0
+#         count = 0
+#
+#         if len(args) == 1:
+#             verify(args, (tuple, Location))
+#             if type(args[0]) is Location:
+#                 x = args[0].x()
+#                 y = args[0].y()
+#             elif type(args[0]) is tuple and len(args[0]) == 2:
+#                 x = args[0][0]
+#                 y = args[0][1]
+#         elif len(args) == 2:
+#             verify(args[0], (float, int), args[1], (float, int))
+#             if type(args[0]) is not float and type(args[0]) is not int \
+#                     and type(args[1]) is not float and type(args[1]) is not int:
+#                 raise InvalidArgumentError('Passed arguments must be numbers (x, y), '
+#                                            'or you may pass a location/tuple.')
+#             x = args[0]
+#             y = args[1]
+#         else:
+#             raise InvalidArgumentError('You must pass in a tuple, Location, or two numbers (x, y)!')
+#
+#         # If the point isn't remotely near us, we don't need to perform any calculations.
+#         if not isinstance(self, CustomRenderable) and self._angle == 0:
+#             if self.y() > 0 and self.x() > 0:
+#                 if not (self.x() <= x <= (self.x() + self.width()) and self.y() <= y <= (self.y() + self.height())):
+#                     return False
+#
+#         # the contains algorithm uses the line-intersects algorithm to determine if a point is within a polygon.
+#         # we are going to cast a ray from our point to the positive x. (left to right)
+#
+#         shape = self.vertices()
+#         shape = tuple(shape[:]) + (shape[0],)  # Add the first vertex back again to get the last edge.
+#
+#         point1 = shape[0]
+#         for i in range(1, len(shape)):
+#             # A cool trick that gets the next index in an array, or the first index if i is the last index.
+#             # (since we start at index 1)
+#             point2 = shape[i % len(shape)]
+#
+#             # make sure we're in the ballpark on the y axis (actually able to intersect on the x axis)
+#             if y > min(point1.y(), point2.y()):
+#
+#                 # Same thing as above
+#                 if y <= max(point1.y(), point2.y()):
+#
+#                     # Make sure our x is at least less than the max x of this line. (since we're travelling right)
+#                     if x <= max(point1.x(), point2.x()):
+#
+#                         # If our y's are equal, that means this line is flat on the x, which makes us tricked until now.
+#                         # (We now realize we were never in the ballpark in the first place.
+#                         if point1.y() != point2.y():
+#
+#                             # Now we get a possible intersection point from left to right.
+#                             intersects_x = (y - point1.y()) * (point2.x() - point1.x()) / \
+#                                            (point2.y() - point1.y()) + point1.x()
+#
+#                             # if the line was vertical or we actually intersected it
+#                             if point1.x() == point2.x() or x <= intersects_x:
+#                                 count += 1
+#
+#             # move up the ladder next vertices and edge
+#             point1 = point2
+#
+#         return not (count % 2 == 0)
+#
+#     def overlaps(self, other: 'Renderable') -> bool:
+#         """
+#         Returns if this object is overlapping with the passed object.
+#         :param other: another Renderable instance.
+#         :return: true if they are overlapping, false if not.
+#         """
+#
+#         if not isinstance(other, Renderable):
+#             raise TypeError('Passed non-renderable into Renderable#overlaps(), which takes only Renderables!')
+#
+#         x = self.x()
+#         y = self.y()
+#         width = self.width()
+#         height = self.height()
+#
+#         other_x = other.x()
+#         other_y = other.y()
+#         other_width = other.width()
+#         other_height = other.height()
+#
+#         # Only optimize if the angle is not zero.
+#         if self._angle % 360 == 0 and other._angle % 360 == 0:
+#             min_ax = x
+#             max_ax = x + width
+#
+#             min_bx = other_x
+#             max_bx = other_x + other_width
+#
+#             min_ay = y
+#             max_ay = y + height
+#
+#             min_by = other_y
+#             max_by = other_y + other_height
+#
+#             a_left_b = max_ax < min_bx
+#             a_right_b = min_ax > max_bx
+#             a_above_b = min_ay > max_by
+#             a_below_b = max_ay < min_by
+#         else:
+#             hypotenuse = math.sqrt(width ** 2 + height ** 2) + 1
+#             other_hypotenuse = math.sqrt(other_width ** 2 + other_height ** 2) + 1
+#
+#             center = Location(x + width / 2, y + height / 2)
+#             other_center = Location(other_x + other_width / 2, other_y + other_height / 2)
+#
+#             min_ax = center.x() - (hypotenuse / 2)
+#             max_ax = center.x() + (hypotenuse / 2)
+#
+#             min_bx = other_center.x() - (other_hypotenuse / 2)
+#             max_bx = other_center.x() + (other_hypotenuse / 2)
+#
+#             min_ay = center.y() - (hypotenuse / 2)
+#             max_ay = center.y() + (hypotenuse / 2)
+#
+#             min_by = other_center.y() - (other_hypotenuse / 2)
+#             max_by = other_center.y() + (other_hypotenuse / 2)
+#
+#             a_left_b = max_ax < min_bx
+#             a_right_b = min_ax > max_bx
+#             a_above_b = min_ay > max_by
+#             a_below_b = max_ay < min_by
+#
+#
+#
+#         # Do a base check to make sure they are even remotely near each other.
+#         # TODO: Re-optimize with rotation in mind.
+#         # if other._angle % 360 == 0 and self._angle % 360 == 0:
+#         if a_left_b or a_right_b or a_above_b or a_below_b:
+#             return False
+#
+#         # Check if one shape is entirely inside the other shape
+#         if (min_ax >= min_bx and max_ax <= max_bx) and (min_ay >= min_by and max_ay <= max_by):
+#             return True
+#
+#         if (min_bx >= min_ax and max_bx <= max_ax) and (min_by >= min_ay and max_by <= max_ay):
+#             return True
+#
+#         # Next we are going to use a sweeping line algorithm.
+#         # Essentially we will process the lines on the x axis, one coordinate at a time (imagine a vertical line scan).
+#         # Then we will look for their orientations. We will essentially make sure its impossible they do not cross.
+#         shape1 = self.vertices()
+#
+#         # noinspection PyProtectedMember
+#         shape2 = other.vertices()
+#
+#         # Orientation method that will determine if it is a triangle (and in what direction [cc or ccw]) or a line.
+#         def orientation(point1: Location, point2: Location, point3: Location) -> str:
+#             """
+#             Internal method that will determine the orientation of three points. They can be a clockwise triangle,
+#             counterclockwise triangle, or a co-linear line segment.
+#             :param point1: the first point of the main line segment
+#             :param point2: the second point of the main line segment
+#             :param point3: the third point to check from another line segment
+#             :return: the orientation of the passed points
+#             """
+#             result = (float(point2.y() - point1.y()) * (point3.x() - point2.x())) - \
+#                      (float(point2.x() - point1.x()) * (point3.y() - point2.y()))
+#
+#             if result > 0:
+#                 return 'clockwise'
+#             elif result < 0:
+#                 return 'counter-clockwise'
+#             else:
+#                 return 'co-linear'
+#
+#         def point_on_segment(point1: Location, point2: Location, point3: Location) -> bool:
+#             """
+#             Returns if point3 lies on the segment formed by point1 and point2.
+#             """
+#
+#             return max(point1.x(), point3.x()) >= point2.x() >= min(point1.x(), point3.x()) \
+#                    and max(point1.y(), point3.y()) >= point2.y() >= min(point1.y(), point3.y())
+#
+#         # Okay to begin actually detecting orientations, we want to loop through some edges. But only ones that are
+#         # relevant. In order to do this we will first have to turn the list of vertices into a list of edges.
+#         # Then we will look through the lists of edges and find the ones closest to each other.
+#
+#         shape1_edges = []
+#         shape2_edges = []
+#
+#         shape1 = tuple(shape1[:]) + (shape1[0],)
+#         shape2 = tuple(shape2[:]) + (shape2[0],)
+#
+#         shape1_point1 = shape1[0]
+#         for i in range(1, len(shape1)):
+#             shape1_point2 = shape1[i % len(shape1)]  # 1, 2, 3, 3 % 5
+#             shape1_edges.append((shape1_point1, shape1_point2))
+#             shape1_point1 = shape1_point2
+#
+#         shape2_point1 = shape2[0]
+#         for i in range(1, len(shape2)):
+#             shape2_point2 = shape2[i % len(shape2)]
+#             shape2_edges.append((shape2_point1, shape2_point2))
+#             shape2_point1 = shape2_point2
+#
+#         # Now we are going to test the four orientations that the segments form
+#         for edge1 in shape1_edges:
+#             for edge2 in shape2_edges:
+#                 orientation1 = orientation(edge1[0], edge1[1], edge2[0])
+#                 orientation2 = orientation(edge1[0], edge1[1], edge2[1])
+#                 orientation3 = orientation(edge2[0], edge2[1], edge1[0])
+#                 orientation4 = orientation(edge2[0], edge2[1], edge1[1])
+#
+#                 # If orientations 1 and 2 are different as well as 3 and 4 then they intersect!
+#                 if orientation1 != orientation2 and orientation3 != orientation4:
+#                     return True
+#
+#                 # There's some special cases we should check where a point from one segment is on the other segment
+#                 if orientation1 == 'co-linear' and point_on_segment(edge1[0], edge2[0], edge1[1]):
+#                     return True
+#
+#                 if orientation2 == 'co-linear' and point_on_segment(edge1[0], edge2[1], edge1[1]):
+#                     return True
+#
+#                 if orientation3 == 'co-linear' and point_on_segment(edge2[0], edge1[0], edge2[1]):
+#                     return True
+#
+#                 if orientation4 == 'co-linear' and point_on_segment(edge2[0], edge1[1], edge2[1]):
+#                     return True
+#
+#         # If none of the above conditions were ever met we just return False. Hopefully we are correct xD.
+#         return False
+#
+#     # noinspection PyProtectedMember
+#     # noinspection PyUnresolvedReferences
+#     def _get_vertices(self):
+#         real_shape = self._vertices
+#         # real_shape.reverse()
+#         #
+#         # min_distance = 999999
+#         # top_left_index = 0
+#         # for i, location in enumerate(real_shape):
+#         #     distance = math.sqrt((location.x()) ** 2 + (location.y()) ** 2)
+#         #     if distance < min_distance:
+#         #         min_distance = distance
+#         #         top_left_index = i
+#         #
+#         # real_shape = real_shape[top_left_index:] + real_shape[:top_left_index]
+#
+#         return real_shape
+#
+#     def _setup(self):
+#         if not hasattr(self, '_shape'):
+#             raise AttributeError('An error occured while initializing a Renderable: '
+#                                  'Is _shape set? (Advanced Users Only)')
+#
+#         shape = self._shape  # List of normal vertices.
+#
+#         width = self._width
+#         height = self._height
+#
+#         scale_factor = (width / PIXEL_RATIO, height / PIXEL_RATIO)
+#
+#         cx = 0
+#         cy = 0
+#
+#         vertices = [Location(vertex[0], vertex[1]) for vertex in shape]
+#
+#         for vertex in vertices:
+#             vertex.moveto(scale_factor[0] * (vertex.x() - cx) + cx, -scale_factor[1] * (vertex.y() - cy) + cy)
+#
+#             vertex.move(self.x() + width / 2, self.y() + height / 2)
+#
+#         self._vertices = vertices
+#
+#         self._vertices = self._rotate(self._vertices, self._angle)
+#
+#         tk_vertices = []  # we need to convert to tk's coordinate system.
+#         for vertex in self._vertices:
+#             tk_vertices.append((vertex.x() - (self._screen.width() / 2),
+#                                 (vertex.y() - (self._screen.height() / 2))))
+#
+#         state = tk.NORMAL if self._visible else tk.HIDDEN
+#         color_state = self._color if self._fill else Color.NONE
+#
+#         # noinspection PyProtectedMember
+#         self._ref = self._screen._canvas.create_polygon(
+#             tk_vertices,
+#             fill=self._screen._colorstr(color_state),
+#             outline=self._screen._screen._colorstr(self._border.__value__()),
+#             width=self._border_width,
+#             state=state,
+#             joinstyle=tk.MITER
+#         )
+#         # self.update() # CustomPolygon(self._screen, vertices)
+#
+#     def _rotate(self, vertices: list, angle: float, pivot: Location = None) -> list:
+#         # We have to update here since we cannot remember previous rotations (update method call won't cut it)!
+#         # vertices = self._vertices
+#
+#         # First get some values that we going to use later
+#         theta = math.radians(angle)
+#         cosine = math.cos(theta)
+#         sine = math.sin(theta)
+#
+#         if pivot is None:
+#             centroid_x = self.center().x()
+#             centroid_y = self.center().y()
+#         else:
+#             centroid_x = pivot.x()
+#             centroid_y = pivot.y()
+#
+#         new_vertices = []
+#         for vertex in vertices:
+#             # We have to create these separately because they're ironically used in each others calculations xD
+#             old_x = vertex.x() - centroid_x
+#             old_y = vertex.y() - centroid_y
+#
+#             new_x = (old_x * cosine - old_y * sine) + centroid_x
+#             new_y = (old_x * sine + old_y * cosine) + centroid_y
+#             new_vertices.append(Location(new_x, new_y))
+#
+#         return new_vertices
+#
+#     def update(self):
+#         self._check()
+#
+#         old_ref = self._ref
+#         shape = self._shape  # List of normal vertices.
+#
+#         width = self._width
+#         height = self._height
+#
+#         scale_factor = (width / PIXEL_RATIO, height / PIXEL_RATIO)
+#
+#         cx = 0
+#         cy = 0
+#
+#         vertices = [Location(vertex[0], vertex[1]) for vertex in shape]
+#         self._vertices = vertices
+#
+#         for vertex in vertices:
+#             vertex.moveto(scale_factor[0] * (vertex.x() - cx) + cx, -scale_factor[1] * (vertex.y() - cy) + cy)
+#
+#             vertex.move(self.x() + width / 2, self.y() + height / 2)
+#
+#         self._vertices = self._rotate(self._vertices, self._angle)
+#         self._last_angle = self._angle
+#
+#         tk_vertices = []  # we need to convert to tk's coordinate system.
+#         for vertex in self._vertices:
+#             tk_vertices.append((vertex.x() - (self._screen.width() / 2),
+#                                 (vertex.y() - (self._screen.height() / 2))))
+#
+#         state = tk.NORMAL if self._visible else tk.HIDDEN
+#         color_state = self._color if self._fill else Color.NONE
+#
+#         try:
+#             # noinspection PyProtectedMember
+#             self._ref = self._screen._canvas.create_polygon(
+#                 tk_vertices,
+#                 fill=self._screen._colorstr(color_state),
+#                 outline=self._screen._screen._colorstr(self._border.__value__()),
+#                 width=self._border_width,
+#                 state=state,
+#                 joinstyle=tk.MITER
+#             )
+#
+#             self._screen._canvas.tag_lower(self._ref, old_ref)
+#             self._screen._canvas.delete(old_ref)
+#         except:
+#             pass
+#
 
 class Renderable(Object):
     """
     Test class for new itemconfigure-based pyDraw objects.
 
     Update method is now only used for changes in position (and possibly changes that cannot be configured and require
     the item to be remade)
@@ -1187,26 +1193,28 @@
         :return: None
         """
 
         self._location.move(*args, **kwargs)
 
         new_location = self._screen.canvas_location(self._location.x(), self._location.y())
         self._screen._canvas.moveto(self._ref, new_location.x(), new_location.y())
+        self._update_coords()
         # self.update()
 
     def moveto(self, *args, **kwargs) -> None:
         """
         Move to a new location takes a Location, tuple, or two numbers (x, y)
         :return: None
         """
 
         self._location.moveto(*args, **kwargs)
 
         new_location = self._screen.canvas_location(self._location.x(), self._location.y())
         self._screen._canvas.moveto(self._ref, new_location.x(), new_location.y())
+        self._update_coords()
         # self.update()
 
     def width(self, width: float = None) -> float:
         """
         Get or set the width of the object.
         :param width: the width to set to in pixels, if any
         :return: the width of the object
@@ -1214,15 +1222,15 @@
 
         if width is not None:
             verify(width, (float, int))
             self._width = width
             new_location = self._screen.canvas_location(self._location.x(), self._location.y())
             new_location2 = self._screen.canvas_location(self._location.x() + self._width,
                                                          self._location.y() + self._height)
-            print(f'old coords {self._screen._canvas.coords(self._ref)}')
+
             new_coords = [new_location[0], new_location[1], new_location2[0], new_location[1],
                           new_location2[0], new_location2[1], new_location[0], new_location2[1]]
 
             if self._angle % 360 != 0:
                 self._update_coords()
             else:
                 self._screen._canvas.coords(self._ref, new_coords)
@@ -1323,15 +1331,15 @@
         if move_to is not None:
             verify(move_to, Location)
             self.moveto(move_to.x() - self.width() / 2, move_to.y() - self.height() / 2)
 
         if not centroid:
             return Location(self.x() + self.width() / 2, self.y() + self.height() / 2)
 
-        # We gonna create a centroid so we can rotate the points around a realistic center
+        # We are going to create a centroid, so we can rotate the points around a realistic center
         # Sorry for those of you that get weird rotations..
         x_list = []
         y_list = []
 
         for vertex in self._vertices:
             x_list.append(vertex.x())
             y_list.append(vertex.y())
@@ -1577,24 +1585,28 @@
     # noinspection PyProtectedMember
     def bounds(self) -> (Location, float, float):
         """
         Get the location and dimensions of a bounding box that contains the entire shape
         :return: a tuple containing the Location, width, and height.
         """
 
-        x0, y0, x1, y1 = self._screen._screen.cv.bbox(self._ref)
-        location = self._screen.create_location(x0, y0, canvas=True)
+        x0 = y0 = x1 = y1 = 0
+        try:
+            x0, y0, x1, y1 = self._screen._screen.cv.bbox(self._ref)
+            location = self._screen.create_location(x0, y0, canvas=True)
+        except tk.TclError:
+            return self.location(), self.width(), self.height()
 
         return location, (x1 - x0), (y1 - y0)
 
     def contains(self, *args) -> bool:
         """
-        Returns whether or not a Location is contained within the object.
+        Returns whether a Location is contained within the object.
         :param args: You may pass in either two numbers, a Location, or a tuple containing and x and y point.
-        :return: a boolean value representing whether or not the point is within the vertices of the object.
+        :return: a boolean value representing whether the point is within the vertices of the object.
         """
 
         x, y = 0, 0
         count = 0
 
         if len(args) == 1:
             verify(args, (tuple, Location))
@@ -1629,25 +1641,25 @@
 
         point1 = shape[0]
         for i in range(1, len(shape)):
             # A cool trick that gets the next index in an array, or the first index if i is the last index.
             # (since we start at index 1)
             point2 = shape[i % len(shape)]
 
-            # make sure we're in the ballpark on the y axis (actually able to intersect on the x axis)
+            # make sure we're in the ballpark on the y-axis (actually able to intersect on the x-axis)
             if y > min(point1.y(), point2.y()):
 
                 # Same thing as above
                 if y <= max(point1.y(), point2.y()):
 
                     # Make sure our x is at least less than the max x of this line. (since we're travelling right)
                     if x <= max(point1.x(), point2.x()):
 
                         # If our y's are equal, that means this line is flat on the x, which makes us tricked until now.
-                        # (We now realize we were never in the ballpark in the first place.
+                        # We now realize we were never in the ballpark in the first place.
                         if point1.y() != point2.y():
 
                             # Now we get a possible intersection point from left to right.
                             intersects_x = (y - point1.y()) * (point2.x() - point1.x()) / \
                                            (point2.y() - point1.y()) + point1.x()
 
                             # if the line was vertical or we actually intersected it
@@ -1665,65 +1677,76 @@
         :param other: another Renderable instance.
         :return: true if they are overlapping, false if not.
         """
 
         if not isinstance(other, Renderable):
             raise TypeError('Passed non-renderable into Renderable#overlaps(), which takes only Renderables!')
 
-        x = self.x()
-        y = self.y()
-        width = self.width()
-        height = self.height()
-
-        other_x = other.x()
-        other_y = other.y()
-        other_width = other.width()
-        other_height = other.height()
 
-        # Only optimize if the angle is not zero.
-        if self._angle % 360 == 0 and other._angle % 360 == 0:
-            min_ax = x
-            max_ax = x + width
-
-            min_bx = other_x
-            max_bx = other_x + other_width
-
-            min_ay = y
-            max_ay = y + height
-
-            min_by = other_y
-            max_by = other_y + other_height
-
-            a_left_b = max_ax < min_bx
-            a_right_b = min_ax > max_bx
-            a_above_b = min_ay > max_by
-            a_below_b = max_ay < min_by
-        else:
-            hypotenuse = math.sqrt(width ** 2 + height ** 2) + 1
-            other_hypotenuse = math.sqrt(other_width ** 2 + other_height ** 2) + 1
+        bounds = self.bounds()
+        other_bounds = other.bounds()
 
-            center = Location(x + width / 2, y + height / 2)
-            other_center = Location(other_x + other_width / 2, other_y + other_height / 2)
+        min_ax = bounds[0].x()
+        max_ax = min_ax + bounds[1]
 
-            min_ax = center.x() - (hypotenuse / 2)
-            max_ax = center.x() + (hypotenuse / 2)
+        min_bx = other_bounds[0].x()
+        max_bx = min_bx + other_bounds[1]
 
-            min_bx = other_center.x() - (other_hypotenuse / 2)
-            max_bx = other_center.x() + (other_hypotenuse / 2)
+        min_ay = bounds[0].y()
+        max_ay = min_ay + bounds[2]
 
-            min_ay = center.y() - (hypotenuse / 2)
-            max_ay = center.y() + (hypotenuse / 2)
+        min_by = other_bounds[0].y()
+        max_by = min_by + other_bounds[2]
 
-            min_by = other_center.y() - (other_hypotenuse / 2)
-            max_by = other_center.y() + (other_hypotenuse / 2)
+        a_left_b = max_ax < min_bx
+        a_right_b = min_ax > max_bx
+        a_above_b = min_ay > max_by
+        a_below_b = max_ay < min_by
 
-            a_left_b = max_ax < min_bx
-            a_right_b = min_ax > max_bx
-            a_above_b = min_ay > max_by
-            a_below_b = max_ay < min_by
+        # Only optimize if the angle is not zero.
+        # if self._angle % 360 == 0 and other._angle % 360 == 0:
+        #     min_ax = x
+        #     max_ax = x + width
+        #
+        #     min_bx = other_x
+        #     max_bx = other_x + other_width
+        #
+        #     min_ay = y
+        #     max_ay = y + height
+        #
+        #     min_by = other_y
+        #     max_by = other_y + other_height
+        #
+        #     a_left_b = max_ax < min_bx
+        #     a_right_b = min_ax > max_bx
+        #     a_above_b = min_ay > max_by
+        #     a_below_b = max_ay < min_by
+        # else:
+        #     hypotenuse = math.sqrt(width ** 2 + height ** 2) + 1
+        #     other_hypotenuse = math.sqrt(other_width ** 2 + other_height ** 2) + 1
+        #
+        #     center = Location(x + width / 2, y + height / 2)
+        #     other_center = Location(other_x + other_width / 2, other_y + other_height / 2)
+        #
+        #     min_ax = center.x() - (hypotenuse / 2)
+        #     max_ax = center.x() + (hypotenuse / 2)
+        #
+        #     min_bx = other_center.x() - (other_hypotenuse / 2)
+        #     max_bx = other_center.x() + (other_hypotenuse / 2)
+        #
+        #     min_ay = center.y() - (hypotenuse / 2)
+        #     max_ay = center.y() + (hypotenuse / 2)
+        #
+        #     min_by = other_center.y() - (other_hypotenuse / 2)
+        #     max_by = other_center.y() + (other_hypotenuse / 2)
+        #
+        #     a_left_b = max_ax < min_bx
+        #     a_right_b = min_ax > max_bx
+        #     a_above_b = min_ay > max_by
+        #     a_below_b = max_ay < min_by
 
         # Do a base check to make sure they are even remotely near each other.
         # TODO: Re-optimize with rotation in mind.
         # if other._angle % 360 == 0 and self._angle % 360 == 0:
         if a_left_b or a_right_b or a_above_b or a_below_b:
             return False
 
@@ -1731,15 +1754,15 @@
         if (min_ax >= min_bx and max_ax <= max_bx) and (min_ay >= min_by and max_ay <= max_by):
             return True
 
         if (min_bx >= min_ax and max_bx <= max_ax) and (min_by >= min_ay and max_by <= max_ay):
             return True
 
         # Next we are going to use a sweeping line algorithm.
-        # Essentially we will process the lines on the x axis, one coordinate at a time (imagine a vertical line scan).
+        # Essentially we will process the lines on the x-axis, one coordinate at a time (imagine a vertical line scan).
         # Then we will look for their orientations. We will essentially make sure its impossible they do not cross.
         shape1 = self.vertices()
 
         # noinspection PyProtectedMember
         shape2 = other.vertices()
 
         # Orientation method that will determine if it is a triangle (and in what direction [cc or ccw]) or a line.
@@ -1796,14 +1819,16 @@
         for edge1 in shape1_edges:
             for edge2 in shape2_edges:
                 orientation1 = orientation(edge1[0], edge1[1], edge2[0])
                 orientation2 = orientation(edge1[0], edge1[1], edge2[1])
                 orientation3 = orientation(edge2[0], edge2[1], edge1[0])
                 orientation4 = orientation(edge2[0], edge2[1], edge1[1])
 
+                # print(orientation1, orientation2, orientation3, orientation4)
+
                 # If orientations 1 and 2 are different as well as 3 and 4 then they intersect!
                 if orientation1 != orientation2 and orientation3 != orientation4:
                     return True
 
                 # There's some special cases we should check where a point from one segment is on the other segment
                 if orientation1 == 'co-linear' and point_on_segment(edge1[0], edge2[0], edge1[1]):
                     return True
@@ -1814,14 +1839,15 @@
                 if orientation3 == 'co-linear' and point_on_segment(edge2[0], edge1[0], edge2[1]):
                     return True
 
                 if orientation4 == 'co-linear' and point_on_segment(edge2[0], edge1[1], edge2[1]):
                     return True
 
         # If none of the above conditions were ever met we just return False. Hopefully we are correct xD.
+        # print('no conditions met')
         return False
 
     def _get_vertices(self):
         real_shape = self._vertices
         return real_shape
 
     def _setup(self):
@@ -1869,29 +1895,29 @@
         )
         # self.update() # CustomPolygon(self._screen, vertices)
 
     def _rotate(self, vertices: list, angle: float, pivot: Location = None) -> list:
         # We have to update here since we cannot remember previous rotations (update method call won't cut it)!
         # vertices = self._vertices
 
-        # First get some values that we gonna use later
+        # First get some values that we're going to use later
         theta = math.radians(angle)
         cosine = math.cos(theta)
         sine = math.sin(theta)
 
         if pivot is None:
             centroid_x = self.center().x()
             centroid_y = self.center().y()
         else:
             centroid_x = pivot.x()
             centroid_y = pivot.y()
 
         new_vertices = []
         for vertex in vertices:
-            # We have to create these separately because they're ironically used in each others calculations xD
+            # We have to create these separately because they're ironically used in each other's calculations xD
             old_x = vertex.x() - centroid_x
             old_y = vertex.y() - centroid_y
 
             new_x = (old_x * cosine - old_y * sine) + centroid_x
             new_y = (old_x * sine + old_y * cosine) + centroid_y
             new_vertices.append(Location(new_x, new_y))
 
@@ -1967,16 +1993,16 @@
                 fill=self._screen._colorstr(color_state),
                 outline=self._screen._screen._colorstr(self._border.__value__()),
                 width=self._border_width,
                 state=state,
                 joinstyle=tk.MITER
             )
 
-            self._screen._canvas.tag_lower(self._ref, old_ref)
-            self._screen._canvas.delete(old_ref)
+            self._screen._canvas.tag_lower(self._ref, old_ref)  # noqa
+            self._screen._canvas.delete(old_ref)  # noqa
         except:
             pass
 
 
 class CustomRenderable(Renderable):
     """
     A wrapper class to distintify classes that extend Renderable but have some custom functionality.
@@ -2008,15 +2034,15 @@
         self._width = width
         self._height = height
         self._color = color
         self._border = color
         self._fill = fill
         self._angle = rotation
         self._visible = visible
-        self._borderwidth = radius
+        self._border_width = radius
 
         self._setup()
 
     @overload(Screen, (int, float), (int, float), (int, float), (int, float), Color)
     def __init__(self, screen: Screen, x: float, y: float, width: float, height: float,
                  color: Color = Color('black'),
                  radius: float = 10,
@@ -2034,15 +2060,15 @@
         self._width = width
         self._height = height
         self._color = color
         self._border = color
         self._fill = fill
         self._angle = rotation
         self._visible = visible
-        self._borderwidth = radius
+        self._border_width = radius
 
         self._setup()
 
     @overload(Screen, Location, (int, float), (int, float))
     def __init__(self, screen: Screen, location: Location, width: float, height: float,
                  color: Color = Color('black'),
                  radius: float = 10,
@@ -2060,15 +2086,15 @@
         self._width = width
         self._height = height
         self._color = color
         self._border = color
         self._fill = fill
         self._angle = rotation
         self._visible = visible
-        self._borderwidth = radius
+        self._border_width = radius
 
         self._setup()
 
     @overload(Screen, Location, (int, float), (int, float), Color)
     def __init__(self, screen: Screen, location: Location, width: float, height: float,
                  color: Color = Color('black'),
                  radius: float = 10,
@@ -2086,15 +2112,15 @@
         self._width = width
         self._height = height
         self._color = color
         self._border = color
         self._fill = fill
         self._angle = rotation
         self._visible = visible
-        self._borderwidth = radius
+        self._border_width = radius
 
         self._setup()
 
     # We redefine the border method to do nothing
     # def border(self, color: Color = None, width: float = 1, fill: bool = None) -> Color:
     #     raise NotImplemented("This method is not allowed for `Rounded` shapes.")
     border = property(doc='(!) Disallowed inherited')
@@ -2103,18 +2129,18 @@
         """
         Set the border radius of the rounded shape.
         :param radius: the radius to set to (not pixel accurate)
         :return: the radius
         """
 
         if radius is not None:
-            self._borderwidth = radius
-            self._update()
+            self._border_width = radius
+            self.update()
 
-        return self._borderwidth
+        return self._border_width
 
     def _setup(self):
         if not hasattr(self, '_shape'):
             raise AttributeError('An error occured while initializing a Renderable: '
                                  'Is _shape set? (Advanced Users Only)')
 
         shape = self._shape  # List of normal vertices.
@@ -2142,21 +2168,21 @@
         for vertex in self._vertices:
             tk_vertices.append((vertex.x() - (self._screen.width() / 2),
                                 (vertex.y() - (self._screen.height() / 2))))
 
         state = tk.NORMAL if self._visible else tk.HIDDEN
         color_state = self._color if self._fill else Color.NONE
 
-        print(self._borderwidth)
+        print(self._border_width)
         # noinspection PyProtectedMember
         self._ref = self._screen._canvas.create_polygon(
             tk_vertices,
             fill=self._screen._colorstr(color_state),
             outline=self._screen._colorstr(self._color),  # self._screen._screen._colorstr(self._border.__value__()),
-            width=self._borderwidth,
+            width=self._border_width,
             state=state,
             joinstyle=tk.ROUND
         )
         # self.update() # CustomPolygon(self._screen, vertices)
 
     def update(self):
         self._check()
@@ -2193,15 +2219,15 @@
 
         try:
             # noinspection PyProtectedMember
             self._ref = self._screen._canvas.create_polygon(
                 tk_vertices,
                 fill=self._screen._colorstr(color_state),
                 outline=self._screen._screen._colorstr(self._border.__value__()),
-                width=self._borderwidth,
+                width=self._border_width,
                 state=state,
                 joinstyle=tk.ROUND
             )
 
             self._screen._canvas.tag_lower(self._ref, old_ref)
             self._screen._canvas.delete(old_ref)
         except:
@@ -2403,17 +2429,24 @@
                 if type(kwargs['y']) is float or type(kwargs['y']) is int:
                     location.y(kwargs['y'])
                 else:
                     raise InvalidArgumentError(".center() requires either a Location/tuple or two numbers!")
 
         return self._center(location)
 
-    def _center(self, moveto: Location = None) -> Location:
+    def _center(self, moveto: Location = None, centroid = True) -> Location:
+
+        if not centroid:
+            if moveto is not None:
+                verify(moveto, Location)
+                self.move(moveto.x() - self._location.x(), moveto.y() - self._location.y())
+
+            return Location(self._location.x() + self._width / 2, self._location.y() + self._height / 2)
 
-        # We gonna create a centroid so we can rotate the points around a realistic center
+        # We are going to create a centroid, so we can rotate the points around a realistic center
         # Sorry for those of you that get weird rotations..
         x_list = []
         y_list = []
         for vertex in self._vertices:
             x_list.append(vertex.x())
             y_list.append(vertex.y())
 
@@ -2450,51 +2483,44 @@
 
         return self.width(), self.height(), self.rotation()
 
     def _rotate(self, angle: float) -> list:
         # We have to update here since we cannot remember previous rotations (update method call won't cut it)!
         vertices = self._current_vertices
 
-        # First get some values that we gonna use later
+        # First get some values that we are going to use later
         theta = math.radians(angle)
         cosine = math.cos(theta)
         sine = math.sin(theta)
 
         centroid_x = self.center().x()
         centroid_y = self.center().y()
 
         new_vertices = []
         for vertex in vertices:
-            # We have to create these separately because they're ironically used in each others calculations xD
+            # We have to create these separately because they're ironically used in each other's calculations xD
             old_x = vertex.x() - centroid_x
             old_y = vertex.y() - centroid_y
 
             new_x = (old_x * cosine - old_y * sine) + centroid_x
             new_y = (old_x * sine + old_y * cosine) + centroid_y
             new_vertices.append(Location(new_x, new_y))
 
         return new_vertices
 
     def _get_ref_vertices(self) -> list:
-        def pairwise(iterable):
-            i = iter(iterable)
-            while True:
-                yield i.next(), i.next()
-
         new_vertices = []
         tk_coords = self._screen._canvas.coords(self._ref)
         print(len(tk_coords), tk_coords)
         last = None
 
         for j in range(0, len(tk_coords), 2):
             x = tk_coords[j]
             y = tk_coords[j + 1]
             new_vertices.append(Location(x + self._screen.width() / 2, y + self._screen.height() / 2))
-        # for x, y in pairwise(tk_coords):
-        #     new_vertices.append(Location(x + self._screen.width() / 2, y + self._screen.height() / 2))
         return new_vertices
 
     def _update_coords(self, width: float = None, height: float = None):
         width = width if width is not None else self._width
         height = height if height is not None else self._height
 
         cx = self.x() + (self._width / 2)
@@ -3127,15 +3153,15 @@
         state = tk.NORMAL if self._visible else tk.HIDDEN
 
         # noinspection PyProtectedMember
         self._ref = self._screen._canvas.create_polygon(
             tk_vertices,
             fill=self._screen._colorstr(self._color),
             outline=self._screen._screen._colorstr(self._border.__value__()),
-            width=self._borderwidth,
+            width=self._border_width,
             state=state
         )
 
     # noinspection PyProtectedMember
     def update(self):
         self._check()
 
@@ -3182,15 +3208,15 @@
 
         try:
             # noinspection PyProtectedMember
             self._ref = self._screen._canvas.create_polygon(
                 tk_vertices,
                 fill=self._screen._colorstr(color_state),
                 outline=self._screen._screen._colorstr(self._border.__value__()),
-                width=self._borderwidth,
+                width=self._border_width,
                 state=state,
                 joinstyle=tk.MITER
             )
 
             self._screen._canvas.tag_lower(self._ref, old_ref)
             self._screen._canvas.delete(old_ref)
         except:
@@ -3249,15 +3275,15 @@
         self._height = self._image.height()
 
         self._frame = -1
         self._frames = -1
 
         self._mask = 123
 
-        # We have to monkey patch PIL if we modify the image, but we don't wanna cause a RecursionError (call once)
+        # We have to monkey patch PIL if we modify the image, but we don't want to cause a RecursionError (call once)
         self._patched = False
 
         super().__init__(screen, x, y, self._width, self._height, color=Color.NONE, border=border,
                          rotation=rotation, visible=visible)
         self._setup()
 
         if width is not None and width != self._width:
@@ -3310,15 +3336,15 @@
         self._height = self._image.height()
 
         self._frame = -1
         self._frames = -1
 
         self._mask = 123
 
-        # We have to monkey patch PIL if we modify the image, but we don't wanna cause a RecursionError (call once)
+        # We have to monkey patch PIL if we modify the image, but we don't want to cause a RecursionError (call once)
         self._patched = False
 
         super().__init__(screen, x, y, self._width, self._height, color=Color.NONE, border=border,
                          rotation=rotation, visible=visible)
         self._setup()
 
         if width is not None and width != self._width:
@@ -3371,15 +3397,15 @@
         self._height = self._image.height()
 
         self._frame = -1
         self._frames = -1
 
         self._mask = 123
 
-        # We have to monkey patch PIL if we modify the image, but we don't wanna cause a RecursionError (call once)
+        # We have to monkey patch PIL if we modify the image, but we don't want to cause a RecursionError (call once)
         self._patched = False
 
         super().__init__(screen, x, y, self._width, self._height, color=Color.NONE, border=border,
                          rotation=rotation, visible=visible)
         self._setup()
 
         if width is not None and width != self._width:
@@ -3432,15 +3458,15 @@
         self._height = self._image.height()
 
         self._frame = -1
         self._frames = -1
 
         self._mask = 123
 
-        # We have to monkey patch PIL if we modify the image, but we don't wanna cause a RecursionError (call once)
+        # We have to monkey patch PIL if we modify the image, but we don't want to cause a RecursionError (call once)
         self._patched = False
 
         super().__init__(screen, x, y, self._width, self._height, color=Color.NONE, border=border,
                          rotation=rotation, visible=visible)
         self._setup()
 
         if width is not None and width != self._width:
@@ -3498,15 +3524,15 @@
         self._height = self._image.height()
 
         self._frame = -1
         self._frames = -1
 
         self._mask = 123
 
-        # We have to monkey patch PIL if we modify the image, but we don't wanna cause a RecursionError (call once)
+        # We have to monkey patch PIL if we modify the image, but we don't want to cause a RecursionError (call once)
         self._patched = False
 
         super().__init__(screen, x, y, self._width, self._height, color=Color.NONE, border=border,
                          rotation=rotation, visible=visible)
         self._setup()
 
         if width is not None and width != self._width:
@@ -3562,15 +3588,15 @@
         self._height = self._image.height()
 
         self._frame = -1
         self._frames = -1
 
         self._mask = 123
 
-        # We have to monkey patch PIL if we modify the image, but we don't wanna cause a RecursionError (call once)
+        # We have to monkey patch PIL if we modify the image, but we don't want to cause a RecursionError (call once)
         self._patched = False
 
         super().__init__(screen, x, y, self._width, self._height, color=Color.NONE, border=border,
                          rotation=rotation, visible=visible)
         self._setup()
 
         if width is not None and width != self._width:
@@ -3626,15 +3652,15 @@
         self._height = self._image.height()
 
         self._frame = -1
         self._frames = -1
 
         self._mask = 123
 
-        # We have to monkey patch PIL if we modify the image, but we don't wanna cause a RecursionError (call once)
+        # We have to monkey patch PIL if we modify the image, but we don't want to cause a RecursionError (call once)
         self._patched = False
 
         super().__init__(screen, x, y, self._width, self._height, color=Color.NONE, border=border,
                          rotation=rotation, visible=visible)
         self._setup()
 
         if width is not None and width != self._width:
@@ -3812,25 +3838,25 @@
 
         vertices = [self.location(), Location(self.x() + self.width(), self.y()),
                     Location(self.x() + self.width(), self.y() + self.height()),
                     Location(self.x(), self.y() + self.height())]
 
         if self._angle != 0:
 
-            # First get some values that we gonna use later
+            # First get some values that we're going to use later
             theta = math.radians(self._angle)
             cosine = math.cos(theta)
             sine = math.sin(theta)
 
             center_x = self.x() + self.width() / 2
             center_y = self.y() + self.width() / 2
 
             new_vertices = []
             for vertex in vertices:
-                # We have to create these separately because they're ironically used in each others calculations xD
+                # We have to create these separately because they're ironically used in each other's calculations xD
                 old_x = vertex.x() - center_x
                 old_y = vertex.y() - center_y
 
                 new_x = (old_x * cosine - old_y * sine) + center_x
                 new_y = (old_x * sine + old_y * cosine) + center_y
                 new_vertices.append(Location(new_x, new_y))
 
@@ -3845,15 +3871,15 @@
     def load(self) -> None:
         """
         Load animated GIF (reads frames)
         :return: None
         """
 
         from PIL import Image
-        from PIL import GifImagePlugin
+        # from PIL import GifImagePlugin
 
         image = Image.open(self._image_name)
         if hasattr(image, 'n_frames'):
             self._frames = image.n_frames
             self._frame = 0
         else:
             raise PydrawError('GIF is not animated, so it cannot be loaded!')
@@ -3890,20 +3916,20 @@
         """
 
         return self._frames
 
     def clone(self) -> 'Image':
         constructor = type(self)
         return constructor(self._screen, self._image_name, self.x(), self.y(), self.height(), self.width(),
-                           self.color(), self.border(), self.rotation(), self.visible(()))
+                           self.color(), self.border(), self.rotation(), self.visible())
 
     @staticmethod
     def _monkey_patch_del():
         """
-        We monkey patch the del function for PIL so it doesn't do stupid things.
+        We monkey patch the del function for PIL, so it doesn't do stupid things.
         :return:
         """
         from PIL import ImageTk
 
         # monkey patch TKinter from this dumb bug they don't catch in TK.PhotoImage
         old_del = ImageTk.PhotoImage.__del__
 
@@ -3958,15 +3984,15 @@
                                                    self._mask))
                     result.putalpha(alpha)
                     image = result
 
                 if self._border is not None and self._border is not Color.NONE:
                     image = ImageOps.expand(image, border=10, fill=self._border.rgb())
 
-                # Do resizing last so we can make sure the other manipulations work properly
+                # Do the resizing last, so we can make sure the other manipulations work properly
                 image = image.resize((int(self.width()), int(self.height())), Image.ANTIALIAS)
 
                 if self._angle != 0:
                     image = image.rotate(-self._angle, resample=Image.BILINEAR, expand=1, fillcolor=None)
 
                 self._image = ImageTk.PhotoImage(image=image)
             except (RuntimeError, AttributeError) as e:
@@ -3988,15 +4014,15 @@
             self._screen._canvas.tag_lower(self._ref, old_ref)
             self._screen._canvas.delete(old_ref)
         except tk.TclError:
             pass
 
 
 class Text(CustomRenderable):
-    _anchor = 'nw'  # sw technically means southwest but it means bottom left anchor. (we change to top left in code)
+    _anchor = 'nw'  # sw technically means southwest, but it means bottom left anchor. (we change to top left in code)
     _aligns = {'left': tk.LEFT, 'center': tk.CENTER, 'right': tk.RIGHT}
 
     # noinspection PyProtectedMember
     @overload(Screen, str, (int, float), (int, float))
     def __init__(self, screen: Screen, text: str, x: float, y: float, color: Color = Color('black'),  # noqa
                  font: str = 'Arial', size: int = 16, align: str = 'left', bold: bool = False, italic: bool = False,
                  underline: bool = False, strikethrough: bool = False, rotation: float = 0, visible: bool = True):
@@ -4304,19 +4330,44 @@
         :param text: text to set to (str), if any
         :return: the text
         """
 
         if text is not None:
             verify(text, str)
             self._text = text
-            self._screen._canvas.itemconfigure(self._ref, text=self._text)
+            try:
+                self._screen._canvas.itemconfigure(self._ref, text=self._text)
+            except tk.TclError:
+                pass
             # self.update()
 
         return self._text
 
+    def move(self, *args, **kwargs) -> None:
+        """
+        Can take either a tuple, Location, or two numbers (dx, dy)
+        :return: None
+        """
+
+        self._location.move(*args, **kwargs)
+
+        new_location = self._screen.canvas_location(self._location.x(), self._location.y())
+        self._screen._canvas.moveto(self._ref, new_location.x(), new_location.y())
+
+    def moveto(self, *args, **kwargs) -> None:
+        """
+        Move to a new location takes a Location, tuple, or two numbers (x, y)
+        :return: None
+        """
+
+        self._location.moveto(*args, **kwargs)
+
+        new_location = self._screen.canvas_location(self._location.x(), self._location.y())
+        self._screen._canvas.moveto(self._ref, new_location.x(), new_location.y())
+
     # noinspection PyMethodOverriding
     def width(self) -> float:
         """
         Get the width of the text (cannot be modified)
         :return the width of the text
         """
 
@@ -4551,25 +4602,25 @@
         :return: a list of Locations
         """
 
         vertices = [Location(self.x(), self.y()), Location(self.x() + self.width(), self.y()),
                     Location(self.x() + self.width(), self.y() + self.height()),
                     Location(self.x(), self.y() + self.height())]
         if self._angle != 0:
-            # First get some values that we gonna use later
+            # First get some values that we're going to use later
             theta = math.radians(self._angle)
             cosine = math.cos(theta)
             sine = math.sin(theta)
 
             centroid_x = self.center().x()
             centroid_y = self.center().y()
 
             new_vertices = []
             for vertex in vertices:
-                # We have to create these separately because they're ironically used in each others calculations xD
+                # We have to create these separately because they're ironically used in each other's calculations xD
                 old_x = vertex.x() - centroid_x
                 old_y = vertex.y() - centroid_y
 
                 new_x = (old_x * cosine - old_y * sine) + centroid_x
                 new_y = (old_x * sine + old_y * cosine) + centroid_y
                 new_vertices.append(Location(new_x, new_y))
             vertices = new_vertices
@@ -4760,14 +4811,19 @@
         self._ref = self._screen._screen.cv.create_line(self._pos1.x() - screen.width() / 2,
                                                         self._pos1.y() - screen.height() / 2,
                                                         self._pos2.x() - screen.width() / 2,
                                                         self._pos2.y() - screen.height() / 2,
                                                         fill=self._screen._screen._colorstr(self._color.__value__()),
                                                         width=self._thickness, dash=self._dashes, state=state)
 
+        # Set angle
+        theta = math.atan2(self.pos1().y() - self.pos2().y(), self.pos1().x() - self.pos2().x())
+        theta = math.degrees(theta)
+        self._angle = theta
+
     def pos1(self, *args) -> Location:
         """
         Get or set the position of the first endpoint.
         :param args: Either a location or two numbers (x, y) may be passed here.
         :return: the position of the first endpoint.
         """
 
@@ -4933,15 +4989,15 @@
 
         if 'point' in kwargs:
             if type(kwargs['point']) is not int:
                 raise InvalidArgumentError('Point must be an int.')
 
             point = kwargs['point']
 
-        # so now we have a location but we need to shorten it to be the same length of our line right now.
+        # so now we have a location, but we need to shorten it to be the same length of our line right now.
         # slope = (self.pos2().y() - self.pos1().y()) / (self.pos2.x() - self.pos1.x())
         length = self.length()
 
         if point == 2:
             ray_length = self._length(self.pos1().x(), location.x(), self.pos1().y(), location.y())
 
             # hypotenuse = (ray_length - length)  # extraneous length (we need to cut this)
@@ -4958,32 +5014,33 @@
         else:
             raise InvalidArgumentError('Point is not 1 or 2! (2 by default)')
 
         self.rotate(math.degrees(theta))
 
     def rotation(self, angle: float = None):
         """
-        Get or set the rotation of the line (works via pos2().
+        Get or set the rotation of the line (works via pos2()).
         :param angle: the angle in degrees to rotate by, if any
         :return: the angle of the line
         """
 
-        theta = math.atan2(self.pos1().y() - self.pos2().y(), self.pos1().x() - self.pos2().x())
-        theta = math.degrees(theta)
+        # theta = math.atan2(self.pos1().y() - self.pos2().y(), self.pos1().x() - self.pos2().x())
+        # theta = math.degrees(theta)
+
         if angle is not None:
-            self.rotate(angle + theta)
+            self.rotate(angle - self._angle)
 
-        return theta
+        return self._angle
 
-    def rotate(self, angle_diff: float, point: int = 1):
+    def rotate(self, angle_diff: float, point: int = 1) -> float:
         """
-        Rotate the line around one of the vertices (1 by default)
+        Rotate the line around one of its vertices (1 by default)
         :param angle_diff: the angle to rotate by
         :param point: the point to serve as the origin.
-        :return:
+        :return: the new angle
         """
 
         origin = self._pos1 if point == 1 else self._pos2
         point = self._pos2 if point == 1 else self._pos1
 
         theta = math.radians(angle_diff)
 
@@ -4997,15 +5054,17 @@
         new_y = (old_x * sine + old_y * cosine) + origin.y()
 
         point.moveto(new_x, new_y)
         self._screen._canvas.coords(self._ref, [self._pos1.x() - self._screen.width() / 2,
                                                 self._pos1.y() - self._screen.height() / 2,
                                                 self._pos2.x() - self._screen.width() / 2,
                                                 self._pos2.y() - self._screen.height() / 2])
-        # self.update()
+
+        self._angle += angle_diff
+        return self._angle
 
     def location(self) -> tuple:
         """
         Returns the locations of both the endpoints
         :return: the locations of both the endpoints
         """
 
@@ -5050,15 +5109,15 @@
             verify(thickness, int)
             self._thickness = thickness
             self._screen._canvas.itemconfigure(self._ref, width=self._thickness)
             # self.update()
 
         return self._thickness
 
-    def dashes(self, dashes: int = None) -> Union[int, tuple]:
+    def dashes(self, dashes: Union[int, tuple] = None) -> Union[int, tuple]:
         """
         Retrieve or enable/disable the dashes for the line
 
         On systems which support only a limited set of dash patterns, the dash pattern will be displayed as the closest
         dash pattern that is available. For example, on Windows only a few dash patterns are available, most of which
         do not allow for special dash-spacing (if passing in a tuple).
 
@@ -5117,30 +5176,30 @@
         return Line(self._screen, self._pos1, self._pos2, color=self._color, thickness=self._thickness,
                     dashes=self._dashes, visible=self._visible)
 
     def intersects(self, obj) -> bool:
         """
         Check if a line intersects with another line or Renderable
         :param obj: Line, Renderable, or List/Tuple
-        :return: Whether or not the line intersects with the object
+        :return: Whether the line intersects with the object
         """
 
         shape1 = (self.pos1(), self.pos2())
 
         if type(obj) == Line:
             shape2 = (obj.pos1(), obj.pos2())
         elif type(obj) == Renderable:
             shape2 = obj.vertices()
         elif type(obj) == list or type(obj) == tuple:
             shape2 = obj
         else:
             raise InvalidArgumentError('Line.intersects() accepts only: Lines, Renderables, Lists or Tuples')
 
         if len(shape2) < 2:
-            raise InvalidArgumentError('Passed object did not have more than 1 vertice!')
+            raise InvalidArgumentError('Passed object did not have more than 1 vertex!')
 
         # Orientation method that will determine if it is a triangle (and in what direction [cc or ccw]) or a line.
         def orientation(point1: Location, point2: Location, point3: Location) -> str:
             """
             Internal method that will determine the orientation of three points. They can be a clockwise triangle,
             counterclockwise triangle, or a co-linear line segment.
             :param point1: the first point of the main line segment
```

### Comparing `pydraw-2.2a6/pydraw/overload.py` & `pydraw-2.2a7/pydraw/overload.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/pydraw/scene.py` & `pydraw-2.2a7/pydraw/scene.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/pydraw/screen.py` & `pydraw-2.2a7/pydraw/screen.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/pydraw/sound.py` & `pydraw-2.2a7/pydraw/sound.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/pydraw/turtle.py` & `pydraw-2.2a7/pydraw/turtle.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/pydraw/util.py` & `pydraw-2.2a7/pydraw/util.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/pydraw.egg-info/PKG-INFO` & `pydraw-2.2a7/pydraw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydraw
-Version: 2.2a6
+Version: 2.2a7
 Summary: A package designed to make graphics with Python simple and easy!
 Home-page: https://github.com/pydraw/pydraw
 Author: Noah Coetsee
 Author-email: noah@noahcoetsee.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydraw-2.2a6/pydraw.egg-info/SOURCES.txt` & `pydraw-2.2a7/pydraw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/setup.py` & `pydraw-2.2a7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import setuptools
 
 with open("/Users/noah/Projects/pydraw/README_pypi.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pydraw",
-    version="2.2a6",
+    version="2.2a7",
     author="Noah Coetsee",
     author_email="noah@noahcoetsee.me",
     description="A package designed to make graphics with Python simple and easy!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pydraw/pydraw",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'pillow'
+        'pillow',
+        # 'PyObjC',
+        'pygobject',
     ],
     python_requires='>=3.6',
 )
```

### Comparing `pydraw-2.2a6/tests/algorithms_test.py` & `pydraw-2.2a7/tests/algorithms_test.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/tests/blank_test.py` & `pydraw-2.2a7/tests/blank_test.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/tests/color_test.py` & `pydraw-2.2a7/tests/color_test.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/tests/image_test.py` & `pydraw-2.2a7/tests/image_test.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/tests/launcher.py` & `pydraw-2.2a7/tests/launcher.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/tests/location_test.py` & `pydraw-2.2a7/tests/location_test.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/tests/objects_test.py` & `pydraw-2.2a7/tests/objects_test.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/tests/polygon_test.py` & `pydraw-2.2a7/tests/polygon_test.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/tests/scene_test.py` & `pydraw-2.2a7/tests/scene_test.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/tests/screen_test.py` & `pydraw-2.2a7/tests/screen_test.py`

 * *Files identical despite different names*

### Comparing `pydraw-2.2a6/tests/tutorial.py` & `pydraw-2.2a7/tests/tutorial.py`

 * *Files identical despite different names*

