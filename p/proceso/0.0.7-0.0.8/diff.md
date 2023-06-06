# Comparing `tmp/proceso-0.0.7.tar.gz` & `tmp/proceso-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proceso-0.0.7.tar", last modified: Wed May  3 03:03:09 2023, max compression
+gzip compressed data, was "proceso-0.0.8.tar", last modified: Tue Jun  6 01:46:11 2023, max compression
```

## Comparing `proceso-0.0.7.tar` & `proceso-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-03 03:03:09.657988 proceso-0.0.7/
--rw-r--r--   0 nick       (501) staff       (20)     7652 2023-04-27 14:59:44.000000 proceso-0.0.7/LICENSE
--rw-r--r--   0 nick       (501) staff       (20)     4056 2023-05-03 03:03:09.658053 proceso-0.0.7/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     3416 2023-05-03 02:26:52.000000 proceso-0.0.7/README.md
--rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 14:06:11.000000 proceso-0.0.7/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)      778 2023-05-03 03:03:09.658318 proceso-0.0.7/setup.cfg
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-03 03:03:09.653005 proceso-0.0.7/src/
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-03 03:03:09.656633 proceso-0.0.7/src/proceso/
--rw-r--r--   0 nick       (501) staff       (20)       25 2023-05-03 02:55:31.000000 proceso-0.0.7/src/proceso/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)      341 2023-05-02 18:03:20.000000 proceso-0.0.7/src/proceso/_binding.py
--rw-r--r--   0 nick       (501) staff       (20)    11523 2023-05-02 18:03:22.000000 proceso-0.0.7/src/proceso/colors.py
--rw-r--r--   0 nick       (501) staff       (20)     9800 2023-05-02 18:03:25.000000 proceso-0.0.7/src/proceso/constants.py
--rw-r--r--   0 nick       (501) staff       (20)     3858 2023-05-03 03:02:50.000000 proceso-0.0.7/src/proceso/core.py
--rw-r--r--   0 nick       (501) staff       (20)     3563 2023-05-03 02:43:35.000000 proceso-0.0.7/src/proceso/data.py
--rw-r--r--   0 nick       (501) staff       (20)     9197 2023-05-02 18:03:30.000000 proceso-0.0.7/src/proceso/dom.py
--rw-r--r--   0 nick       (501) staff       (20)     8773 2023-05-02 18:03:32.000000 proceso-0.0.7/src/proceso/environment.py
--rw-r--r--   0 nick       (501) staff       (20)     1516 2023-05-02 18:03:35.000000 proceso-0.0.7/src/proceso/events.py
--rw-r--r--   0 nick       (501) staff       (20)    14015 2023-05-02 18:03:38.000000 proceso-0.0.7/src/proceso/images.py
--rw-r--r--   0 nick       (501) staff       (20)     1266 2023-05-03 02:49:03.000000 proceso-0.0.7/src/proceso/io.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-03 03:03:09.657841 proceso-0.0.7/src/proceso/math/
--rw-r--r--   0 nick       (501) staff       (20)      271 2023-05-02 16:58:34.000000 proceso-0.0.7/src/proceso/math/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     5959 2023-05-02 16:55:18.000000 proceso-0.0.7/src/proceso/math/calculation.py
--rw-r--r--   0 nick       (501) staff       (20)     3644 2023-05-02 16:55:50.000000 proceso-0.0.7/src/proceso/math/noise.py
--rw-r--r--   0 nick       (501) staff       (20)     1711 2023-05-02 16:57:42.000000 proceso-0.0.7/src/proceso/math/random.py
--rw-r--r--   0 nick       (501) staff       (20)     3871 2023-05-02 16:56:53.000000 proceso-0.0.7/src/proceso/math/trigonometry.py
--rw-r--r--   0 nick       (501) staff       (20)    61205 2023-05-02 18:29:09.000000 proceso-0.0.7/src/proceso/math/vector.py
--rw-r--r--   0 nick       (501) staff       (20)     6518 2023-05-02 22:30:00.000000 proceso-0.0.7/src/proceso/rendering.py
--rw-r--r--   0 nick       (501) staff       (20)    29994 2023-05-03 01:45:13.000000 proceso-0.0.7/src/proceso/shape.py
--rw-r--r--   0 nick       (501) staff       (20)     6114 2023-05-02 18:03:46.000000 proceso-0.0.7/src/proceso/structure.py
--rw-r--r--   0 nick       (501) staff       (20)    16233 2023-05-02 18:03:48.000000 proceso-0.0.7/src/proceso/sysvars.py
--rw-r--r--   0 nick       (501) staff       (20)    15708 2023-05-02 18:03:51.000000 proceso-0.0.7/src/proceso/three_d.py
--rw-r--r--   0 nick       (501) staff       (20)     7325 2023-05-02 18:03:55.000000 proceso-0.0.7/src/proceso/transform.py
--rw-r--r--   0 nick       (501) staff       (20)     6198 2023-05-02 18:03:57.000000 proceso-0.0.7/src/proceso/typography.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-03 03:03:09.657166 proceso-0.0.7/src/proceso.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     4056 2023-05-03 03:03:09.000000 proceso-0.0.7/src/proceso.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      801 2023-05-03 03:03:09.000000 proceso-0.0.7/src/proceso.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-05-03 03:03:09.000000 proceso-0.0.7/src/proceso.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)       12 2023-05-03 03:03:09.000000 proceso-0.0.7/src/proceso.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)        8 2023-05-03 03:03:09.000000 proceso-0.0.7/src/proceso.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-06 01:46:11.133770 proceso-0.0.8/
+-rw-r--r--   0 nick       (501) staff       (20)     7652 2023-04-27 14:59:44.000000 proceso-0.0.8/LICENSE
+-rw-r--r--   0 nick       (501) staff       (20)     7057 2023-06-06 01:46:11.133848 proceso-0.0.8/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     6421 2023-06-06 01:46:00.000000 proceso-0.0.8/README.md
+-rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 14:06:11.000000 proceso-0.0.8/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)      774 2023-06-06 01:46:11.134123 proceso-0.0.8/setup.cfg
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-06 01:46:11.128762 proceso-0.0.8/src/
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-06 01:46:11.131775 proceso-0.0.8/src/proceso/
+-rw-r--r--   0 nick       (501) staff       (20)       25 2023-05-13 19:35:20.000000 proceso-0.0.8/src/proceso/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      752 2023-06-06 01:36:01.000000 proceso-0.0.8/src/proceso/_binding.py
+-rw-r--r--   0 nick       (501) staff       (20)    11610 2023-05-14 15:52:15.000000 proceso-0.0.8/src/proceso/colors.py
+-rw-r--r--   0 nick       (501) staff       (20)     9800 2023-05-02 18:03:25.000000 proceso-0.0.8/src/proceso/constants.py
+-rw-r--r--   0 nick       (501) staff       (20)     3858 2023-05-03 03:02:50.000000 proceso-0.0.8/src/proceso/core.py
+-rw-r--r--   0 nick       (501) staff       (20)     3563 2023-05-03 02:43:35.000000 proceso-0.0.8/src/proceso/data.py
+-rw-r--r--   0 nick       (501) staff       (20)     9197 2023-05-02 18:03:30.000000 proceso-0.0.8/src/proceso/dom.py
+-rw-r--r--   0 nick       (501) staff       (20)     8773 2023-05-02 18:03:32.000000 proceso-0.0.8/src/proceso/environment.py
+-rw-r--r--   0 nick       (501) staff       (20)     1516 2023-05-02 18:03:35.000000 proceso-0.0.8/src/proceso/events.py
+-rw-r--r--   0 nick       (501) staff       (20)    14015 2023-05-02 18:03:38.000000 proceso-0.0.8/src/proceso/images.py
+-rw-r--r--   0 nick       (501) staff       (20)     1242 2023-05-03 03:10:04.000000 proceso-0.0.8/src/proceso/io.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-06 01:46:11.133611 proceso-0.0.8/src/proceso/math/
+-rw-r--r--   0 nick       (501) staff       (20)      271 2023-05-02 16:58:34.000000 proceso-0.0.8/src/proceso/math/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     5959 2023-05-02 16:55:18.000000 proceso-0.0.8/src/proceso/math/calculation.py
+-rw-r--r--   0 nick       (501) staff       (20)     3644 2023-05-02 16:55:50.000000 proceso-0.0.8/src/proceso/math/noise.py
+-rw-r--r--   0 nick       (501) staff       (20)     1711 2023-05-02 16:57:42.000000 proceso-0.0.8/src/proceso/math/random.py
+-rw-r--r--   0 nick       (501) staff       (20)     3871 2023-05-02 16:56:53.000000 proceso-0.0.8/src/proceso/math/trigonometry.py
+-rw-r--r--   0 nick       (501) staff       (20)    61205 2023-05-02 18:29:09.000000 proceso-0.0.8/src/proceso/math/vector.py
+-rw-r--r--   0 nick       (501) staff       (20)     6518 2023-05-02 22:30:00.000000 proceso-0.0.8/src/proceso/rendering.py
+-rw-r--r--   0 nick       (501) staff       (20)    30014 2023-05-16 23:59:32.000000 proceso-0.0.8/src/proceso/shape.py
+-rw-r--r--   0 nick       (501) staff       (20)     6114 2023-05-02 18:03:46.000000 proceso-0.0.8/src/proceso/structure.py
+-rw-r--r--   0 nick       (501) staff       (20)    16233 2023-05-02 18:03:48.000000 proceso-0.0.8/src/proceso/sysvars.py
+-rw-r--r--   0 nick       (501) staff       (20)    15708 2023-05-02 18:03:51.000000 proceso-0.0.8/src/proceso/three_d.py
+-rw-r--r--   0 nick       (501) staff       (20)     7325 2023-05-02 18:03:55.000000 proceso-0.0.8/src/proceso/transform.py
+-rw-r--r--   0 nick       (501) staff       (20)     6198 2023-05-02 18:03:57.000000 proceso-0.0.8/src/proceso/typography.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-06 01:46:11.132793 proceso-0.0.8/src/proceso.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     7057 2023-06-06 01:46:11.000000 proceso-0.0.8/src/proceso.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      801 2023-06-06 01:46:11.000000 proceso-0.0.8/src/proceso.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-06-06 01:46:11.000000 proceso-0.0.8/src/proceso.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)       12 2023-06-06 01:46:11.000000 proceso-0.0.8/src/proceso.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)        8 2023-06-06 01:46:11.000000 proceso-0.0.8/src/proceso.egg-info/top_level.txt
```

### Comparing `proceso-0.0.7/LICENSE` & `proceso-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/colors.py` & `proceso-0.0.8/src/proceso/colors.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,114 +5,114 @@
 
 
 class Colors(BaseSketch):
     # ==================
     # Creating & Reading
     # ==================
     def alpha(self, color: list[int] | str) -> int:
-        """Extracts the alpha value from a color or pixel array."""
+        """Extracts the alpha value from a color or pixel list."""
         if isinstance(color, list):
             return self._p5js.alpha(to_js(color))
         return self._p5js.alpha(color)
 
     def blue(self, color: list[int] | str) -> int:
-        """Extracts the blue value from a color or pixel array."""
+        """Extracts the blue value from a color or pixel list."""
         if isinstance(color, list):
             return self._p5js.blue(to_js(color))
         return self._p5js.blue(color)
 
     def brightness(self, color: list[int] | str) -> int:
-        """Extracts the HSB brightness value from a color or pixel array."""
+        """Extracts the HSB brightness value from a color or pixel list."""
         if isinstance(color, list):
             return self._p5js.brightness(to_js(color))
         return self._p5js.brightness(color)
 
     def color(
         self,
         value: str | int | list[int],
         v2: int | None = None,
         v3: int | None = None,
         v4: int | None = None,
     ) -> str:
         """Creates colors for storing in variables of the color datatype.
         The parameters are interpreted as RGB or HSB values depending on the
-        current color_mode(). The default mode is RGB values from 0 to 255 and,
-        therefore, the function call color(255, 204, 0) will return a bright
-        yellow color.
-
-        Note that if only one value is provided to color(), it will be interpreted
-        as a grayscale value. Add a second value, and it will be used for alpha
-        transparency. When three values are specified, they are interpreted as
-        either RGB or HSB values. Adding a fourth value applies alpha
-        transparency.
+        current color_mode(). The default mode is RGB values from 0 to 255
+        and, therefore, the function call color(255, 204, 0) will return a
+        bright yellow color.
+
+        Note that if only one value is provided to color(), it will be
+        interpreted as a grayscale value. Add a second value, and it will be
+        used for alpha transparency. When three values are specified, they are
+        interpreted as either RGB or HSB values. Adding a fourth value applies
+        alpha transparency.
 
         If a single string argument is provided, RGB, RGBA and Hex CSS color
-        strings and all named color strings are supported. In this case, an alpha
-        number value as a second argument is not supported, the RGBA form should
-        be used.
+        strings and all named color strings are supported. In this case, an
+        alpha number value as a second argument is not supported, the RGBA
+        form should be used.
         """
         if v4:
             return self._p5js.color(value, v2, v3, v4).toString()
         if v3:
             return self._p5js.color(value, v2, v3).toString()
         if v2:
             return self._p5js.color(value, v2).toString()
         return self._p5js.color(to_js(value)).toString()
 
     def green(self, color: str | list[int]) -> int:
-        """Extracts the green value from a color or pixel array."""
+        """Extracts the green value from a color or pixel list."""
         if isinstance(color, list):
             return self._p5js.green(to_js(color))
         return self._p5js.green(color)
 
     def hue(self, color: str | list[int]) -> int:
-        """Extracts the hue value from a color or pixel array.
+        """Extracts the hue value from a color or pixel list.
 
         Hue exists in both HSB and HSL. This function will return the
         HSB-normalized hue when supplied with an HSB color object (or when
-        supplied with a pixel array while the color mode is HSB),but will
+        supplied with a pixel list while the color mode is HSB),but will
         default to the HSL-normalized hue otherwise.
         (The values will only be different if the maximum hue setting for
         each system is different.)
         """
         if isinstance(color, list):
             return self._p5js.hue(to_js(color))
         return self._p5js.hue(color)
 
     def lerp_color(self, c1: str | list[int], c2: str | list[int], amt: float) -> str:
         """Blends two colors to find a third color somewhere between them.
         The amt parameter is the amount to interpolate between the two values
-        where 0.0 is equal to the first color, 0.1 is very near the first color,
-        0.5 is halfway in between, etc. An amount below 0 will be treated as 0.
-        Likewise, amounts above 1 will be capped at 1. This is different from the
-        behavior of lerp(), but necessary because otherwise numbers outside the
-        range will produce strange and unexpected colors.
+        where 0.0 is equal to the first color, 0.1 is very near the first
+        color, 0.5 is halfway in between, etc. An amount below 0 will be
+        treated as 0. Likewise, amounts above 1 will be capped at 1. This is
+        different from the behavior of lerp(), but necessary because otherwise
+        numbers outside the range will produce strange and unexpected colors.
 
         The way that colors are interpolated depends on the current color mode.
         """
         _c1 = self._p5js.color(to_js(c1))
         _c2 = self._p5js.color(to_js(c2))
         return self._p5js.lerpColor(_c1, _c2, amt).toString()
 
     def lightness(self, color: str | list[int]) -> int:
-        """Extracts the HSL lightness value from a color or pixel array."""
+        """Extracts the HSL lightness value from a color or pixel list."""
         if isinstance(color, list):
             return self._p5js.lightness(to_js(color))
         return self._p5js.lightness(color)
 
     def red(self, color: str | list[int]) -> int:
-        """Extracts the red value from a color or pixel array."""
+        """Extracts the red value from a color or pixel list."""
         return self._p5js.red(to_js(color))
 
     def saturation(self, color: str | list[int]) -> int:
-        """Extracts the saturation value from a color or pixel array.
+        """Extracts the saturation value from a color or pixel list.
 
         Saturation is scaled differently in HSB and HSL. This function will return
         the HSB saturation when supplied with an HSB color object (or when
-        supplied with a pixel array while the color mode is HSB), but will default
+        supplied with a pixel list while the color mode is HSB), but will default
         to the HSL saturation otherwise.
         """
         if isinstance(color, list):
             return self._p5js.saturation(to_js(color))
         return self._p5js.saturation(color)
 
     # =======
@@ -121,66 +121,75 @@
     def background(
         self,
         value: str | int | list[int],
         v2: int | None = None,
         v3: int | None = None,
         v4: int | None = None,
     ):
-        """The background() function sets the color used for the background of the p5 canvas.
-        The default background is transparent. This function is typically used within draw() to
-        clear the display window at the beginning of each frame, but it can be used inside setup()
-        to set the background on the first frame of animation or if the background need only be set once.
-
-        The color is either specified in terms of the RGB, HSB, or HSL color depending on the current color_mode.
-        (The default color space is RGB, with each value in the range from 0 to 255). The alpha range by default
-        is also 0 to 255.
-
-        A p5.Color object can also be provided to set the background color.
+        """The background() function sets the color used for the background of
+        the p5 canvas. The default background is transparent. This function is
+        typically used within draw() to clear the display window at the
+        beginning of each frame, but it can be used inside setup() to set the
+        background on the first frame of animation or if the background need
+        only be set once.
+
+        The color is either specified in terms of the RGB, HSB, or HSL color
+        depending on the current color_mode. (The default color space is RGB,
+        with each value in the range from 0 to 255). The alpha range by
+        default is also 0 to 255.
         """
         if v4:
             self._p5js.background(value, v2, v3, v4)
         elif v3:
             self._p5js.background(value, v2, v3)
         elif v2:
             self._p5js.background(value, v2)
         else:
             self._p5js.background(to_js(value))
 
-    def clear(self):
+    def clear(
+        self,
+        r: int | None = None,
+        g: int | None = None,
+        b: int | None = None,
+        a: int | None = None,
+    ):
         """Clears the pixels within a buffer.
-        This function only clears the canvas. It will not clear objects created by
-        create_x() functions such as createVideo() or createDiv(). Unlike the main
-        graphics context, pixels in additional graphics areas created with
-        create_graphics() can be entirely or partially transparent. This function
-        clears everything to make all of the pixels 100% transparent.
+        This function only clears the canvas. It will not clear objects
+        created by create_x() functions such as create_video() or
+        create_div(). Unlike the main graphics context, pixels in additional
+        graphics areas created with create_graphics() can be entirely or
+        partially transparent. This function clears everything to make all of
+        the pixels 100% transparent.
 
         Note: In WebGL mode, this function can be passed normalized RGBA color
-        values in order to clear the screen to a specific color. In addition to
-        color, it will also clear the depth buffer. If you are not using the
-        WebGL renderer these color values will have no effect.
+        values in order to clear the screen to a specific color. In addition
+        to color, it will also clear the depth buffer. If you are not using
+        the WebGL renderer these color values will have no effect.
         """
-        self._p5js.clear()
+        self._p5js.clear(r, g, b, a)
 
     def color_mode(
         self,
         mode: str,
         max1: int | None = None,
         max2: int | None = None,
         max3: int | None = None,
         max4: int | None = None,
     ):
         """color_mode() changes the way p5 interprets color data. By default,
         the parameters for fill(), stroke(), background(), and color() are
         defined by values between 0 and 255 using the RGB color model.
-        This is equivalent to setting color_mode(RGB, 255). Setting color_mode(HSB)
-        lets you use the HSB system instead. By default,
+        This is equivalent to setting color_mode(RGB, 255). Setting
+        color_mode(HSB) lets you use the HSB system instead. By default,
         this is color_mode(HSB, 360, 100, 100, 1). You can also use HSL.
 
-        Note: existing color objects remember the mode that they were created in,
-        so you can change modes as you like without affecting their appearance.
+        Note: existing color objects remember the mode that they were created
+        in, so you can change modes as you like without affecting their
+        appearance.
         """
         if max4:
             self._p5js.colorMode(mode, max1, max2, max3, max4)
         elif max3:
             self._p5js.colorMode(mode, max1, max2, max3)
         elif max2:
             self._p5js.colorMode(mode, max1, max2)
@@ -194,25 +203,24 @@
         value: str | int | list[int],
         v2: int | None = None,
         v3: int | None = None,
         v4: int | None = None,
     ):
         """Sets the color used to fill shapes.
         For example, if you run fill(204, 102, 0), all shapes drawn after the
-        fill() command will be filled with the color orange. This color is either
-        specified in terms of the RGB or HSB color depending on the current
-        color_mode(). (The default color space is RGB, with each value in the
-        range from 0 to 255). The alpha range by default is also 0 to 255.
+        fill() command will be filled with the color orange. This color is
+        either specified in terms of the RGB or HSB color depending on the
+        current color_mode(). (The default color space is RGB, with each value
+        in the range from 0 to 255). The alpha range by default is also 0 to
+        255.
 
         If a single string argument is provided, RGB, RGBA and Hex CSS color
-        strings and all named color strings are supported. In this case, an alpha
-        number value as a second argument is not supported, the RGBA form should
-        be used.
-
-        A p5.Color object can also be provided to set the fill color.
+        strings and all named color strings are supported. In this case, an
+        alpha number value as a second argument is not supported, the RGBA
+        form should be used.
         """
         if v4:
             self._p5js.fill(value, v2, v3, v4)
         elif v3:
             self._p5js.fill(value, v2, v3)
         elif v2:
             self._p5js.fill(value, v2)
@@ -222,57 +230,58 @@
     def no_fill(self):
         """Disables filling geometry. If both no_stroke() and no_fill() are
         called, nothing will be drawn to the screen.
         """
         self._p5js.noFill()
 
     def no_stroke(self):
-        """Disables drawing the stroke (outline). If both no_stroke() and
-        no_fill() are called, nothing will be drawn to the screen.
+        """Disables drawing the stroke (outline).
+        If both no_stroke() and no_fill() are called, nothing will be drawn to
+        the screen.
         """
         self._p5js.noStroke()
 
     def stroke(
         self,
         value: str | int | list[int],
         v2: int | None = None,
         v3: int | None = None,
         v4: int | None = None,
     ):
         """Sets the color used to draw lines and borders around shapes.
-        This color is either specified in terms of the RGB or HSB color depending
-        on the current color_mode() (the default color space is RGB, with each
-        value in the range from 0 to 255). The alpha range by default is also 0
-        to 255.
+        This color is either specified in terms of the RGB or HSB color
+        depending on the current color_mode() (the default color space is RGB,
+        with each value in the range from 0 to 255). The alpha range by
+        default is also 0 to 255.
 
         If a single string argument is provided, RGB, RGBA and Hex CSS color
-        strings and all named color strings are supported. In this case, an alpha
-        number value as a second argument is not supported, the RGBA form should
-        be used.
-
-        A p5.Color object can also be provided to set the stroke color.
+        strings and all named color strings are supported. In this case, an
+        alpha number value as a second argument is not supported, the RGBA
+        form should be used.
         """
         if v4:
             self._p5js.stroke(value, v2, v3, v4)
         elif v3:
             self._p5js.stroke(value, v2, v3)
         elif v2:
             self._p5js.stroke(value, v2)
         else:
             self._p5js.stroke(to_js(value))
 
-    def erase(self):
+    def erase(
+        self, strength_fill: int | None = None, strength_stroke: int | None = None
+    ):
         """All drawing that follows erase() will subtract from the canvas.
-        Erased areas will reveal the web page underneath the canvas. Erasing can
-        be canceled with no_rase().
+        Erased areas will reveal the web page underneath the canvas. Erasing
+        can be canceled with no_erase().
 
         Drawing done with image() and background() in between erase() and
         no_erase() will not erase the canvas but works as usual.
         """
-        self._p5js.erase()
+        self._p5js.erase(strength_fill, strength_stroke)
 
     def no_erase(self):
         """Ends erasing that was started with erase().
-        The fill(), stroke(), and blend_mode() settings will return to what they
-        were prior to calling erase().
+        The fill(), stroke(), and blend_mode() settings will return to what
+        they were prior to calling erase().
         """
         self._p5js.noErase()
```

### Comparing `proceso-0.0.7/src/proceso/constants.py` & `proceso-0.0.8/src/proceso/constants.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/core.py` & `proceso-0.0.8/src/proceso/core.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/data.py` & `proceso-0.0.8/src/proceso/data.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/dom.py` & `proceso-0.0.8/src/proceso/dom.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/environment.py` & `proceso-0.0.8/src/proceso/environment.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/events.py` & `proceso-0.0.8/src/proceso/events.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/images.py` & `proceso-0.0.8/src/proceso/images.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/io.py` & `proceso-0.0.8/src/proceso/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from ._binding import BaseSketch
 
 
 class IO(BaseSketch):
     def day(self) -> int:
         """The day() function returns the current day as a value from 1 - 31."""
         return self._p5js.day()
-    
+
     def hour(self) -> int:
         """The hour() function returns the current hour as a value from 0 - 23."""
         return self._p5js.hour()
-    
+
     def minute(self) -> int:
         """The minute() function returns the current minute as a value from 0 - 59."""
         return self._p5js.minute()
-    
+
     def millis(self) -> int:
         """Returns the number of milliseconds (thousandths of a second) since
         starting the sketch (when setup() is called).
         This information is often used for timing events and animation sequences.
         """
         return self._p5js.millis()
-    
+
     def month(self) -> int:
         """The month() function returns the current month as a value from 1 - 12."""
         return self._p5js.month()
-    
+
     def second(self) -> int:
         """The second() function returns the current second as a value from 0 - 59."""
         return self._p5js.second()
-    
+
     def year(self) -> int:
         """The year() function returns the current year as an integer (2014, 2015, 2016, etc)."""
         return self._p5js.year()
```

### Comparing `proceso-0.0.7/src/proceso/math/calculation.py` & `proceso-0.0.8/src/proceso/math/calculation.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/math/noise.py` & `proceso-0.0.8/src/proceso/math/noise.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/math/random.py` & `proceso-0.0.8/src/proceso/math/random.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/math/trigonometry.py` & `proceso-0.0.8/src/proceso/math/trigonometry.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/math/vector.py` & `proceso-0.0.8/src/proceso/math/vector.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/rendering.py` & `proceso-0.0.8/src/proceso/rendering.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/shape.py` & `proceso-0.0.8/src/proceso/shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,18 +92,18 @@
         detail_x: int | None = None,
         detail_y: int | None = None,
         *args,
     ):
         """Draws a quad on the canvas.
         A quad is a quadrilateral, a four-sided polygon. It is similar to a
         rectangle, but the angles between its edges are not constrained to ninety
-        degrees. The first pair of parameters (x1,y1) sets the first vertex and
-        the subsequent pairs should proceed clockwise or counter-clockwise around
-        the defined shape. z-arguments only work when quad() is used in WEBGL
-        mode.
+        degrees. The first pair of parameters (x1, y1) sets the first vertex
+        and the subsequent pairs should proceed clockwise or counter-clockwise
+        around the defined shape. z-arguments only work when quad() is used in
+        WEBGL mode.
         """
         self._p5js.quad(x1, y1, x2, y2, x3, y3, x4, y4, detail_x, detail_y, *args)
 
     def rect(
         self,
         x: float,
         y: float,
@@ -203,49 +203,51 @@
 
         In 3D mode, no_smooth() is enabled by default, so it is necessary to call
         smooth() if you would like smooth (antialiased) edges on your geometry.
         """
         self._p5js.noSmooth()
 
     def rect_mode(self, mode: str):
-        """Modifies the location from which rectangles are drawn by changing the
-        way in which parameters given to rect() are interpreted.
+        """Modifies the location from which rectangles are drawn by changing
+        the way in which parameters given to rect() are interpreted.
 
-        The default mode is CORNER, which interprets the first two parameters as
-        the upper-left corner of the shape, while the third and fourth parameters
-        are its width and height.
-
-        rectMode(CORNERS) interprets the first two parameters as the location of
-        one of the corners, and the third and fourth parameters as the location
-        of the diagonally opposite corner. Note, the rectangle is drawn between
-        the coordinates, so it is not necessary that the first corner be the
-        upper left corner.
-
-        rectMode(CENTER) interprets the first two parameters as the shape's center
-        point, while the third and fourth parameters are its width and height.
-
-        rectMode(RADIUS) also uses the first two parameters as the shape's center
-        point, but uses the third and fourth parameters to specify half of the
-        shape's width and height respectively.
+        The default mode is CORNER, which interprets the first two parameters
+        as the upper-left corner of the shape, while the third and fourth
+        parameters are its width and height.
+
+        rect_mode(CORNERS) interprets the first two parameters as the location
+        of one of the corners, and the third and fourth parameters as the
+        location of the diagonally opposite corner. Note, the rectangle is
+        drawn between the coordinates, so it is not necessary that the first
+        corner be the upper left corner.
 
-        The parameter to this function must be written in ALL CAPS because they
-        are predefined as constants in ALL CAPS and Python is a case-sensitive
-        language.
+        rect_mode(CENTER) interprets the first two parameters as the shape's
+        center point, while the third and fourth parameters are its width and
+        height.
+
+        rect_mode(RADIUS) also uses the first two parameters as the shape's
+        center point, but uses the third and fourth parameters to specify half
+        of the shape's width and height respectively.
+
+        The parameter to this function must be written in ALL CAPS because
+        they are predefined as constants in ALL CAPS and Python is a
+        case-sensitive language.
         """
         self._p5js.rectMode(mode)
 
     def smooth(self):
         """Draws all geometry with smooth (anti-aliased) edges.
         smooth() will also improve image quality of resized images.
 
         Note that smooth() is active by default in 2D mode; no_smooth() can be
         used to disable smoothing of geometry, images, and fonts.
 
-        In 3D mode, no_smooth() is enabled by default, so it is necessary to call
-        smooth() if you would like smooth (antialiased) edges on your geometry.
+        In 3D mode, no_smooth() is enabled by default, so it is necessary to
+        call smooth() if you would like smooth (antialiased) edges on your
+        geometry.
         """
         self._p5js.smooth()
 
     def stroke_cap(self, cap: str):
         """Sets the style for rendering line endings.
         These ends are either rounded, squared, or extended, each of which
         specified with the corresponding parameters: ROUND, SQUARE, or PROJECT.
```

### Comparing `proceso-0.0.7/src/proceso/structure.py` & `proceso-0.0.8/src/proceso/structure.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/sysvars.py` & `proceso-0.0.8/src/proceso/sysvars.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/three_d.py` & `proceso-0.0.8/src/proceso/three_d.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/transform.py` & `proceso-0.0.8/src/proceso/transform.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso/typography.py` & `proceso-0.0.8/src/proceso/typography.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.7/src/proceso.egg-info/SOURCES.txt` & `proceso-0.0.8/src/proceso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

