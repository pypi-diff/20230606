# Comparing `tmp/SimpleShape-1.3.tar.gz` & `tmp/SimpleShape-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleShape-1.3.tar", last modified: Mon Jun  5 14:54:53 2023, max compression
+gzip compressed data, was "SimpleShape-1.3.1.tar", last modified: Tue Jun  6 14:21:41 2023, max compression
```

## Comparing `SimpleShape-1.3.tar` & `SimpleShape-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 14:54:53.732040 SimpleShape-1.3/
--rw-rw-rw-   0        0        0     1069 2023-06-03 17:41:01.000000 SimpleShape-1.3/License.txt
--rw-rw-rw-   0        0        0     4925 2023-06-05 14:54:53.732040 SimpleShape-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4516 2023-06-05 12:17:47.000000 SimpleShape-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 14:54:53.714419 SimpleShape-1.3/SimpleShape/
--rw-rw-rw-   0        0        0      778 2023-06-04 16:46:20.000000 SimpleShape-1.3/SimpleShape/Example.py
--rw-rw-rw-   0        0        0    14118 2023-06-05 14:49:32.000000 SimpleShape-1.3/SimpleShape/SimpleShape.py
--rw-rw-rw-   0        0        0        2 2023-06-03 17:34:06.000000 SimpleShape-1.3/SimpleShape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:54:53.731056 SimpleShape-1.3/SimpleShape.egg-info/
--rw-rw-rw-   0        0        0     4925 2023-06-05 14:54:53.000000 SimpleShape-1.3/SimpleShape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-06-05 14:54:53.000000 SimpleShape-1.3/SimpleShape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 14:54:53.000000 SimpleShape-1.3/SimpleShape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-05 14:54:53.000000 SimpleShape-1.3/SimpleShape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-06-05 14:54:53.733028 SimpleShape-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-06-05 14:51:32.000000 SimpleShape-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:21:41.393876 SimpleShape-1.3.1/
+-rw-rw-rw-   0        0        0     1069 2023-06-03 17:41:01.000000 SimpleShape-1.3.1/License.txt
+-rw-rw-rw-   0        0        0     4945 2023-06-06 14:21:41.393876 SimpleShape-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4539 2023-06-06 12:50:04.000000 SimpleShape-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 14:21:41.378250 SimpleShape-1.3.1/SimpleShape/
+-rw-rw-rw-   0        0        0      780 2023-06-06 06:03:25.000000 SimpleShape-1.3.1/SimpleShape/Example.py
+-rw-rw-rw-   0        0        0    14010 2023-06-06 11:28:46.000000 SimpleShape-1.3.1/SimpleShape/SimpleShape.py
+-rw-rw-rw-   0        0        0        2 2023-06-03 17:34:06.000000 SimpleShape-1.3.1/SimpleShape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:21:41.393876 SimpleShape-1.3.1/SimpleShape.egg-info/
+-rw-rw-rw-   0        0        0     4945 2023-06-06 14:21:41.000000 SimpleShape-1.3.1/SimpleShape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-06-06 14:21:41.000000 SimpleShape-1.3.1/SimpleShape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 14:21:41.000000 SimpleShape-1.3.1/SimpleShape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-06 14:21:41.000000 SimpleShape-1.3.1/SimpleShape.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-06-06 14:21:41.393876 SimpleShape-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-06-06 14:20:42.000000 SimpleShape-1.3.1/setup.py
```

### Comparing `SimpleShape-1.3/License.txt` & `SimpleShape-1.3.1/License.txt`

 * *Files identical despite different names*

### Comparing `SimpleShape-1.3/PKG-INFO` & `SimpleShape-1.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SimpleShape
-Version: 1.3
-Summary: A simple package for creating geometric objects and 
+Version: 1.3.1
+Summary: A simple package for creating geometric objects
 Author: Tilen Žel
 Author-email: tilen.zel@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -20,42 +20,42 @@
 - Create and visualise various geometric objects: Triangle, Rectangle, Polygon, Circle and Ellipse
 - Calculate their perimeter and their area
 - Check if two objects intersect
 - Save and load geometric objects to and from JSON files
 
 ## Installation
 
-Download and expand the zip (.whl) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document, or use **pip install SimpleShape**. Then, write **import SimpleShape** in your python document to begin using the package.
+Download and expand the zip (.tar.gz) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document, or use **pip install SimpleShape**. Then, write **import SimpleShape** in your python document to begin using the package.
 
 ## 1. Instructions
 
 To start using this project, create the Geometric object with available classes and perform different methods (see section 1.1). You can also check example.py, located in the SimpleShape subfolder, for a quick overwiev on how to use this package.
 
 This package also provides various functions that are described in section 1.2.
 
 ### 1.1 Geometric Classes and Methods
 
 ##### Class Geometry(coordinates): 
 
-Parent class for creating geometric objects. Here, coordinates is 2-D array of arrays that represent coordinates in x-y plane (one example being coordinates = [(0,0), (2,0), (4,4), (0,4)]). In case of Ellipse and Circle, different parameters are inserted (see below), for example the coordinates of their center.
+Parent class for creating geometric objects. Here, coordinates is 2-D array of arrays that represent points in x-y plane (one example being coordinates = [(0,0), (2,0), (4,4), (0,4)]). In case of Ellipse and Circle, different parameters are inserted (see below), for example the coordinates of their center.
 
 ###### Parent class has following methods:
 
 - \_\_init__(self, coordinates): Initialization method for the object.
 - \_\_str__(self) -> str: String representation of the object, obtained using print(object)
 - perimeter(self) -> float: Returns the perimeter of the geometric object
 - area(self) -> float: Returns the area of the geometric object
 - intersect(self, other) -> bool: Check if two objects intersect. Note that tangency also counts as intersection
 - visualize(self): Visualize the object using matplotlib module
 
 Aside from these methods, there are various functions to convert geometric objects to and from JSON format. See section 1.2 for more details.
 
 ##### Class Triangle(coordinates):
 
-A class for creating triangles using three points (f.e. [(0,0), (2,0), (4,4)]).
+A class for creating triangles using three points (f.e. coordinates = [(0,0), (2,0), (4,4)]).
 
 ##### Class Rectangle(coordinates):
 
 A class for creating rectangles using four points that need to be inserted in clockwise or counter-clockwise order. 
 
 ##### Class Polygon(coordinates):
 
@@ -63,29 +63,29 @@
 
 ##### Class Circle(r, center = (0, 0)):
 
 A class for creating circles. Here, r is radius (r > 0) and center (default value (0,0)) represents center of the circle on x-y plane. 
 
 ##### Class Ellipse(a, b, f = 0, center = (0, 0)):
 
-A class for creating ellipses. Here, a is the major axis, b is the minor axis (a,b > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
+A class for creating ellipses. Here, a is the width of the ellipse, b is its height (a,b > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
 
 ### 1.2 Functions
 
 This package contains functions for working with JSON data as well as other functions that perform different operations on geometric objects.
 
 ##### JSON functions:
 
-- **to_json(self) -> json**: Convert the geometric object to .JSON format
-- **from\_json(json\_data) -> object**: Create a geometric object from JSON data
-- **save_shapes(shapes, filename)**: Save json_data (shapes) to file (filename)
-- **load_shapes(filename):** Load json_data from a file (filename)
+- **to\_json(object\_list):** Convert the list of objects to JSON string using object attributes
+- **save\_shapes(json\_data, filename):** Write JSON string to a .json file
+- **load\_shapes(filename):** Create JSON string from a .json file
+- **from\_json(json\_data):** Create a list of objects from a JSON string
 
 ##### Other functions:
 
 - **random_shape(shape)**: Create a geometric object of random dimensions. If the shape parameter is not specified, an arbitrary geometric object will be returned. Otherwise, insert one of the following as an argument: "Rectangle", "Triangle", "Circle", "Ellipse", "Polygon".
 - **rotate(P1, P2, f)**: Rotate point P1 (x1,y1) around point P2 (x2,y2) for angle f in radians.        
 - **intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
 - **parallel(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) are parallel
 - **Line_Intersect_Circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
 
-**Note: Tangency is also considered an intersection!**
+**Note: Tangency also counts as intersection!**
```

### Comparing `SimpleShape-1.3/README.md` & `SimpleShape-1.3.1/SimpleShape.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,61 @@
+Metadata-Version: 2.1
+Name: SimpleShape
+Version: 1.3.1
+Summary: A simple package for creating geometric objects
+Author: Tilen Žel
+Author-email: tilen.zel@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: License.txt
+
 # README
 
 This project enables the creation of different geometric objects, on which we can perform different operations, like calculation of their perimeter.
 
 ## Features
 
 - Create and visualise various geometric objects: Triangle, Rectangle, Polygon, Circle and Ellipse
 - Calculate their perimeter and their area
 - Check if two objects intersect
 - Save and load geometric objects to and from JSON files
 
 ## Installation
 
-Download and expand the zip (.whl) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document, or use **pip install SimpleShape**. Then, write **import SimpleShape** in your python document to begin using the package.
+Download and expand the zip (.tar.gz) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document, or use **pip install SimpleShape**. Then, write **import SimpleShape** in your python document to begin using the package.
 
 ## 1. Instructions
 
 To start using this project, create the Geometric object with available classes and perform different methods (see section 1.1). You can also check example.py, located in the SimpleShape subfolder, for a quick overwiev on how to use this package.
 
 This package also provides various functions that are described in section 1.2.
 
 ### 1.1 Geometric Classes and Methods
 
 ##### Class Geometry(coordinates): 
 
-Parent class for creating geometric objects. Here, coordinates is 2-D array of arrays that represent coordinates in x-y plane (one example being coordinates = [(0,0), (2,0), (4,4), (0,4)]). In case of Ellipse and Circle, different parameters are inserted (see below), for example the coordinates of their center.
+Parent class for creating geometric objects. Here, coordinates is 2-D array of arrays that represent points in x-y plane (one example being coordinates = [(0,0), (2,0), (4,4), (0,4)]). In case of Ellipse and Circle, different parameters are inserted (see below), for example the coordinates of their center.
 
 ###### Parent class has following methods:
 
 - \_\_init__(self, coordinates): Initialization method for the object.
 - \_\_str__(self) -> str: String representation of the object, obtained using print(object)
 - perimeter(self) -> float: Returns the perimeter of the geometric object
 - area(self) -> float: Returns the area of the geometric object
 - intersect(self, other) -> bool: Check if two objects intersect. Note that tangency also counts as intersection
 - visualize(self): Visualize the object using matplotlib module
 
 Aside from these methods, there are various functions to convert geometric objects to and from JSON format. See section 1.2 for more details.
 
 ##### Class Triangle(coordinates):
 
-A class for creating triangles using three points (f.e. [(0,0), (2,0), (4,4)]).
+A class for creating triangles using three points (f.e. coordinates = [(0,0), (2,0), (4,4)]).
 
 ##### Class Rectangle(coordinates):
 
 A class for creating rectangles using four points that need to be inserted in clockwise or counter-clockwise order. 
 
 ##### Class Polygon(coordinates):
 
@@ -50,29 +63,29 @@
 
 ##### Class Circle(r, center = (0, 0)):
 
 A class for creating circles. Here, r is radius (r > 0) and center (default value (0,0)) represents center of the circle on x-y plane. 
 
 ##### Class Ellipse(a, b, f = 0, center = (0, 0)):
 
-A class for creating ellipses. Here, a is the major axis, b is the minor axis (a,b > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
+A class for creating ellipses. Here, a is the width of the ellipse, b is its height (a,b > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
 
 ### 1.2 Functions
 
 This package contains functions for working with JSON data as well as other functions that perform different operations on geometric objects.
 
 ##### JSON functions:
 
-- **to_json(self) -> json**: Convert the geometric object to .JSON format
-- **from\_json(json\_data) -> object**: Create a geometric object from JSON data
-- **save_shapes(shapes, filename)**: Save json_data (shapes) to file (filename)
-- **load_shapes(filename):** Load json_data from a file (filename)
+- **to\_json(object\_list):** Convert the list of objects to JSON string using object attributes
+- **save\_shapes(json\_data, filename):** Write JSON string to a .json file
+- **load\_shapes(filename):** Create JSON string from a .json file
+- **from\_json(json\_data):** Create a list of objects from a JSON string
 
 ##### Other functions:
 
 - **random_shape(shape)**: Create a geometric object of random dimensions. If the shape parameter is not specified, an arbitrary geometric object will be returned. Otherwise, insert one of the following as an argument: "Rectangle", "Triangle", "Circle", "Ellipse", "Polygon".
 - **rotate(P1, P2, f)**: Rotate point P1 (x1,y1) around point P2 (x2,y2) for angle f in radians.        
 - **intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
 - **parallel(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) are parallel
 - **Line_Intersect_Circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
 
-**Note: Tangency is also considered an intersection!**
+**Note: Tangency also counts as intersection!**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `SimpleShape-1.3/SimpleShape/Example.py` & `SimpleShape-1.3.1/SimpleShape/Example.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Example document to provide quick overwiev on how to use this package
+Example document to provide a quick overwiev on how to use this package
 """
 
 # Import the Main file
 import SimpleShape as sh
 
 # a) Create a Triangle and perform simple operations
```

### Comparing `SimpleShape-1.3/SimpleShape/SimpleShape.py` & `SimpleShape-1.3.1/SimpleShape/SimpleShape.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 """
 Main document with definitions of classes, methods, and functions
 """
 
+# Import libraries
+
 import json
 from math import pi, sqrt, sin, cos
 from matplotlib import pyplot as plt
 from matplotlib.patches import Ellipse as _Ellipse
 import numpy as np
 
+# Parent Class
+
 class Geometry:
     """Parent class for creating geometric objects"""
     
     def __init__(self, coordinates):
         """Initialization of the object. Somewhat different for
         circle and ellipse"""
+        self.type = self.__class__.__name__
         self.coordinates = coordinates
+
+        for element in self.coordinates:
+            if len(element) != 2:
+                raise Warning("Provide 2 elements for each point")
     
     def __str__(self) -> str:
         """A string representation of the object"""
         return ("The coordinates of the " + self.__class__.__name__ + " are " + 
         str(self.coordinates))
 
     def perimeter(self) -> float:
@@ -35,15 +44,15 @@
         for i in range(len(self.coordinates)):             
             s += (self.coordinates[i-1][0] * self.coordinates[i][1] -
                   self.coordinates[i][0] * self.coordinates[i-1][1])
         return abs(s/2)
             
     
     def intersect(self, other) -> bool:
-        """Check if there is an intersection. Note that tangency also counts as intersection"""
+        """Check if there is an intersection. This includes tangency"""
         if self.__class__.__name__ in ('Triangle','Rectangle','Polygon'):
             if isinstance(other, (Triangle or Rectangle or Polygon)):
                 for i in range(len(self.coordinates)):
                     for j in range(len(other.coordinates)):
                         if intersect(self.coordinates[i-1],self.coordinates[i],
                                      other.coordinates[j-1],other.coordinates[j]):
                             return True
@@ -64,15 +73,15 @@
         
        
         elif self.__class__.__name__ == ('Circle'):
             if isinstance(other, Circle):
                 distance = sqrt((self.center[0]-other.center[0])**2+
                             (self.center[1]-other.center[1])**2)
                 if distance > abs(self.r - other.r): 
-                    return distance < (self.r + other.r)
+                    return distance <= (self.r + other.r)
                 return False
             elif isinstance(other, (Triangle or Rectangle or Polygon)):
                 for i in range(len(other.coordinates)):
                     if Line_Intersect_Circle(other.coordinates[i-1], 
                                              other.coordinates[i], 
                                              self.center, self.r):
                         return True
@@ -92,157 +101,100 @@
     def visualize(self) -> None:
         
         X = np.array(self.coordinates)
         plt.figure()
         plt.scatter(X[:, 0], X[:, 1], s = 20)
         t1 = plt.Polygon(X[:,:])
         plt.gca().add_patch(t1)
-            
-# Functions for working with json data
-
-def to_json(self, name) -> json:
-        """Convert the object to .json format"""
-        if self.__class__.__name__ in ('Triangle', 'Rectangle', 'Polygon'):
-            return {
-		        'name': name,
-                'type': self.__class__.__name__,
-                'coordinates': self.coordinates
-            }
-        elif self.__class__.__name__ == 'Circle':
-            return {
-		        'name': name,
-                'type': self.__class__.__name__,
-                'r': self.r,
-                'center':self.center
-            }
-        elif self.__class__.__name__ == 'Ellipse':
-            return {
-		        'name': name,
-                'type': self.__class__.__name__,
-                'a': self.a,
-                'b': self.b,
-                'f': self.f,
-                'center':self.center
-            }
-        else:
-            raise Warning('Invalid JSON data. Try something else')
-
-def from_json(json_data) -> object:
-    """Create a geometric object from JSON data."""
-    
-    if json_data['type'] == 'Triangle':
-        return Triangle(json_data['coordinates'])
-    elif json_data['type'] == 'Rectangle':
-        return Rectangle(json_data['coordinates'])
-    elif json_data['type'] == 'Polygon':
-        return Polygon(json_data['coordinates'])
-    elif json_data['type'] == 'Circle':
-        return Circle(json_data['r'], json_data['center'])
-    elif json_data['type'] == 'Ellipse':
-        return Ellipse(json_data['a'],json_data['b'],
-                       json_data['f'], json_data['center'])
-    else:
-        raise Warning('Invalid JSON data. Try something else')
-        
-def save_shapes(shapes, filename):
-    """Save json_data to file"""
-    json_object = json.dumps(shapes)
-    with open(filename, 'a') as outfile:
-        outfile.write(json_object)
-
-def load_shapes(filename):
-    """Load json_data from a file"""
-    with open(filename, 'r') as file:
-        json_data = json.load(file)
-        return json_data 
-
+        plt.show()
 
-# Basic shapes (rectangle, Triangle, circle, elipsoid, point, line)
+# Child classes (Triangle, Rectangle, Polygon, Circle, Ellipse)
 
 class Triangle(Geometry):
     
     def __init__(self, coordinates):
         super().__init__(coordinates)
 
         self.a = coordinates[0]
         self.b = coordinates[1]
         self.c = coordinates[2]
-        
-        if (2 != len(self.a) or 2 != len(self.b) or 2 != len(self.c)):
-            raise Warning("Provide a 3x2 array or tuple")
+
         if (len(self.coordinates) != 3):
             raise Warning("Provide a 3x2 array or tuple")
         if parallel(self.a,self.b,self.b,self.c):
             raise Warning("Not a triangle. Try again") 
-        if (self.a == self.b or self.a == self.c or self.b == self.c):
+        if (self.a in (self.b, self.c) or self.b == self.c):
             raise Warning("Not a triangle. Try again")
 
     
     
 class Rectangle(Geometry):
-    """Insert coordinates in clockwise or counter-clockwise direction"""
+    """Insert points in clockwise or counter-clockwise direction"""
     def __init__(self, coordinates):
         super().__init__(coordinates)
         self.a = coordinates[0]
         self.b = coordinates[1]
         self.c = coordinates[2]
         self.d = coordinates[3]
+
+        self.ab = (self.a[0]-self.b[0],self.a[1]-self.b[1])
+        self.bc = (self.b[0]-self.c[0],self.b[1]-self.c[1])
+        self.cd = (self.c[0]-self.d[0],self.c[1]-self.d[1])
+        self.da = (self.d[0]-self.a[0],self.d[1]-self.a[1])
         
-        if (2 != len(self.a) or 2 != len(self.b) or 2 != len(self.c) or 2 != len(self.d)):
-            raise Warning("Provide a 4x2 array or tuple")
+        self.ac = sqrt((self.a[0]-self.c[0])**2+(self.a[1]-self.c[1])**2)
+        self.bd = sqrt((self.b[0]-self.d[0])**2+(self.b[1]-self.d[1])**2)
+
+        eps = 1e-6
         if (len(self.coordinates) != 4):
             raise Warning("Provide a 4x2 array or tuple")
-        if not (parallel(self.a,self.b,self.c,self.d) and parallel(self.b,self.c,self.a,self.d)):
+        if (self.ab[0]+self.cd[0]>eps or self.bc[0]+self.da[0]>eps or self.ac-self.bd>eps):
             raise Warning('Not a rectangle. Try again')
-        if (self.a == self.b or self.a == self.c or self.a == self.d):
+        if (self.ab[1]+self.cd[1]>eps or self.bc[1]+self.da[1]>eps):
+            raise Warning('Not a rectangle. Try again')
+        if self.a in (self.b, self.c, self.d):
             raise Warning("Not a rectangle. Try again")
-        if (self.b == self.c or self.b == self.d or self.c == self.d):
+        if (self.b in (self.c, self.d) or self.c == self.d):
             raise Warning("Not a rectangle. Try again")
             
 class Polygon(Geometry):
     """Insert coordinates in specific order"""
     def __init__(self, coordinates):
         super().__init__(coordinates)
 
-
         if len(self.coordinates) < 3:
             raise Warning("Provide a nx2 array or tuple, where n > 2")
-        for element in self.coordinates:
-            if len(element) != 2:
-                raise Warning("Provide a nx2 array or tuple, where n > 2")
-                break
+        # Check for parallelism
+        for i in range(len(self.coordinates)):
+            if parallel(self.coordinates[i-1],self.coordinates[i],
+                         self.coordinates[i-2],self.coordinates[i-1]):
+                raise Warning("One of the edges in polygon is 180°. Try again")
         # Check if polygon is self intersectiong
         self.is_intersected = 0
         for i in range(1, len(self.coordinates)):
             if self.is_intersected == 1: break
             for j in range(i-1): # To not consider neighbours
                 if intersect(self.coordinates[i-1],self.coordinates[i],
                              self.coordinates[j-1],self.coordinates[j]):
                     if i - j != len(self.coordinates)-1: # To not consider last and first element together
                         self.is_intersected = 1
-                        print("""This Polygon is not a simple polygon. Therefore, the calculated area will presumably be incorrect""")
+                        print("This polygon is not a simple polygon. The result of area() method will presumably be incorrect")
                         break
 
-
-        # Check for parallelism
-        for i in range(len(self.coordinates)):
-            if parallel(self.coordinates[i-1],self.coordinates[i],
-                         self.coordinates[i-2],self.coordinates[i-1]):
-                raise Warning("One of the edges in polygon is 180°. Try again")
-            
-                            
-
+       
+                        
 class Circle(Geometry):
     
     def __init__(self, r, center = (0,0)):
+        self.type = self.__class__.__name__
         self.r = r
         self.center = center
         
         if r <= 0: raise Warning("Radius is 0 or less. Use another radius")
-        if len(self.center) != 2: raise Warning("Not a center point. Try again")
+        if len(self.center) != 2: raise Warning("Use a center point with two dimensions")
     
     def __str__(self):
         return ("Circle with radius " + str(self.r) + " and center in " +
                 str(self.center)) 
 
     def area(self):
         return pi * self.r**2
@@ -250,71 +202,113 @@
     def perimeter(self):
         return 2 * pi * self.r
            
            
     def visualize(self):
         circle=plt.Circle(self.center, self.r)
         fig, ax = plt.subplots()
-        ax.set_xlim(((self.center[0]-self.r)*0.9, (self.center[0]+self.r)*1.1))
-        ax.set_ylim(((self.center[1]-self.r)*0.9, (self.center[1]+self.r)*1.1))
+        ax.set_xlim((self.center[0]-1.1*self.r, self.center[0]+self.r*1.1))
+        ax.set_ylim((self.center[1]-1.1*self.r, self.center[1]+self.r*1.1))
         ax.add_patch(circle)
-        
+        plt.show()
+
     
 class Ellipse(Geometry):
     def __init__(self, a, b, f = 0, center = (0,0)):
+        self.type = self.__class__.__name__
         self.a = a
         self.b = b
         self.f = f
         self.center = center
 
         if a <= 0: raise Warning("a is 0 or less. Use another a")
         if b <= 0: raise Warning("b is 0 or less. Use another b")
-        if len(self.center) != 2: raise Warning("Not a center point. Try again")
+        if len(self.center) != 2: raise Warning("Use a center point with two dimensions")
         
     def __str__(self):
         return ("Ellipse with a = " + str(self.a) + ", b = " + str(self.b) +
                 ", rotation of " + str(self.f) + "° and center at " + str(self.center)) 
 
     def area(self):
         return pi * self.a * self.b
 
     def perimeter(self):
         """Approximate calculation using Ramaujan formula"""
         return pi * (3*(self.a+self.b) - 
-                     sqrt( (3*self.a + self.b) * (self.a + 3*self.b) ) )
+                     sqrt((3*self.a + self.b) * (self.a + 3*self.b)))
            
     def visualize(self):
         fig, ax = plt.subplots()
 
         ax.axis('equal')
         ell = _Ellipse(xy=self.center, width=self.a, height=self.b, angle=self.f
                        , lw=4)
         
         ax.add_artist(ell)
         
         temp = max(self.a,self.b)
-        ax.set_xlim(((self.center[0]-temp)*0.9, (self.center[0]+temp)*1.1))
-        ax.set_ylim(((self.center[1]-temp)*0.9, (self.center[1]+temp)*1.1))
+        ax.set_xlim((self.center[0]-1.1*temp, self.center[0]+temp*1.1))
+        ax.set_ylim((self.center[1]-1.1*temp, self.center[1]+temp*1.1))
         
         plt.show()
 
 
+# JSON functions
 
+def to_json(object_list):
+    """Convert the list of objects to JSON string using object attributes"""
+    return json.dumps([obj.__dict__ for obj in object_list])
+    
+def save_shapes(json_data, filename):
+    """Write JSON string to a .json file"""
+    with open(filename, 'w') as outfile:
+        outfile.write(json_data)
         
+def load_shapes(filename):
+    """Convert a .json file to a JSON string"""
+    with open(filename, 'r') as file:
+        json_data = json.load(file)
+    return json_data 
+        
+
+def from_json(json_data):
+    """Create a list of objects from JSON string"""
+    object_list = []
+    for element in json_data:
+        if element['type'] == 'Triangle':
+            object_list.append(Triangle(element['coordinates']))
+        elif element['type'] == 'Rectangle':
+            object_list.append(Rectangle(element['coordinates']))
+        elif element['type'] == 'Polygon':
+            object_list.append(Polygon(element['coordinates']))
+        elif element['type'] == 'Circle':
+            object_list.append(Circle(element['r'], element['center']))
+        elif element['type'] == 'Ellipse':
+            object_list.append(Ellipse(element['a'],element['b'],
+                           element['f'], element['center']))
+        else:
+            print('Invalid JSON data. Will not be used to create an object')
+    return object_list
+
+# Other functions
+
 def random_shape(shape = next(iter({"Rectangle", "Triangle", "Circle", "Ellipse", "Polygon"}))):
     
     if shape == "Triangle":
-        return Triangle(np.random.uniform(-1000, 1000, (3,2)))
+        a,b,c = np.random.uniform(-1000, 1000,(3,2))
+        return Triangle(([a[0],a[1]],[b[0],b[1]],[c[0],c[1]]))
     elif shape == "Rectangle":
         [a, b] = np.random.uniform(-1000,1000, (2,1))
         _min = min(a,b)[0]
         _max = max(a,b)[0]
+        avg = (_min+_max)/2
+        center=(avg,avg)
         f = 2*pi*np.random.uniform(0,1) # Radians
         P1,P2,P3,P4 = [_min,_min],[_max,_min],[_max,_max],[_min,_max]
-        P2,P3,P4 = rotate(P2,P1,f), rotate(P3,P1,f), rotate(P4,P1,f)
+        P1,P2,P3,P4 = rotate(P1,center,f),rotate(P2,center,f), rotate(P3,center,f), rotate(P4,center,f)
         return Rectangle([P1,P2,P3,P4])
     elif shape == "Polygon":
         num = np.random.randint(3,100)	
         return Polygon(np.random.uniform(-1000, 1000, (num,2)))
     elif shape == "Circle":
         r = np.random.uniform(0.1,1000)
         [x, y] = np.random.uniform(-1000,1000, (2,1))
@@ -343,15 +337,16 @@
 def intersect(A,B,C,D):
     def ccw(A,B,C):
         return (C[1]-A[1])*(B[0]-A[0]) > (B[1]-A[1])*(C[0]-A[0])
     return ccw(A,C,D) != ccw(B,C,D) and ccw(A,B,C) != ccw(A,B,D)
 
 def parallel(A,B,C,D):
     if B[0] == A[0]: return (True if C[0] == D[0] else False)
-    return abs((B[1]-A[1])/(B[0]-A[0])) == abs((D[1]-C[1])/(D[0]-C[0]))
+    if C[0] == D[0]: return (True if A[0] == B[0] else False)
+    return (B[1]-A[1])/(B[0]-A[0]) == (D[1]-C[1])/(D[0]-C[0])
 
 # Taken and modified from 
 # https://stackoverflow.com/questions/1073336/circle-line-segment-collision-detection-algorithm
 # (chmike answer)
 
 def Line_Intersect_Circle(A, B, c, r):
```

### Comparing `SimpleShape-1.3/SimpleShape.egg-info/PKG-INFO` & `SimpleShape-1.3.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,48 @@
-Metadata-Version: 2.1
-Name: SimpleShape
-Version: 1.3
-Summary: A simple package for creating geometric objects and 
-Author: Tilen Žel
-Author-email: tilen.zel@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: License.txt
-
 # README
 
 This project enables the creation of different geometric objects, on which we can perform different operations, like calculation of their perimeter.
 
 ## Features
 
 - Create and visualise various geometric objects: Triangle, Rectangle, Polygon, Circle and Ellipse
 - Calculate their perimeter and their area
 - Check if two objects intersect
 - Save and load geometric objects to and from JSON files
 
 ## Installation
 
-Download and expand the zip (.whl) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document, or use **pip install SimpleShape**. Then, write **import SimpleShape** in your python document to begin using the package.
+Download and expand the zip (.tar.gz) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document, or use **pip install SimpleShape**. Then, write **import SimpleShape** in your python document to begin using the package.
 
 ## 1. Instructions
 
 To start using this project, create the Geometric object with available classes and perform different methods (see section 1.1). You can also check example.py, located in the SimpleShape subfolder, for a quick overwiev on how to use this package.
 
 This package also provides various functions that are described in section 1.2.
 
 ### 1.1 Geometric Classes and Methods
 
 ##### Class Geometry(coordinates): 
 
-Parent class for creating geometric objects. Here, coordinates is 2-D array of arrays that represent coordinates in x-y plane (one example being coordinates = [(0,0), (2,0), (4,4), (0,4)]). In case of Ellipse and Circle, different parameters are inserted (see below), for example the coordinates of their center.
+Parent class for creating geometric objects. Here, coordinates is 2-D array of arrays that represent points in x-y plane (one example being coordinates = [(0,0), (2,0), (4,4), (0,4)]). In case of Ellipse and Circle, different parameters are inserted (see below), for example the coordinates of their center.
 
 ###### Parent class has following methods:
 
 - \_\_init__(self, coordinates): Initialization method for the object.
 - \_\_str__(self) -> str: String representation of the object, obtained using print(object)
 - perimeter(self) -> float: Returns the perimeter of the geometric object
 - area(self) -> float: Returns the area of the geometric object
 - intersect(self, other) -> bool: Check if two objects intersect. Note that tangency also counts as intersection
 - visualize(self): Visualize the object using matplotlib module
 
 Aside from these methods, there are various functions to convert geometric objects to and from JSON format. See section 1.2 for more details.
 
 ##### Class Triangle(coordinates):
 
-A class for creating triangles using three points (f.e. [(0,0), (2,0), (4,4)]).
+A class for creating triangles using three points (f.e. coordinates = [(0,0), (2,0), (4,4)]).
 
 ##### Class Rectangle(coordinates):
 
 A class for creating rectangles using four points that need to be inserted in clockwise or counter-clockwise order. 
 
 ##### Class Polygon(coordinates):
 
@@ -63,29 +50,29 @@
 
 ##### Class Circle(r, center = (0, 0)):
 
 A class for creating circles. Here, r is radius (r > 0) and center (default value (0,0)) represents center of the circle on x-y plane. 
 
 ##### Class Ellipse(a, b, f = 0, center = (0, 0)):
 
-A class for creating ellipses. Here, a is the major axis, b is the minor axis (a,b > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
+A class for creating ellipses. Here, a is the width of the ellipse, b is its height (a,b > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
 
 ### 1.2 Functions
 
 This package contains functions for working with JSON data as well as other functions that perform different operations on geometric objects.
 
 ##### JSON functions:
 
-- **to_json(self) -> json**: Convert the geometric object to .JSON format
-- **from\_json(json\_data) -> object**: Create a geometric object from JSON data
-- **save_shapes(shapes, filename)**: Save json_data (shapes) to file (filename)
-- **load_shapes(filename):** Load json_data from a file (filename)
+- **to\_json(object\_list):** Convert the list of objects to JSON string using object attributes
+- **save\_shapes(json\_data, filename):** Write JSON string to a .json file
+- **load\_shapes(filename):** Create JSON string from a .json file
+- **from\_json(json\_data):** Create a list of objects from a JSON string
 
 ##### Other functions:
 
 - **random_shape(shape)**: Create a geometric object of random dimensions. If the shape parameter is not specified, an arbitrary geometric object will be returned. Otherwise, insert one of the following as an argument: "Rectangle", "Triangle", "Circle", "Ellipse", "Polygon".
 - **rotate(P1, P2, f)**: Rotate point P1 (x1,y1) around point P2 (x2,y2) for angle f in radians.        
 - **intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
 - **parallel(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) are parallel
 - **Line_Intersect_Circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
 
-**Note: Tangency is also considered an intersection!**
+**Note: Tangency also counts as intersection!**
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SimpleShape-1.3/setup.py` & `SimpleShape-1.3.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
  
     setup(
         
     name="SimpleShape",
-    version="1.3",
+    version="1.3.1",
     author="Tilen Žel",
     author_email="tilen.zel@gmail.com",
  
     #Small Description about module
-    description="""A simple package for creating geometric objects and 
-    performing different operations on them""",
+    description="""A simple package for creating geometric objects""",
  
     # Specifying that we are using markdown file for description
     long_description=long_description,
     long_description_content_type="text/markdown",
  
     # Any link to reach this module, ***if*** you have any webpage or github profile
     # url="https://github.com/username/",
-    packages=find_packages(),
+    packages=['SimpleShape'],
  
  
     license="MIT",
  
     # classifiers like program is suitable for python3, just leave as it is.
     classifiers=[
         "Programming Language :: Python :: 3",
```

