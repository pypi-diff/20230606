# Comparing `tmp/pyiges-0.2.1.tar.gz` & `tmp/pyiges-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiges-0.2.1.tar", last modified: Wed Jan  5 15:39:59 2022, max compression
+gzip compressed data, was "pyiges-0.3.0.tar", last modified: Tue Jun  6 18:46:03 2023, max compression
```

## Comparing `pyiges-0.2.1.tar` & `pyiges-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 15:39:59.000000 pyiges-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-05 15:39:59.000000 pyiges-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 15:39:59.000000 pyiges-0.2.1/pyiges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-05 15:39:59.000000 pyiges-0.2.1/pyiges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-05 15:39:59.000000 pyiges-0.2.1/pyiges.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-01-05 15:39:59.000000 pyiges-0.2.1/pyiges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-05 15:39:59.000000 pyiges-0.2.1/pyiges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-01-05 15:39:59.000000 pyiges-0.2.1/pyiges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-01-05 15:39:31.000000 pyiges-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-01-05 15:39:59.000000 pyiges-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-01-05 15:39:31.000000 pyiges-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 15:39:59.000000 pyiges-0.2.1/pyiges/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-05 15:39:31.000000 pyiges-0.2.1/pyiges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-01-05 15:39:31.000000 pyiges-0.2.1/pyiges/faces.py
--rw-r--r--   0 runner    (1001) docker     (121)    14975 2022-01-05 15:39:31.000000 pyiges-0.2.1/pyiges/iges.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-01-05 15:39:31.000000 pyiges-0.2.1/pyiges/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      411 2022-01-05 15:39:31.000000 pyiges-0.2.1/pyiges/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-01-05 15:39:31.000000 pyiges-0.2.1/pyiges/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)    27403 2022-01-05 15:39:31.000000 pyiges-0.2.1/pyiges/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 15:39:59.000000 pyiges-0.2.1/pyiges/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     5103 2022-01-05 15:39:31.000000 pyiges-0.2.1/pyiges/examples/sample.igs
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-01-05 15:39:31.000000 pyiges-0.2.1/pyiges/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  4033498 2022-01-05 15:39:31.000000 pyiges-0.2.1/pyiges/examples/impeller.igs
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-01-05 15:39:31.000000 pyiges-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-01-05 15:39:31.000000 pyiges-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:46:03.944400 pyiges-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-06-06 18:45:22.000000 pyiges-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-06 18:45:22.000000 pyiges-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-06 18:45:22.000000 pyiges-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-06 18:46:03.944400 pyiges-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-06 18:45:22.000000 pyiges-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:46:03.940400 pyiges-0.3.0/pyiges/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/check_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:46:03.944400 pyiges-0.3.0/pyiges/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4033498 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/examples/impeller.igs
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/examples/sample.igs
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/faces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/iges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:46:03.940400 pyiges-0.3.0/pyiges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-06 18:46:03.000000 pyiges-0.3.0/pyiges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-06 18:46:03.000000 pyiges-0.3.0/pyiges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:46:03.000000 pyiges-0.3.0/pyiges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 18:46:03.000000 pyiges-0.3.0/pyiges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 18:46:03.000000 pyiges-0.3.0/pyiges.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 18:46:03.944400 pyiges-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-06 18:45:22.000000 pyiges-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:46:03.944400 pyiges-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    22031 2023-06-06 18:45:22.000000 pyiges-0.3.0/tests/test_pyiges.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiges-0.2.1/LICENSE` & `pyiges-0.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License
 
-Copyright (c) 2017-2019 The PyVista Developers
+Copyright (c) 2017-2023 The PyVista Developers
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyiges-0.2.1/setup.py` & `pyiges-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 """Setup for pyiges"""
-from setuptools import setup
-import os
 from io import open as io_open
+import os
+
+from setuptools import setup
 
 # Get version
 __version__ = None
 filepath = os.path.dirname(__file__)
-version_file = os.path.join(filepath, 'pyiges', '_version.py')
-with io_open(version_file, mode='r') as fd:
+version_file = os.path.join(filepath, "pyiges", "_version.py")
+with io_open(version_file, mode="r") as fd:
     exec(fd.read())
 
-readme_file = os.path.join(filepath, 'README.rst')
+readme_file = os.path.join(filepath, "README.rst")
 
 setup(
-    name='pyiges',
-    packages=['pyiges', 'pyiges.examples'],
+    name="pyiges",
+    packages=["pyiges", "pyiges.examples"],
     version=__version__,
-    author='PyVista Developers',
-    author_email='info@pyvista.org',
+    author="PyVista Developers",
+    author_email="info@pyvista.org",
     long_description=io_open(readme_file, encoding="utf-8").read(),
-    license='MIT',
+    long_description_content_type="text/x-rst",
+    license="MIT",
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Science/Research',
-        'Topic :: Scientific/Engineering :: Information Analysis',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: Microsoft :: Windows',
-        'Operating System :: POSIX',
-        'Operating System :: MacOS',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Science/Research",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: POSIX",
+        "Operating System :: MacOS",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    description='Pythonic IGES reader',
-    url='https://github.com/pyvista/pyiges',
-    install_requires=['tqdm', 'geomdl', 'pyvista>=0.28.0'],
-    package_data={'pyiges.examples': ['impeller.igs', 'sample.igs']}
+    description="Pythonic IGES reader",
+    url="https://github.com/pyvista/pyiges",
+    install_requires=["tqdm", "numpy"],
+    extras_require={"full": ["geomdl", "pyvista>=0.28.0"]},
+    package_data={"pyiges.examples": ["impeller.igs", "sample.igs"]},
 )
```

### Comparing `pyiges-0.2.1/pyiges/iges.py` & `pyiges-0.3.0/pyiges/iges.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from tqdm import tqdm
-from pyiges.entity import Entity
+
 from pyiges import geometry
+from pyiges.check_imports import assert_full_module_variant, pyvista, vtkAppendPolyData
+from pyiges.entity import Entity
 
-try: 
-    import pyvista 
-    from pyvista._vtk import vtkAppendPolyData
-except ImportError:
-    pass 
 
-class Iges():
+class Iges:
     """pyiges.Iges object
 
     Parameters
     ----------
     filename : str
         Filename of an IGES file.
 
@@ -24,32 +21,40 @@
         pyiges.Iges object
         Description:
         Number of Entities: 4615
     """
 
     def __init__(self, filename):
         self._read(filename)
-        self._desc = ''
+        self._desc = ""
 
     def entities(self):
         """Return a list of all entities
 
         Examples
         --------
         >>> iges.entities
         [<pyiges.geometry.Point at 0x7f7056069c10>,
          <pyiges.geometry.Point at 0x7f7056069790>,
          <pyiges.geometry.Point at 0x7f7056069a50>,
          <pyiges.geometry.Point at 0x7f7056069b10>,
          <pyiges.entity.Entity at 0x7f7056069910>]
         """
 
-    def to_vtk(self, lines=True, bsplines=True,
-               surfaces=True, points=True, delta=0.025, merge=True,
-               progress=tqdm):
+    @assert_full_module_variant
+    def to_vtk(
+        self,
+        lines=True,
+        bsplines=True,
+        surfaces=True,
+        points=True,
+        delta=0.025,
+        merge=True,
+        progress=tqdm,
+    ):
         """Converts entities to a vtk object
 
         Parameters
         ----------
         lines : bool, optional
             Convert lines.
 
@@ -61,15 +66,15 @@
 
         delta : float, optional
             Resolution when converting spline entities.  Higher
             resolution creates a better plot at the cost of computing
             time.
 
         merge : bool, optional
-            Merge all converted entites into one output.
+            Merge all converted entities into one output.
 
         progress: function, optional
             Report conversion progress by use of this function. Example::
 
                 def silent_progress(iterable, *args, **kwargs):
                     return iterable
 
@@ -93,15 +98,15 @@
           N Points:	96218
           X Bounds:	-4.299e+01, 6.912e+14
           Y Bounds:	-4.255e+01, 6.290e+14
           Z Bounds:	-9.980e+02, 6.702e+14
           N Arrays:	0
         """
         items = pyvista.MultiBlock()
-        for entity in progress(self, desc='Converting entities to vtk'):
+        for entity in progress(self, desc="Converting entities to vtk"):
             if isinstance(entity, geometry.RationalBSplineCurve) and bsplines:
                 items.append(entity.to_vtk(delta))
             elif isinstance(entity, geometry.RationalBSplineSurface) and surfaces:
                 items.append(entity.to_vtk(delta))
             elif isinstance(entity, geometry.Line) and lines:
                 items.append(entity.to_vtk())
             elif isinstance(entity, geometry.Point) and points:
@@ -132,16 +137,15 @@
 
     def lines(self, as_vtk=False, merge=False, **kwargs):
         """All lines"""
         return self._return_type(geometry.Line, as_vtk, merge, **kwargs)
 
     def bsplines(self, as_vtk=False, merge=False, **kwargs):
         """All bsplines"""
-        return self._return_type(geometry.RationalBSplineCurve, as_vtk, merge,
-                                 **kwargs)
+        return self._return_type(geometry.RationalBSplineCurve, as_vtk, merge, **kwargs)
 
     def bspline_surfaces(self, as_vtk=False, merge=False, **kwargs):
         """All bsplines
 
         Examples
         --------
         Convert and plot all bspline surfaces.  This takes a while
@@ -171,34 +175,35 @@
             Knot 2: [0. 0. 0. 0. 1. 1. 1. 1.]
             u0: 1.000000
             u1: 0.000000
             v0: 1.000000
             v1: 128.000000
             Control Points: 16
         """
-        return self._return_type(geometry.RationalBSplineSurface, as_vtk, merge,
-                                 **kwargs)
+        return self._return_type(
+            geometry.RationalBSplineSurface, as_vtk, merge, **kwargs
+        )
 
     def circular_arcs(self, to_vtk=False, merge=False, **kwargs):
         """All circular_arcs"""
         return self._return_type(geometry.CircularArc, to_vtk, merge, **kwargs)
 
     def conic_arcs(self, as_vtk=False, merge=False, **kwargs):
-        return self._return_type(geometry.ConicArc, as_vtk, merge,**kwargs)
+        return self._return_type(geometry.ConicArc, as_vtk, merge, **kwargs)
 
     def faces(self, as_vtk=False, merge=False, **kwargs):
-        return self._return_type(geometry.Face, as_vtk, merge,**kwargs)
+        return self._return_type(geometry.Face, as_vtk, merge, **kwargs)
 
     def loops(self, as_vtk=False, merge=False, **kwargs):
-        return self._return_type(geometry.Loop, as_vtk, merge,**kwargs)
+        return self._return_type(geometry.Loop, as_vtk, merge, **kwargs)
 
     def _return_type(self, iges_type, to_vtk=False, merge=False, **kwargs):
         """Return an iges type"""
         items = []
-        for entity in (self):
+        for entity in self:
             if isinstance(entity, iges_type):
                 if to_vtk:
                     items.append(entity.to_vtk(**kwargs))
                 else:
                     items.append(entity)
 
         # merge to a single mesh
@@ -208,65 +213,86 @@
                 afilter.AddInputData(item)
             afilter.Update()
 
             return pyvista.wrap(afilter.GetOutput())
 
         return items
 
-    def __getitem__(self, indices):
-        return self._entities[indices]
-
     def __iter__(self):
-        for entity in self._entities:
-            yield entity
+        yield from self._entities
 
     def __len__(self):
         return len(self._entities)
 
     def __repr__(self):
-        info = 'pyiges.Iges object\n'
-        info += 'Description: %s\n' % self._desc
-        info += 'Number of Entities: %d' % len(self)
+        info = "pyiges.Iges object\n"
+        info += "Description: %s\n" % self._desc
+        info += "Number of Entities: %d" % len(self)
         return info
 
     def from_pointer(self, ptr):
         """Return an iges object according to an iges pointer"""
         return self[self._pointers[ptr]]
 
+    @staticmethod
+    def _parse_separators_from_first_global_line(line):
+        if line[0] == ",":
+            a = ","
+            if line[1] == a:
+                b = ";"
+            elif line[1:3] == "1H":
+                b = line[3]
+            else:
+                raise RuntimeError("Invalid Global section format")
+        elif line[0:2] == "1H":
+            a = line[2]
+            if line[4:6] == "1H":
+                b = line[6]
+            elif line[3] == a:
+                b = ";"
+            else:
+                raise RuntimeError("Invalid Global section format")
+        else:
+            raise RuntimeError("Invalid Global section format")
+        return a, b
+
     def _read(self, filename):
-        with open(filename, 'r') as f:
-            param_string = ''
+        with open(filename) as f:
+            param_string = ""
             entity_list = []
             entity_index = 0
             first_dict_line = True
             first_global_line = True
             first_param_line = True
             global_string = ""
             pointer_dict = {}
+            entities_to_discard = []
 
             # for line in tqdm(f.readlines(), desc='Reading file'):
-            for line in f.readlines():
+            for line_no, line in enumerate(f.readlines(), start=1):
                 data = line[:80]
                 id_code = line[72]
 
-                if id_code == 'S':     # Start
+                if id_code == "S":  # Start
                     desc = line[:72].strip()
 
-                elif id_code == 'G':   # Global
-                    global_string += data   # Consolidate all global lines
+                elif id_code == "G":  # Global
+                    global_string += data  # Consolidate all global lines
                     if first_global_line:
-                        param_sep = data[2]
-                        record_sep = data[6]
+                        (
+                            param_sep,
+                            record_sep,
+                        ) = self._parse_separators_from_first_global_line(data)
                         first_global_line = False
 
-                elif id_code == 'D':   # Directory entry
+                elif id_code == "D":  # Directory entry
                     if first_dict_line:
                         entity_type_number = int(data[0:8].strip())
                         # Curve and surface entities.  See IGES spec v5.3, p. 38, Table 3
-                        if entity_type_number == 100:   # Circular arc
+                        if entity_type_number == 100:  # Circular arc
                             e = geometry.CircularArc(self)
                         elif entity_type_number == 102:  # Composite curve
                             e = Entity(self)
                         elif entity_type_number == 104:  # Conic arc
                             e = geometry.ConicArc(self)
                         elif entity_type_number == 108:  # Plane
                             e = Entity(self)
@@ -292,78 +318,94 @@
                             e = geometry.RationalBSplineSurface(self)
 
                         # CSG Entities. See IGES spec v5.3, p. 42, Section 3.3
                         elif entity_type_number == 150:  # Block
                             e = Entity(self)
 
                         # B-Rep entities.  See IGES spec v5.3, p. 43, Section 3.4
-                        elif  entity_type_number == 186:
+                        elif entity_type_number == 186:
                             e = Entity(self)
 
                         # Annotation entities.  See IGES spec v5.3, p. 46, Section 3.5
-                        elif  entity_type_number == 202:
+                        elif entity_type_number == 202:
                             e = Entity(self)
 
                         # Structural entities.  See IGES spec v5.3, p. 50, Section 3.6
-                        elif  entity_type_number == 132:
+                        elif entity_type_number == 132:
                             e = Entity(self)
-                        elif  entity_type_number == 502:
+                        elif entity_type_number == 502:
                             e = geometry.VertexList(self)
-                        elif  entity_type_number == 504:
+                        elif entity_type_number == 504:
                             e = geometry.EdgeList(self)
-                        elif  entity_type_number == 508:
+                        elif entity_type_number == 508:
                             e = geometry.Loop(self)
-                        elif  entity_type_number == 510:
+                        elif entity_type_number == 510:
                             e = geometry.Face(self)
                         else:
                             e = Entity(self)
 
-                        e.add_section(data[0:8], 'entity_type_number')
-                        e.add_section(data[8:16], 'parameter_pointer')
-                        e.add_section(data[16:24], 'structure')
-                        e.add_section(data[24:32], 'line_font_pattern')
-                        e.add_section(data[32:40], 'level')
-                        e.add_section(data[40:48], 'view')
-                        e.add_section(data[48:56], 'transform')
-                        e.add_section(data[56:65], 'label_assoc')
-                        e.add_section(data[65:72], 'status_number')
+                        e.add_section(data[0:8], "entity_type_number")
+                        e.add_section(data[8:16], "parameter_pointer")
+                        e.add_section(data[16:24], "structure")
+                        e.add_section(data[24:32], "line_font_pattern")
+                        e.add_section(data[32:40], "level")
+                        e.add_section(data[40:48], "view")
+                        e.add_section(data[48:56], "transform")
+                        e.add_section(data[56:65], "label_assoc")
+                        e.add_section(data[65:72], "status_number")
                         e.sequence_number = int(data[73:].strip())
 
                         first_dict_line = False
                     else:
-                        e.add_section(data[8:16], 'line_weight_number')
-                        e.add_section(data[16:24], 'color_number')
-                        e.add_section(data[24:32], 'param_line_count')
-                        e.add_section(data[32:40], 'form_number')
-                        e.add_section(data[56:64], 'entity_label', type='string')
-                        e.add_section(data[64:72], 'entity_subs_num')
+                        e.add_section(data[8:16], "line_weight_number")
+                        e.add_section(data[16:24], "color_number")
+                        e.add_section(data[24:32], "param_line_count")
+                        e.add_section(data[32:40], "form_number")
+                        e.add_section(data[56:64], "entity_label", type="string")
+                        e.add_section(data[64:72], "entity_subs_num")
 
                         first_dict_line = True
                         entity_list.append(e)
-                        pointer_dict.update({e.sequence_number : entity_index})
+                        pointer_dict.update({e.sequence_number: entity_index})
                         entity_index += 1
 
-                elif id_code == 'P':   # Parameter data
+                elif id_code == "P":  # Parameter data
                     # Concatenate multiple lines into one string
                     if first_param_line:
                         param_string = data[:64]
                         directory_pointer = int(data[64:72].strip())
                         first_param_line = False
                     else:
                         param_string += data[:64]
 
                     if param_string.strip()[-1] == record_sep:
                         first_param_line = True
                         param_string = param_string.strip()[:-1]
                         parameters = param_string.split(param_sep)
-                        entity_list[pointer_dict[directory_pointer]]._add_parameters(parameters)
+                        this_entity = entity_list[pointer_dict[directory_pointer]]
+                        try:
+                            this_entity._add_parameters(parameters)
+                        except Exception as err:
+                            print(
+                                "Warning: Could not initialize entity from parameters with Parameter section "
+                                "ending on line {}. Possibly wrong or (yet) unsupported format. Entity will be discarded.".format(
+                                    line_no
+                                )
+                            )
+                            entities_to_discard.append(this_entity)
 
-                elif id_code == 'T':   # Terminate
+                elif id_code == "T":  # Terminate
                     pass
 
+        for e in entities_to_discard:
+            try:
+                entity_list.remove(e)
+            except:
+                pass
+
         self._entities = entity_list
         self.desc = desc
         self._pointers = pointer_dict
 
     def __getitem__(self, index):
         """Get an item by its pointer"""
         return self._entities[self._pointers[index]]
```

### Comparing `pyiges-0.2.1/pyiges/entity.py` & `pyiges-0.3.0/pyiges/entity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+"""Module for the entity class."""
 import os
+
 from pyiges.constants import line_font_pattern
 
 
-class Entity():
+class Entity:
     """Generic IGES entity
 
     Examples
     --------
     >>> import pyiges
     >>> from pyiges import examples
     >>> iges = pyiges.read(examples.impeller)
@@ -32,50 +34,53 @@
     """
 
     def __init__(self, iges):
         self.d = dict()
         self.parameters = []
         self.iges = iges
 
-    def add_section(self, string, key, type='int'):
+    def add_section(self, string, key, type="int"):
         string = string.strip()
-        if type == 'string':
+        if type == "string":
             self.d[key] = string
         else:
             # Status numbers are made of four 2-digit numbers, together making an 8-digit number.
             # It includes spaces, so  0 0 0 0 is a valid 8-digit for which int casting won't work.
             if key == "status_number":
                 # Get a list of four 2-digit numbers with spaces removed.
-                separated_status_numbers = [string[i:i+2].replace(' ', '0') for i in range(0, len(string), 2)]
-                
+                separated_status_numbers = [
+                    string[i : i + 2].replace(" ", "0")
+                    for i in range(0, len(string), 2)
+                ]
+
                 # Join these status numbers together as a single string.
-                status_number_string = ''.join(separated_status_numbers)
+                status_number_string = "".join(separated_status_numbers)
 
                 # The string can now be properly cast as an int
                 self.d[key] = int(status_number_string)
             elif len(string) > 0:
                 self.d[key] = int(string)
             else:
                 self.d[key] = None
 
     def __str__(self):
         s = "----- Entity -----" + os.linesep
-        s += str(self.d['entity_type_number']) + os.linesep
-        s += str(self.d['parameter_pointer']) + os.linesep
-        s += str(self.d['structure']) + os.linesep
-        s += line_font_pattern[self.d['line_font_pattern']] + os.linesep
-        s += str(self.d['level']) + os.linesep
-        s += str(self.d['view']) + os.linesep
-        s += str(self.d['transform']) + os.linesep
-        s += str(self.d['label_assoc']) + os.linesep
-        s += str(self.d['status_number']) + os.linesep
-        s += str(self.d['line_weight_number']) + os.linesep
-        s += str(self.d['color_number']) + os.linesep
-        s += str(self.d['param_line_count']) + os.linesep
-        s += str(self.d['form_number']) + os.linesep
-        s += str(self.d['entity_label']) + os.linesep
-        s += str(self.d['entity_subs_num'])
+        s += str(self.d["entity_type_number"]) + os.linesep
+        s += str(self.d["parameter_pointer"]) + os.linesep
+        s += str(self.d["structure"]) + os.linesep
+        s += line_font_pattern[self.d["line_font_pattern"]] + os.linesep
+        s += str(self.d["level"]) + os.linesep
+        s += str(self.d["view"]) + os.linesep
+        s += str(self.d["transform"]) + os.linesep
+        s += str(self.d["label_assoc"]) + os.linesep
+        s += str(self.d["status_number"]) + os.linesep
+        s += str(self.d["line_weight_number"]) + os.linesep
+        s += str(self.d["color_number"]) + os.linesep
+        s += str(self.d["param_line_count"]) + os.linesep
+        s += str(self.d["form_number"]) + os.linesep
+        s += str(self.d["entity_label"]) + os.linesep
+        s += str(self.d["entity_subs_num"])
 
         return s
 
     def _add_parameters(self, parameters):
         self.parameters.append(parameters)
```

### Comparing `pyiges-0.2.1/pyiges/geometry.py` & `pyiges-0.3.0/pyiges/geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import os
 
-from geomdl import NURBS, BSpline
 import numpy as np
-import pyvista as pv
 
+from pyiges.check_imports import assert_full_module_variant, pyvista as pv
 from pyiges.entity import Entity
 
 
 def parse_float(str_value):
     """
-    This fuction converts a string to float just like the built-in
+    This function converts a string to float just like the built-in
     float() function. In addition to "normal" numbers it also handles
-    numbers such as 1.2D3 (equivalent to 1.2E3)
+    numbers such as 1.2D3 (equivalent to 1.2E3).
     """
     try:
         return float(str_value)
     except ValueError:
         return float(str_value.lower().replace("d", "e"))
 
 
-
 class Point(Entity):
     """IGES Point"""
 
     def _add_parameters(self, parameters):
         self._x = parse_float(parameters[1])
         self._y = parse_float(parameters[2])
         self._z = parse_float(parameters[3])
@@ -45,21 +43,22 @@
 
     @property
     def coordinate(self):
         """Coordinate of the point as a numpy array"""
         return np.array([self._x, self._y, self._z])
 
     def __repr__(self):
-        s = '--- IGES Point ---' + os.linesep
-        s += "{0}, {1}, {2} {3}".format(self._x, self._y, self._z, os.linesep)
+        s = "--- IGES Point ---" + os.linesep
+        s += f"{self._x}, {self._y}, {self._z} {os.linesep}"
         return s
 
     def __str__(self):
         return self.__repr__()
 
+    @assert_full_module_variant
     def to_vtk(self):
         """Point represented as a ``pyvista.PolyData`` Mesh
 
         Returns
         -------
         mesh : ``pyvista.PolyData``
             ``pyvista`` mesh
@@ -77,34 +76,37 @@
         self._x2 = parse_float(parameters[4])
         self._y2 = parse_float(parameters[5])
         self._z2 = parse_float(parameters[6])
 
     @property
     def coordinates(self):
         """Starting and ending point of the line as a ``numpy`` array"""
-        return np.array([[self._x1, self._y1, self._z1],
-                         [self._x2, self._y2, self._z2]])
+        return np.array(
+            [[self._x1, self._y1, self._z1], [self._x2, self._y2, self._z2]]
+        )
 
     def __repr__(self):
-        s = '--- IGES Line ---' + os.linesep
+        s = "--- IGES Line ---" + os.linesep
         s += Entity.__str__(self) + os.linesep
-        s += "From point {0}, {1}, {2} {3}".format(self._x1, self._y1, self._z1, os.linesep)
-        s += "To point {0}, {1}, {2}".format(self._x2, self._y2, self._z2)
+        s += f"From point {self._x1}, {self._y1}, {self._z1} {os.linesep}"
+        s += f"To point {self._x2}, {self._y2}, {self._z2}"
         return s
 
+    @assert_full_module_variant
     def to_vtk(self, resolution=1):
         """Line represented as a ``pyvista.PolyData`` Mesh
 
         Returns
         -------
         mesh : ``pyvista.PolyData``
             ``pyvista`` mesh
         """
-        return pv.Line([self._x1, self._y1, self._z1],
-                       [self._x2, self._y2, self._z2], resolution)
+        return pv.Line(
+            [self._x1, self._y1, self._z1], [self._x2, self._y2, self._z2], resolution
+        )
 
 
 class Transformation(Entity):
     """Transforms entities by matrix multiplication and vector
     addition to give a translation, as shown below:
 
     Notes
@@ -139,57 +141,63 @@
         self.t2 = parse_float(parameters[8])
         self.r31 = parse_float(parameters[9])
         self.r32 = parse_float(parameters[10])
         self.r33 = parse_float(parameters[11])
         self.t3 = parse_float(parameters[12])
 
     def __repr__(self):
-        txt = 'IGES 124 Transformation Matrix\n'
+        txt = "IGES 124 Transformation Matrix\n"
         txt += str(self.to_affine())
         return txt
 
     def to_affine(self):
         """Return a 4x4 affline transformation matrix"""
-        return np.array([[self.r11, self.r12, self.r13, self.t1],
-                         [self.r21, self.r22, self.r23, self.t2],
-                         [self.r31, self.r32, self.r33, self.t3],
-                         [0, 0, 0, 1]])
+        return np.array(
+            [
+                [self.r11, self.r12, self.r13, self.t1],
+                [self.r21, self.r22, self.r23, self.t2],
+                [self.r31, self.r32, self.r33, self.t3],
+                [0, 0, 0, 1],
+            ]
+        )
 
+    @assert_full_module_variant
     def _to_vtk(self):
         """Convert to a vtk transformation matrix"""
         vtkmatrix = pv.vtkmatrix_from_array(self.to_affine())
         import vtk
+
         trans = vtk.vtkTransform()
         trans.SetMatrix(vtkmatrix)
         return trans
 
 
 class ConicArc(Entity):
     """Conic Arc (Type 104)
     Arc defined by the equation:
     ``A*x**2 + B*x*y + C*y**2 + D*x + E*y + F = 0``
 
     with a Transformation Matrix (Entity 124). Can define
     an ellipse, parabola, or hyperbola.
 
     """
+
     # The definitions of the terms ellipse, parabola, and hyperbola
     # are given in terms of the quantities Q1, Q2, and Q3. These
     # quantities are:
 
     #     |  A   B/2  D/2 |        |  A   B/2 |
     # Q1= | B/2   C   E/2 |   Q2 = | B/2   C  |   Q3 = A + C
     #     | D/2  E/2   F  |
     # A parent conic curve is:
 
     # An ellipse if Q2 > 0 and Q1, Q3 < 0.
     # A hyperbola if Q2 < 0 and Q1 != 0.
     # A parabola if Q2 = 0 and Q1 != 0.
 
-
     def _add_parameters(self, parameters):
         """
         Index	Type	Name	Description
         1	REAL	A	coefficient of xt^2
         2	REAL	B	coefficient of xtyt
         3	REAL	C	coefficient of yt^2
         4	REAL	D	coefficient of xt
@@ -212,27 +220,27 @@
         self.y1 = parameters[8]  #  y coordinate of start point
         self.z1 = parameters[9]  #  z coordinate of start point
         self.x2 = parameters[10]  #  x coordinate of end point
         self.y2 = parameters[11]  #  y coordinate of end point
         self.z2 = parameters[12]  #  z coordinate of end point
 
     def __repr__(self):
-        info = 'Conic Arc\nIGES Type 104\n'
-        info += 'Start:  (%f, %f, %f)\n' % (self.x1, self.y1, self.z1)
-        info += 'End:    (%f, %f, %f)\n' % (self.x2, self.y2, self.z2)
-        info += 'Coefficient of x**2: %f' % self.a
-        info += 'Coefficient of x*y:  %f' % self.b
-        info += 'Coefficient of y**2: %f' % self.c
-        info += 'Coefficient of x:    %f' % self.d
-        info += 'Coefficient of y:    %f' % self.e
-        info += 'Scalar coefficient:  %f' % self.f
+        info = "Conic Arc\nIGES Type 104\n"
+        info += f"Start:  ({self.x1:f}, {self.y1:f}, {self.z1:f})\n"
+        info += f"End:    ({self.x2:f}, {self.y2:f}, {self.z2:f})\n"
+        info += "Coefficient of x**2: %f" % self.a
+        info += "Coefficient of x*y:  %f" % self.b
+        info += "Coefficient of y**2: %f" % self.c
+        info += "Coefficient of x:    %f" % self.d
+        info += "Coefficient of y:    %f" % self.e
+        info += "Scalar coefficient:  %f" % self.f
         return info
 
+    @assert_full_module_variant
     def to_vtk(self):
-
         # a*x**2 + b*x*y + c*y**2 + d*x + e*y + f = 0
         # from sympy import Symbol
         # from sympy.solvers import Solve
         # a = Symbol('a')
         # b = Symbol('b')
         # c = Symbol('c')
         # d = Symbol('d')
@@ -241,15 +249,15 @@
         # x = Symbol('x')
         # y = Symbol('y')
         # solve(a*x**2 + b*x*y + c*y**2 + d*x + e*y + f, x)
 
         # x0 = (-b*y - d + sqrt(-4*a*c*y**2 - 4*a*e*y - 4*a*f + b**2*y**2 + 2*b*d*y + d**2))/(2*a)
         # x1 = -(b*y + d + sqrt(-4*a*c*y**2 - 4*a*e*y - 4*a*f + b**2*y**2 + 2*b*d*y + d**2))/(2*a)
 
-        raise NotImplementedError('Not yet implemented')
+        raise NotImplementedError("Not yet implemented")
 
 
 class RationalBSplineCurve(Entity):
     """Rational B-Spline Curve
     IGES Spec v5.3 p. 123 Section 4.23
     See also Appendix B, p. 545
     """
@@ -273,16 +281,20 @@
         # Weights
         self.W = []
         for i in range(self.A + 8, self.A + self.K + 8):
             self.W.append(parse_float(parameters[i]))
 
         # Control points
         self.control_points = []
-        for i in range(9 + self.A + self.K, 9 + self.A + 4*self.K + 1, 3):
-            point = (parse_float(parameters[i]), parse_float(parameters[i+1]), parse_float(parameters[i+2]))
+        for i in range(9 + self.A + self.K, 9 + self.A + 4 * self.K + 1, 3):
+            point = (
+                parse_float(parameters[i]),
+                parse_float(parameters[i + 1]),
+                parse_float(parameters[i + 2]),
+            )
             self.control_points.append(point)
 
         # Parameter values
         self.V0 = parse_float(parameters[12 + self.A + 4 * self.K])
         self.V1 = parse_float(parameters[13 + self.A + 4 * self.K])
 
         # Unit normal (only for planar curves)
@@ -291,35 +303,38 @@
             self.XNORM = parse_float(parameters[14 + self.A + 4 * self.K])
             self.YNORM = parse_float(parameters[15 + self.A + 4 * self.K])
             self.ZNORM = parse_float(parameters[16 + self.A + 4 * self.K])
         else:
             self.planar_curve = False
 
     def __str__(self):
-        s = '--- Rational B-Spline Curve ---' + os.linesep
+        s = "--- Rational B-Spline Curve ---" + os.linesep
         s += Entity.__str__(self) + os.linesep
         s += str(self.T) + os.linesep
         s += str(self.W) + os.linesep
         s += str(self.control_points) + os.linesep
-        s += "Parameter: v(0) = {0}    v(1) = {1}".format(self.V0, self.V1) + os.linesep
+        s += f"Parameter: v(0) = {self.V0}    v(1) = {self.V1}" + os.linesep
         if self.planar_curve:
-            s += "Unit normal: {0} {1} {2}".format(self.XNORM, self.YNORM, self.ZNORM)
+            s += f"Unit normal: {self.XNORM} {self.YNORM} {self.ZNORM}"
         return s
 
+    @assert_full_module_variant
     def to_geomdl(self):
+        from geomdl import NURBS
+
         curve = NURBS.Curve()
         curve.degree = self.M
         curve.ctrlpts = self.control_points
         curve.weights = self.W + [1]
         curve.knotvector = self.T  # Set knot vector
         return curve
 
+    @assert_full_module_variant
     def to_vtk(self, delta=0.01):
-        """Set evaluation delta (controls the number of curve points)
-        """
+        """Set evaluation delta (controls the number of curve points)"""
         # Create a 3-dimensional B-spline Curve
         curve = self.to_geomdl()
         curve.delta = delta
 
         # spline segfaults here sometimes...
         # return pv.Spline(np.array(curve.evalpts))
 
@@ -379,25 +394,25 @@
            [-28.89230518,  -9.2355426 , -21.16779478],
            [-29.05313537,  -9.28695263, -33.51982653],
            [-30.54742519,  -9.76460843, -45.77299513]])
     """
 
     @property
     def k1(self):
-        """ Upper index of first sum"""
+        """Upper index of first sum"""
         return self._k1
 
     @property
     def k2(self):
-        """ Upper index of second sum"""
+        """Upper index of second sum"""
         return self._k2
 
     @property
     def m1(self):
-        """ Degree of first basis functions"""
+        """Degree of first basis functions"""
         return self._m1
 
     @property
     def m2(self):
         """Degree of second basis functions"""
         return self._m2
 
@@ -466,89 +481,108 @@
 
     @property
     def v1(self):
         """End second parameter value"""
         return self._v1
 
     def _add_parameters(self, input_parameters):
-        parameters = np.array([parse_float(param) for param in input_parameters], dtype=float)
+        parameters = np.array(
+            [parse_float(param) for param in input_parameters], dtype=float
+        )
 
         self._k1 = int(parameters[1])  # Upper index of first sum
         self._k2 = int(parameters[2])  # Upper index of second sum
         self._m1 = int(parameters[3])  # Degree of first basis functions
         self._m2 = int(parameters[4])  # Degree of second basis functions
         self._flag1 = bool(parameters[5])  # 0=closed in first direction, 1=not closed
         self._flag2 = bool(parameters[6])  # 0=closed in second direction, 1=not closed
         self._flag3 = bool(parameters[7])  # 0=rational, 1=polynomial
-        self._flag4 = bool(parameters[8])  # 0=nonperiodic in first direction , 1=periodic
-        self._flag5 = bool(parameters[9])  # 0=nonperiodic in second direction , 1=periodic
+        self._flag4 = bool(
+            parameters[8]
+        )  # 0=nonperiodic in first direction , 1=periodic
+        self._flag5 = bool(
+            parameters[9]
+        )  # 0=nonperiodic in second direction , 1=periodic
 
         # load knot sequences
-        self._knot1 = parameters[10:12 + self._k1 + self._m1]
-        self._knot2 = parameters[12 + self._k1 + self._m1: 14 + self._k2 + self._m1 + self._k1 + self._m2]
+        self._knot1 = parameters[10 : 12 + self._k1 + self._m1]
+        self._knot2 = parameters[
+            12 + self._k1 + self._m1 : 14 + self._k2 + self._m1 + self._k1 + self._m2
+        ]
 
         # weights
         st = 14 + self._k2 + self._m1 + self._k1 + self._m2
-        en = st + (1 + self._k2)*(1 + self._k1)
+        en = st + (1 + self._k2) * (1 + self._k1)
         self._weights = parameters[st:en]
 
         # control points
-        st = 14 + self._k2 + self._k1 + self._m1 + self._m2 + (1 + self._k2)*(1 + self._k1)
-        en = st + 3*(1 + self._k2)*(1 + self._k1)
+        st = (
+            14
+            + self._k2
+            + self._k1
+            + self._m1
+            + self._m2
+            + (1 + self._k2) * (1 + self._k1)
+        )
+        en = st + 3 * (1 + self._k2) * (1 + self._k1)
         self._cp = parameters[st:en].reshape(-1, 3)
 
         self._u0 = parameters[-3]  # Start first parameter value
         self._u1 = parameters[-2]  # End first parameter value
         self._v0 = parameters[-1]  # Start second parameter value
         self._v1 = parameters[-0]  # End second parameter value
 
     def __repr__(self):
-        info = 'Rational B-Spline Surface\n'
-        info += '    Upper index of first sum:          %d\n' % self._k1
-        info += '    Upper index of second sum:         %d\n' % self._k2
-        info += '    Degree of first basis functions:   %d\n' % self._m1
-        info += '    Degree of second basis functions:  %d\n' % self._m2
+        info = "Rational B-Spline Surface\n"
+        info += "    Upper index of first sum:          %d\n" % self._k1
+        info += "    Upper index of second sum:         %d\n" % self._k2
+        info += "    Degree of first basis functions:   %d\n" % self._m1
+        info += "    Degree of second basis functions:  %d\n" % self._m2
 
         if self.flag1:
-            info += '    Closed in the first direction\n'
+            info += "    Closed in the first direction\n"
         else:
-            info += '    Open in the first direction\n'
+            info += "    Open in the first direction\n"
 
         if self.flag2:
-            info += '    Closed in the second direction\n'
+            info += "    Closed in the second direction\n"
         else:
-            info += '    Open in the second direction\n'
+            info += "    Open in the second direction\n"
 
         if self.flag3:
-            info += '    Rational\n'
+            info += "    Rational\n"
         else:
-            info += '    Polynomial\n'
+            info += "    Polynomial\n"
 
         if self.flag4:
-            info += '    Nonperiodic in first direction\n'
+            info += "    Nonperiodic in first direction\n"
         else:
-            info += '    Periodic in the first direction\n'
+            info += "    Periodic in the first direction\n"
 
         if self.flag5:
-            info += '    Nonperiodic in second direction\n'
+            info += "    Nonperiodic in second direction\n"
         else:
-            info += '    Periodic in the second direction\n'
+            info += "    Periodic in the second direction\n"
 
-        info += '    Knot 1: %s\n' % str(self.knot1)
-        info += '    Knot 2: %s\n' % str(self.knot2)
+        info += "    Knot 1: %s\n" % str(self.knot1)
+        info += "    Knot 2: %s\n" % str(self.knot2)
 
-        info += '    u0: %f\n' % self.u0
-        info += '    u1: %f\n' % self.u1
-        info += '    v0: %f\n' % self.v0
-        info += '    v1: %f\n' % self.v1
+        info += "    u0: %f\n" % self.u0
+        info += "    u1: %f\n" % self.u1
+        info += "    v0: %f\n" % self.v0
+        info += "    v1: %f\n" % self.v1
 
-        info += '    Control Points: %d' % len(self._cp)
+        info += "    Control Points: %d" % len(self._cp)
+        return info
 
+    @assert_full_module_variant
     def to_geomdl(self):
         """Return a ``geommdl.BSpline.Surface``"""
+        from geomdl import BSpline
+
         surf = BSpline.Surface()
 
         # Set degrees
         surf.degree_u = self._m2
         surf.degree_v = self._m1
 
         # set control points and knots
@@ -557,14 +591,15 @@
         surf.knotvector_u = self._knot2
         surf.knotvector_v = self._knot1
 
         # set weights
         surf.weights = self._weights
         return surf
 
+    @assert_full_module_variant
     def to_vtk(self, delta=0.025):
         """Return a pyvista.PolyData Mesh
 
         Parameters
         ----------
         delta : float, optional
             Resolution of the surface.  Higher number result in a
@@ -614,48 +649,48 @@
         self.z = parse_float(parameters[1])
         self.x = parse_float(parameters[2])
         self.y = parse_float(parameters[3])
         self.x1 = parse_float(parameters[4])
         self.y1 = parse_float(parameters[5])
         self.x2 = parse_float(parameters[6])
         self.y2 = parse_float(parameters[7])
-        self._transform = self.d.get('transform', None)
+        self._transform = self.d.get("transform", None)
 
+    @assert_full_module_variant
     def to_vtk(self, resolution=20):
         """Circular arc represented as a ``pyvista.PolyData`` Mesh
 
         Returns
         -------
         mesh : ``pyvista.PolyData``
             ``pyvista`` mesh
         """
         start = [self.x1, self.y1, 0]
         end = [self.x2, self.y2, 0]
         center = [self.x, self.y, 0]
-        arc = pv.CircularArc(center=center,
-                             pointa=start,
-                             pointb=end,
-                             resolution=resolution)
+        arc = pv.CircularArc(
+            center=center, pointa=start, pointb=end, resolution=resolution
+        )
         arc.points += [0, 0, self.z]
         if self.transform is not None:
             arc.transform(self.transform._to_vtk())
 
         return arc
 
     @property
     def transform(self):
         if self._transform is not None:
             return self.iges[self._transform]
 
     def __repr__(self):
-        info = 'Circular Arc\nIGES Type 100\n'
-        info += 'Center: (%f, %f)\n' % (self.x, self.y)
-        info += 'Start:  (%f, %f)\n' % (self.x1, self.y1)
-        info += 'End:    (%f, %f)\n' % (self.x2, self.y2)
-        info += 'Z Disp: %f' % self.z
+        info = "Circular Arc\nIGES Type 100\n"
+        info += f"Center: ({self.x:f}, {self.y:f})\n"
+        info += f"Start:  ({self.x1:f}, {self.y1:f})\n"
+        info += f"End:    ({self.x2:f}, {self.y2:f})\n"
+        info += "Z Disp: %f" % self.z
         return info
 
 
 class Face(Entity):
     """Defines a bound portion of three dimensional space (R^3) which
     has a finite area. Used to construct B-Rep Geometries."""
 
@@ -684,15 +719,15 @@
         loops = []
         for ptr in self.loop_pointers:
             loops.append(self.iges.from_pointer(ptr))
 
         return loops
 
     def __repr__(self):
-        info = 'IGES Type 510: Face\n'
+        info = "IGES Type 510: Face\n"
         # info += 'Center: (%f, %f)\n' % (self.x, self.y)
         # info += 'Start:  (%f, %f)\n' % (self.x1, self.y1)
         # info += 'End:    (%f, %f)\n' % (self.x2, self.y2)
         # info += 'Z Disp: %f' % self.z
         return info
 
 
@@ -721,45 +756,50 @@
         """
         self.parameters = parameters
         self.n_edges = int(self.parameters[1])
         self._edges = []
 
         c = 0
         for i in range(self.n_edges):
-            edge = {'type': int(self.parameters[2 + c]),
-                    'e1': int(self.parameters[3 + c]),  # first vertex or edge list
-                    'index1': int(self.parameters[4 + c]),  # index of edge in e1
-                    'flag1': bool(self.parameters[5 + c]),  # orientation flag
-                    'k1': int(self.parameters[6 + c])}  # n curves
+            edge = {
+                "type": int(self.parameters[2 + c]),
+                "e1": int(self.parameters[3 + c]),  # first vertex or edge list
+                "index1": int(self.parameters[4 + c]),  # index of edge in e1
+                "flag1": bool(self.parameters[5 + c]),  # orientation flag
+                "k1": int(self.parameters[6 + c]),
+            }  # n curves
             curves = []
-            for j in range(edge['k1']):
-                curve = {'iso': bool(self.parameters[7 + c + j*2]),  # isopara flag
-                         'psc': int(self.parameters[8 + c + j*2])}  # space curve
+            for j in range(edge["k1"]):
+                curve = {
+                    "iso": bool(self.parameters[7 + c + j * 2]),  # isopara flag
+                    "psc": int(self.parameters[8 + c + j * 2]),
+                }  # space curve
                 curves.append(curve)
-            c += 5 + 2*edge['k1']
+            c += 5 + 2 * edge["k1"]
 
-            edge['curves'] = curves
+            edge["curves"] = curves
             self._edges.append(edge)
 
     # @property
     # def edge_lists(self):
-    #     for 
+    #     for
 
     def curves(self):
         """list of curves"""
         pass
 
     def __repr__(self):
-        info = 'IGES Type 508: Loop\n'
+        info = "IGES Type 508: Loop\n"
         return info
 
 
 class EdgeList(Entity):
     """Provides a list of edges, comprised of vertices, for specifying
     B-Rep Geometries."""
+
     _iges_type = 504
 
     def _add_parameters(self, parameters):
         """
         Parameter Data
         Index in list	Type of data	Name	Description
         INT	N	Number of Edges in list
@@ -767,56 +807,60 @@
         3	Pointer	SVL1	Vertex list for start vertex
         4	INT	S1	Index of start vertex in SVL1
         5	Pointer	EVL1	Vertex list for end vertex
         6	INT	E1	Index of end vertex in EVL1
         .
         .	.
         .	.
-        .	
+        .
         5N-3	Pointer	CurveN	First model space curve
         5N-2	Pointer	SVLN	Vertex list for start vertex
         5N-1	INT	SN	Index of start vertex in SVLN
         5N	Pointer	EVLN	Vertex list for end vertex
         5N+1	INT	EN	Index of end vertex in EVLN
         """
         self.parameters = parameters
         self.n_edges = int(parameters[1])
 
         self.edges = []
         for i in range(self.n_edges):
-            edge = {'curve1': int(parameters[2 + 5*i]),  # first model space curve
-                    'svl': int(parameters[3 + 5*i]),  # vertex list for start vertex
-                    's': int(parameters[4 + 5*i]),  # start index
-                    'evl': int(parameters[5 + 5*i]), # vertex list for end vertex
-                    'e': int(parameters[6 + 5*i])} # index of end vertex in evl n
+            edge = {
+                "curve1": int(parameters[2 + 5 * i]),  # first model space curve
+                "svl": int(parameters[3 + 5 * i]),  # vertex list for start vertex
+                "s": int(parameters[4 + 5 * i]),  # start index
+                "evl": int(parameters[5 + 5 * i]),  # vertex list for end vertex
+                "e": int(parameters[6 + 5 * i]),
+            }  # index of end vertex in evl n
             self.edges.append(edge)
 
     # @property
     # def curve(self, ):
     #     for
 
     def __getitem__(self, indices):
         # TODO: limit spline based on start and end point
-        ptr = self.edges[indices]['curve1']
+        ptr = self.edges[indices]["curve1"]
         return self.iges.from_pointer(ptr)
 
     def __len__(self):
         return len(self.edges)
 
     def __repr__(self):
-        info = 'IGES Type %d: Edge List\n' % self._iges_type
-        return info
+        """Return the representation of EdgesList."""
+        return "IGES Type {self._iges_type}: Edge List\n"
 
 
 class VertexList(Entity):
     """Vertex List (Type 502 Form 1)"""
+
     _iges_type = 502
 
     def _add_parameters(self, parameters):
-        """Parameter Data
+        """Adds Parameter Data.
+
         Index in list	Type of data	Name	Description
         INT	N	Number of vertices in list
         2	REAL	X1	Coordinates of first vertex
         3	REAL	Y1
         4	REAL	Z1
         .
         .	.
@@ -826,11 +870,13 @@
         3N	REAL	YN
         3N+1	REAL	ZN
         """
         self.parameters = parameters
         self.n_points = int(parameters[1])
         self.points = []
         for i in range(self.n_points):
-            point = [parse_float(self.parameters[2 + i*3]),
-                     parse_float(self.parameters[3 + i*3]),
-                     parse_float(self.parameters[4 + i*3])]
+            point = [
+                parse_float(self.parameters[2 + i * 3]),
+                parse_float(self.parameters[3 + i * 3]),
+                parse_float(self.parameters[4 + i * 3]),
+            ]
             self.points.append(point)
```

### Comparing `pyiges-0.2.1/pyiges/examples/sample.igs` & `pyiges-0.3.0/pyiges/examples/sample.igs`

 * *Files identical despite different names*

### Comparing `pyiges-0.2.1/pyiges/examples/impeller.igs` & `pyiges-0.3.0/pyiges/examples/impeller.igs`

 * *Files identical despite different names*

### Comparing `pyiges-0.2.1/README.rst` & `pyiges-0.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -17,28 +17,36 @@
 - Conic Arc (Type 104)
 - Line
 - Point
 
 
 Installation
 ------------
+
+``pyiges`` is offered in a "full" variant including the conversion features
+and a "pure" parsing module variant.
+The pure variant has no conversion features, no dependencies to ``pyvista,geomdl``,
+and can be installed by removing the ``[full]`` specificator from the following commands.
+
 Install with pip using:
 
 .. code::
 
-   pip install pyiges
+   pip install pyiges[full]
 
 Otherwise, if you want the bleeding edge version, feel free to clone
 this repo and install with:
 
 .. code:: bash
 
    git clone https://github.com/pyvista/pyiges
    cd pyiges
-   pip install .
+   pip install .[full]
+
+Note that the square brackets might need to be escaped or quoted when using ``zsh``.
 
 
 Usage
 -----
 The ``pyiges`` module can read in many entities as raw text, but only
 NURBS surfaces and bsplines can be converted to ``pyvista`` meshes.
 
@@ -66,20 +74,20 @@
     mesh.save('mesh.ply')  # as ply
     mesh.save('mesh.stl')  # as stl
     mesh.save('mesh.vtk')  # as vtk
 
 
 Lines
 ~~~~~
-.. image:: https://github.com/pyvista/pyiges/raw/master/docs/images/impeller_lines.png
+.. image:: https://github.com/pyvista/pyiges/raw/main/docs/images/impeller_lines.png
 
 
 Surfaces
 ~~~~~~~~
-.. image:: https://github.com/pyvista/pyiges/raw/master/docs/images/impeller_surf.png
+.. image:: https://github.com/pyvista/pyiges/raw/main/docs/images/impeller_surf.png
 
 
 
 Acknowledgments
 ---------------
 Substantial code was obtained from or inspired by https://github.com/cfinch/IGES-File-Reader
```

