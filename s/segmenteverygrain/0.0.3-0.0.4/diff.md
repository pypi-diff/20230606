# Comparing `tmp/segmenteverygrain-0.0.3.tar.gz` & `tmp/segmenteverygrain-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmenteverygrain-0.0.3.tar", last modified: Mon Jun  5 01:12:51 2023, max compression
+gzip compressed data, was "segmenteverygrain-0.0.4.tar", last modified: Tue Jun  6 14:44:34 2023, max compression
```

## Comparing `segmenteverygrain-0.0.3.tar` & `segmenteverygrain-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-05 01:12:51.605831 segmenteverygrain-0.0.3/
--rw-r--r--   0 zoltan     (502) staff       (20)    11350 2023-05-24 19:25:16.000000 segmenteverygrain-0.0.3/LICENSE.txt
--rw-r--r--   0 zoltan     (502) staff       (20)     4020 2023-06-05 01:12:51.605684 segmenteverygrain-0.0.3/PKG-INFO
--rw-r--r--   0 zoltan     (502) staff       (20)     3268 2023-06-05 01:05:16.000000 segmenteverygrain-0.0.3/README.md
--rw-r--r--   0 zoltan     (502) staff       (20)      664 2023-06-05 01:12:13.000000 segmenteverygrain-0.0.3/pyproject.toml
-drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-05 01:12:51.598718 segmenteverygrain-0.0.3/segmenteverygrain/
--rw-r--r--   0 zoltan     (502) staff       (20)       59 2023-05-25 16:54:43.000000 segmenteverygrain-0.0.3/segmenteverygrain/__init__.py
--rw-r--r--   0 zoltan     (502) staff       (20)    31539 2023-06-05 00:55:34.000000 segmenteverygrain-0.0.3/segmenteverygrain/segmenteverygrain.py
-drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-05 01:12:51.605422 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/
--rw-r--r--   0 zoltan     (502) staff       (20)     4020 2023-06-05 01:12:51.000000 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/PKG-INFO
--rw-r--r--   0 zoltan     (502) staff       (20)      318 2023-06-05 01:12:51.000000 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/SOURCES.txt
--rw-r--r--   0 zoltan     (502) staff       (20)        1 2023-06-05 01:12:51.000000 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/dependency_links.txt
--rw-r--r--   0 zoltan     (502) staff       (20)      116 2023-06-05 01:12:51.000000 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/requires.txt
--rw-r--r--   0 zoltan     (502) staff       (20)       18 2023-06-05 01:12:51.000000 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/top_level.txt
--rw-r--r--   0 zoltan     (502) staff       (20)       38 2023-06-05 01:12:51.605887 segmenteverygrain-0.0.3/setup.cfg
--rw-r--r--   0 zoltan     (502) staff       (20)      961 2023-06-05 01:12:17.000000 segmenteverygrain-0.0.3/setup.py
+drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-06 14:44:34.279748 segmenteverygrain-0.0.4/
+-rw-r--r--   0 zoltan     (502) staff       (20)    11350 2023-05-24 19:25:16.000000 segmenteverygrain-0.0.4/LICENSE.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)     4020 2023-06-06 14:44:34.279633 segmenteverygrain-0.0.4/PKG-INFO
+-rw-r--r--   0 zoltan     (502) staff       (20)     3268 2023-06-05 01:05:16.000000 segmenteverygrain-0.0.4/README.md
+-rw-r--r--   0 zoltan     (502) staff       (20)      664 2023-06-06 14:43:07.000000 segmenteverygrain-0.0.4/pyproject.toml
+drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-06 14:44:34.278875 segmenteverygrain-0.0.4/segmenteverygrain/
+-rw-r--r--   0 zoltan     (502) staff       (20)       59 2023-05-25 16:54:43.000000 segmenteverygrain-0.0.4/segmenteverygrain/__init__.py
+-rw-r--r--   0 zoltan     (502) staff       (20)    31890 2023-06-06 01:46:38.000000 segmenteverygrain-0.0.4/segmenteverygrain/segmenteverygrain.py
+drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-06 14:44:34.279476 segmenteverygrain-0.0.4/segmenteverygrain.egg-info/
+-rw-r--r--   0 zoltan     (502) staff       (20)     4020 2023-06-06 14:44:34.000000 segmenteverygrain-0.0.4/segmenteverygrain.egg-info/PKG-INFO
+-rw-r--r--   0 zoltan     (502) staff       (20)      318 2023-06-06 14:44:34.000000 segmenteverygrain-0.0.4/segmenteverygrain.egg-info/SOURCES.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)        1 2023-06-06 14:44:34.000000 segmenteverygrain-0.0.4/segmenteverygrain.egg-info/dependency_links.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)      116 2023-06-06 14:44:34.000000 segmenteverygrain-0.0.4/segmenteverygrain.egg-info/requires.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)       18 2023-06-06 14:44:34.000000 segmenteverygrain-0.0.4/segmenteverygrain.egg-info/top_level.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)       38 2023-06-06 14:44:34.279782 segmenteverygrain-0.0.4/setup.cfg
+-rw-r--r--   0 zoltan     (502) staff       (20)      961 2023-06-06 14:43:01.000000 segmenteverygrain-0.0.4/setup.py
```

### Comparing `segmenteverygrain-0.0.3/LICENSE.txt` & `segmenteverygrain-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `segmenteverygrain-0.0.3/PKG-INFO` & `segmenteverygrain-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmenteverygrain
-Version: 0.0.3
+Version: 0.0.4
 Summary: A SAM-based model for segmenting grains in images of grains
 Home-page: https://github.com/zsylvester/segmenteverygrain
 Author: Zoltan Sylvester
 Author-email: Zoltan Sylvester <zoltan.sylvester@beg.utexas.edu>
 Project-URL: Homepage, https://github.com/zsylvester/segmenteverygrain
 Project-URL: Bug Tracker, https://github.com/zsylvester/segmenteverygrain/issues
 Keywords: sedimentology,geomorphology,grain size,segment anything model
```

### Comparing `segmenteverygrain-0.0.3/README.md` & `segmenteverygrain-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `segmenteverygrain-0.0.3/pyproject.toml` & `segmenteverygrain-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "segmenteverygrain"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Zoltan Sylvester", email="zoltan.sylvester@beg.utexas.edu" },
 ]
 description = "A SAM-based model for segmenting grains in images of grains"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `segmenteverygrain-0.0.3/segmenteverygrain/segmenteverygrain.py` & `segmenteverygrain-0.0.4/segmenteverygrain/segmenteverygrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,26 +408,24 @@
 
 def sam_segmentation(sam, big_im, big_im_pred, coords, labels, min_area):
     predictor = SamPredictor(sam)
     predictor.set_image(big_im)
     fig, ax = plt.subplots(figsize=(15,10))
     ax.imshow(big_im) #, alpha=0.5)
     all_grains = []
-    masks = []
     for i in trange(len(coords[:,0])):
         x = coords[i,0]
         y = coords[i,1]
         sx, sy, mask = one_point_prompt(x, y, ax, big_im, predictor)
         labels_per_mask = len(np.unique(labels[mask]))
         if (labels_per_mask < 10) and (np.mean(big_im_pred[:,:,0][mask]) < 0.7): # skip masks that are mostly background
             poly = Polygon(np.vstack((sx, sy)).T)
             if not poly.is_valid:
                 poly = poly.buffer(0)
             all_grains.append(poly)
-            masks.append(mask)
     ax.clear()
     r = big_im.shape[0]
     c = big_im.shape[1]
     overlapping_polygons, overlap_areas = find_overlapping_polygons(all_grains, min_overlap_area=min_area)
     g = nx.Graph(overlapping_polygons)
     comps = list(nx.connected_components(g))
     connected_grains = set()
@@ -435,15 +433,15 @@
         connected_grains.update(comp)
     new_grains = []
     for i in range(len(all_grains)): # first collect the objects that do not overlap each other
         if i not in connected_grains and all_grains[i].area > min_area:
             if not all_grains[i].is_valid:
                 all_grains[i] = all_grains[i].buffer(0)
             new_grains.append(all_grains[i])
-    for j in trange(len(comps)): # second deal with the overlapping objects, one connected component at a time
+    for j in trange(len(comps)): # second: deal with the overlapping objects, one connected component at a time
         polygons = [] # polygons in the connected component
         for i in comps[j]:
             polygons.append(all_grains[i])
         most_similar_polygon = pick_most_similar_polygon(polygons)
         if most_similar_polygon.area > min_area:
             new_grains.append(most_similar_polygon)
     all_grains = new_grains # replace original list of polygons
@@ -511,23 +509,27 @@
             all_touched=False,
             default_value=1,
             dtype=None,
         )
         mask_all[mask == 1] = 1
         mask_all[boundary_mask == 1] = 2
         labels[(mask==1) & (labels==0)] = i+1
+    labels = labels.astype('int')
     ax.imshow(big_im)
     plot_image_w_colorful_grains(big_im, all_grains, ax, cmap='Paired')
     plot_grain_axes_and_centroids(all_grains, labels, ax, linewidth=1, markersize=10)
     plt.xticks([])
     plt.yticks([])
     plt.xlim([0, np.shape(big_im)[1]])
     plt.ylim([np.shape(big_im)[0], 0])
     plt.tight_layout()
-    return all_grains, labels, mask_all, fig, ax
+    props = regionprops_table(labels, intensity_image = big_im, properties=('label', 'area', 'centroid', 'major_axis_length', 'minor_axis_length', 
+                                                                                    'orientation', 'perimeter', 'max_intensity', 'mean_intensity', 'min_intensity'))
+    grain_data = pd.DataFrame(props)
+    return all_grains, labels, mask_all, grain_data, fig, ax
 
 def load_and_preprocess(image_path, mask_path):
     # Load images
     image = tf.io.read_file(image_path)
     image = tf.image.decode_png(image, channels=3)
     # Load mask and one-hot encode it
     mask = tf.io.read_file(mask_path)
```

### Comparing `segmenteverygrain-0.0.3/segmenteverygrain.egg-info/PKG-INFO` & `segmenteverygrain-0.0.4/segmenteverygrain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmenteverygrain
-Version: 0.0.3
+Version: 0.0.4
 Summary: A SAM-based model for segmenting grains in images of grains
 Home-page: https://github.com/zsylvester/segmenteverygrain
 Author: Zoltan Sylvester
 Author-email: Zoltan Sylvester <zoltan.sylvester@beg.utexas.edu>
 Project-URL: Homepage, https://github.com/zsylvester/segmenteverygrain
 Project-URL: Bug Tracker, https://github.com/zsylvester/segmenteverygrain/issues
 Keywords: sedimentology,geomorphology,grain size,segment anything model
```

