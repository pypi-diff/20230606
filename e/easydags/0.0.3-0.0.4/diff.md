# Comparing `tmp/easydags-0.0.3.tar.gz` & `tmp/easydags-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydags-0.0.3.tar", last modified: Tue Jun  6 08:01:24 2023, max compression
+gzip compressed data, was "easydags-0.0.4.tar", last modified: Tue Jun  6 15:18:26 2023, max compression
```

## Comparing `easydags-0.0.3.tar` & `easydags-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 08:01:24.032981 easydags-0.0.3/
--rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.3/LICENSE
--rw-r--r--   0 mateograciano   (501) staff       (20)     9014 2023-06-06 08:01:24.032770 easydags-0.0.3/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)     8775 2023-06-06 07:48:07.000000 easydags-0.0.3/README.md
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 08:01:24.031892 easydags-0.0.3/easydags/
--rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.3/easydags/__init__.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.3/easydags/config.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    21593 2023-06-03 18:40:29.000000 easydags-0.0.3/easydags/dag.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.3/easydags/errors.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    10737 2023-06-03 09:24:23.000000 easydags-0.0.3/easydags/node.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.3/easydags/ops.py
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 08:01:24.032599 easydags-0.0.3/easydags.egg-info/
--rw-r--r--   0 mateograciano   (501) staff       (20)     9014 2023-06-06 08:01:23.000000 easydags-0.0.3/easydags.egg-info/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-06 08:01:24.000000 easydags-0.0.3/easydags.egg-info/SOURCES.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-06 08:01:24.000000 easydags-0.0.3/easydags.egg-info/dependency_links.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-06 08:01:24.000000 easydags-0.0.3/easydags.egg-info/requires.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-06 08:01:24.000000 easydags-0.0.3/easydags.egg-info/top_level.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)      104 2023-06-06 07:55:47.000000 easydags-0.0.3/pyproject.toml
--rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-06 08:01:24.033019 easydags-0.0.3/setup.cfg
--rw-r--r--   0 mateograciano   (501) staff       (20)     1011 2023-06-06 08:01:21.000000 easydags-0.0.3/setup.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 15:18:26.257042 easydags-0.0.4/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.4/LICENSE
+-rw-r--r--   0 mateograciano   (501) staff       (20)    12166 2023-06-06 15:18:26.256843 easydags-0.0.4/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)    11971 2023-06-06 14:56:55.000000 easydags-0.0.4/README.md
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 15:18:26.255995 easydags-0.0.4/easydags/
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.4/easydags/__init__.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.4/easydags/config.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    21593 2023-06-03 18:40:29.000000 easydags-0.0.4/easydags/dag.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.4/easydags/errors.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    10737 2023-06-03 09:24:23.000000 easydags-0.0.4/easydags/node.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.4/easydags/ops.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 15:18:26.256686 easydags-0.0.4/easydags.egg-info/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    12166 2023-06-06 15:18:26.000000 easydags-0.0.4/easydags.egg-info/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-06 15:18:26.000000 easydags-0.0.4/easydags.egg-info/SOURCES.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-06 15:18:26.000000 easydags-0.0.4/easydags.egg-info/dependency_links.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-06 15:18:26.000000 easydags-0.0.4/easydags.egg-info/requires.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-06 15:18:26.000000 easydags-0.0.4/easydags.egg-info/top_level.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)      104 2023-06-06 07:55:47.000000 easydags-0.0.4/pyproject.toml
+-rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-06 15:18:26.257084 easydags-0.0.4/setup.cfg
+-rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-06 15:18:12.000000 easydags-0.0.4/setup.py
```

### Comparing `easydags-0.0.3/LICENSE` & `easydags-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easydags-0.0.3/PKG-INFO` & `easydags-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Metadata-Version: 2.1
-Name: easydags
-Version: 0.0.3
-Summary: Dags made easy
-Author: Mateo Graciano
-Author-email: magralo@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Easydags: DAGs made easy
 
 This library heavily inspired this package: https://github.com/mindee/tawazi, and a little bit by Airflow.
 
+
+## Easy install using pypi
+You can easily install this in a separate conda envioronment with the following:
+
+```bash
+conda create -n easydags python=3.10 -y
+conda activate easydags
+pip install easydags
+```
+
+Now you can run your DAG's on your local envioronment
+
 ## Define a DAG
 
 Maybe all of you already know what a Directed Acyclic Graph (DAG) is..., but please think about this definition when using this library:
 
 
 A DAG represents a collection of tasks you want to run; this is also organized to show relationships between tasks.
 
@@ -278,7 +280,144 @@
 ```python
 
 node = ExecNode(id_= 'id',
               exec_function = your_function,
               n_trials= 3 # set number of trials
               )
 ```
+
+
+## Deploying your DAGs
+
+#### Deploying on serverless (GCP example)
+
+Basically the idea is that you can run one API where each endpoint is a different dag... as an example you can have the following api_example.py
+
+```python 
+
+from fastapi import FastAPI
+from easydags import  ExecNode, DAG
+import time
+
+app = FastAPI()
+
+
+@app.get("/dag1")
+async def dag1():
+
+    nodes = []
+
+
+    def example0():
+        print('beginning 0')
+        time.sleep(3)
+        print('end 0')
+        return 4
+
+    nodes.append( ExecNode(id_= 'f0',
+                exec_function = example0
+                ) )  
+
+    def example1(**kwargs):
+        f0_result = kwargs['f0_result']
+        print('beginning 1')
+        print('end 1')
+        print(f0_result + 8 )
+
+    nodes.append( ExecNode(id_= 'f1',
+                exec_function = example1 ,
+                depends_on_hard= ['f0']
+                ) )   
+
+
+
+    
+    dag = DAG(nodes,name = 'Example DAG hard dependency',max_concurrency=8, debug = False)
+
+    dag.execute()
+
+    #DO SOMETHING WITH "Example DAG hard dependency_states_run.html" in case you need it
+
+    return {"message": "Updated!"}
+
+@app.get("/dag2")
+async def dag2():
+
+    nodes = []
+    def prepro():
+        print('beginning pre pro')
+        time.sleep(3)
+        print('end pre pro')
+        return 'df with cool features'
+
+
+
+    nodes.append( ExecNode(id_= 'pre_process',
+                exec_function = prepro,
+                output_name = 'my_cool_df'
+                ) )  
+
+
+    def model1(**kwargs):
+        df = kwargs['my_cool_df']
+        
+        print(f'i am using {df} in model 1')
+        time.sleep(3)
+        print('finish training model1')
+        
+        return 'model 1 37803'
+
+    nodes.append( ExecNode(id_= 'model1',
+                exec_function = model1 ,
+                depends_on_hard= ['pre_process'],
+                output_name = 'model1'
+                ) )   
+
+
+
+    def model2(**kwargs):
+        df = kwargs['my_cool_df']
+        
+        print(f'i am using {df} in model 2')
+        time.sleep(3)
+        print('finished training model2')
+        
+        return 'model 2 78373'
+
+    nodes.append( ExecNode(id_= 'model2',
+                exec_function = model2 ,
+                depends_on_hard= ['pre_process'],
+                output_name = 'model2'
+                ) )  
+
+
+
+    def ensemble(**kwargs):
+        model1 = kwargs['model1']
+        model2 = kwargs['model2']
+        
+        result = f'{model1} and {model2}'
+        
+        print(result)
+        
+        return result 
+
+    nodes.append( ExecNode(id_= 'ensemble',
+                exec_function = ensemble ,
+                depends_on_hard= ['model1','model2'],
+                output_name = 'ensemble'
+                ) )  
+
+
+
+    dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
+
+    dag.execute()
+
+    return {"message": "Updated!"}
+
+@app.get("/ready")
+async def ready():
+    return {"ready"}
+
+
+```
```

### Comparing `easydags-0.0.3/easydags/dag.py` & `easydags-0.0.4/easydags/dag.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.3/easydags/node.py` & `easydags-0.0.4/easydags/node.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.3/easydags/ops.py` & `easydags-0.0.4/easydags/ops.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.3/easydags.egg-info/PKG-INFO` & `easydags-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 Metadata-Version: 2.1
 Name: easydags
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dags made easy
 Author: Mateo Graciano
 Author-email: magralo@gmail.com
-Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easydags: DAGs made easy
 
 This library heavily inspired this package: https://github.com/mindee/tawazi, and a little bit by Airflow.
 
+
+## Easy install using pypi
+You can easily install this in a separate conda envioronment with the following:
+
+```bash
+conda create -n easydags python=3.10 -y
+conda activate easydags
+pip install easydags
+```
+
+Now you can run your DAG's on your local envioronment
+
 ## Define a DAG
 
 Maybe all of you already know what a Directed Acyclic Graph (DAG) is..., but please think about this definition when using this library:
 
 
 A DAG represents a collection of tasks you want to run; this is also organized to show relationships between tasks.
 
@@ -278,7 +289,144 @@
 ```python
 
 node = ExecNode(id_= 'id',
               exec_function = your_function,
               n_trials= 3 # set number of trials
               )
 ```
+
+
+## Deploying your DAGs
+
+#### Deploying on serverless (GCP example)
+
+Basically the idea is that you can run one API where each endpoint is a different dag... as an example you can have the following api_example.py
+
+```python 
+
+from fastapi import FastAPI
+from easydags import  ExecNode, DAG
+import time
+
+app = FastAPI()
+
+
+@app.get("/dag1")
+async def dag1():
+
+    nodes = []
+
+
+    def example0():
+        print('beginning 0')
+        time.sleep(3)
+        print('end 0')
+        return 4
+
+    nodes.append( ExecNode(id_= 'f0',
+                exec_function = example0
+                ) )  
+
+    def example1(**kwargs):
+        f0_result = kwargs['f0_result']
+        print('beginning 1')
+        print('end 1')
+        print(f0_result + 8 )
+
+    nodes.append( ExecNode(id_= 'f1',
+                exec_function = example1 ,
+                depends_on_hard= ['f0']
+                ) )   
+
+
+
+    
+    dag = DAG(nodes,name = 'Example DAG hard dependency',max_concurrency=8, debug = False)
+
+    dag.execute()
+
+    #DO SOMETHING WITH "Example DAG hard dependency_states_run.html" in case you need it
+
+    return {"message": "Updated!"}
+
+@app.get("/dag2")
+async def dag2():
+
+    nodes = []
+    def prepro():
+        print('beginning pre pro')
+        time.sleep(3)
+        print('end pre pro')
+        return 'df with cool features'
+
+
+
+    nodes.append( ExecNode(id_= 'pre_process',
+                exec_function = prepro,
+                output_name = 'my_cool_df'
+                ) )  
+
+
+    def model1(**kwargs):
+        df = kwargs['my_cool_df']
+        
+        print(f'i am using {df} in model 1')
+        time.sleep(3)
+        print('finish training model1')
+        
+        return 'model 1 37803'
+
+    nodes.append( ExecNode(id_= 'model1',
+                exec_function = model1 ,
+                depends_on_hard= ['pre_process'],
+                output_name = 'model1'
+                ) )   
+
+
+
+    def model2(**kwargs):
+        df = kwargs['my_cool_df']
+        
+        print(f'i am using {df} in model 2')
+        time.sleep(3)
+        print('finished training model2')
+        
+        return 'model 2 78373'
+
+    nodes.append( ExecNode(id_= 'model2',
+                exec_function = model2 ,
+                depends_on_hard= ['pre_process'],
+                output_name = 'model2'
+                ) )  
+
+
+
+    def ensemble(**kwargs):
+        model1 = kwargs['model1']
+        model2 = kwargs['model2']
+        
+        result = f'{model1} and {model2}'
+        
+        print(result)
+        
+        return result 
+
+    nodes.append( ExecNode(id_= 'ensemble',
+                exec_function = ensemble ,
+                depends_on_hard= ['model1','model2'],
+                output_name = 'ensemble'
+                ) )  
+
+
+
+    dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
+
+    dag.execute()
+
+    return {"message": "Updated!"}
+
+@app.get("/ready")
+async def ready():
+    return {"ready"}
+
+
+```
```

### Comparing `easydags-0.0.3/setup.py` & `easydags-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'easydags',         # How you named your package folder (MyLib)
   packages = ['easydags'],   # Chose the same as "name"
-  version = '0.0.3',      # Start with a small number and increase it with every change you make
+  version = '0.0.4',      # Start with a small number and increase it with every change you make
   description = 'Dags made easy',   # Give a short description about your library
   author = 'Mateo Graciano',                   # Type in your name
   author_email = 'magralo@gmail.com',      # Type in your E-Mail
   install_requires=[            # I get to this in a second
           'networkx==2.6.3',
           'pydantic==1.10',
           'loguru==0.6.0',
           'matplotlib==3.6.3',
           'pyvis==0.3.1'
       ],
   long_description=long_description,
   long_description_content_type='text/markdown',
-  classifiers=[
-    'Development Status :: 3 - Alpha',      
-  ],
 )
```

