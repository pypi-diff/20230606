# Comparing `tmp/pco-2.0.0.tar.gz` & `tmp/pco-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pco-2.0.0.tar", last modified: Fri May 12 14:23:03 2023, max compression
+gzip compressed data, was "pco-2.0.1.tar", last modified: Mon Jun  5 09:56:00 2023, max compression
```

## Comparing `pco-2.0.0.tar` & `pco-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:23:03.160584 pco-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-12 07:13:25.000000 pco-2.0.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-05-12 07:13:25.000000 pco-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12964 2023-05-12 14:23:03.160584 pco-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11547 2023-05-12 07:13:25.000000 pco-2.0.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)   104867 2023-05-12 07:13:26.000000 pco-2.0.0/license.pdf
--rw-rw-rw-   0 root         (0) root         (0)   105021 2023-05-12 07:13:26.000000 pco-2.0.0/license_3rdParty.pdf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:23:03.152584 pco-2.0.0/pco/
--rw-r--r--   0 root         (0) root         (0)     1344 2023-05-12 14:23:02.000000 pco-2.0.0/pco/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-05-12 07:13:25.000000 pco-2.0.0/pco/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    59049 2023-05-12 07:13:25.000000 pco-2.0.0/pco/camera.py
--rw-rw-rw-   0 root         (0) root         (0)    48437 2023-05-12 07:13:25.000000 pco-2.0.0/pco/convert.py
--rw-rw-rw-   0 root         (0) root         (0)    12517 2023-05-12 07:13:25.000000 pco-2.0.0/pco/flim.py
--rw-r--r--   0 root         (0) root         (0)   104867 2023-05-12 14:23:02.000000 pco-2.0.0/pco/license.pdf
--rw-r--r--   0 root         (0) root         (0)   105021 2023-05-12 14:23:02.000000 pco-2.0.0/pco/license_3rdParty.pdf
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-05-12 07:13:25.000000 pco-2.0.0/pco/logging.py
--rw-rw-rw-   0 root         (0) root         (0)    38376 2023-05-12 07:13:25.000000 pco-2.0.0/pco/recorder.py
--rw-rw-rw-   0 root         (0) root         (0)   283652 2023-05-12 07:13:25.000000 pco-2.0.0/pco/sdk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:23:03.156584 pco-2.0.0/pco.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12964 2023-05-12 14:23:03.000000 pco-2.0.0/pco.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-12 14:23:03.000000 pco-2.0.0/pco.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:23:03.000000 pco-2.0.0/pco.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-12 14:23:03.000000 pco-2.0.0/pco.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-12 14:23:03.000000 pco-2.0.0/pco.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-12 14:23:03.160584 pco-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5215 2023-05-12 07:13:25.000000 pco-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:56:00.496728 pco-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-06-05 07:07:36.000000 pco-2.0.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-05 07:07:36.000000 pco-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9286 2023-06-05 09:56:00.496728 pco-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7869 2023-06-05 07:07:36.000000 pco-2.0.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)   104867 2023-06-05 07:07:37.000000 pco-2.0.1/license.pdf
+-rw-rw-rw-   0 root         (0) root         (0)   105021 2023-06-05 07:07:37.000000 pco-2.0.1/license_3rdParty.pdf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:56:00.484728 pco-2.0.1/pco/
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-06-05 09:55:59.000000 pco-2.0.1/pco/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-05 07:07:36.000000 pco-2.0.1/pco/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    59380 2023-06-05 07:07:36.000000 pco-2.0.1/pco/camera.py
+-rw-rw-rw-   0 root         (0) root         (0)    48437 2023-06-05 07:07:36.000000 pco-2.0.1/pco/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)    12517 2023-06-05 07:07:36.000000 pco-2.0.1/pco/flim.py
+-rw-r--r--   0 root         (0) root         (0)   104867 2023-06-05 09:55:59.000000 pco-2.0.1/pco/license.pdf
+-rw-r--r--   0 root         (0) root         (0)   105021 2023-06-05 09:55:59.000000 pco-2.0.1/pco/license_3rdParty.pdf
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-06-05 07:07:36.000000 pco-2.0.1/pco/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)    38617 2023-06-05 07:07:36.000000 pco-2.0.1/pco/recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)   283652 2023-06-05 07:07:36.000000 pco-2.0.1/pco/sdk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:56:00.496728 pco-2.0.1/pco.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9286 2023-06-05 09:56:00.000000 pco-2.0.1/pco.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-05 09:56:00.000000 pco-2.0.1/pco.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 09:56:00.000000 pco-2.0.1/pco.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-05 09:56:00.000000 pco-2.0.1/pco.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-05 09:56:00.000000 pco-2.0.1/pco.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-05 09:56:00.496728 pco-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5870 2023-06-05 07:49:09.000000 pco-2.0.1/setup.py
```

### Comparing `pco-2.0.0/LICENSE.txt` & `pco-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pco-2.0.0/README.rst` & `pco-2.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,401 +1,277 @@
+Metadata-Version: 2.1
+Name: pco
+Version: 2.0.1
+Summary: This class provides methods for using pco cameras.
+Home-page: https://www.excelitas.com/de/product/pco-software-development-kits/
+Author: Excelitas PCO GmbH
+Author-email: support.pco@excelitas.com
+License: MIT
+Keywords: pco,camera,flim,scmos,microscopy
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Microsoft :: Windows :: Windows 7
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
 
 .. image:: https://www.pco.de/fileadmin/user_upload/company/pco_logo.png
    :width: 100pt
 
 |PyPI-Versions| |LICENCE| |Platform| |PyPI-Status|
 
-The Python package **pco** offers all functions for working with pco cameras that are based
-on the current SDK. All shared libraries for the communication with the
-camera and subsequent image processing are included.
-
-- Easy to use camera class
-- Powerful API to `pco.software development kit <https://www.pco.de/fileadmin/user_upload/pco-manuals/pco.sdk_manual.pdf>`_
-- Image recording and processing with `pco.recorder <https://www.pco.de/fileadmin/fileadmin/user_upload/pco-manuals/pco.recorder_manual.pdf>`_
+The Python package **pco** is a powerful and easy to use high level Software Development Kit (SDK)
+for working with PCO cameras. It contains everything needed for camera setup, image acquistion,
+readout and color conversion.
+
+The high-level class architecture makes it very easy to integrate PCO cameras into your own
+software, while still having access to the underlying pco.sdk and pco.recorder interface for a
+detailed control of all possible functionalities.
+
+- **Documentation**: `Manual <https://www.pco.de/fileadmin/user_upload/pco-manuals/MA_PCOPYTHON.pdf>`_
+- **Website**: https://www.excelitas.com/de/product-category/pco
+- **Support**: support.pco@excelitas.com
 
 Installation
 ============
 Install from pypi (recommended)::
 
     $ pip install pco
 
 Basic Usage
 ===========
 .. code-block:: python
 
-    import pco
     import matplotlib.pyplot as plt
+    import pco
 
     with pco.Camera() as cam:
 
-        cam.record()
+        cam.record(mode="sequence")
         image, meta = cam.image()
 
         plt.imshow(image, cmap='gray')
         plt.show()
 
 .. image:: https://www.pco.de/fileadmin/user_upload/company/screen.png
 
-Logging
-=======
-
-Logging is implemented according to the python logging package (https://docs.python.org/3/library/logging.html).
-Supported logging levels are:
-- `ERROR`
-- `WARNING`
-- `INFO`
-- `DEBUG`
-
-
-.. code-block:: python
-
-    logger = logging.getLogger("pco")
-    logger.setLevel(logging.INFO)
-    logger.addHandler(pco.stream_handler)
-
-
-
-.. code-block:: python
-
-    ...
-    [][sdk] get_camera_type: OK.
-    ...
-    [2019-11-25 15:54:15.317855 / 0.016 s] [][sdk] get_camera_type: OK.
-
-
-Documentation
-=============
-
-The pco.Camera class offers the following methods:
-
-- ``__init()__`` Opens and initializes a camera with its default configuration
-- ``__exit()__`` Closes the camera and cleans up everything (e.g. end of with-statement)
-- ``default_configuration()`` Set default configuration to the camera
-- `record()`_ Initialize and start the recording of images
-- `stop()`_ Stop the current recording
-- `close()`_ Closes the camera and cleans up everything
-- `wait_for_first_image()`_ Wait until the first image has been recorded
-- `wait_for_new_image()`_ Wait until a new image has been recorded
-- ``get_convert_control()`` Get current color convert settings
-- ``set_convert_control()`` Set new color convert settings
-- ``load_lut()`` Set the lut file for the convert control setting
-- ``adapt_white_balance()`` Do a white-balance according to a transferred image
-- `image()`_ Read a recorded image as numpy array
-- `images()`_ Read a series of recorded images as a list of numpy arrays.
-- `image_average()`_ Read an averaged image (averaged over all recorded images) as numpy array.
-
-The pco.Camera class has the following properties:
-
-- ``camera_name`` gets the camera name
-- ``camera_serial`` gets the serial number of the camera
-- ``is_recording`` gets a flag to indicate if the camera is currently recording
-- ``is_color`` gets a flag to indicate if the camera is a color camera
-- ``recorded_image_count`` gets the number of currently recorded images
-- ``configuration`` gets/sets the camera configuration
-- ``description`` gets the (static) camera description parameters
-- ``exposure_time`` gets/sets the exposure time (in seconds)
-- ``delay_time`` gets/sets the delay time (in seconds)
-
-The pco.Camera class holds the following objects:
-
-- `sdk`_ offers direct access to all underlying functions of the pco.sdk.
-- `rec`_ offers direct access to all underlying functions of the pco.recorder.
-- `conv`_ offers direct access to all underlying functions of the pco.convert according to the selected data_format.
-
-.. ---------------------------------------------------------------------------
-
-record()
---------
-
-Creates, configures and starts a new recorder instance.
-
-.. code-block:: python
-
-    def record(self, number_of_images=1, mode='sequence', file_path=None):
-
-- ``number_of_images`` sets the number of images allocated in the driver. The RAM of the PC is limiting the maximum value.
-
-- ``mode`` sets the type of recorder.
+Recorder Modes
+==============
+Depending on your workflow you can choose between different recording modes. 
+
+Some modes are blocking, i.e. the ``record()`` function waits until recording is finished, some are non-blocking.
+Some of them are storing the images in memory, the others directly as file(s) on the disk.
+However, for the recorder modes which store the images as files,
+accessing the recorded images is identical with the modes which store the images in memory.
 
 .. list-table:: record modes
   :widths: 20 10 10 60
   :header-rows: 1
 
   * - Mode
     - Storage
     - Blocking
     - Description
   
   * - ``sequence``
     - Memory
     - yes
-    - Record a sequence of images
+    - Record a sequence of images.
   
   * - ``sequence non blocking``
     - Memory
     - no 
-    - Record a sequence of images, do not wait until record is finished
+    - Record a sequence of images, do not wait until record is finished.
   
   * - ``ring buffer``
     - Memory
     - no 
-    - Continuously record images in a ringbuffer, once the buffer is full, old images are overwritten
+    - Continuously record images in a ringbuffer, once the buffer is full, old images are overwritten.
   
   * - ``fifo``
     - Memory
     - no 
-    - Record images in fifo mode, i.e. you will always read images sequentially and once the buffer is full, recording will pause until older images have been read
+    - Record images in fifo mode, i.e. you will always read images sequentially and once the buffer is full, recording will pause until older images have been read.
   
   * - ``sequence dpcore``
     - Memory
     - yes
-    - Same as ``sequence``, but with DotPhoton preparation enabled
+    - Same as ``sequence``, but with DotPhoton preparation enabled.
   
   * - ``sequence non blocking dpcore``
     - Memory
     - no 
-    - Same as ``sequence_non_blocking``, but with DotPhoton preparation enabled
+    - Same as ``sequence_non_blocking``, but with DotPhoton preparation enabled.
   
   * - ``ring buffer dpcore``
     - Memory
     - no 
-    - Same as ``ring_buffer``, but with DotPhoton preparation enabled
+    - Same as ``ring_buffer``, but with DotPhoton preparation enabled.
   
   * - ``fifo dpcore``
     - Memory
     - no 
-    - Same as ``fifo``, but with DotPhoton preparation enabled
+    - Same as ``fifo``, but with DotPhoton preparation enabled.
   
   * - ``tif``
     - File  
     - no 
-    - Record images directly as tif files  
+    - Record images directly as tif files.
   
   * - ``multitif``
     - File  
     - no 
-    - Record images directly as one or more multitiff file()s 
+    - Record images directly as one or more multitiff file(s).
   
   * - ``pcoraw``
     - File  
     - no 
-    - Record images directly as one pcoraw file  
+    - Record images directly as one pcoraw file.
   
   * - ``dicom``
     - File  
     - no 
-    - Record images directly as dicom files
+    - Record images directly as dicom files.
   
   * - ``multidicom``
     - File  
     - no 
-    - Record images directly as one or more multi-dicom file(s)
-
-- ``file_path`` Path where the image file(s) should be stored (only for modes who directly save to file)
-
-.. ---------------------------------------------------------------------------
-
-stop()
-------
-
-Stops the current recording.
-
-.. code-block:: python
-
-    def stop(self):
-
-In ``'ring buffer'`` and ``'fifo'`` mode this function must to be called by the user.
-In ``'sequence'`` and ``'sequence non blocking'`` mode, this function is automatically called up
-when the ``number_of_images`` is reached.
-
-
-.. ---------------------------------------------------------------------------
-
-close()
--------
-.. code-block:: python
-
-    def close(self):
-
-Closes the activated camera and releases the blocked ressources.
-This function must be called before the application is terminated.
-Otherwise the resources remain occupied.
-
-This function is called automatically, if the camera object is
-created by the ``with`` statement. An explicit call to ``close()`` is no
-longer necessary.
-
-.. code-block:: python
-
-    with pco.Camera() as cam:
-        # do some stuff
-
-
-.. ---------------------------------------------------------------------------
-
-image()
--------
-
-Returns an image from the recorder. The type of the image is a ``numpy.ndarray``.
-This array is shaped depending on the resolution and ROI of the image.
-
-.. code-block:: python
-
-    def image(self, image_number=0, roi=None):
-
-- ``image_number`` specifies the number of the image to read. In ``'sequence'`` or ``'sequence non blocking'`` mode the recorder
-  index matches the image number.
-  If ``image_number`` is set to ``0xFFFFFFFF`` the last recorded image is copied. This allows
-  e.g. thumbnail while recording.
-
-- ``roi`` sets the region fo interest. Only this region of the image is copied to the return value.
-
-  .. code-block:: python
-
-      >>> cam.record(number_of_images=1, mode='sequence')
-
-      >>> image, meta = cam.image()
-
-      >>> type(image)
-      numpy.ndarray
-
-      >>> image.shape
-      (2160, 2560)
-
-      >>> image, metadata = cam.image(roi=(1, 1, 300, 300))
-
-      >>> image.shape
-      (300, 300)
-
-.. ---------------------------------------------------------------------------
-
-images()
---------
-
-Returns all recorded images from the recorder as list of numpy arrays.
-
-.. code-block:: python
-
-    def images(self, roi=None, blocksize=None):
-
-- ``roi`` sets the region fo interest. Only this region of the image is copied to the return value.
-
-- ``blocksize`` defines the maximum number of images that are returned.
-  This parameter is only useful in ``'fifo'`` mode and under special conditions.
-
-  .. code-block:: python
-
-      >>> cam.record(number_of_images=20, mode='sequence')
-
-      >>> images, metadatas = cam.images()
-
-      >>> len(images)
-      20
-
-      >>> for image in images:
-      ...     print('Mean: {:7.2f} DN'.format(image.mean()))
-      ...
-      Mean: 2147.64 DN
-      Mean: 2144.61 DN
-      ...
-
-     >>> images = cam.images(roi=(1, 1, 300, 300))
-     
-     >>> images[0].shape
-    (300, 300)
-
-.. ---------------------------------------------------------------------------
-
-image_average()
-------------------------
-
-Returns the averaged image. This image is calculated from all recorded images in the buffer.
-
-.. code-block:: python
-
-    def image_average(self, roi=None):
-
-- ``roi`` defines the region fo interest. Only this region of the image is copied to the return value.
-
-  .. code-block:: python
-
-      >>> cam.record(number_of_images=100, mode='sequence')
-
-      >>> avg = cam.image_average()
-
-      >>> avg = cam.image_average(roi=(1, 1, 300, 300))
+    - Record images directly as one or more multi-dicom file(s).
 
+Image Formats
+=============
+All image data is always transferred as 2D or 3D numpy array.
+Besides the standard 16 bit raw image data you also have the possibility to get your images in different formats,
+shown in the table below.
 
-.. ---------------------------------------------------------------------------
+The format is selected when calling the ``image()`` / ``images()`` / ``image_average()`` functions of the Camera class. 
+The image data is stored as numpy array, which enables you to work with it in the most pythonic way.
 
-wait_for_first_image()
--------------------------
-Waits for the first available image in the recorder memory.
+.. list-table:: image formats
+  :widths: 30 70
+  :header-rows: 1
 
-.. code-block:: python
+  * - Format
+    - Description
+  
+  * - ``Mono8,mono8``
+    - Get image as 8 bit grayscale data.
+  
+  * - ``Mono16,mono16,raw16,bw16``
+    - Get image as 16 bit grayscale/raw data.
+  
+  * - ``BGR8,bgr``
+    - Get image as 24 bit color data in bgr format.
+  
+  * - ``RGB8,rgb``
+    - Get image as 24 bit color data in rgb format.
+  
+  * - ``BGRA8,bgra8,bgra``
+    - Get image as 32 bit color data (with alpha channel) in bgra format.
+  
+  * - ``RGBA8,rgba8,rgba``
+    - Get image as 32 bit color data (with alpha channel) in rgba format.
+  
+  * - ``BGR16,bgr16``
+    - Get image as 48 bit color data in bgr format (only possible for color cameras).
+  
+  * - ``RGB16,rgb16``
+    - Get image as 48 bit color data in rgb format (only possible for color cameras).
 
-    def wait_for_first_image(self, delay=True, timeout=None):
 
+Logging
+=======
 
-.. ---------------------------------------------------------------------------
+Logging is implemented according to the python logging package (https://docs.python.org/3/library/logging.html).
+Supported logging levels are:
 
-wait_for_new_image()
--------------------------
-Wait until a new image has been recorded and is available (i.e. an image that has not been read
-yet).
+- `ERROR`
+- `WARNING`
+- `INFO`
+- `DEBUG`
 
 .. code-block:: python
 
-    def wait_for_new_image(self, delay=True, timeout=None):
-
-
-.. ---------------------------------------------------------------------------
-
-sdk
----
-The object ``sdk`` allows direct access to all underlying functions of the pco.sdk.
+    logger = logging.getLogger("pco")
+    logger.setLevel(logging.INFO)
+    logger.addHandler(pco.stream_handler)
 
 .. code-block:: python
 
-       >>> cam.sdk.get_temperature()
-       {'sensor temperature': 7.0, 'camera temperature': 38.2, 'power temperature': 36.7}
-
-All return values form ``sdk`` functions are dictionarys.
-Not all camera settings are currently covered by the ``camera`` class.
-Special settings have to be set directly  by calling the respective SDK function.
-
-.. ---------------------------------------------------------------------------
-
-rec
---------
+    ...
+    [][sdk] get_camera_type: OK.
+    ...
+    [2019-11-25 15:54:15.317855 / 0.016 s] [][sdk] get_camera_type: OK.
 
-The object ``rec`` offers direct access to all underlying functions of the pco.recorder.
-It is not necessary to call a recorder class method directly. 
-All functions are fully covered by the methods of the ``camera`` class.
 
+Documentation (overview)
+========================
+The full Documentation can be found in the `manual <https://www.pco.de/fileadmin/user_upload/pco-manuals/MA_PCOPYTHON.pdf>`_
 
-.. ---------------------------------------------------------------------------
+The pco.Camera class offers the following methods:
 
-conv
---------
+- ``__init()__`` Opens and initializes a camera with its default configuration.
+- ``__exit()__`` Closes the camera and cleans up everything (e.g. end of with-statement).
+- ``close()`` Closes the camera and cleans up everything.
+- ``default_configuration()`` Set default configuration to the camera
+- ``record()`` Initialize and start the recording of images.
+- ``stop()`` Stop the current recording.
+- ``wait_for_first_image()`` Wait until the first image has been recorded.
+- ``wait_for_new_image()`` Wait until a new image has been recorded.
+- ``get_convert_control()`` Get current color convert settings.
+- ``set_convert_control()`` Set new color convert settings.
+- ``load_lut()`` Set the lut file for the convert control setting.
+- ``adapt_white_balance()`` Do a white-balance according to a transferred image.
+- ``image()`` Read a recorded image as numpy array.
+- ``images()`` Read a series of recorded images as a list of numpy arrays.
+- ``image_average()`` Read an averaged image (averaged over all recorded images) as numpy array.
 
-The object ``conv``  is a dictionary of convert objects to offer direct access to all
-underlying functions of the pco.convert.
-It is not necessary to call a ``conv`` class method directly. 
-All functions are fully covered by the methods of the ``camera`` class.
+The pco.Camera class has the following properties:
 
+- ``camera_name`` gets the camera name.
+- ``camera_serial`` gets the serial number of the camera.
+- ``is_recording`` gets a flag to indicate if the camera is currently recording.
+- ``is_color`` gets a flag to indicate if the camera is a color camera.
+- ``recorded_image_count`` gets the number of currently recorded images.
+- ``configuration`` gets/sets the camera configuration.
+- ``description`` gets the (static) camera description parameters.
+- ``exposure_time`` gets/sets the exposure time (in seconds).
+- ``delay_time`` gets/sets the delay time (in seconds).
 
+The pco.Camera class holds the following objects:
 
+- ``sdk`` offers direct access to all underlying functions of the pco.sdk.
+- ``rec`` offers direct access to all underlying functions of the pco.recorder.
+- ``conv`` offers direct access to all underlying functions of the pco.convert according to the selected image format.
 
 
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/pco.svg
    :target: https://pypi.python.org/pypi/pco
 
 .. |LICENCE| image:: https://img.shields.io/badge/License-MIT-green.svg
    :target: https://opensource.org/licenses/MIT
 
 .. |Platform| image:: https://img.shields.io/badge/platform-win_x64%20%7C%20linux_x64-green.svg
    :target: https://pypi.python.org/pypi/pco
    
 .. |PyPI-Status| image:: https://img.shields.io/pypi/v/pco.svg
   :target: https://pypi.python.org/pypi/pco
 
+
+
```

### Comparing `pco-2.0.0/license.pdf` & `pco-2.0.1/license.pdf`

 * *Files identical despite different names*

### Comparing `pco-2.0.0/license_3rdParty.pdf` & `pco-2.0.1/license_3rdParty.pdf`

 * *Files identical despite different names*

### Comparing `pco-2.0.0/pco/LICENSE.txt` & `pco-2.0.1/pco/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pco-2.0.0/pco/camera.py` & `pco-2.0.1/pco/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import sys
 import time
 import copy
 import numpy as np
 import logging
 import warnings
+import os.path
 
 from pco.sdk import Sdk
 from pco.recorder import Recorder
 from pco.convert import Convert
 
 
 logger = logging.getLogger(__name__)
@@ -991,15 +992,22 @@
                 or mode == "pcoraw"
                 or mode == "b16"
                 or mode == "dicom"
                 or mode == 'multidicom'):
             blocking = "off"
             if file_path is None:
                 raise ValueError
-            m = self.rec.create("file", file_path=file_path)["maximum available images"]
+            base_path = os.path.dirname(os.path.abspath(file_path))
+            if not os.path.exists(base_path):
+                base_path = file_path
+                if not os.path.exists(base_path):
+                    logger.error("Invalid file path, folder doesn't exist")
+                    raise ValueError
+
+            m = self.rec.create("file", file_path=base_path)["maximum available images"]
 
         else:
             raise ValueError
 
         # m = self.rec.create('memory')['maximum available images']
         if number_of_images > m:
             print("Not enough space for your application.")
```

### Comparing `pco-2.0.0/pco/convert.py` & `pco-2.0.1/pco/convert.py`

 * *Files identical despite different names*

### Comparing `pco-2.0.0/pco/flim.py` & `pco-2.0.1/pco/flim.py`

 * *Files identical despite different names*

### Comparing `pco-2.0.0/pco/license.pdf` & `pco-2.0.1/pco/license.pdf`

 * *Files identical despite different names*

### Comparing `pco-2.0.0/pco/license_3rdParty.pdf` & `pco-2.0.1/pco/license_3rdParty.pdf`

 * *Files identical despite different names*

### Comparing `pco-2.0.0/pco/logging.py` & `pco-2.0.1/pco/logging.py`

 * *Files identical despite different names*

### Comparing `pco-2.0.0/pco/recorder.py` & `pco-2.0.1/pco/recorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,49 +366,43 @@
     def create(self, mode, dpcore=False, file_path=None):
         """
         Initilize and create recorder
         """
 
         self.recorder_handle = C.c_void_p(0)
 
+        path = C.c_char_p() # nullptr
         if file_path is not None:
-            letter = file_path[0]
-        else:
-            letter = "C"
-
-        path = C.c_char_p()
-        path.value = letter.encode("utf-8")
+            path = C.c_char_p(file_path.encode("utf-8"))
 
         recorder_mode = {"file": 1, "memory": 2, "camram": 3}
 
-        dwImgDistributionArr = C.c_uint32(1)
+        dwImgDistributionArr = C.POINTER(C.c_uint32)()  # C.c_uint32(1)
         wArrLength = C.c_uint16(1)
         wRecMode = C.c_uint16()
-        cDriveLetter = path
         dwMaxImgCountArr = C.c_uint32()
 
         wRecMode = recorder_mode[mode]
         if dpcore:
             wRecMode = wRecMode | 0x1000
 
         time_start = time.perf_counter()
         error = self.PCO_Recorder.PCO_RecorderCreate(
             self.recorder_handle,
             self.camera_handle,
             dwImgDistributionArr,
             wArrLength,
             wRecMode,
-            cDriveLetter,
+            path,
             dwMaxImgCountArr,
         )
         duration = time.perf_counter() - time_start
         error_msg = self.get_error_text(error)
 
         ret = {}
-
         if error == 0:
             ret.update({"maximum available images": dwMaxImgCountArr.value})
 
         logger.info("[{:5.3f} s] [rec] {}: {}".format(duration, sys._getframe().f_code.co_name, error_msg))
 
         if error:
             raise ValueError("{}: {}".format(error, error_msg))
@@ -442,32 +436,40 @@
         dwImgCountArr = C.c_uint32(number_of_images)
         wArrLength = C.c_uint16(1)
         wType = C.c_uint16()
         wNoOverwrite = C.c_uint16(0)
 
         path = C.c_char_p()
         if file_path is not None:
-            path.value = file_path.encode("utf-8")
+            path = C.c_char_p(file_path.encode("utf-8"))
         else:
-            path.value = "C:\\".encode("utf-8")
+            path = C.c_char_p("".encode("utf-8"))
 
-        wRamSegmentArr = C.c_uint16()
+        wRamSegmentArr = C.POINTER(C.c_uint16)()
 
         recorder_mode = {
             "sequence": 1,
             "ring buffer": 2,
             "fifo": 3,
             "tif": 1,
             "multitif": 2,
             "pcoraw": 3,
             "b16": 4,
             "dicom": 5,
             "multidicom": 6,
         }
 
+        if (recorder_type in ["tif",
+                              "multitif",
+                              "pcoraw",
+                              "b16",
+                              "dicom",
+                              "multidicom"]):
+            wNoOverwrite = C.c_uint16(1)
+
         wType = recorder_mode[recorder_type]
 
         time_start = time.perf_counter()
         error = self.PCO_Recorder.PCO_RecorderInit(
             self.recorder_handle,
             dwImgCountArr,
             wArrLength,
```

### Comparing `pco-2.0.0/pco/sdk.py` & `pco-2.0.1/pco/sdk.py`

 * *Files identical despite different names*

### Comparing `pco-2.0.0/setup.py` & `pco-2.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,36 +20,43 @@
     path.abspath(path.join(run_path, 'sc2_cam.dll')),
     path.abspath(path.join(run_path, 'sc2_clhs.dll')),
     path.abspath(path.join(run_path, 'sc2_genicam.dll')),
     path.abspath(path.join(run_path, 'sc2_gige.dll')),
     path.abspath(path.join(run_path, 'sc2_cl_me4.dll'))
 ]
 
-linux_majors = {}  # major copies
+linux_so = {}  # major copies
 for f in glob.glob(path.abspath(path.join(run_path, "lib*.so.*.*.*"))):
-    linux_majors.update({f: path.basename(f[:f[:f.rfind('.')].rfind('.')])})
+    linux_so.update({f: path.basename(f[:f[:f.rfind('.')].rfind('.')])})
+
+# .so
+for f in glob.glob(path.abspath(path.join(run_path, "libpco_f*.so.*.*.*"))):
+    if path.basename(f[:f[:f[:f.rfind('.')].rfind('.')].rfind('.')]) == 'libpco_file.so':
+        continue
+    linux_so.update({f: path.basename(f[:f[:f[:f.rfind('.')].rfind('.')].rfind('.')])})
+
 
 package_list = [
     './genicam',
     './LICENSE.txt',
     './license.pdf',
     './license_3rdParty.pdf']
 package_list += [path.join('pco', path.basename(i)) for i in win_dlls]
-package_list += [path.join('pco', linux_majors[i]) for i in linux_majors]
+package_list += [path.join('pco', linux_so[i]) for i in linux_so]
 
 
 class RuntimeInstall(install):
     """Install setup to copy shared libraries"""
 
     def run(self):
         install.run(self)
 
         dest_path = path.join(path.abspath(self.root), 'pco')
-        for full_lib in linux_majors:
-            shutil.copy(full_lib, path.abspath(path.join(dest_path, linux_majors[full_lib])))
+        for full_lib in linux_so:
+            shutil.copy(full_lib, path.abspath(path.join(dest_path, linux_so[full_lib])))
 
         for file in win_dlls:
             shutil.copy(file, dest_path)
         shutil.copytree(path.abspath(path.join(run_path, 'genicam')), path.abspath(path.join(dest_path, 'genicam')))
 
 
 class RuntimeDevelop(develop):
@@ -57,15 +64,15 @@
 
     def run(self):
         develop.run(self)
 
         if sys.platform.startswith('win32'):
             run_path = 'C:\\pco_runtime\\bin64'
         elif sys.platform.startswith('linux'):
-            self.__dll_name = '/opt/pco/pco_runtime'
+            run_path = '/opt/pco/pco_runtime/bin64'
         else:
             print("Package not supported on platform " + sys.platform)
             raise SystemError
         win_dlls = []
         win_dlls = glob.glob(path.abspath(path.join(run_path, 'pco_f*.dll')))
         win_dlls += [
             path.abspath(path.join(run_path, 'pco_recorder.dll')),
@@ -73,31 +80,42 @@
             path.abspath(path.join(run_path, 'sc2_cam.dll')),
             path.abspath(path.join(run_path, 'sc2_clhs.dll')),
             path.abspath(path.join(run_path, 'sc2_genicam.dll')),
             path.abspath(path.join(run_path, 'sc2_gige.dll')),
             path.abspath(path.join(run_path, 'sc2_cl_me4.dll'))
         ]
 
-        linux_majors = {}  # major copies
+        dest_path = path.join(path.abspath(this_directory), 'pco')
+
+        # .so.<major>
+        linux_so = {}
         for f in glob.glob(path.abspath(path.join(run_path, "lib*.so.*.*.*"))):
-            linux_majors.update({f: path.basename(f[:f[:f.rfind('.')].rfind('.')])})
+            linux_so.update({f: path.basename(f[:f[:f.rfind('.')].rfind('.')])})
 
-        dest_path = path.join(path.abspath(this_directory), 'pco')
-        for full_lib in linux_majors:
-            shutil.copy(full_lib, path.abspath(path.join(dest_path, linux_majors[full_lib])))
+        # .so
+        for f in glob.glob(path.abspath(path.join(run_path, "libpco_f*.so.*.*.*"))):
+            if path.basename(f[:f[:f[:f.rfind('.')].rfind('.')].rfind('.')]) == 'libpco_file.so':
+                continue
+            linux_so.update({f: path.basename(f[:f[:f[:f.rfind('.')].rfind('.')].rfind('.')])})
+
+        for full_lib in linux_so:
+            shutil.copy(full_lib, path.abspath(path.join(dest_path, linux_so[full_lib])))
+
+            # .so.<major>.<minor>.<patch>
+            # shutil.copy(full_lib, dest_path)
 
         for file in win_dlls:
             shutil.copy(file, dest_path)
         shutil.copytree(path.abspath(path.join(run_path, 'genicam')), path.abspath(path.join(dest_path, 'genicam')))
 
 
 setup(
     name='pco',
     packages=['pco'],
-    version='2.0.0',
+    version='2.0.1',
     license='MIT',
 
     description='This class provides methods for using pco cameras.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
 
     author='Excelitas PCO GmbH',
```

