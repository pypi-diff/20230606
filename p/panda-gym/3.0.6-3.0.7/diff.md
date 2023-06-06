# Comparing `tmp/panda_gym-3.0.6.tar.gz` & `tmp/panda_gym-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_gym-3.0.6.tar", last modified: Thu Apr 27 08:56:10 2023, max compression
+gzip compressed data, was "panda_gym-3.0.7.tar", last modified: Tue Jun  6 16:00:18 2023, max compression
```

## Comparing `panda_gym-3.0.6.tar` & `panda_gym-3.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.811579 panda_gym-3.0.6/
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     1075 2023-04-27 07:54:06.000000 panda_gym-3.0.6/LICENSE
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3928 2023-04-27 08:56:10.807579 panda_gym-3.0.6/PKG-INFO
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3291 2023-04-27 07:54:06.000000 panda_gym-3.0.6/README.md
-drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym/
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     1821 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/__init__.py
-drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym/assets/
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)      104 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/assets/__init__.py
-drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym/envs/
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)      162 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/envs/__init__.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)    12094 2023-04-27 08:35:37.000000 panda_gym-3.0.6/panda_gym/envs/core.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)    14044 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/envs/panda_tasks.py
-drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym/envs/robots/
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/envs/robots/__init__.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     6321 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/envs/robots/panda.py
-drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym/envs/tasks/
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/envs/tasks/__init__.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3647 2023-04-27 08:34:57.000000 panda_gym-3.0.6/panda_gym/envs/tasks/flip.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3885 2023-04-27 08:35:00.000000 panda_gym-3.0.6/panda_gym/envs/tasks/pick_and_place.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3804 2023-04-27 08:35:03.000000 panda_gym-3.0.6/panda_gym/envs/tasks/push.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     2202 2023-04-27 08:35:07.000000 panda_gym-3.0.6/panda_gym/envs/tasks/reach.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3967 2023-04-27 08:35:10.000000 panda_gym-3.0.6/panda_gym/envs/tasks/slide.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     5630 2023-04-27 08:35:14.000000 panda_gym-3.0.6/panda_gym/envs/tasks/stack.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)    26817 2023-04-27 08:30:08.000000 panda_gym-3.0.6/panda_gym/pybullet.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)      800 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/utils.py
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)        5 2023-04-27 08:42:08.000000 panda_gym-3.0.6/panda_gym/version.txt
-drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym.egg-info/
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3928 2023-04-27 08:56:10.000000 panda_gym-3.0.6/panda_gym.egg-info/PKG-INFO
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)      669 2023-04-27 08:56:10.000000 panda_gym-3.0.6/panda_gym.egg-info/SOURCES.txt
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)        1 2023-04-27 08:56:10.000000 panda_gym-3.0.6/panda_gym.egg-info/dependency_links.txt
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)      102 2023-04-27 08:56:10.000000 panda_gym-3.0.6/panda_gym.egg-info/requires.txt
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)       10 2023-04-27 08:56:10.000000 panda_gym-3.0.6/panda_gym.egg-info/top_level.txt
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)       38 2023-04-27 08:56:10.811579 panda_gym-3.0.6/setup.cfg
--rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     1195 2023-04-27 07:54:06.000000 panda_gym-3.0.6/setup.py
+drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-06-06 16:00:18.658011 panda_gym-3.0.7/
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     1075 2021-10-12 17:31:44.000000 panda_gym-3.0.7/LICENSE
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     3891 2023-06-06 16:00:18.657722 panda_gym-3.0.7/PKG-INFO
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     3291 2023-01-02 15:40:01.000000 panda_gym-3.0.7/README.md
+drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-06-06 16:00:18.653042 panda_gym-3.0.7/panda_gym/
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)      898 2023-06-06 15:59:34.000000 panda_gym-3.0.7/panda_gym/__init__.py
+drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-06-06 16:00:18.653785 panda_gym-3.0.7/panda_gym/assets/
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)      104 2021-11-24 13:21:10.000000 panda_gym-3.0.7/panda_gym/assets/__init__.py
+drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-06-06 16:00:18.654722 panda_gym-3.0.7/panda_gym/envs/
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)      162 2023-01-23 15:31:17.000000 panda_gym-3.0.7/panda_gym/envs/__init__.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)    12094 2023-05-29 15:16:22.000000 panda_gym-3.0.7/panda_gym/envs/core.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)    14044 2023-03-18 10:04:26.000000 panda_gym-3.0.7/panda_gym/envs/panda_tasks.py
+drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-06-06 16:00:18.655382 panda_gym-3.0.7/panda_gym/envs/robots/
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)        0 2022-01-28 13:40:33.000000 panda_gym-3.0.7/panda_gym/envs/robots/__init__.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     6503 2023-05-31 08:36:27.000000 panda_gym-3.0.7/panda_gym/envs/robots/panda.py
+drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-06-06 16:00:18.657346 panda_gym-3.0.7/panda_gym/envs/tasks/
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)        0 2022-01-28 13:40:33.000000 panda_gym-3.0.7/panda_gym/envs/tasks/__init__.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     3647 2023-05-29 15:16:22.000000 panda_gym-3.0.7/panda_gym/envs/tasks/flip.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     3885 2023-05-29 15:16:22.000000 panda_gym-3.0.7/panda_gym/envs/tasks/pick_and_place.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     3804 2023-05-29 15:16:22.000000 panda_gym-3.0.7/panda_gym/envs/tasks/push.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     2202 2023-05-29 15:16:22.000000 panda_gym-3.0.7/panda_gym/envs/tasks/reach.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     3967 2023-05-29 15:16:22.000000 panda_gym-3.0.7/panda_gym/envs/tasks/slide.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     5630 2023-05-29 15:16:22.000000 panda_gym-3.0.7/panda_gym/envs/tasks/stack.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)    26867 2023-06-06 15:59:34.000000 panda_gym-3.0.7/panda_gym/pybullet.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)      800 2022-10-19 15:32:25.000000 panda_gym-3.0.7/panda_gym/utils.py
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)        5 2023-06-06 15:59:34.000000 panda_gym-3.0.7/panda_gym/version.txt
+drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-06-06 16:00:18.653651 panda_gym-3.0.7/panda_gym.egg-info/
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     3891 2023-06-06 16:00:18.000000 panda_gym-3.0.7/panda_gym.egg-info/PKG-INFO
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)      669 2023-06-06 16:00:18.000000 panda_gym-3.0.7/panda_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)        1 2023-06-06 16:00:18.000000 panda_gym-3.0.7/panda_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)      102 2023-06-06 16:00:18.000000 panda_gym-3.0.7/panda_gym.egg-info/requires.txt
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)       10 2023-06-06 16:00:18.000000 panda_gym-3.0.7/panda_gym.egg-info/top_level.txt
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)       38 2023-06-06 16:00:18.658056 panda_gym-3.0.7/setup.cfg
+-rw-r--r--   0 quentingallouedec   (501) staff       (20)     1195 2023-05-29 15:16:22.000000 panda_gym-3.0.7/setup.py
```

### Comparing `panda_gym-3.0.6/LICENSE` & `panda_gym-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/PKG-INFO` & `panda_gym-3.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: panda_gym
-Version: 3.0.6
+Version: 3.0.7
 Summary: Set of robotic environments based on PyBullet physics engine and gymnasium.
 Home-page: https://github.com/qgallouedec/panda-gym
 Author: Quentin GALLOUÉDEC
 Author-email: gallouedec.quentin@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: develop
@@ -94,9 +92,7 @@
   author       = {Gallou{\'e}dec, Quentin and Cazin, Nicolas and Dellandr{\'e}a, Emmanuel and Chen, Liming},
   year         = 2021,
   journal      = {4th Robot Learning Workshop: Self-Supervised and Lifelong Learning at NeurIPS},
 }
 ```
 
 Environments are widely inspired from [OpenAI Fetch environments](https://openai.com/blog/ingredients-for-robotics-research/). 
-
-
```

### Comparing `panda_gym-3.0.6/README.md` & `panda_gym-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/panda_gym/envs/core.py` & `panda_gym-3.0.7/panda_gym/envs/core.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/panda_gym/envs/panda_tasks.py` & `panda_gym-3.0.7/panda_gym/envs/panda_tasks.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/panda_gym/envs/robots/panda.py` & `panda_gym-3.0.7/panda_gym/envs/robots/panda.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,7 +134,11 @@
     def get_ee_position(self) -> np.ndarray:
         """Returns the position of the end-effector as (x, y, z)"""
         return self.get_link_position(self.ee_link)
 
     def get_ee_velocity(self) -> np.ndarray:
         """Returns the velocity of the end-effector as (vx, vy, vz)"""
         return self.get_link_velocity(self.ee_link)
+    
+    def get_ee_orientation(self) -> np.ndarray:
+        """Returns the orientation of the end-effector as (x, y, z, w)"""
+        return self.get_link_orientation(self.ee_link)
```

### Comparing `panda_gym-3.0.6/panda_gym/envs/tasks/flip.py` & `panda_gym-3.0.7/panda_gym/envs/tasks/flip.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/panda_gym/envs/tasks/pick_and_place.py` & `panda_gym-3.0.7/panda_gym/envs/tasks/pick_and_place.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/panda_gym/envs/tasks/push.py` & `panda_gym-3.0.7/panda_gym/envs/tasks/push.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/panda_gym/envs/tasks/reach.py` & `panda_gym-3.0.7/panda_gym/envs/tasks/reach.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/panda_gym/envs/tasks/slide.py` & `panda_gym-3.0.7/panda_gym/envs/tasks/slide.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/panda_gym/envs/tasks/stack.py` & `panda_gym-3.0.7/panda_gym/envs/tasks/stack.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/panda_gym/pybullet.py` & `panda_gym-3.0.7/panda_gym/pybullet.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,16 @@
     def step(self) -> None:
         """Step the simulation."""
         for _ in range(self.n_substeps):
             self.physics_client.stepSimulation()
 
     def close(self) -> None:
         """Close the simulation."""
-        self.physics_client.disconnect()
+        if self.physics_client.isConnected():
+            self.physics_client.disconnect()
 
     def save_state(self) -> int:
         """Save the current simulation state.
 
         Returns:
             int: A state id assigned by PyBullet, which is the first non-negative
             integer available for indexing.
```

### Comparing `panda_gym-3.0.6/panda_gym/utils.py` & `panda_gym-3.0.7/panda_gym/utils.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/panda_gym.egg-info/PKG-INFO` & `panda_gym-3.0.7/panda_gym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: panda-gym
-Version: 3.0.6
+Version: 3.0.7
 Summary: Set of robotic environments based on PyBullet physics engine and gymnasium.
 Home-page: https://github.com/qgallouedec/panda-gym
 Author: Quentin GALLOUÉDEC
 Author-email: gallouedec.quentin@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: develop
@@ -94,9 +92,7 @@
   author       = {Gallou{\'e}dec, Quentin and Cazin, Nicolas and Dellandr{\'e}a, Emmanuel and Chen, Liming},
   year         = 2021,
   journal      = {4th Robot Learning Workshop: Self-Supervised and Lifelong Learning at NeurIPS},
 }
 ```
 
 Environments are widely inspired from [OpenAI Fetch environments](https://openai.com/blog/ingredients-for-robotics-research/). 
-
-
```

### Comparing `panda_gym-3.0.6/panda_gym.egg-info/SOURCES.txt` & `panda_gym-3.0.7/panda_gym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.6/setup.py` & `panda_gym-3.0.7/setup.py`

 * *Files identical despite different names*

