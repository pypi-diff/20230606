# Comparing `tmp/pyxel-dic-3.0.5.tar.gz` & `tmp/pyxel-dic-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxel-dic-3.0.5.tar", last modified: Fri Jun  2 13:19:47 2023, max compression
+gzip compressed data, was "pyxel-dic-3.0.6.tar", last modified: Mon Jun  5 22:07:43 2023, max compression
```

## Comparing `pyxel-dic-3.0.5.tar` & `pyxel-dic-3.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 13:19:47.073130 pyxel-dic-3.0.5/
--rw-rw-rw-   0        0        0     4930 2023-06-02 13:19:47.073130 pyxel-dic-3.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4250 2023-04-17 15:11:38.000000 pyxel-dic-3.0.5/README.md
--rw-rw-rw-   0        0        0      777 2023-06-02 13:19:10.000000 pyxel-dic-3.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      898 2023-06-02 13:19:47.080002 pyxel-dic-3.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-02 13:19:46.864096 pyxel-dic-3.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 13:19:47.029597 pyxel-dic-3.0.5/src/pyxel/
--rw-rw-rw-   0        0        0      332 2023-04-17 15:11:38.000000 pyxel-dic-3.0.5/src/pyxel/__init__.py
--rw-rw-rw-   0        0        0    31183 2023-04-17 15:11:38.000000 pyxel-dic-3.0.5/src/pyxel/camera.py
--rw-rw-rw-   0        0        0    24424 2023-05-16 15:41:06.000000 pyxel-dic-3.0.5/src/pyxel/dic.py
--rw-rw-rw-   0        0        0     2317 2023-04-17 15:11:38.000000 pyxel-dic-3.0.5/src/pyxel/exportpixmap.py
--rw-rw-rw-   0        0        0    13368 2023-04-17 15:11:38.000000 pyxel-dic-3.0.5/src/pyxel/image.py
--rw-rw-rw-   0        0        0     9658 2023-04-17 15:11:38.000000 pyxel-dic-3.0.5/src/pyxel/levelset.py
--rw-rw-rw-   0        0        0     3293 2023-04-17 15:11:38.000000 pyxel-dic-3.0.5/src/pyxel/material.py
--rw-rw-rw-   0        0        0   131651 2023-06-02 13:10:55.000000 pyxel-dic-3.0.5/src/pyxel/mesh.py
--rw-rw-rw-   0        0        0    18605 2023-06-02 13:11:51.000000 pyxel-dic-3.0.5/src/pyxel/mesher.py
--rw-rw-rw-   0        0        0     6859 2023-04-17 15:11:38.000000 pyxel-dic-3.0.5/src/pyxel/meshparser.py
--rw-rw-rw-   0        0        0     3245 2023-04-17 15:11:38.000000 pyxel-dic-3.0.5/src/pyxel/utils.py
--rw-rw-rw-   0        0        0    16353 2023-04-17 15:11:38.000000 pyxel-dic-3.0.5/src/pyxel/vtktools.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:19:47.067957 pyxel-dic-3.0.5/src/pyxel_dic.egg-info/
--rw-rw-rw-   0        0        0     4930 2023-06-02 13:19:46.000000 pyxel-dic-3.0.5/src/pyxel_dic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-06-02 13:19:46.000000 pyxel-dic-3.0.5/src/pyxel_dic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 13:19:46.000000 pyxel-dic-3.0.5/src/pyxel_dic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-02 13:19:46.000000 pyxel-dic-3.0.5/src/pyxel_dic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-02 13:19:46.000000 pyxel-dic-3.0.5/src/pyxel_dic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 22:07:43.359533 pyxel-dic-3.0.6/
+-rw-rw-rw-   0        0        0     4930 2023-06-05 22:07:43.360541 pyxel-dic-3.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4250 2023-04-17 15:11:38.000000 pyxel-dic-3.0.6/README.md
+-rw-rw-rw-   0        0        0      777 2023-06-05 22:06:52.000000 pyxel-dic-3.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      898 2023-06-05 22:07:43.366947 pyxel-dic-3.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 22:07:43.141990 pyxel-dic-3.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 22:07:43.317604 pyxel-dic-3.0.6/src/pyxel/
+-rw-rw-rw-   0        0        0      332 2023-04-17 15:11:38.000000 pyxel-dic-3.0.6/src/pyxel/__init__.py
+-rw-rw-rw-   0        0        0    31183 2023-04-17 15:11:38.000000 pyxel-dic-3.0.6/src/pyxel/camera.py
+-rw-rw-rw-   0        0        0    24425 2023-06-05 20:22:25.000000 pyxel-dic-3.0.6/src/pyxel/dic.py
+-rw-rw-rw-   0        0        0     2317 2023-04-17 15:11:38.000000 pyxel-dic-3.0.6/src/pyxel/exportpixmap.py
+-rw-rw-rw-   0        0        0    13368 2023-04-17 15:11:38.000000 pyxel-dic-3.0.6/src/pyxel/image.py
+-rw-rw-rw-   0        0        0     9658 2023-04-17 15:11:38.000000 pyxel-dic-3.0.6/src/pyxel/levelset.py
+-rw-rw-rw-   0        0        0     3293 2023-04-17 15:11:38.000000 pyxel-dic-3.0.6/src/pyxel/material.py
+-rw-rw-rw-   0        0        0   133025 2023-06-05 20:00:34.000000 pyxel-dic-3.0.6/src/pyxel/mesh.py
+-rw-rw-rw-   0        0        0    18605 2023-06-02 13:11:51.000000 pyxel-dic-3.0.6/src/pyxel/mesher.py
+-rw-rw-rw-   0        0        0     6859 2023-04-17 15:11:38.000000 pyxel-dic-3.0.6/src/pyxel/meshparser.py
+-rw-rw-rw-   0        0        0     3475 2023-06-05 19:55:50.000000 pyxel-dic-3.0.6/src/pyxel/utils.py
+-rw-rw-rw-   0        0        0    16353 2023-04-17 15:11:38.000000 pyxel-dic-3.0.6/src/pyxel/vtktools.py
+drwxrwxrwx   0        0        0        0 2023-06-05 22:07:43.354595 pyxel-dic-3.0.6/src/pyxel_dic.egg-info/
+-rw-rw-rw-   0        0        0     4930 2023-06-05 22:07:43.000000 pyxel-dic-3.0.6/src/pyxel_dic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-06-05 22:07:43.000000 pyxel-dic-3.0.6/src/pyxel_dic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 22:07:43.000000 pyxel-dic-3.0.6/src/pyxel_dic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-05 22:07:43.000000 pyxel-dic-3.0.6/src/pyxel_dic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 22:07:43.000000 pyxel-dic-3.0.6/src/pyxel_dic.egg-info/top_level.txt
```

### Comparing `pyxel-dic-3.0.5/PKG-INFO` & `pyxel-dic-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-dic
-Version: 3.0.5
+Version: 3.0.6
 Summary: Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics
 Home-page: https://github.com/jcpassieux/pyxel
 Author: Jean-Charles Passieux
 Author-email: JC Passieux <jc.passieux@gmail.com>
 License: CeCILL
 Project-URL: Homepage, https://github.com/jcpassieux/pyxel
 Project-URL: Bug Tracker, https://github.com/jcpassieux/pyxel/issues
```

### Comparing `pyxel-dic-3.0.5/README.md` & `pyxel-dic-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.5/pyproject.toml` & `pyxel-dic-3.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyxel-dic"
-version = "3.0.5"
+version = "3.0.6"
 authors = [
   { name="JC Passieux", email="jc.passieux@gmail.com" },
 ]
 description = "Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyxel-dic-3.0.5/setup.cfg` & `pyxel-dic-3.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.5/src/pyxel/camera.py` & `pyxel-dic-3.0.6/src/pyxel/camera.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.5/src/pyxel/dic.py` & `pyxel-dic-3.0.6/src/pyxel/dic.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
         print('reduced basis')
         H_LU = splalg.splu(Basis.T @ H @ Basis)
     else:
         if l0 is not None:
             # Tikhonov regularisation
             if L is None:
                 L = m.Tikhonov()
-            used_nodes = m.conn[:, 0] > 0
+            used_nodes = m.conn[:, 0] > -1
             T = 10 * m.GetApproxElementSize()
             V = np.zeros(m.ndof)
             V[m.conn[used_nodes, 0]] = np.cos(m.n[used_nodes, 1] / T * 2 * np.pi)
             H0 = V.dot(H.dot(V))
             L0 = V.dot(L.dot(V))
             l = (l0/T)**2 * H0 / L0
             H_LU = splalg.splu(H + l * L)
```

### Comparing `pyxel-dic-3.0.5/src/pyxel/exportpixmap.py` & `pyxel-dic-3.0.6/src/pyxel/exportpixmap.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.5/src/pyxel/image.py` & `pyxel-dic-3.0.6/src/pyxel/image.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.5/src/pyxel/levelset.py` & `pyxel-dic-3.0.6/src/pyxel/levelset.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.5/src/pyxel/material.py` & `pyxel-dic-3.0.6/src/pyxel/material.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.5/src/pyxel/mesh.py` & `pyxel-dic-3.0.6/src/pyxel/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,21 +446,21 @@
                 (y - 1, 1 - y, 1 + y, -1 - y)).reshape((4,len(x))).T 
 
         def dN_eta(x, y):
             return 0.25 * np.concatenate(
                 (x - 1, -1 - x, 1 + x, 1 - x)).reshape((4,len(x))).T 
 
         # reduced integration
-        xg = np.array([0])
-        yg = np.array([0])
-        wg = np.array([4])
+        # xg = np.array([0])
+        # yg = np.array([0])
+        # wg = np.array([4])
         # full integration        
-        # xg = np.sqrt(3) / 3 * np.array([-1, 1, -1, 1])
-        # yg = np.sqrt(3) / 3 * np.array([-1, -1, 1, 1])
-        # wg = np.ones(4)
+        xg = np.sqrt(3) / 3 * np.array([-1, 1, -1, 1])
+        yg = np.sqrt(3) / 3 * np.array([-1, -1, 1, 1])
+        wg = np.ones(4)
         return xg, yg, wg, N, dN_xi, dN_eta
     elif eltype == 9:
         """
         #############
             tri6
         #############
         """
@@ -2385,15 +2385,15 @@
         plt.figure()
         plt.scatter(self.pgx[rep], self.pgy[rep], c=res, cmap="RdBu", s=1)
         plt.axis("equal")
         plt.clim(-3 * stdr, 3 * stdr)
         plt.colorbar()
         plt.show()
 
-    def PlotContourDispl(self, U=None, n=None, s=1.0, stype='comp', newfig=True, **kwargs):
+    def PlotContourDispl(self, U=None, n=None, s=1.0, stype='comp', newfig=True, plotmesh=True, cmap='RdBu', **kwargs):
         """
         Plots the displacement field using Matplotlib Library.        
 
         Parameters
         ----------
         U : 1D NUMPY.ARRAY
             displacement dof vector
@@ -2434,30 +2434,35 @@
             elif ie == 2 or ie == 9:  # triangles
                 triangles = np.vstack((triangles, self.e[ie]))
         alpha = kwargs.pop("alpha", 1)
         if stype == 'mag':
             Vmag = np.sqrt(V[self.conn[:, 0]]**2 + V[self.conn[:, 1]]**2)
             if newfig:
                 plt.figure()
-            plt.tricontourf(n[:, 0], n[:, 1], triangles, Vmag, 20, alpha=alpha)
+            plt.tricontourf(n[:, 0], n[:, 1], triangles, Vmag, 20, alpha=alpha, cmap=cmap)
             plt.colorbar()
-            self.Plot(n=n, alpha=0.1)
+            if plotmesh:
+                self.Plot(n=n, alpha=0.1)
+            plt.axis('equal')
             plt.axis("off")
             plt.title("Magnitude")
         else:
             plt.figure()
-            plt.tricontourf(n[:, 0], n[:, 1], triangles, V[self.conn[:, 0]], 20, alpha=alpha)
-            self.Plot(n=n, alpha=0.1)
+            plt.tricontourf(n[:, 0], n[:, 1], triangles, V[self.conn[:, 0]], 20, alpha=alpha, cmap=cmap)
+            if plotmesh:
+                self.Plot(n=n, alpha=0.1)
+            plt.axis('equal')
             plt.axis("off")
             plt.title("x")
             plt.colorbar()
             plt.figure()
-            plt.tricontourf(n[:, 0], n[:, 1], triangles, V[self.conn[:, 1]], 20, alpha=alpha)
+            plt.tricontourf(n[:, 0], n[:, 1], triangles, V[self.conn[:, 1]], 20, alpha=alpha, cmap=cmap)
             plt.colorbar()
-            self.Plot(n=n, alpha=0.1)
+            if plotmesh:
+                self.Plot(n=n, alpha=0.1)
             plt.axis("equal")
             plt.title("y")
             plt.axis("off")
             plt.show()
 
     def PlotContourStrain(self, U, n=None, s=1.0, stype='comp', newfig=True, **kwargs):
         """
@@ -2755,18 +2760,20 @@
         """
         Returns the dof of all the nodes lying within a rectangle defined
         by the coordinates of two diagonal points (in the mesh coordinate sys).
         Used to apply BC for instance.
         box = np.array([[xmin, ymin],
                         [xmax, ymax]])    in mesh unit
         """
-        dofs = np.zeros((0, 2), dtype="int")
-        for jn in range(len(self.n)):
-            if isInBox(box, self.n[jn, 0], self.n[jn, 1]):
-                dofs = np.vstack((dofs, self.conn[jn]))
+        if self.dim == 2:
+            rep, = np.where(isInBox(box, self.n[:,0], self.n[:,1]))
+        else:
+            rep, = np.where(isInBox(box, self.n[:,0], self.n[:,1], self.n[:,2]))
+        reprep, = np.where(self.conn[rep, 0]>-1)
+        dofs = self.conn[rep[reprep]]
         return dofs
 
     def KeepEdgeElems(self):
         """
         Removes every but edge elements.
         """
         newe = dict()
@@ -2799,27 +2806,34 @@
         Removes all the elements whose center lie in the Region of Interest of
         an image f.
         Usage :
             m.RemoveElemsOutsideRoi(cam, roi)
 
         where  roi = f.SelectROI()
         """
-        if cam is None:
+        if self.dim == 3:
+            if cam is None:
+                u, v, w = self.n[:,0], self.n[:,1], self.n[:,2]
+            else:
+                u, v, w = cam.P(self.n[:,0], self.n[:,1], self.n[:,2])
             for je in self.e.keys():
-                u = np.mean(self.n[self.e[je], 0], axis=1)
-                v = np.mean(self.n[self.e[je], 1], axis=1)
-                inside = isInBox(roi, u, v)
-                self.e[je] = self.e[je][inside, :]
+                umoy = np.mean(u[self.e[je]], axis=1)
+                vmoy = np.mean(v[self.e[je]], axis=1)
+                wmoy = np.mean(w[self.e[je]], axis=1)
+                inside = isInBox(roi, umoy, vmoy, wmoy)
         else:
+            if cam is None:
+                u, v = self.n[:,0], self.n[:,1]
+            else:
+                u, v = cam.P(self.n[:,0], self.n[:,1])
             for je in self.e.keys():
-                xc = np.mean(self.n[self.e[je], 0], axis=1)
-                yc = np.mean(self.n[self.e[je], 1], axis=1)
-                u, v = cam.P(xc, yc)
-                inside = isInBox(roi, v, u)
-                self.e[je] = self.e[je][inside, :]
+                umoy = np.mean(u[self.e[je]], axis=1)
+                vmoy = np.mean(v[self.e[je]], axis=1)
+                inside = isInBox(roi, umoy, vmoy)
+        self.e[je] = self.e[je][inside, :]
 
     def RemoveDoubleNodes(self):
         """
         Removes the double nodes thus changes connectivity 
         Warning: both self.e and self.n are modified!
 
         Usage : 
@@ -2942,17 +2956,16 @@
         """
         plt.figure()
         self.Plot()
         figManager = plt.get_current_fig_manager()
         if hasattr(figManager.window, 'showMaximized'):
             figManager.window.showMaximized()
         else:
-            if hasattr(figManager.window, 'maxsize'):
-                figManager.resize(figManager.window.maxsize())
-
+            if hasattr(figManager.window, 'maximize'):
+                figManager.resize(figManager.window.maximize())
         if title is None:
             if n < 0:
                 plt.title("Select several points... and press enter")
             else:
                 plt.title("Select " + str(n) + " points... and press enter")
         else:
             plt.title(title)
@@ -2963,15 +2976,19 @@
     def SelectNodes(self, n=-1):
         """
         Selection of nodes by hand in a mesh.
         """
         plt.figure()
         self.Plot()
         figManager = plt.get_current_fig_manager()
-        figManager.window.showMaximized()
+        if hasattr(figManager.window, 'showMaximized'):
+            figManager.window.showMaximized()
+        else:
+            if hasattr(figManager.window, 'maximize'):
+                figManager.resize(figManager.window.maximize())
         plt.title("Select " + str(n) + " points... and press enter")
         pts1 = np.array(plt.ginput(n, timeout=0))
         plt.close()
         dx = np.kron(np.ones(pts1.shape[0]), self.n[:, [0]]) - np.kron(
             np.ones((self.n.shape[0], 1)), pts1[:, 0]
         )
         dy = np.kron(np.ones(pts1.shape[0]), self.n[:, [1]]) - np.kron(
@@ -2986,15 +3003,19 @@
         """
         Selection of all the nodes of a mesh lying in a box defined by two
         points clics.
         """
         plt.figure()
         self.Plot()
         figManager = plt.get_current_fig_manager()
-        figManager.window.showMaximized()
+        if hasattr(figManager.window, 'showMaximized'):
+            figManager.window.showMaximized()
+        else:
+            if hasattr(figManager.window, 'maximize'):
+                figManager.resize(figManager.window.maximize())
         plt.title("Select 2 points... and press enter")
         pts1 = np.array(plt.ginput(2, timeout=0))
         plt.close()
         inside = (
             (self.n[:, 0] > pts1[0, 0])
             * (self.n[:, 0] < pts1[1, 0])
             * (self.n[:, 1] > pts1[0, 1])
@@ -3008,15 +3029,19 @@
     def SelectLine(self, eps=1e-8):
         """
         Selection of the nodes along a line defined by 2 nodes.
         """
         plt.figure()
         self.Plot()
         figManager = plt.get_current_fig_manager()
-        figManager.window.showMaximized()
+        if hasattr(figManager.window, 'showMaximized'):
+            figManager.window.showMaximized()
+        else:
+            if hasattr(figManager.window, 'maximize'):
+                figManager.resize(figManager.window.maximize())
         plt.title("Select 2 points of a line... and press enter")
         pts1 = np.array(plt.ginput(2, timeout=0))
         plt.close()
         n1 = np.argmin(np.linalg.norm(self.n - pts1[0, :], axis=1))
         n2 = np.argmin(np.linalg.norm(self.n - pts1[1, :], axis=1))
         v = np.diff(self.n[[n1, n2]], axis=0)[0]
         nv = np.linalg.norm(v)
@@ -3036,15 +3061,19 @@
     def SelectCircle(self):
         """
         Selection of the nodes around a circle defined by 3 nodes.
         """
         plt.figure()
         self.Plot()
         figManager = plt.get_current_fig_manager()
-        figManager.window.showMaximized()
+        if hasattr(figManager.window, 'showMaximized'):
+            figManager.window.showMaximized()
+        else:
+            if hasattr(figManager.window, 'maximize'):
+                figManager.resize(figManager.window.maximize())
         plt.title("Select 3 points on a circle... and press enter")
         pts1 = np.array(plt.ginput(3, timeout=0))
         plt.close()
         n1 = np.argmin(np.linalg.norm(self.n - pts1[0, :], axis=1))
         n2 = np.argmin(np.linalg.norm(self.n - pts1[1, :], axis=1))
         n3 = np.argmin(np.linalg.norm(self.n - pts1[2, :], axis=1))
         pts1 = self.n[[n1, n2, n3], :]
```

### Comparing `pyxel-dic-3.0.5/src/pyxel/mesher.py` & `pyxel-dic-3.0.6/src/pyxel/mesher.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.5/src/pyxel/meshparser.py` & `pyxel-dic-3.0.6/src/pyxel/meshparser.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.5/src/pyxel/utils.py` & `pyxel-dic-3.0.6/src/pyxel/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -105,14 +105,20 @@
         n += U[m.conn]
     plt.figure()
     f.Plot()
     if cam is None:
         u, v, w = n[:, 0], n[:, 1], n[:, 2]
     else:
         u, v, w = cam.P(n[:, 0], n[:, 1], n[:, 2])
+    # if volume elements, build surface mesh
+    if list(m.e.keys())[0] in [5, 4, 11, 17]:
+        mb = m.BuildBoundaryMesh()
+    else:
+        mb = m.Copy()
+    mb.dim = 2
     plt.subplot(221)
-    plt.plot(w, v, "yo", alpha=0.6)
+    mb.Plot(n = np.c_[w, v], edgecolor='y', alpha=0.6)
     plt.subplot(223)
-    plt.plot(w, u, "yo", alpha=0.6)
+    mb.Plot(n = np.c_[w, u], edgecolor='y', alpha=0.6)
     plt.subplot(224)
-    plt.plot(v, u, "yo", alpha=0.6)
+    mb.Plot(n = np.c_[v, u], edgecolor='y', alpha=0.6)
```

### Comparing `pyxel-dic-3.0.5/src/pyxel/vtktools.py` & `pyxel-dic-3.0.6/src/pyxel/vtktools.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.5/src/pyxel_dic.egg-info/PKG-INFO` & `pyxel-dic-3.0.6/src/pyxel_dic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-dic
-Version: 3.0.5
+Version: 3.0.6
 Summary: Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics
 Home-page: https://github.com/jcpassieux/pyxel
 Author: Jean-Charles Passieux
 Author-email: JC Passieux <jc.passieux@gmail.com>
 License: CeCILL
 Project-URL: Homepage, https://github.com/jcpassieux/pyxel
 Project-URL: Bug Tracker, https://github.com/jcpassieux/pyxel/issues
```

