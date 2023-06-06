# Comparing `tmp/GraphCASE-0.0.7.tar.gz` & `tmp/GraphCASE-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphCASE-0.0.7.tar", last modified: Tue Jun  6 05:41:27 2023, max compression
+gzip compressed data, was "GraphCASE-0.0.8.tar", last modified: Tue Jun  6 18:11:47 2023, max compression
```

## Comparing `GraphCASE-0.0.7.tar` & `GraphCASE-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 05:41:27.719297 GraphCASE-0.0.7/
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 05:41:27.716630 GraphCASE-0.0.7/GAE/
--rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.7/GAE/__init__.py
--rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.7/GAE/dataFeeder.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11515 2023-06-02 10:58:22.000000 GraphCASE-0.0.7/GAE/data_feeder_graphframes.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.7/GAE/data_feeder_nx.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    15818 2023-06-02 13:31:05.000000 GraphCASE-0.0.7/GAE/graph_case_controller.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     3867 2023-06-02 13:25:09.000000 GraphCASE-0.0.7/GAE/graph_case_tools.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     8247 2023-06-05 08:32:48.000000 GraphCASE-0.0.7/GAE/graph_reconstructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    13464 2023-06-05 17:58:06.000000 GraphCASE-0.0.7/GAE/input_layer_constructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.7/GAE/model.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    13478 2023-06-05 18:29:55.000000 GraphCASE-0.0.7/GAE/position_manager.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.7/GAE/transformation_layer.py
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 05:41:27.718446 GraphCASE-0.0.7/GraphCASE.egg-info/
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-06 05:41:27.000000 GraphCASE-0.0.7/GraphCASE.egg-info/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-06-06 05:41:27.000000 GraphCASE-0.0.7/GraphCASE.egg-info/SOURCES.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-06-06 05:41:27.000000 GraphCASE-0.0.7/GraphCASE.egg-info/dependency_links.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-06-06 05:41:27.000000 GraphCASE-0.0.7/GraphCASE.egg-info/top_level.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.7/LICENSE.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-06 05:41:27.718949 GraphCASE-0.0.7/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.7/README.md
--rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-06-06 05:41:27.719412 GraphCASE-0.0.7/setup.cfg
--rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-06-06 05:41:09.000000 GraphCASE-0.0.7/setup.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 18:11:47.617424 GraphCASE-0.0.8/
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 18:11:47.614632 GraphCASE-0.0.8/GAE/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.8/GAE/__init__.py
+-rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.8/GAE/dataFeeder.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11515 2023-06-02 10:58:22.000000 GraphCASE-0.0.8/GAE/data_feeder_graphframes.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.8/GAE/data_feeder_nx.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    16805 2023-06-06 18:04:13.000000 GraphCASE-0.0.8/GAE/graph_case_controller.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     3867 2023-06-02 13:25:09.000000 GraphCASE-0.0.8/GAE/graph_case_tools.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     8247 2023-06-05 08:32:48.000000 GraphCASE-0.0.8/GAE/graph_reconstructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    13464 2023-06-05 17:58:06.000000 GraphCASE-0.0.8/GAE/input_layer_constructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.8/GAE/model.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    13478 2023-06-05 18:29:55.000000 GraphCASE-0.0.8/GAE/position_manager.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.8/GAE/transformation_layer.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 18:11:47.616646 GraphCASE-0.0.8/GraphCASE.egg-info/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-06 18:11:46.000000 GraphCASE-0.0.8/GraphCASE.egg-info/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-06-06 18:11:47.000000 GraphCASE-0.0.8/GraphCASE.egg-info/SOURCES.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-06-06 18:11:47.000000 GraphCASE-0.0.8/GraphCASE.egg-info/dependency_links.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-06-06 18:11:47.000000 GraphCASE-0.0.8/GraphCASE.egg-info/top_level.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.8/LICENSE.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-06 18:11:47.617104 GraphCASE-0.0.8/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.8/README.md
+-rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-06-06 18:11:47.617532 GraphCASE-0.0.8/setup.cfg
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-06-06 18:11:05.000000 GraphCASE-0.0.8/setup.py
```

### Comparing `GraphCASE-0.0.7/GAE/dataFeeder.py` & `GraphCASE-0.0.8/GAE/dataFeeder.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.7/GAE/data_feeder_graphframes.py` & `GraphCASE-0.0.8/GAE/data_feeder_graphframes.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.7/GAE/data_feeder_nx.py` & `GraphCASE-0.0.8/GAE/data_feeder_nx.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.7/GAE/graph_case_controller.py` & `GraphCASE-0.0.8/GAE/graph_case_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         self.weight_label = weight_label
         self.encoder_labels = encoder_labels
         self.useBN = useBN
         self.dropout = dropout
         self.val_fraction = val_fraction
         self.data_feeder_cls = data_feeder_cls
         self.pos_enc_cls = pos_enc_cls
+        self.mpu, self.cpu = self.determine_mpu()
         if graph is not None:
             self.__consistency_checks()
             self.sampler = self.__init_sampler(graph, val_fraction, pos_enc_cls)
             self.model = self.__init_model()
         if model_config is not None:
             custom_objects = {
                 "DecTransLayer": DecTransLayer,
@@ -83,40 +84,42 @@
             with tf.keras.utils.custom_object_scope(custom_objects):
                 self.model = GraphAutoEncoderModel.from_config(model_config)
 
     def __init_sampler(self, graph, val_fraction, pos_enc_cls):
         """
         Initialises the datafeeder
         """
-        return InputLayerConstructor(
-            graph, support_size=self.support_size, val_fraction=val_fraction,
-            batch_size=self.batch_size, verbose=self.verbose, seed=self.seed,
-            weight_label=self.weight_label, encoder_labels=self.encoder_labels,
-            data_feeder_cls=self.data_feeder_cls, pos_enc_cls=pos_enc_cls
-        )
+        with tf.device(self.cpu):
+            return InputLayerConstructor(
+                graph, support_size=self.support_size, val_fraction=val_fraction,
+                batch_size=self.batch_size, verbose=self.verbose, seed=self.seed,
+                weight_label=self.weight_label, encoder_labels=self.encoder_labels,
+                data_feeder_cls=self.data_feeder_cls, pos_enc_cls=pos_enc_cls
+            )
 
     def __init_model(self):
         """
         Initialises the model
         """
-        model = GraphAutoEncoderModel(
-            self.dims, self.support_size, self.sampler.get_feature_size(),
-            hub0_feature_with_neighb_dim=self.hub0_feature_with_neighb_dim,
-            number_of_node_labels=self.sampler.get_number_of_node_labels(),
-            verbose=self.verbose, seed=self.seed, dropout=self.dropout, act=self.act,
-            useBN=self.useBN)
-
-        optimizer = tf.optimizers.Adam(learning_rate=self.learning_rate)
-        optimizer = tf.optimizers.RMSprop(learning_rate=self.learning_rate)
-        model.compile(optimizer=optimizer, loss='mse')
-
-        self.sampler.init_train_batch()
-        train_data = self.sampler.get_train_samples()
-        for n in train_data.take(1):
-            model(n[0])
+        with tf.device(self.cpu):
+            model = GraphAutoEncoderModel(
+                self.dims, self.support_size, self.sampler.get_feature_size(),
+                hub0_feature_with_neighb_dim=self.hub0_feature_with_neighb_dim,
+                number_of_node_labels=self.sampler.get_number_of_node_labels(),
+                verbose=self.verbose, seed=self.seed, dropout=self.dropout, act=self.act,
+                useBN=self.useBN)
+
+            optimizer = tf.optimizers.Adam(learning_rate=self.learning_rate)
+            optimizer = tf.optimizers.RMSprop(learning_rate=self.learning_rate)
+            model.compile(optimizer=optimizer, loss='mse')
+
+            self.sampler.init_train_batch()
+            train_data = self.sampler.get_train_samples()
+            for n in train_data.take(1):
+                model(n[0])
         return model
 
     def calculate_embeddings(self, graph=None, nodes=None, verbose=False):
         """
         Calculated the embedding of the nodes specified. If no nodes are
         specified, then the embedding for all nodes are calculated.
 
@@ -128,37 +131,39 @@
 
         Returns:
             A 2d numpy array with one embedding per row.
         """
         self.verbose = verbose
         if verbose:
             print("calculating all embeddings")
+            
+        with tf.device(self.cpu):
+            if graph is not None:
+                self.sampler = self.__init_sampler(graph, self.val_fraction, self.pos_enc_cls)
+
+            embedding = None
+            counter = 0
+            for i in self.sampler.init_incr_batch(nodes):
+                counter += 1
+                try:
+                    with tf.device(self.mpu):
+                        embed = self.model.calculate_embedding(i)
+                    if embedding is None:
+                        embedding = embed
+                    else:
+                        embedding = np.vstack([embedding, embed])
 
-        if graph is not None:
-            self.sampler = self.__init_sampler(graph, self.val_fraction, self.pos_enc_cls)
+                    if counter % 100 == 0:
+                        print("processed ", counter, " batches time: ", datetime.now())
 
-        embedding = None
-        counter = 0
-        for i in self.sampler.init_incr_batch(nodes):
-            counter += 1
-            try:
-                embed = self.model.calculate_embedding(i)
-                if embedding is None:
-                    embedding = embed
-                else:
-                    embedding = np.vstack([embedding, embed])
+                except tf.errors.OutOfRangeError:
+                    break
 
-                if counter % 100 == 0:
-                    print("processed ", counter, " batches time: ", datetime.now())
-
-            except tf.errors.OutOfRangeError:
-                break
-
-        if verbose:
-            print("reached end of batch")
+            if verbose:
+                print("reached end of batch")
         return embedding
 
     def save_model(self, save_path):
         """
         Saves the model. Note that a reloaded model can only be called.
 
         Args:
@@ -236,50 +241,52 @@
             layer_wise: Boolean to indicate whether the model needs to trained layer by layer or
                         all at once.
             epochs: Number of epochs used for training.
 
         Returns:
             Dict with the training results.
         """
-        hist = {}
-        if verbose is not None:
-            self.verbose = verbose
-        model_verbose = 1 if self.verbose else 0
-
-        if graph is not None:
-            self.sampler = self.__init_sampler(graph, self.val_fraction)
-
-        layers = [None]
-        if layer_wise:
-            layers = [i for i in range(len(self.dims))] + layers
-
-        for _, l in enumerate(layers):
-            self.model.sub_model_layer = l
-            self.sampler.init_train_batch()
-            train_data = self.sampler.get_train_samples()
-            validation_data = self.sampler.get_val_samples()
-
-            train_epoch_size, val_epoch_size = self.sampler.get_epoch_sizes()
-            steps_per_epoch = int(train_epoch_size / self.batch_size)
-            assert steps_per_epoch>0, "batch_size greater then 1 train epoch"
-            validation_steps = int(val_epoch_size / self.batch_size)
-            assert validation_steps>0, "batch_size greater then 1 validation epoch"
-            # early_stop = tf.keras.callbacks.EarlyStopping(
-            #     monitor='val_loss', min_delta=0, patience=3, verbose=0
-            # )
-            history = self.model.fit(
-                train_data,
-                validation_data=validation_data,
-                epochs=epochs,
-                verbose=model_verbose,
-                steps_per_epoch=steps_per_epoch,
-                validation_steps=validation_steps,
-                # callbacks=[early_stop]
-            )
-            hist[l] = history
+        with tf.device(self.cpu):
+            hist = {}
+            if verbose is not None:
+                self.verbose = verbose
+            model_verbose = 1 if self.verbose else 0
+
+            if graph is not None:
+                self.sampler = self.__init_sampler(graph, self.val_fraction)
+
+            layers = [None]
+            if layer_wise:
+                layers = [i for i in range(len(self.dims))] + layers
+
+            for _, l in enumerate(layers):
+                self.model.sub_model_layer = l
+                self.sampler.init_train_batch()
+                train_data = self.sampler.get_train_samples()
+                validation_data = self.sampler.get_val_samples()
+
+                train_epoch_size, val_epoch_size = self.sampler.get_epoch_sizes()
+                steps_per_epoch = int(train_epoch_size / self.batch_size)
+                assert steps_per_epoch>0, "batch_size greater then 1 train epoch"
+                validation_steps = int(val_epoch_size / self.batch_size)
+                assert validation_steps>0, "batch_size greater then 1 validation epoch"
+                # early_stop = tf.keras.callbacks.EarlyStopping(
+                #     monitor='val_loss', min_delta=0, patience=3, verbose=0
+                # )
+                with tf.device(self.mpu):
+                    history = self.model.fit(
+                        train_data,
+                        validation_data=validation_data,
+                        epochs=epochs,
+                        verbose=model_verbose,
+                        steps_per_epoch=steps_per_epoch,
+                        validation_steps=validation_steps,
+                        # callbacks=[early_stop]
+                    )
+                hist[l] = history
         return hist
 
     def fit_supervised(
         self, label_name, model, compiler_dict, train_dict, graph=None, verbose=None):
         """
         expends the GAE with a supervised model and trains the model and the given graph or if
         none is provide the current graph.
@@ -387,7 +394,17 @@
             return feat_out, df_out, recon_graph
 
         if incl_graph == 'pyvis':
             nt = graph_rec.show_pyvis(recon_graph)
             return feat_out, df_out, nt
 
         return feat_out, df_out, None
+    
+    def determine_mpu(self):
+        """ determine the gpu and cpu name"""
+        devices = tf.config.list_logical_devices()
+        GPUs = [d for d in devices if d.device_type=='GPU']
+        CPUs = [d for d in devices if d.device_type=='CPU']
+        if len(GPUs)>0:
+            return (GPUs[0].name, CPUs[0].name)
+        else:
+            return (CPUs[0].name, CPUs[0].name)
```

### Comparing `GraphCASE-0.0.7/GAE/graph_case_tools.py` & `GraphCASE-0.0.8/GAE/graph_case_tools.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.7/GAE/graph_reconstructor.py` & `GraphCASE-0.0.8/GAE/graph_reconstructor.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.7/GAE/input_layer_constructor.py` & `GraphCASE-0.0.8/GAE/input_layer_constructor.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.7/GAE/model.py` & `GraphCASE-0.0.8/GAE/model.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.7/GAE/position_manager.py` & `GraphCASE-0.0.8/GAE/position_manager.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.7/GAE/transformation_layer.py` & `GraphCASE-0.0.8/GAE/transformation_layer.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.7/LICENSE.txt` & `GraphCASE-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.7/README.md` & `GraphCASE-0.0.8/README.md`

 * *Files identical despite different names*

