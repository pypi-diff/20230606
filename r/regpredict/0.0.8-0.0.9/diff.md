# Comparing `tmp/regpredict-0.0.8.tar.gz` & `tmp/regpredict-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nr/Desktop/portfolio/projects/python/regpredict/dist/tmpk0bw7ve9/regpredict-0.0.8.tar", last modified: Sat Jan 22 13:36:28 2022, max compression
+gzip compressed data, was "regpredict-0.0.9.tar", last modified: Sun Mar 27 19:09:13 2022, max compression
```

## Comparing `regpredict-0.0.8.tar` & `regpredict-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 nr        (1000) nr        (1000)        0 2022-01-22 13:36:28.000000 regpredict-0.0.8/
--rw-rw-r--   0 nr        (1000) nr        (1000)     1058 2022-01-22 13:07:16.000000 regpredict-0.0.8/LICENSE
--rw-rw-r--   0 nr        (1000) nr        (1000)       99 2021-08-24 13:19:45.000000 regpredict-0.0.8/MANIFEST.in
--rw-rw-r--   0 nr        (1000) nr        (1000)     1220 2022-01-22 13:36:28.000000 regpredict-0.0.8/PKG-INFO
--rw-rw-r--   0 nr        (1000) nr        (1000)      700 2022-01-22 13:16:52.000000 regpredict-0.0.8/README.md
--rw-rw-r--   0 nr        (1000) nr        (1000)      135 2022-01-22 13:12:26.000000 regpredict-0.0.8/pyproject.toml
--rw-rw-r--   0 nr        (1000) nr        (1000)      689 2022-01-22 13:36:28.000000 regpredict-0.0.8/setup.cfg
--rw-rw-r--   0 nr        (1000) nr        (1000)      717 2022-01-22 13:20:01.000000 regpredict-0.0.8/setup.py
-drwxrwxr-x   0 nr        (1000) nr        (1000)        0 2022-01-22 13:36:28.000000 regpredict-0.0.8/src/
-drwxrwxr-x   0 nr        (1000) nr        (1000)        0 2022-01-22 13:36:28.000000 regpredict-0.0.8/src/regpredict/
--rw-rw-r--   0 nr        (1000) nr        (1000)        1 2021-08-24 10:07:15.000000 regpredict-0.0.8/src/regpredict/__init__.py
--rw-rw-r--   0 nr        (1000) nr        (1000)   219740 2022-01-22 13:14:43.000000 regpredict-0.0.8/src/regpredict/finalized_model.h5
--rw-rw-r--   0 nr        (1000) nr        (1000)      488 2022-01-22 13:14:54.000000 regpredict-0.0.8/src/regpredict/logscaler.gz
--rw-rw-r--   0 nr        (1000) nr        (1000)     1225 2022-01-22 13:05:09.000000 regpredict-0.0.8/src/regpredict/regbot.py
-drwxrwxr-x   0 nr        (1000) nr        (1000)        0 2022-01-22 13:36:28.000000 regpredict-0.0.8/src/regpredict.egg-info/
--rw-rw-r--   0 nr        (1000) nr        (1000)     1220 2022-01-22 13:36:28.000000 regpredict-0.0.8/src/regpredict.egg-info/PKG-INFO
--rw-rw-r--   0 nr        (1000) nr        (1000)      366 2022-01-22 13:36:28.000000 regpredict-0.0.8/src/regpredict.egg-info/SOURCES.txt
--rw-rw-r--   0 nr        (1000) nr        (1000)        1 2022-01-22 13:36:28.000000 regpredict-0.0.8/src/regpredict.egg-info/dependency_links.txt
--rw-rw-r--   0 nr        (1000) nr        (1000)       38 2022-01-22 13:36:28.000000 regpredict-0.0.8/src/regpredict.egg-info/requires.txt
--rw-rw-r--   0 nr        (1000) nr        (1000)       11 2022-01-22 13:36:28.000000 regpredict-0.0.8/src/regpredict.egg-info/top_level.txt
+drwxrwxr-x   0 defi      (1000) defi      (1000)        0 2022-03-27 19:09:13.730278 regpredict-0.0.9/
+-rwxrwxr-x   0 defi      (1000) defi      (1000)     1058 2022-03-27 15:48:08.000000 regpredict-0.0.9/LICENSE
+-rwxrwxr-x   0 defi      (1000) defi      (1000)       99 2022-03-27 15:48:08.000000 regpredict-0.0.9/MANIFEST.in
+-rw-rw-r--   0 defi      (1000) defi      (1000)     1237 2022-03-27 19:09:13.730278 regpredict-0.0.9/PKG-INFO
+-rwxrwxr-x   0 defi      (1000) defi      (1000)      717 2022-03-27 19:05:42.000000 regpredict-0.0.9/README.md
+-rwxrwxr-x   0 defi      (1000) defi      (1000)      135 2022-03-27 15:48:08.000000 regpredict-0.0.9/pyproject.toml
+-rwxrwxr-x   0 defi      (1000) defi      (1000)      689 2022-03-27 19:09:13.730278 regpredict-0.0.9/setup.cfg
+-rwxrwxr-x   0 defi      (1000) defi      (1000)      717 2022-03-27 19:06:48.000000 regpredict-0.0.9/setup.py
+drwxrwxr-x   0 defi      (1000) defi      (1000)        0 2022-03-27 19:09:13.730278 regpredict-0.0.9/src/
+drwxrwxr-x   0 defi      (1000) defi      (1000)        0 2022-03-27 19:09:13.730278 regpredict-0.0.9/src/regpredict/
+-rwxrwxr-x   0 defi      (1000) defi      (1000)        1 2022-03-27 15:48:08.000000 regpredict-0.0.9/src/regpredict/__init__.py
+-rw-rw-r--   0 defi      (1000) defi      (1000)   507911 2022-03-27 15:28:06.000000 regpredict-0.0.9/src/regpredict/finalized_model.h5
+-rw-rw-r--   0 defi      (1000) defi      (1000)      521 2022-03-27 15:14:31.000000 regpredict-0.0.9/src/regpredict/logscaler.gz
+-rwxrwxr-x   0 defi      (1000) defi      (1000)     1146 2022-03-27 17:40:28.000000 regpredict-0.0.9/src/regpredict/regbot.py
+-rw-rw-r--   0 defi      (1000) defi      (1000)      310 2022-03-27 18:30:49.000000 regpredict-0.0.9/src/regpredict/test.py
+drwxrwxr-x   0 defi      (1000) defi      (1000)        0 2022-03-27 19:09:13.730278 regpredict-0.0.9/src/regpredict.egg-info/
+-rw-rw-r--   0 defi      (1000) defi      (1000)     1237 2022-03-27 19:09:13.000000 regpredict-0.0.9/src/regpredict.egg-info/PKG-INFO
+-rw-rw-r--   0 defi      (1000) defi      (1000)      389 2022-03-27 19:09:13.000000 regpredict-0.0.9/src/regpredict.egg-info/SOURCES.txt
+-rw-rw-r--   0 defi      (1000) defi      (1000)        1 2022-03-27 19:09:13.000000 regpredict-0.0.9/src/regpredict.egg-info/dependency_links.txt
+-rw-rw-r--   0 defi      (1000) defi      (1000)       38 2022-03-27 19:09:13.000000 regpredict-0.0.9/src/regpredict.egg-info/requires.txt
+-rw-rw-r--   0 defi      (1000) defi      (1000)       11 2022-03-27 19:09:13.000000 regpredict-0.0.9/src/regpredict.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `regpredict-0.0.8/LICENSE` & `regpredict-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `regpredict-0.0.8/PKG-INFO` & `regpredict-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: regpredict
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for predicting buy and sell signals
 Home-page: https://nkrtech.com
+Download-URL: https://github.com/moinonin/evxpredictor/archive/refs/heads/main.zip
 Author: Nicolus Rotich
 Author-email: nicholas.rotich@gmail.com
 License: MIT
-Download-URL: https://github.com/moinonin/evxpredictor/archive/refs/heads/main.zip
 Project-URL: Bug Tracker, https://github.com/pypa/regpredict/issues
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,12 +20,12 @@
 You can read more about EVX in the whitepaper [here](https://www.researchgate.net/publication/345313655_DeFiPaper)
 
 # Usage
 
 In your python script simply import the module and use as follows  
 from regpredict import regbot
 
-print(regbot.signal(20,65,120))
+print(regbot.signal(20,65,0.4587))
 
-The above methods take an assets opening, closing, and volume of the asset based on the time interval you have chosen. A zero classification output would instruct the user not to buy or sell the asset if it is registerd in the database, while one output means buy the asset.
+The above methods take an assets opening, closing, and bids volume fraction of the asset based on the time interval you have chosen. A zero classification output would instruct the user not to buy or sell the asset if it is registerd in the database, while one output means buy the asset.
```

### Comparing `regpredict-0.0.8/README.md` & `regpredict-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,10 +4,10 @@
 You can read more about EVX in the whitepaper [here](https://www.researchgate.net/publication/345313655_DeFiPaper)
 
 # Usage
 
 In your python script simply import the module and use as follows  
 from regpredict import regbot
 
-print(regbot.signal(20,65,120))
+print(regbot.signal(20,65,0.4587))
 
-The above methods take an assets opening, closing, and volume of the asset based on the time interval you have chosen. A zero classification output would instruct the user not to buy or sell the asset if it is registerd in the database, while one output means buy the asset.
+The above methods take an assets opening, closing, and bids volume fraction of the asset based on the time interval you have chosen. A zero classification output would instruct the user not to buy or sell the asset if it is registerd in the database, while one output means buy the asset.
```

### Comparing `regpredict-0.0.8/setup.cfg` & `regpredict-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = regpredict
-version = 0.0.8
+version = 0.0.9
 author = Nicolus Rotich
 author_email = nicholas.rotich@gmail.com
 description = A package for predicting buy and sell signals based on excess volume index(EVX) algorithm
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/moinonin/regpredict
 project_urls =
```

### Comparing `regpredict-0.0.8/setup.py` & `regpredict-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from distutils.core import setup, find_packages
 
 setup(
     name='regpredict',
     packages=find_packages(),
     include_package_data=True,
     platforms='any',
-    version='0.0.8',
+    version='0.0.9',
     description='A package for predicting buy and sell signals',
     license='MIT',
     author='Nicolus Rotich',
     author_email='nicholas.rotich@gmail.com',
     install_requires=[
     	"setuptools>=57",
     	"wheel",
```

### Comparing `regpredict-0.0.8/src/regpredict/regbot.py` & `regpredict-0.0.9/src/regpredict/regbot.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,36 +15,34 @@
   	self.model_scaler_path = model_scaler_path
 
   @classmethod
   def loadmodel(cls):
     loaded_model = joblib.load(open(f'{cls.reg_model_path}', 'rb'))
     return loaded_model
 
-
   @classmethod
-  def prepareInput(cls,opening,closing,volume):
-  	ask_ind = closing*volume/(opening + closing)
-  	bid_ind = opening*volume/(opening + closing)
-  	testdata = np.array([[ask_ind,bid_ind]])
+  def prepareInput(cls,opening,closing,bvr):
+  	bvr = opening/(opening + closing)
+  	testdata = np.array([[opening,closing,bvr]])
   	scaler = joblib.load(f'{cls.model_scaler_path}')
   	testdata = scaler.transform(testdata)
 
   	return testdata
 
 
   @classmethod
-  def buySignalGenerator(cls,opening,closing,volume):
-    scalledInput = cls.prepareInput(opening,closing,volume)
-    return cls.loadmodel().predict(scalledInput)[0].round()
+  def buySignalGenerator(cls,opening,closing,bvr):
+    scalledInput = cls.prepareInput(opening,closing,bvr)
+    return cls.loadmodel().predict(scalledInput)[0]
 
 
 
 
-def signal(opening,closing,volume):
+def signal(opening,closing,bvr):
   try:
-    return Regbot.buySignalGenerator(opening,closing,volume)
+    return Regbot.buySignalGenerator(opening,closing,bvr)
   except Exception as e:
     print(e)
 
 
 if __name__ == '__main__':
   fire.Fire(signal)
```

### Comparing `regpredict-0.0.8/src/regpredict.egg-info/PKG-INFO` & `regpredict-0.0.9/src/regpredict.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: regpredict
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for predicting buy and sell signals
 Home-page: https://nkrtech.com
+Download-URL: https://github.com/moinonin/evxpredictor/archive/refs/heads/main.zip
 Author: Nicolus Rotich
 Author-email: nicholas.rotich@gmail.com
 License: MIT
-Download-URL: https://github.com/moinonin/evxpredictor/archive/refs/heads/main.zip
 Project-URL: Bug Tracker, https://github.com/pypa/regpredict/issues
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,12 +20,12 @@
 You can read more about EVX in the whitepaper [here](https://www.researchgate.net/publication/345313655_DeFiPaper)
 
 # Usage
 
 In your python script simply import the module and use as follows  
 from regpredict import regbot
 
-print(regbot.signal(20,65,120))
+print(regbot.signal(20,65,0.4587))
 
-The above methods take an assets opening, closing, and volume of the asset based on the time interval you have chosen. A zero classification output would instruct the user not to buy or sell the asset if it is registerd in the database, while one output means buy the asset.
+The above methods take an assets opening, closing, and bids volume fraction of the asset based on the time interval you have chosen. A zero classification output would instruct the user not to buy or sell the asset if it is registerd in the database, while one output means buy the asset.
```

