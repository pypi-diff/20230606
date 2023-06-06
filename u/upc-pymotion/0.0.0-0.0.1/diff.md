# Comparing `tmp/upc_pymotion-0.0.0.tar.gz` & `tmp/upc_pymotion-0.0.1.tar.gz`

## Comparing `upc_pymotion-0.0.0.tar` & `upc_pymotion-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/io/__init__.py
--rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/io/bvh.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/ops/__init__.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/ops/forward_kinematics.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/ops/forward_kinematics_torch.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/ops/skeleton.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/ops/skeleton_torch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/rotations/__init__.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/rotations/dual_quat.py
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/rotations/dual_quat_torch.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/rotations/ortho6d.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/rotations/ortho6d_torch.py
--rw-r--r--   0        0        0    13749 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/rotations/quat.py
--rw-r--r--   0        0        0    14656 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/rotations/quat_torch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/visualizer/__init__.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pymotion/visualizer/blender.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/.gitignore
--rw-r--r--   0        0        0    20564 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/LICENSE
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/README.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/pyproject.toml
--rw-r--r--   0        0        0    32244 2020-02-02 00:00:00.000000 upc_pymotion-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/io/__init__.py
+-rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/io/bvh.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/ops/__init__.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/ops/forward_kinematics.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/ops/forward_kinematics_torch.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/ops/skeleton.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/ops/skeleton_torch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/rotations/__init__.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/rotations/dual_quat.py
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/rotations/dual_quat_torch.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/rotations/ortho6d.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/rotations/ortho6d_torch.py
+-rw-r--r--   0        0        0    13749 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/rotations/quat.py
+-rw-r--r--   0        0        0    14700 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/rotations/quat_torch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/visualizer/__init__.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pymotion/visualizer/blender.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/.gitignore
+-rw-r--r--   0        0        0    20564 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/LICENSE
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0    32274 2020-02-02 00:00:00.000000 upc_pymotion-0.0.1/PKG-INFO
```

### Comparing `upc_pymotion-0.0.0/pymotion/io/bvh.py` & `upc_pymotion-0.0.1/pymotion/io/bvh.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/pymotion/ops/forward_kinematics.py` & `upc_pymotion-0.0.1/pymotion/ops/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/pymotion/ops/forward_kinematics_torch.py` & `upc_pymotion-0.0.1/pymotion/ops/forward_kinematics_torch.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,13 +42,13 @@
     mat[..., 0, :3, 3] = global_pos
     # other joints are transformed by the transform matrix
     for i, parent in enumerate(parents):
         # root
         if i == 0:
             continue
         mat[..., i, :, :] = torch.matmul(
-            mat[..., parent, :, :],
-            mat[..., i, :, :],
+            mat[..., parent, :, :].clone(),
+            mat[..., i, :, :].clone(),
         )
     positions = mat[..., :3, 3]
     rotmats = mat[..., :3, :3]
     return positions, rotmats
```

### Comparing `upc_pymotion-0.0.0/pymotion/ops/skeleton.py` & `upc_pymotion-0.0.1/pymotion/ops/skeleton.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/pymotion/ops/skeleton_torch.py` & `upc_pymotion-0.0.1/pymotion/ops/skeleton_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     parents : torch.Tensor[n_joints]
 
     Returns
     -------
     rotations : torch.Tensor[..., n_joints, 4]
     translations : torch.Tensor[..., n_joints, 3]
     """
-    device = dq.device
     n_joints = dq.shape[-2]
     # rotations has shape (..., frames, n_joints, 4)
     # translations has shape (..., frames, n_joints, 3)
     rotations, translations = dquat.to_rotation_translation(dq.clone())
     # make transformations local to the parents
     # (initially local to the root)
     for j in reversed(range(1, n_joints)):
```

### Comparing `upc_pymotion-0.0.0/pymotion/rotations/dual_quat.py` & `upc_pymotion-0.0.1/pymotion/rotations/dual_quat.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/pymotion/rotations/dual_quat_torch.py` & `upc_pymotion-0.0.1/pymotion/rotations/dual_quat_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/pymotion/rotations/ortho6d.py` & `upc_pymotion-0.0.1/pymotion/rotations/ortho6d.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/pymotion/rotations/ortho6d_torch.py` & `upc_pymotion-0.0.1/pymotion/rotations/ortho6d_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/pymotion/rotations/quat.py` & `upc_pymotion-0.0.1/pymotion/rotations/quat.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/pymotion/rotations/quat_torch.py` & `upc_pymotion-0.0.1/pymotion/rotations/quat_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,14 +364,17 @@
     q0 : torch.Tensor[..., [w,x,y,z]]
     q1 : torch.Tensor[..., [w,x,y,z]]
 
     Returns
     -------
     quat : torch.Tensor[..., [w,x,y,z]]
     """
+
+    q0 = q0.clone()
+    q1 = q1.clone()
     w0, x0, y0, z0 = q0[..., 0:1], q0[..., 1:2], q0[..., 2:3], q0[..., 3:4]
     w1, x1, y1, z1 = q1[..., 0:1], q1[..., 1:2], q1[..., 2:3], q1[..., 3:4]
     # (w0,v0)(w1,v1) = (w0w1 - v0·v1, w0v1 + w1v0 + v0 x v1)
     return torch.cat(
         (
             w0 * w1 - x0 * x1 - y0 * y1 - z0 * z1,  # w
             w0 * x1 + w1 * x0 + y0 * z1 - z0 * y1,  # x
```

### Comparing `upc_pymotion-0.0.0/pymotion/visualizer/blender.py` & `upc_pymotion-0.0.1/pymotion/visualizer/blender.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/.gitignore` & `upc_pymotion-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/LICENSE` & `upc_pymotion-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.0.0/README.md` & `upc_pymotion-0.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # PyMotion: A Python Library for Motion Data
 
 PyMotion is a Python library that provides various functions for manipulating and processing motion data in NumPy or PyTorch. It is designed to facilitate the development of neural networks for character animation.
 
 Some of the features of PyMotion are:
 
 - A comprehensive set of quaternion operations and conversions to other rotation representations, such as rotation matrix, axis-angle, euler, and 6D representation
-- A dual quaternion representation for rigid displacements, which can help neural networks better understand poses, as proposed by [Andreou et al. [2022]](https://doi.org/10.1111/cgf.14632) and later adopted by [Ponton et al. [2023]](https://TODO)
+- A dual quaternion representation for rigid displacements, which can help neural networks better understand poses, as proposed by [Andreou et al. [2022]](https://doi.org/10.1111/cgf.14632) and later adopted by [Ponton et al. [2023]](https://upc-virvig.github.io/SparsePoser/)
 - A continuous 6D rotation representation, as introduced by [Zhou et al. [2019]](https://doi.org/10.1109/CVPR.2019.00589)
 - A BVH file reader and preprocessor for loading and transforming motion data
 - Skeletal operations such as Forward Kinematics for computing global joint positions from local joint rotations
 - [Beta] A blender visualizer for debugging and visualizing character animation
 - NumPy and PyTorch implementations and tests for all functions
 
 ## Contents
@@ -255,15 +255,17 @@
 
 5. Press ESC key in Blender to stop the server
 
 </details>
 
 ## Roadmap
 
-This repository is authored and maintained by [Jose Luis Ponton](https://github.com/JLPM22) as part of his Ph.D. Features will be added when new operations or rotation representations are needed in the development of research projects. Here it is a list of possible features and improvements for the future:
+This repository is authored and maintained by [Jose Luis Ponton](https://github.com/JLPM22) as part of his Ph.D.
+
+Features will be added when new operations or rotation representations are needed in the development of research projects. Here it is a list of possible features and improvements for the future:
 
 - Extend documentation and add examples in the description of each function.
 - Include new animation importers such as FBX
 - Improve the usability of the Blender visualization workflow
 - Include useful operations for data augmentation such as animation mirroring
 - Create an Inverse Kinematics module
```

### Comparing `upc_pymotion-0.0.0/pyproject.toml` & `upc_pymotion-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [tool.hatch.build]
 include = ["pymotion/*"]
 exclude = ["*test*"]
 
 [project]
 name = "upc-pymotion"
-version = "0.0.0"
+version = "0.0.1"
 description = "A Python library for working with motion data in numpy or PyTorch."
 readme = "README.md"
 authors = [{ name = "Jose Luis Ponton", email = "jose.luis.ponton@upc.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `upc_pymotion-0.0.0/PKG-INFO` & `upc_pymotion-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upc-pymotion
-Version: 0.0.0
+Version: 0.0.1
 Summary: A Python library for working with motion data in numpy or PyTorch.
 Project-URL: Homepage, https://github.com/UPC-ViRVIG/pymotion
 Author-email: Jose Luis Ponton <jose.luis.ponton@upc.edu>
 License: Attribution-ShareAlike 4.0 International
         
         =======================================================================
         
@@ -448,15 +448,15 @@
 # PyMotion: A Python Library for Motion Data
 
 PyMotion is a Python library that provides various functions for manipulating and processing motion data in NumPy or PyTorch. It is designed to facilitate the development of neural networks for character animation.
 
 Some of the features of PyMotion are:
 
 - A comprehensive set of quaternion operations and conversions to other rotation representations, such as rotation matrix, axis-angle, euler, and 6D representation
-- A dual quaternion representation for rigid displacements, which can help neural networks better understand poses, as proposed by [Andreou et al. [2022]](https://doi.org/10.1111/cgf.14632) and later adopted by [Ponton et al. [2023]](https://TODO)
+- A dual quaternion representation for rigid displacements, which can help neural networks better understand poses, as proposed by [Andreou et al. [2022]](https://doi.org/10.1111/cgf.14632) and later adopted by [Ponton et al. [2023]](https://upc-virvig.github.io/SparsePoser/)
 - A continuous 6D rotation representation, as introduced by [Zhou et al. [2019]](https://doi.org/10.1109/CVPR.2019.00589)
 - A BVH file reader and preprocessor for loading and transforming motion data
 - Skeletal operations such as Forward Kinematics for computing global joint positions from local joint rotations
 - [Beta] A blender visualizer for debugging and visualizing character animation
 - NumPy and PyTorch implementations and tests for all functions
 
 ## Contents
@@ -702,15 +702,17 @@
 
 5. Press ESC key in Blender to stop the server
 
 </details>
 
 ## Roadmap
 
-This repository is authored and maintained by [Jose Luis Ponton](https://github.com/JLPM22) as part of his Ph.D. Features will be added when new operations or rotation representations are needed in the development of research projects. Here it is a list of possible features and improvements for the future:
+This repository is authored and maintained by [Jose Luis Ponton](https://github.com/JLPM22) as part of his Ph.D.
+
+Features will be added when new operations or rotation representations are needed in the development of research projects. Here it is a list of possible features and improvements for the future:
 
 - Extend documentation and add examples in the description of each function.
 - Include new animation importers such as FBX
 - Improve the usability of the Blender visualization workflow
 - Include useful operations for data augmentation such as animation mirroring
 - Create an Inverse Kinematics module
```

