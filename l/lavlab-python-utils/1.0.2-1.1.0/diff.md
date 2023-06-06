# Comparing `tmp/lavlab-python-utils-1.0.2.tar.gz` & `tmp/lavlab-python-utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavlab-python-utils-1.0.2.tar", last modified: Wed May 31 19:36:31 2023, max compression
+gzip compressed data, was "lavlab-python-utils-1.1.0.tar", last modified: Tue Jun  6 11:46:16 2023, max compression
```

## Comparing `lavlab-python-utils-1.0.2.tar` & `lavlab-python-utils-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:36:31.481476 lavlab-python-utils-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 19:36:31.481476 lavlab-python-utils-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:36:31.477476 lavlab-python-utils-1.0.2/lavlab/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/lavlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/lavlab/omero_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    26962 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/lavlab/omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/lavlab/python_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:36:31.481476 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 19:36:31.000000 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-31 19:36:31.000000 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:36:31.000000 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-31 19:36:31.000000 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 19:36:31.000000 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:36:31.481476 lavlab-python-utils-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/src/lavlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/src/lavlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/src/lavlab/omero_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27776 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/src/lavlab/omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/src/lavlab/python_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-06 11:46:16.000000 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-06 11:46:16.000000 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:46:16.000000 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 11:46:16.000000 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 11:46:16.000000 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/test/test_omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/test/test_python_utils.py
```

### Comparing `lavlab-python-utils-1.0.2/lavlab/omero_asyncio.py` & `lavlab-python-utils-1.1.0/src/lavlab/omero_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-"""This module can be tricky to work with and requires decent python experience. Primarily a dependency for omero_util"""
+"""Primarily a dependency for omero_util. Lab users can safely ignore."""
 # written by manics https://github.com/microscopepony/omero-asyncio/commits?author=manics
 import asyncio
 from functools import partial, update_wrapper
 import logging
 import Ice
 import omero.clients
```

### Comparing `lavlab-python-utils-1.0.2/lavlab/omero_util.py` & `lavlab-python-utils-1.1.0/src/lavlab/omero_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Helper functions that handle high-level operations and translating asynchronous requests for easy development.
 """
 import os
 import asyncio
 import tempfile
 
 import numpy as np
+from PIL import Image
 from skimage import draw
 
 from collections.abc import AsyncGenerator
 
 from omero.gateway import _BlitzGateway, ImageWrapper, FileAnnotationWrapper, ShapeWrapper
 import omero.model.enums as omero_enums
 from omero.rtypes import rint, rstring
@@ -18,15 +19,15 @@
 from omero_model_PolygonI import PolygonI
 from omero_model_EllipseI import EllipseI
 from omero_model_PolygonI import PolygonI
 from omero_model_RectangleI import RectangleI
 from omero_model_FileAnnotationI import FileAnnotationI
 
 from lavlab import omero_asyncio
-from lavlab.python_util import chunkify, merge_async_iters, interlace_lists, lookup_filetype_by_name, FILETYPE_DICTIONARY, save_image_binary, rgba_to_int, resize_image_array
+from lavlab.python_util import chunkify, merge_async_iters, interlace_lists, lookup_filetype_by_name, FILETYPE_DICTIONARY, rgba_to_uint, uint_to_rgba
 
 PARALLEL_STORE_COUNT=4
 """Number of pixel stores to be created for an image."""
 
 OMERO_DICTIONARY = {
     # TODO add real pixeltype support
     "PIXEL_TYPES": {
@@ -102,15 +103,15 @@
     what resolution level are these tiles on, default highest res
 rps_bypass: default: True
     passthrough for rawPixelsStore.setPixelsId(pixels.id, rps_bypass)
 
 Returns
 -------
 Async tile generator
-    python async generator that yields omero tiles as numpy arrays
+    Python async generator that yields omero tiles as numpy arrays with the tile's coordinates
 
 Examples
 --------
 ```
 import asyncio
 async def work(img, tiles, res_lvl, dims):
     bin = np.zeros(dims, np.uint8)
@@ -146,51 +147,50 @@
 
 
     # force async client
     session =  omero_asyncio.AsyncSession(img._conn.c.sf)
 
     # create parallel raw pixels stores
     jobs=[]
-    for chunk in chunkify(tiles, int(len(tiles)/PARALLEL_STORE_COUNT)+1):
+    for chunk in chunkify(tiles, PARALLEL_STORE_COUNT):
         jobs.append(work(img.getPrimaryPixels().getId(), chunk, resLvl))
     return merge_async_iters(*jobs)
 
-def getDownsampledYXDimensions(img: ImageWrapper, downsample_factor: int) -> tuple[int,int]:
+def getDownsampledXYDimensions(img: ImageWrapper, downsample_factor: int) -> tuple[float,float]:
     """
-Returns yx (rows,columns) dimensions of given image at the downsample.
+Returns XY (rows,columns) dimensions of given image at the downsample.
 
 Parameters
 ----------
 img: omero.gateway.ImageWrapper
     Omero Image object from conn.getObjects().
 downsample_factor: int
     Takes every nth pixel from the base resolution.
 
 Returns
 -------
-int
-    img.getSizeY() / downsample_factor
-int 
+float 
     img.getSizeX() / downsample_factor
+float
+    img.getSizeY() / downsample_factor
 """
-    return (int(img.getSizeY() / downsample_factor),
-            int(img.getSizeX() / downsample_factor))
+    return (float(img.getSizeX() / downsample_factor), float(img.getSizeY() / downsample_factor))
 
 def getDownsampleFromDimensions(base_shape:tuple[int,...], sample_shape:tuple[int,...]) -> tuple[float,...]:
     """
 Essentially an alias for np.divide().
 
 Finds the ratio between a base array shape and a sample array shape by dividing each axis.
 
 Parameters
 ----------
 base_shape: tuple(int)*x
-    Shape of the larger image. (base_nparray.shape)
+    Shape of the larger image. (Image.size / base_nparray.shape)
 sample_shape: tuple(int)*x
-    Shape of the smaller image. (sample_nparray.shape)
+    Shape of the smaller image. (Image.size / sample_nparray.shape)
 
 Raises
 ------
 AssertionError
     Asserts that the input shapes have the same amount of axes
 
 Returns
@@ -208,15 +208,15 @@
 Finds the closest resolution to desired resolution.
 
 Parameters
 ----------
 img: omero.gateway.ImageWrapper or RawPixelsStore
     Omero Image object from conn.getObjects() or initialized rps
 dim: tuple[int, int]
-    tuple containing desired y,x dimensions. 
+    tuple containing desired x,y dimensions. 
 
 Returns
 -------
 int
     resolution level to be used in rps.setResolution() 
 tuple[int,int,int,int]
     height, width, tilesize_y, tilesize_x of closest resolution
@@ -232,127 +232,166 @@
     # get res info
     lvls = rps.getResolutionLevels()
     resolutions = rps.getResolutionDescriptions()
 
     # search for closest res
     for i in range(lvls) :
         res=resolutions[i]
-        currDif=(res.sizeX-dim[1],res.sizeY-dim[0])
+        currDif=(res.sizeX-dim[0],res.sizeY-dim[1])
         # if this resolution's difference is negative in either axis, the previous resolution is closest
         if currDif[0] < 0 or currDif[1] < 0:
 
             rps.setResolutionLevel(lvls-i)
             tileSize=rps.getTileSize()
 
             if close_rps is True: rps.close()
 
-            return (lvls-i, (resolutions[i-1].sizeY,resolutions[i-1].sizeX,
-                             tileSize[1], tileSize[0]))
+            return (lvls-i, (resolutions[i-1].sizeX,resolutions[i-1].sizeY,
+                             tileSize[0], tileSize[1]))
+    # else smaller than smallest resolution, return smallest resolution
+    rps.setResolutionLevel(lvls)
+    tileSize=rps.getTileSize()
+    return lvls, (resolutions[i-1].sizeX,resolutions[i-1].sizeY,
+                             tileSize[0], tileSize[1])
         
 
-def getImageAtResolution(img: ImageWrapper, yx_dim: tuple[int,int], channels:list[int]=None) -> np.ndarray:
+
+def getChannelsAtResolution(img: ImageWrapper, xy_dim: tuple[int,int], channels:list[int]=None) -> Image.Image:
     """
 Gathers tiles and scales down to desired resolution.
 
 Warns
 -------
 Out of Memory issues ahead! Request a reasonable resolution!
 
 Parameters
 ----------
 img: omero.gateway.ImageWrapper
     Omero Image object from conn.getObjects().
-yx_dim: tuple(y,x)
-    Tuple of desired dimensions (row, col)
+xy_dim: tuple(x,y)
+    Tuple of desired dimensions (x,y)
 channels: tuple(int,...), default: all channels
     Array of channels to gather.
     To grab only blue channel: channels=(2) 
 
 Returns
 -------
-np.ndarray 
-    Array of rbg values for given img.
+PIL.Image.Image 
+    Python Image Object
+    """
+    async def work(img, xy, channels):
+        res_lvl, xy_info = getClosestResolutionLevel(img, xy)
+        images = []
+        for channel in channels:
+            tiles = createTileList2D(0,channel,0,*xy_info)
+            arr = np.zeros((xy_info[1], xy_info[0]), np.uint8)
+            async for tile, (z,c,t,coord) in getTiles(img,tiles,res_lvl):
+                arr [
+                    coord[1]:coord[1]+coord[3],
+                    coord[0]:coord[0]+coord[2], 
+                    c ] = tile 
+            image = Image.fromarray(arr)
+            if image.size != xy:
+                del arr # just to be safe
+                image = image.resize(xy)
+            images.append(image)
+        return images
+    
+    return asyncio.run(work(img, xy_dim, channels))
+
+def getImageAtResolution(img: ImageWrapper, xy_dim: tuple[int,int]) -> Image.Image:
+    """
+Gathers tiles of full rgb image and scales down to desired resolution.
+
+Warns
+-------
+Out of Memory issues ahead! Request a reasonable resolution!
+
+Parameters
+----------
+img: omero.gateway.ImageWrapper
+    Omero Image object from conn.getObjects().
+xy_dim: tuple(x,y)
+    Tuple of desired dimensions (x,y)
+
+Returns
+-------
+PIL.Image.Image 
+    Python Image Object
     """
-    async def work(img, tiles, res_lvl, current_dims, des_shape):
-        bin = np.zeros(current_dims, np.uint8)
+    async def work(img, xy):
+        res_lvl, xy_info = getClosestResolutionLevel(img, xy)
+        tiles = createFullTileList([0,],range(3),[0,], xy_info[0],xy_info[1], xy_info[2:])# rgb tile list
+
+        arr = np.zeros((xy_info[1], xy_info[0], 3), np.uint8)
         async for tile, (z,c,t,coord) in getTiles(img,tiles,res_lvl):
-            bin [
+            arr [
                 coord[1]:coord[1]+coord[3],
                 coord[0]:coord[0]+coord[2], 
                 c ] = tile 
-        if bin.shape != des_shape:
-            bin = resize_image_array(bin,(yx_dim[1],yx_dim[0]))
-        return bin
-    
-    res_lvl, dims = getClosestResolutionLevel(img, yx_dim)
-
-    if channels is None:
-        channels = range(img.getSizeC())
+            
+        image = Image.fromarray(arr)
+        if image.size != xy:
+            del arr # just to be safe
+            image = image.resize(xy)
+            
+        return image
     
-    if len(channels) > 1: 
-        des_shape = (*yx_dim, len(channels))
-        current_dims = (dims[0],dims[1],len(channels))
-    else: 
-        des_shape = yx_dim
-        current_dims = dims[:1]
-        
-    tiles = createFullTileList([0,],channels,[0,],dims[1],dims[0],(dims[3],dims[2]))
-    return asyncio.run(work(img, tiles, res_lvl, current_dims, des_shape))
+    return asyncio.run(work(img, xy_dim))
 
 
-def getLargeRecon(img:ImageWrapper, downsample_factor, workdir='./', save_format="JPEG"):
+def getLargeRecon(img:ImageWrapper, downsample_factor:int = 10, workdir='./', skip_upload=False):
     """
 Checks OMERO for a pregenerated large recon, if none are found, it will generate and upload one.
 
 Parameters
 ----------
 img: omero.gateway.ImageWrapper
     Omero Image object from conn.getObjects().
-downsample_factor: int
+downsample_factor: int, Default: 10
     Which large recon size to get.
 
 Returns
 -------
 omero.gateway.AnnotationWrapper
     remote large recon object
 str
     local path to large recon
     """
-    NS = "LargeRecon."+str(downsample_factor)
-    EXT, MIME = OMERO_DICTIONARY["SKIMAGE_FORMATS"][save_format]
-    recon = img.getAnnotation(NS)
+    namespace = "LargeRecon."+str(downsample_factor)
+    format = OMERO_DICTIONARY["SKIMAGE_FORMATS"]["JPEG"]
+    f_ext = format["EXT"]
+    mimetype = format["MIME"]
+    recon = img.getAnnotation(namespace)
     if recon is None:
         name = img.getName()
         sizeX = img.getSizeX()
         sizeY = img.getSizeY()
 
         print(f"No large recon {downsample_factor} for img: {name} Generating...")
 
-        yx_dim=getDownsampledYXDimensions(img, downsample_factor)
-        reconPath = workdir + os.sep + f"LR{downsample_factor}_{name.replace('.ome.tiff',EXT)}"
-        recon = img.getAnnotation(NS)
+        xy_dim = getDownsampledXYDimensions(img, downsample_factor)
+        reconPath = workdir + os.sep + f"LR{downsample_factor}_{name.replace('.ome.tiff',f_ext)}"
+        recon = img.getAnnotation(namespace)
         
         if recon is None: 
-                print(f"Downsampling: {name} from {(sizeY,sizeX)} to {yx_dim}")
-                reconBin = getImageAtResolution(img, yx_dim)
-                
-                if save_format == 'JPEG': 
-                    jpeg=True 
-                else: 
-                    jpeg=False
-
-                save_image_binary(reconPath,reconBin, jpeg)
-                
-                print("Downsampling Complete! Uploading to OMERO...")
-                recon = img._conn.createFileAnnfromLocalFile(reconPath, mimetype=MIME, ns=NS)
-                img.linkAnnotation(recon)
+                print(f"Downsampling: {name} from {(sizeX,sizeY)} to {xy_dim}")
+                recon_img = getImageAtResolution(img, xy_dim)
+                recon_img.filename = reconPath
+                recon_img.save(reconPath)
+
+                if skip_upload is False:
+                    print("Downsampling Complete! Uploading to OMERO...")
+                    recon = img._conn.createFileAnnfromLocalFile(reconPath, mimetype=mimetype, ns=namespace)
+                    img.linkAnnotation(recon)
         else:
             reconPath = downloadFileAnnotation(recon, workdir)
+            recon_img = Image.open(reconPath)
 
-    return recon, reconPath
+    return recon, recon_img
 
 #
 ## TILES
 #
 def createTileList2D(z:int, c:int, t:int, size_x:int, size_y:int,
         tile_size:tuple[int,int]) -> list[tuple[int,int,int,tuple[int,int,int,int]]]:
     """
@@ -497,15 +536,15 @@
     return createFullTileList(z_indexes,channels,timepoints,width,height,tile_size, rgb)
 
 
 #
 ## ROIS
 #
 def getShapesAsPoints(img: ImageWrapper, point_downsample=4, img_downsample=1, 
-                      roi_service=None) -> list[tuple[int, tuple[int,int,int], tuple[np.ndarray, np.ndarray]]]:
+                      roi_service=None) -> list[tuple[int, tuple[int,int,int], list[tuple[float, float]]]]:
     """
 Gathers Rectangles, Polygons, and Ellipses as a tuple containing the shapeId, its rgb val, and a tuple of yx points of its bounds.
 
 Parameters
 ----------
 img: omero.gateway.ImageWrapper
     Omero Image object from conn.getObjects().
@@ -514,15 +553,15 @@
 img_downsample: int, Default: 1
     How much to scale roi points.
 roi_service: omero.RoiService, optional
     Allows roiservice passthrough for performance.
 
 Returns
 -------
-returns: list[shape.id, (r,g,b), (row_points, column_points))]
+returns: list[ shape.id, (r,g,b), list[tuple(x,y)] ]
     list of tuples containing a shape's id, rgb value, and a tuple of row and column points
     """
     if roi_service is None:
         roi_service=img._conn.getRoiService()
         close_roi=True
 
     sizeX = img.getSizeX() / img_downsample
@@ -531,102 +570,106 @@
 
     result = roi_service.findByImage(img.getId(), None)
 
     shapes=[]
     for roi in result.rois:
         points= None
         for shape in roi.copyShapes():
+            
             if type(shape) == RectangleI:
                 x = float(shape.getX().getValue()) / img_downsample
                 y = float(shape.getY().getValue()) / img_downsample
                 w = float(shape.getWidth().getValue()) / img_downsample
                 h = float(shape.getHeight().getValue()) / img_downsample
+                # points = [(x, y),(x+w, y), (x+w, y+h), (x, y+h), (x, y)]
                 points = draw.rectangle_perimeter((y,x),(y+h,x+w), shape=yx_shape)
+                points = [(points[1][i], points[0][i]) for i in range(0, len(points[0]))]
 
             if type(shape) == EllipseI:
                 points = draw.ellipse_perimeter(float(shape._y._val / img_downsample),float(shape._x._val / img_downsample),
                             float(shape._radiusY._val / img_downsample),float(shape._radiusX._val / img_downsample),
                             shape=yx_shape)
+                points = [(points[1][i], points[0][i]) for i in range(0, len(points[0]))]
+                
             
             if type(shape) == PolygonI:
                 pointStrArr = shape.getPoints()._val.split(" ")
 
-                y = []
-                x = []
+                xy = []
                 for i in range(0, len(pointStrArr)):
                     coordList=pointStrArr[i].split(",")
-                    y.append(float(coordList[1]) / img_downsample)
-                    x.append(float(coordList[0]) / img_downsample)
-
-                points = draw.polygon_perimeter(y, x, shape=yx_shape)
+                    xy.append(float(coordList[0]) / img_downsample,
+                        float(coordList[1]) / img_downsample)
+                if xy:
+                    points = xy
 
             if points is not None:
                 color_val = shape.getStrokeColor()._val
-                masks = OMERO_DICTIONARY["BYTE_MASKS"][np.uint8]
-                red = (color_val & masks["RED"]) >> 24  
-                green = (color_val & masks["GREEN"]) >> 16  
-                blue = (color_val & masks["BLUE"]) >> 8 
+                rgb = uint_to_rgba(color_val)[:2] # ignore alpha value for computation
                 points=(points[0][::point_downsample], points[1][::point_downsample])
                 
-                shapes.append((shape.getId()._val, (red,green,blue), points))
+                shapes.append((shape.getId()._val, rgb, points))
 
     if not shapes : # if no shapes in shapes return none
         return None
     
     if close_roi: roi_service.close()
 
     # make sure is in correct order
     return sorted(shapes)
 
 
-def createPolygon(contour:tuple[np.ndarray, np.ndarray], x_offset=0, y_offset=0, z=None, t=None, comment=None, rgb=(0,0,0)) -> PolygonI:
+def createPolygon(points:list[tuple[float, float]], stride=1, x_offset=0, y_offset=0, z=None, t=None, comment=None, rgb=(0,0,0)) -> PolygonI:
     """ 
 Creates a local omero polygon obj from a list of points, and parameters.
+
+Notes
+-----
+Remember to scale points to full image resolution!
     
 Parameters
 ----------
-contour: tuple[rows, cols]
-    Expects contour as outputed by skimage.measure.find_contours
+points: list[tuple[int,int]]
+    List of xy coordinates defining the polygon contour
+stride: int, Default:1
+    Downsample polygon point quantity.
 x_offset: int, Default: 0
     Inherited from where I ripped this code. Lets you shift coords I guess.
 y_offset: int, Default: 0
     Inherited from where I ripped this code. Lets you shift coords I guess.
 z: int, optional
     Allows polygon to exist in a specific z_index for multi dimensional ROIs.
 t: int, optional
     Allows polygon to exist in a specific timepoint for multi dimensional ROIs.
 comment: str, optional
     Description of polygon, recommended to use to keep track of which programs generate which shapes.
 rgb: tuple[int,int,int], Default: (0,0,0) 
-    What color contour should this polygon's contour be.
+    What color should this polygon's outline be.
     
 Returns
 -------
 omero_model_PolygonI.PolygonI
     Local Omero Polygon object, likely needs to linked to an ROI
     """
-    stride = 64
     coords = []
-    # points in contour are adjacent pixels, which is too verbose
-    # take every nth point
-    for count, xy in enumerate(contour):
+    for count, xy in enumerate(points):
         if count%stride == 0:
             coords.append(xy)
     if len(coords) < 2:
         return
-    points = ["%s,%s" % (xy[1] + x_offset, xy[0] + y_offset) for xy in coords]
+    points = ["%s,%s" % (xy[0] + x_offset, xy[1] + y_offset) for xy in coords]
     points = ", ".join(points)
     polygon = PolygonI()
     if z is not None:
         polygon.theZ = rint(z)
     if t is not None:
         polygon.theT = rint(t)
     if comment is not None:
         polygon.setTextValue(rstring(comment))
-    polygon.strokeColor = rint(rgba_to_int(*rgb))
+    polygon.strokeColor = rint(rgba_to_uint(*rgb))
     polygon.points = rstring(points)
     return polygon
 
 def createRoi(img: ImageWrapper, shapes: list[ShapeWrapper]):
     """
 Creates an omero RoiI object for an image from an array of shapes.
 
@@ -648,40 +691,14 @@
     # use the omero.model.ImageI that underlies the 'image' wrapper
     roi.setImage(img._obj)
     for shape in shapes:
         roi.addShape(shape)
     return roi
 
 
-def drawShapes(input_img: np.ndarray, shape_points:tuple[int,tuple[int,int,int],tuple[np.ndarray, np.ndarray]]) -> None:
-    """
-Draws a list of shape points onto the input numpy array.
-
-Warns
--------
-NO SAFETY CHECKS! MAKE SURE input_img AND shape_points ARE FOR THE SAME DOWNSAMPLE FACTOR!
-
-Parameters
-----------
-input_img: np.ndarray
-    3 channel numpy array
-shape_points: tuple(int, tuple(int,int,int), tuple(row, col))
-    output from getShapesAsPoints
-
-Returns
--------
-``None``
-    """
-    for id, rgb, points in shape_points:
-        rr,cc = draw.polygon(*points)
-        input_img[rr,cc]=rgb
-
-
-
-
 # TODO SLOW AND broken for rgb = 0,0,0 annotations
 # def getShapesAsMasks(img: ImageWrapper, downsample: int, bool_mask=True, 
 #                      point_downsample=4, roi_service=None) -> list[np.ndarray]:
 #     """
 # Gathers Rectangles, Polygons, and Ellipses as masks for the image at the given downsampling
 # Converts rectangles and ellipses into polygons (4 rectangle points into an array of points on the outline)
 #     """
```

### Comparing `lavlab-python-utils-1.0.2/pyproject.toml` & `lavlab-python-utils-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lavlab-python-utils"
 description = "LaViolette Lab utility package"
-version = "1.0.2"
+version = "1.1.0"
 
 authors = [
   { name="Michael Barrett", email="mjbarrett@mcw.edu" },
 ]
 
 readme = "README.rst"
 classifiers = [
@@ -25,8 +25,9 @@
 docs = ["sphinx>=6.2.1","docutils >= 0.18.1"]
 
 [project.urls]
 "Homepage" = "https://github.com/laviolette-lab/lavlab-python-utils"
 "Bug Tracker" = "https://github.com/laviolette-lab/lavlab-python-utils/issues"
 
 [build-system]
+build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
```

