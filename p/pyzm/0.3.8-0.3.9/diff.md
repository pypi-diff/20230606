# Comparing `tmp/pyzm-0.3.8.tar.gz` & `tmp/pyzm-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyzm-0.3.8.tar", last modified: Mon Dec 28 18:59:35 2020, max compression
+gzip compressed data, was "dist/pyzm-0.3.9.tar", last modified: Tue Dec 29 17:33:50 2020, max compression
```

## Comparing `pyzm-0.3.8.tar` & `pyzm-0.3.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 pp        (1000) pp        (1000)        0 2020-12-28 18:59:35.000000 pyzm-0.3.8/
-drwxrwxr-x   0 pp        (1000) pp        (1000)        0 2020-12-28 18:59:35.000000 pyzm-0.3.8/pyzm/
--rw-rw-r--   0 pp        (1000) pp        (1000)     6541 2020-11-28 20:24:14.000000 pyzm-0.3.8/pyzm/ZMEventNotification.py
--rw-rw-r--   0 pp        (1000) pp        (1000)     8508 2020-09-02 15:54:33.000000 pyzm-0.3.8/pyzm/ZMMemory.py
-drwxrwxr-x   0 pp        (1000) pp        (1000)        0 2020-12-28 18:59:35.000000 pyzm-0.3.8/pyzm/helpers/
--rw-rw-r--   0 pp        (1000) pp        (1000)     1933 2020-11-28 20:39:01.000000 pyzm-0.3.8/pyzm/helpers/Base.py
--rw-rw-r--   0 pp        (1000) pp        (1000)     3742 2020-12-25 21:34:22.000000 pyzm-0.3.8/pyzm/helpers/utils.py
--rw-rw-r--   0 pp        (1000) pp        (1000)    12905 2020-12-28 17:06:52.000000 pyzm-0.3.8/pyzm/helpers/Media.py
--rw-r--r--   0 pp        (1000) pp        (1000)     3733 2020-11-28 20:25:54.000000 pyzm-0.3.8/pyzm/helpers/Monitors.py
--rw-r--r--   0 pp        (1000) pp        (1000)     1375 2019-09-23 20:36:25.000000 pyzm-0.3.8/pyzm/helpers/State.py
--rw-rw-r--   0 pp        (1000) pp        (1000)     8349 2020-10-31 10:48:14.000000 pyzm-0.3.8/pyzm/helpers/Event.py
--rw-rw-r--   0 pp        (1000) pp        (1000)     5181 2020-11-28 20:24:44.000000 pyzm-0.3.8/pyzm/helpers/Events.py
--rw-r--r--   0 pp        (1000) pp        (1000)     2360 2019-09-23 20:35:56.000000 pyzm-0.3.8/pyzm/helpers/Configs.py
--rw-rw-r--   0 pp        (1000) pp        (1000)     5365 2020-07-02 21:16:31.000000 pyzm-0.3.8/pyzm/helpers/Monitor.py
--rw-r--r--   0 pp        (1000) pp        (1000)     1739 2020-11-28 20:26:02.000000 pyzm-0.3.8/pyzm/helpers/States.py
-drwxrwxr-x   0 pp        (1000) pp        (1000)        0 2020-12-28 18:59:35.000000 pyzm-0.3.8/pyzm/ml/
--rw-rw-r--   0 pp        (1000) pp        (1000)    25803 2020-12-27 12:25:42.000000 pyzm-0.3.8/pyzm/ml/detect_sequence.py
--rw-rw-r--   0 pp        (1000) pp        (1000)     8635 2020-12-28 16:07:53.000000 pyzm-0.3.8/pyzm/ml/yolo.py
--rw-rw-r--   0 pp        (1000) pp        (1000)    15536 2020-12-28 15:01:04.000000 pyzm-0.3.8/pyzm/ml/alpr.py
--rw-rw-r--   0 pp        (1000) pp        (1000)     3221 2020-11-28 20:30:21.000000 pyzm-0.3.8/pyzm/ml/object.py
--rw-rw-r--   0 pp        (1000) pp        (1000)     4989 2020-12-28 16:07:53.000000 pyzm-0.3.8/pyzm/ml/coral_edgetpu.py
--rw-rw-r--   0 pp        (1000) pp        (1000)    10605 2020-12-28 18:54:54.000000 pyzm-0.3.8/pyzm/ml/face.py
--rw-rw-r--   0 pp        (1000) pp        (1000)     6680 2020-12-28 17:52:20.000000 pyzm-0.3.8/pyzm/ml/face_train.py
--rw-rw-r--   0 pp        (1000) pp        (1000)     1532 2020-11-28 20:29:53.000000 pyzm-0.3.8/pyzm/ml/hog.py
--rw-r--r--   0 pp        (1000) pp        (1000)    15100 2020-11-16 20:37:08.000000 pyzm-0.3.8/pyzm/ZMLog.py
--rw-rw-r--   0 pp        (1000) pp        (1000)    16779 2020-12-26 22:46:09.000000 pyzm-0.3.8/pyzm/api.py
--rw-rw-r--   0 pp        (1000) pp        (1000)       42 2020-12-28 18:59:06.000000 pyzm-0.3.8/pyzm/__init__.py
-drwxrwxr-x   0 pp        (1000) pp        (1000)        0 2020-12-28 18:59:35.000000 pyzm-0.3.8/pyzm.egg-info/
--rw-rw-r--   0 pp        (1000) pp        (1000)      222 2020-12-28 18:59:35.000000 pyzm-0.3.8/pyzm.egg-info/requires.txt
--rw-rw-r--   0 pp        (1000) pp        (1000)        1 2020-12-28 18:59:35.000000 pyzm-0.3.8/pyzm.egg-info/dependency_links.txt
--rw-rw-r--   0 pp        (1000) pp        (1000)     1279 2020-12-28 18:59:35.000000 pyzm-0.3.8/pyzm.egg-info/PKG-INFO
--rw-rw-r--   0 pp        (1000) pp        (1000)      648 2020-12-28 18:59:35.000000 pyzm-0.3.8/pyzm.egg-info/SOURCES.txt
--rw-rw-r--   0 pp        (1000) pp        (1000)        5 2020-12-28 18:59:35.000000 pyzm-0.3.8/pyzm.egg-info/top_level.txt
--rw-r--r--   0 pp        (1000) pp        (1000)    17986 2019-07-28 19:54:56.000000 pyzm-0.3.8/LICENSE
--rw-rw-r--   0 pp        (1000) pp        (1000)       38 2020-12-28 18:59:35.000000 pyzm-0.3.8/setup.cfg
--rw-rw-r--   0 pp        (1000) pp        (1000)     1279 2020-12-28 18:59:35.000000 pyzm-0.3.8/PKG-INFO
--rw-r--r--   0 pp        (1000) pp        (1000)     2583 2020-12-04 13:13:03.000000 pyzm-0.3.8/setup.py
--rw-r--r--   0 pp        (1000) pp        (1000)      674 2020-07-25 19:57:25.000000 pyzm-0.3.8/README.md
--rw-r--r--   0 pp        (1000) pp        (1000)       26 2019-07-28 19:54:56.000000 pyzm-0.3.8/MANIFEST.in
+drwxrwxr-x   0 pp        (1000) pp        (1000)        0 2020-12-29 17:33:50.000000 pyzm-0.3.9/
+drwxrwxr-x   0 pp        (1000) pp        (1000)        0 2020-12-29 17:33:50.000000 pyzm-0.3.9/pyzm/
+-rw-rw-r--   0 pp        (1000) pp        (1000)     6541 2020-11-28 20:24:14.000000 pyzm-0.3.9/pyzm/ZMEventNotification.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)     8508 2020-09-02 15:54:33.000000 pyzm-0.3.9/pyzm/ZMMemory.py
+drwxrwxr-x   0 pp        (1000) pp        (1000)        0 2020-12-29 17:33:50.000000 pyzm-0.3.9/pyzm/helpers/
+-rw-rw-r--   0 pp        (1000) pp        (1000)     1933 2020-11-28 20:39:01.000000 pyzm-0.3.9/pyzm/helpers/Base.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)     3742 2020-12-25 21:34:22.000000 pyzm-0.3.9/pyzm/helpers/utils.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)    13180 2020-12-29 12:56:06.000000 pyzm-0.3.9/pyzm/helpers/Media.py
+-rw-r--r--   0 pp        (1000) pp        (1000)     3733 2020-11-28 20:25:54.000000 pyzm-0.3.9/pyzm/helpers/Monitors.py
+-rw-r--r--   0 pp        (1000) pp        (1000)     1375 2019-09-23 20:36:25.000000 pyzm-0.3.9/pyzm/helpers/State.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)     8349 2020-10-31 10:48:14.000000 pyzm-0.3.9/pyzm/helpers/Event.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)     5181 2020-11-28 20:24:44.000000 pyzm-0.3.9/pyzm/helpers/Events.py
+-rw-r--r--   0 pp        (1000) pp        (1000)     2360 2019-09-23 20:35:56.000000 pyzm-0.3.9/pyzm/helpers/Configs.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)     5365 2020-07-02 21:16:31.000000 pyzm-0.3.9/pyzm/helpers/Monitor.py
+-rw-r--r--   0 pp        (1000) pp        (1000)     1739 2020-11-28 20:26:02.000000 pyzm-0.3.9/pyzm/helpers/States.py
+drwxrwxr-x   0 pp        (1000) pp        (1000)        0 2020-12-29 17:33:50.000000 pyzm-0.3.9/pyzm/ml/
+-rw-rw-r--   0 pp        (1000) pp        (1000)    25917 2020-12-29 17:32:47.000000 pyzm-0.3.9/pyzm/ml/detect_sequence.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)     8638 2020-12-29 17:25:10.000000 pyzm-0.3.9/pyzm/ml/yolo.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)    15536 2020-12-28 15:01:04.000000 pyzm-0.3.9/pyzm/ml/alpr.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)     3221 2020-11-28 20:30:21.000000 pyzm-0.3.9/pyzm/ml/object.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)     5090 2020-12-29 17:31:01.000000 pyzm-0.3.9/pyzm/ml/coral_edgetpu.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)    10566 2020-12-29 17:29:45.000000 pyzm-0.3.9/pyzm/ml/face.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)     6680 2020-12-28 17:52:20.000000 pyzm-0.3.9/pyzm/ml/face_train.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)     1532 2020-11-28 20:29:53.000000 pyzm-0.3.9/pyzm/ml/hog.py
+-rw-r--r--   0 pp        (1000) pp        (1000)    15131 2020-12-29 14:45:50.000000 pyzm-0.3.9/pyzm/ZMLog.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)    17656 2020-12-29 13:36:28.000000 pyzm-0.3.9/pyzm/api.py
+-rw-rw-r--   0 pp        (1000) pp        (1000)       42 2020-12-29 17:33:09.000000 pyzm-0.3.9/pyzm/__init__.py
+drwxrwxr-x   0 pp        (1000) pp        (1000)        0 2020-12-29 17:33:50.000000 pyzm-0.3.9/pyzm.egg-info/
+-rw-rw-r--   0 pp        (1000) pp        (1000)      222 2020-12-29 17:33:49.000000 pyzm-0.3.9/pyzm.egg-info/requires.txt
+-rw-rw-r--   0 pp        (1000) pp        (1000)        1 2020-12-29 17:33:49.000000 pyzm-0.3.9/pyzm.egg-info/dependency_links.txt
+-rw-rw-r--   0 pp        (1000) pp        (1000)     1279 2020-12-29 17:33:49.000000 pyzm-0.3.9/pyzm.egg-info/PKG-INFO
+-rw-rw-r--   0 pp        (1000) pp        (1000)      648 2020-12-29 17:33:49.000000 pyzm-0.3.9/pyzm.egg-info/SOURCES.txt
+-rw-rw-r--   0 pp        (1000) pp        (1000)        5 2020-12-29 17:33:49.000000 pyzm-0.3.9/pyzm.egg-info/top_level.txt
+-rw-r--r--   0 pp        (1000) pp        (1000)    17986 2019-07-28 19:54:56.000000 pyzm-0.3.9/LICENSE
+-rw-rw-r--   0 pp        (1000) pp        (1000)       38 2020-12-29 17:33:50.000000 pyzm-0.3.9/setup.cfg
+-rw-rw-r--   0 pp        (1000) pp        (1000)     1279 2020-12-29 17:33:50.000000 pyzm-0.3.9/PKG-INFO
+-rw-r--r--   0 pp        (1000) pp        (1000)     2583 2020-12-04 13:13:03.000000 pyzm-0.3.9/setup.py
+-rw-r--r--   0 pp        (1000) pp        (1000)      674 2020-07-25 19:57:25.000000 pyzm-0.3.9/README.md
+-rw-r--r--   0 pp        (1000) pp        (1000)       26 2019-07-28 19:54:56.000000 pyzm-0.3.9/MANIFEST.in
```

### Comparing `pyzm-0.3.8/pyzm/ZMEventNotification.py` & `pyzm-0.3.9/pyzm/ZMEventNotification.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/ZMMemory.py` & `pyzm-0.3.9/pyzm/ZMMemory.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/helpers/Base.py` & `pyzm-0.3.9/pyzm/helpers/Base.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/helpers/utils.py` & `pyzm-0.3.9/pyzm/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/helpers/Media.py` & `pyzm-0.3.9/pyzm/helpers/Media.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,19 @@
                 self.logger.Debug (4, 'Saving image to {}'.format(fname))
                 cv2.imwrite(fname,frame)        
 
             return frame
         
         else: # image
             if self.frame_set:
+                if self.next_frame_set_index >= len (self.frame_set):
+                    self.logger.Debug (1,'Reached end of frame_set')
+                    self.more_images_to_read = False
+                    self.next_frameid_to_read = 0
+                    return None 
                 url = '{}&fid={}'.format(self.stream,self.frame_set[self.next_frame_set_index])
             else:
                 url = '{}&fid={}'.format(self.stream,self.next_frameid_to_read)
             
             self.logger.Debug (3, 'Reading {}'.format(url))
             response = None
             try:
```

### Comparing `pyzm-0.3.8/pyzm/helpers/Monitors.py` & `pyzm-0.3.9/pyzm/helpers/Monitors.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/helpers/State.py` & `pyzm-0.3.9/pyzm/helpers/State.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/helpers/Event.py` & `pyzm-0.3.9/pyzm/helpers/Event.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/helpers/Events.py` & `pyzm-0.3.9/pyzm/helpers/Events.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/helpers/Configs.py` & `pyzm-0.3.9/pyzm/helpers/Configs.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/helpers/Monitor.py` & `pyzm-0.3.9/pyzm/helpers/Monitor.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/helpers/States.py` & `pyzm-0.3.9/pyzm/helpers/States.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/ml/detect_sequence.py` & `pyzm-0.3.9/pyzm/ml/detect_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         #self.logger.Debug(1,'WAKANDA FOREVER!!!!!!!!!!!!!!!')
         self.model_sequence = options.get('general', {}).get('model_sequence', 'object').split(',')    
         self.ml_options = options
         self.stream_options = None
         self.models = {}
         self.media = None
         self.has_rescaled = False
+        self.ml_overrides = {}
 
     def _load_models(self, sequences):
         #print (f'***** {sequences}')
         if not sequences:
             sequences = self.model_sequence
         self.logger.Debug (3, "load_models (just init, actual load happens at first detect): {}".format(sequences))
         for seq in sequences:
@@ -266,20 +267,20 @@
                 self.logger.Info('object:{} at {} does not fall into any polygons, removing...'.
                     format(label[idx], obj))
         # out of primary bbox loop
         #print ("NEW ERR IS {}".format(new_err))
         return new_bbox, new_label, new_conf, new_err
 
 
-    def detect_stream(self, stream, options={}):
+    def detect_stream(self, stream, options={}, ml_overrides={}):
         """Implements detection on a video stream
 
         Args:
             stream (string): location of media (file, url or event ID)
-            api (object): instance of the API if the stream need to route via ZM
+            ml_overrides(string): Ignore it. You will almost never need it. zm_detect uses it for ugly foo
             options (dict, optional): Various options that control the detection process. Defaults to {}:
 
                 - download (boolean): if True, will download video before analysis. Defaults to False
                 - download_dir (string): directory where downloads will be kept (only applies to videos). Default is /tmp
                 - start_frame (int): Which frame to start analysis. Default 1.
                 - frame_skip: (int): Number of frames to skip in video (example, 3 means process every 3rd frame)
                 - max_frames (int): Total number of frames to process before stopping
@@ -319,15 +320,15 @@
         OpenCV's frame reading logic and when ``False`` we use ZoneMinder's image.php function
         which uses time based approximation. Therefore, the retrieve different frame offsets, but I assume
         they should be reasonably close.
             
         """
 
         
-
+        self.ml_overrides = ml_overrides
         self.stream_options = options
         frame_strategy = self.stream_options.get('frame_strategy', 'most_models' )
         all_matches = []
         matched_b = []
         matched_e = []
         matched_l = []
         matched_c = []
```

### Comparing `pyzm-0.3.8/pyzm/ml/yolo.py` & `pyzm-0.3.9/pyzm/ml/yolo.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,41 +28,41 @@
         self.processor=self.options.get('object_processor') or 'cpu'
         self.lock_maximum=int(options.get(self.processor+'_max_processes') or 1)
         self.lock_timeout = int(options.get(self.processor+'_max_lock_wait') or 120)
         
         #self.lock_name='pyzm_'+self.processor+'_lock'
         self.lock_name='pyzm_uid{}_{}_lock'.format(os.getuid(),self.processor)
 
-        self.logger.Debug (2,f'Semaphore: max:{self.lock_maximum}, name:{self.lock_name}, timeout:{self.lock_timeout}')
+        self.logger.Debug (2,f'portalock: max:{self.lock_maximum}, name:{self.lock_name}, timeout:{self.lock_timeout}')
         self.lock = portalocker.BoundedSemaphore(maximum=self.lock_maximum, name=self.lock_name,timeout=self.lock_timeout)
         self.model_height = self.options.get('model_height', 416)
         self.model_width = self.options.get('model_width', 416)
          
     def acquire_lock(self):
         if self.is_locked:
-            self.logger.Debug(2, '{} Lock already acquired'.format(self.lock_name))
+            self.logger.Debug(2, '{} portalock already acquired'.format(self.lock_name))
             return
         try:
-            self.logger.Debug (2,f'Waiting for {self.processor} lock...')
+            self.logger.Debug (2,f'Waiting for {self.lock_name} portalock...')
             self.lock.acquire()
-            self.logger.Debug (2,f'Got {self.processor} lock ..')
+            self.logger.Debug (2,f'Got {self.lock_name} portalock')
             self.is_locked = True
            
         except portalocker.AlreadyLocked:
-            self.logger.Error ('Timeout waiting for {} lock for {} seconds'.format(self.processor, self.lock_timeout))
-            raise ValueError ('Timeout waiting for {} lock for {} seconds'.format(self.processor, self.lock_timeout))
+            self.logger.Error ('Timeout waiting for {} portalock for {} seconds'.format(self.lock_name, self.lock_timeout))
+            raise ValueError ('Timeout waiting for {} portallock for {} seconds'.format(self.lock_name, self.lock_timeout))
 
 
     def release_lock(self):
         if not self.is_locked:
-            self.logger.Debug (2, '{} Lock already released'.format(self.lock_name))
+            self.logger.Debug (2, '{} portalock already released'.format(self.lock_name))
             return
         self.lock.release()
         self.is_locked = False
-        self.logger.Debug (2,'Released lock')
+        self.logger.Debug (2,'Released {} portalock'.format(self.lock_name))
 
 
         
     def populate_class_labels(self):
         class_file_abs_path = self.options.get('object_labels')
         f = open(class_file_abs_path, 'r')
         self.classes = [line.strip() for line in f.readlines()]
@@ -146,15 +146,14 @@
                                     crop=False)
         
         self.net.setInput(blob)
         outs = self.net.forward(ln)
 
         if self.options.get('auto_lock',True):
             self.release_lock()
-            self.logger.Debug(2,'detect lock released')
         diff_time = (datetime.datetime.now() - start)
         self.logger.Debug(
             1,'YOLO detection took: {} milliseconds'.format(diff_time))
 
     
         class_ids = []
         confidences = []
```

### Comparing `pyzm-0.3.8/pyzm/ml/alpr.py` & `pyzm-0.3.9/pyzm/ml/alpr.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/ml/object.py` & `pyzm-0.3.9/pyzm/ml/object.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/ml/coral_edgetpu.py` & `pyzm-0.3.9/pyzm/ml/coral_edgetpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,41 +31,41 @@
         self.logger.Debug (4, 'TPU init params: {}'.format(options))
         
         self.processor='tpu'
         self.lock_maximum=int(options.get(self.processor+'_max_processes') or 1)
         self.lock_name='pyzm_uid{}_{}_lock'.format(os.getuid(),self.processor)
         self.lock_timeout = int(options.get(self.processor+'_max_lock_wait') or 120)
 
-        self.logger.Debug (2,f'Semaphore: max:{self.lock_maximum}, name:{self.lock_name}, timeout:{self.lock_timeout}')
+        self.logger.Debug (2,f'portalock: max:{self.lock_maximum}, name:{self.lock_name}, timeout:{self.lock_timeout}')
         self.lock = portalocker.BoundedSemaphore(maximum=self.lock_maximum, name=self.lock_name,timeout=self.lock_timeout)
         self.is_locked = False
         self.model = None
         self.populate_class_labels()
 
     def acquire_lock(self):
         if self.is_locked:
-            self.logger.Debug (2, '{} Lock already acquired'.format(self.lock_name))
+            self.logger.Debug (2, '{} portalock already acquired'.format(self.lock_name))
             return
         try:
-            self.logger.Debug (2,'Waiting for TPU lock...')
+            self.logger.Debug (2,'Waiting for {} portalock...'.format(self.lock_name))
             self.lock.acquire()
-            self.logger.Debug (2,'Got TPU Lock')
+            self.logger.Debug (2,'Got {} portalock'.format(self.lock_name))
             self.is_locked = True
 
         except portalocker.AlreadyLocked:
-            self.logger.Error ('Timeout waiting for {} lock for {} seconds'.format(self.processor, self.lock_timeout))
-            raise ValueError ('Timeout waiting for {} lock for {} seconds'.format(self.processor, self.lock_timeout))
+            self.logger.Error ('Timeout waiting for {} portalock for {} seconds'.format(self.lock_name, self.lock_timeout))
+            raise ValueError ('Timeout waiting for {} portalock for {} seconds'.format(self.lock_name, self.lock_timeout))
 
     def release_lock(self):
         if not self.is_locked:
-            self.logger.Debug (2, '{} Lock already released'.format(self.lock_name))
+            self.logger.Debug (2, '{} portalock already released'.format(self.lock_name))
             return
         self.lock.release()
         self.is_locked = False
-        self.logger.Debug (2,'Released TPU lock')
+        self.logger.Debug (2,'Released portalock {}'.format(self.lock_name))
 
 
     def populate_class_labels(self):
         class_file_abs_path = self.options.get('object_labels')        
         for row in open(class_file_abs_path):
             # unpack the row and update the labels dictionary
             (classID, label) = row.strip().split(" ", maxsplit=1)
```

### Comparing `pyzm-0.3.8/pyzm/ml/face.py` & `pyzm-0.3.9/pyzm/ml/face.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         self.lock_maximum=int(options.get(self.processor+'_max_processes') or 1)
         self.lock_timeout = int(options.get(self.processor+'_max_lock_wait') or 120)
         
         #self.lock_name='pyzm_'+self.processor+'_lock'
         self.lock_name='pyzm_uid{}_{}_lock'.format(os.getuid(),self.processor)
 
-        self.logger.Debug (2,f'Semaphore: max:{self.lock_maximum}, name:{self.lock_name}, timeout:{self.lock_timeout}')
+        self.logger.Debug (2,f'portalock: max:{self.lock_maximum}, name:{self.lock_name}, timeout:{self.lock_timeout}')
         self.lock = portalocker.BoundedSemaphore(maximum=self.lock_maximum, name=self.lock_name,timeout=self.lock_timeout)
         
 
         if self.options.get('face_detection_framework') != 'dlib' and self.options.get('face_recognition_framework') != 'dlib':
             raise ValueError ('Error: As of now,only dlib is supported for face detection and recognition. Unkown {}/{}'.format(self.options.get('face_detection_framework'),self.options.get('face_recognition_framework')))
 
         encoding_file_name = self.options.get('known_images_path') + '/faces.dat'
@@ -93,35 +93,34 @@
                 self.knn = pickle.load(f)
         except Exception as e:
             self.logger.Error ('Error loading KNN model: {}'.format(e))
 
 
     def acquire_lock(self):
         if self.is_locked:
-            self.logger.Debug (2, '{} Lock already acquired'.format(self.lock_name))
+            self.logger.Debug (2, '{} portalock already acquired'.format(self.lock_name))
             return
         try:
-            self.logger.Debug (2,f'Waiting for {self.processor} lock...')
+            self.logger.Debug (2,f'Waiting for {self.lock_name} portalock...')
             self.lock.acquire()
-            self.logger.Debug (2,f'Got {self.processor} lock for initialization...')
-           
-            self.lock.release()
-            self.logger.Debug(2,f'{self.processor} lock released')
+            self.logger.Debug (2,f'Got {self.lock_name} lock...')
+            self.is_locked = True
+
         except portalocker.AlreadyLocked:
-            self.logger.Error ('Timeout waiting for {} lock for {} seconds'.format(self.processor, self.lock_timeout))
-            raise ValueError ('Timeout waiting for {} lock for {} seconds'.format(self.processor, self.lock_timeout))
+            self.logger.Error ('Timeout waiting for {} portalock for {} seconds'.format(self.lock_name, self.lock_timeout))
+            raise ValueError ('Timeout waiting for {} portalock for {} seconds'.format(self.lock_name, self.lock_timeout))
 
 
     def release_lock(self):
         if not self.is_locked:
-            self.logger.Debug (1, '{} Lock already released'.format(self.lock_name))
+            self.logger.Debug (1, '{} portalock already released'.format(self.lock_name))
             return
         self.lock.release()
         self.is_locked = False
-        self.logger.Debug (1,'Released lock')
+        self.logger.Debug (1,'Released {} portalock'.format(self.lock_name))
 
     def get_classes(self):
         if self.knn:
             return self.knn.classes_
         else:
             return []
```

### Comparing `pyzm-0.3.8/pyzm/ml/face_train.py` & `pyzm-0.3.9/pyzm/ml/face_train.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/ml/hog.py` & `pyzm-0.3.9/pyzm/ml/hog.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/pyzm/ZMLog.py` & `pyzm-0.3.9/pyzm/ZMLog.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,16 @@
             uid = pwd.getpwnam(config['webuser']).pw_uid
             gid = grp.getgrnam(config['webgroup']).gr_gid
             os.chown(log_fname, uid,gid)
         except OSError as e:
             syslog.syslog (syslog.LOG_ERR, _format_string("Error opening file log:" + str(e)))
             log_fhandle = None
 
+def set_level(level):
+    pass
 
 def get_config():
     """Returns configuration of ZM logger
     
     Returns:
         dict: config params
     """
```

### Comparing `pyzm-0.3.8/pyzm/api.py` & `pyzm-0.3.9/pyzm/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         self.authenticated = False
         self.auth_enabled = True
         self.access_token = ''
         self.refresh_token = ''
         self.access_token_expires = None
         self.refresh_token_expires = None
         self.refresh_token_datetime = None
+        self.access_token_datetime = None
+
         self.legacy_credentials = None
         self.session = requests.Session()
         if options.get('disable_ssl_cert_check'):
             self.session.verify = False
             self.logger.Debug (1, 'Warning, SSL certificate check has been disbled')
             from urllib3.exceptions import InsecureRequestWarning
             requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
@@ -115,25 +117,38 @@
         """True if login API worked
         
         Returns:
             boolean -- True if Login API worked
         """
         return self.authenticated
 
+
+    # called in _make_request to avoid 401s if possible
+    def _refresh_tokens_if_needed(self):
+        if not (self.access_token_expires and self.refresh_token_expires):
+            return
+        tr = (self.access_token_datetime - datetime.datetime.now()).total_seconds()
+        if (tr >= 60*5): # 5 mins grace 
+            self.logger.Debug(3, 'No need to relogin as access token still has {} minutes remaining'.format(tr/60))
+            return
+        else:
+            self._relogin()
+              
+
     def _relogin(self):
         """ Used for 401. I could use _login too but decided to do a simpler fn
         """
         url = self.api_url+'/host/login.json'
         if self._versiontuple(self.api_version) >= self._versiontuple('2.0'):
             # use tokens
             tr = (self.refresh_token_datetime - datetime.datetime.now()).total_seconds()
 
 
             if (tr >= 60 * 5): # 5 mins grace
-                self.logger.Debug(1, 'Going to use refresh token as it still has {} minutes remaining'.format(tr/60))
+                self.logger.Debug(2, 'Going to use refresh token as it still has {} minutes remaining'.format(tr/60))
                 self.options['token'] = self.refresh_token
             else:
                 self.logger.Debug (1, 'Refresh token only has {}s of lifetime, going to use user/pass'.format(tr))
                 self.options['token'] = None
         self._login()
 
     def _login(self):
@@ -180,15 +195,17 @@
             if self.auth_enabled:
                 if (self._versiontuple(self.api_version) >= self._versiontuple('2.0')):
                     self.logger.Debug(2,'Using new token API')
                     self.access_token = rj.get('access_token','')
                     if rj.get('refresh_token'):
                         self.refresh_token = rj.get('refresh_token')
                     if (rj.get('access_token_expires')):
-                     self.access_token_expires = int(rj.get('access_token_expires'))
+                        self.access_token_expires = int(rj.get('access_token_expires'))
+                        self.access_token_datetime = datetime.datetime.now() + datetime.timedelta(seconds = self.access_token_expires)
+                        self.logger.Debug (1, 'Access token expires on:{} [{}s]'.format(self.access_token_datetime, self.access_token_expires))
                     if (rj.get('refresh_token_expires')):
                         self.refresh_token_expires = int(rj.get('refresh_token_expires'))
                         self.refresh_token_datetime = datetime.datetime.now() + datetime.timedelta(seconds = self.refresh_token_expires)
                         self.logger.Debug (1, 'Refresh token expires on:{} [{}s]'.format(self.refresh_token_datetime, self.refresh_token_expires))
                 else:
                     self.logger.Info('Using old credentials API. Recommended you upgrade to token API')
                     self.legacy_credentials = rj.get('credentials')
@@ -224,14 +241,16 @@
         if self._versiontuple(self.api_version) >= self._versiontuple('2.0'):
             return 'token='+self.access_token
         else:
             return self.legacy_credentials
 
 
     def _make_request(self, url=None, query={}, payload={}, type='get', reauth=True):
+
+        self._refresh_tokens_if_needed()
         type = type.lower()
         if self.auth_enabled:
             if self._versiontuple(self.api_version) >= self._versiontuple('2.0'):
                 query['token'] = self.access_token
                 # ZM 1.34 API bug, will be fixed soon
                 # self.session = requests.Session()
```

### Comparing `pyzm-0.3.8/pyzm.egg-info/PKG-INFO` & `pyzm-0.3.9/pyzm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzm
-Version: 0.3.8
+Version: 0.3.9
 Summary: ZoneMinder API, Logger and other base utilities for python programmers
 Home-page: https://github.com/pliablepixels/pyzm/
 Author: Pliable Pixels
 Author-email: pliablepixels@gmail.com
 License: GPL
 Description: <img src="https://raw.githubusercontent.com/pliablepixels/pyzm/master/images/pyzm.png" width="200"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyzm Version: 0.3.8 Summary: ZoneMinder API, Logger
+Metadata-Version: 2.1 Name: pyzm Version: 0.3.9 Summary: ZoneMinder API, Logger
 and other base utilities for python programmers Home-page: https://github.com/
 pliablepixels/pyzm/ Author: Pliable Pixels Author-email:
 pliablepixels@gmail.com License: GPL Description: [https://
 raw.githubusercontent.com/pliablepixels/pyzm/master/images/pyzm.png] What =====
 Pythonic ZoneMinder wrapper - API - Event Server - Logger - Memory - Machine
 Learning Modules Documentation & Examples ========================= Latest
 documentation is available here. The documentation includes a full example.
```

### Comparing `pyzm-0.3.8/pyzm.egg-info/SOURCES.txt` & `pyzm-0.3.9/pyzm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/LICENSE` & `pyzm-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/PKG-INFO` & `pyzm-0.3.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzm
-Version: 0.3.8
+Version: 0.3.9
 Summary: ZoneMinder API, Logger and other base utilities for python programmers
 Home-page: https://github.com/pliablepixels/pyzm/
 Author: Pliable Pixels
 Author-email: pliablepixels@gmail.com
 License: GPL
 Description: <img src="https://raw.githubusercontent.com/pliablepixels/pyzm/master/images/pyzm.png" width="200"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyzm Version: 0.3.8 Summary: ZoneMinder API, Logger
+Metadata-Version: 2.1 Name: pyzm Version: 0.3.9 Summary: ZoneMinder API, Logger
 and other base utilities for python programmers Home-page: https://github.com/
 pliablepixels/pyzm/ Author: Pliable Pixels Author-email:
 pliablepixels@gmail.com License: GPL Description: [https://
 raw.githubusercontent.com/pliablepixels/pyzm/master/images/pyzm.png] What =====
 Pythonic ZoneMinder wrapper - API - Event Server - Logger - Memory - Machine
 Learning Modules Documentation & Examples ========================= Latest
 documentation is available here. The documentation includes a full example.
```

### Comparing `pyzm-0.3.8/setup.py` & `pyzm-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyzm-0.3.8/README.md` & `pyzm-0.3.9/README.md`

 * *Files identical despite different names*

