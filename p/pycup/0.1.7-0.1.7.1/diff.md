# Comparing `tmp/pycup-0.1.7.tar.gz` & `tmp/pycup-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pycup-0.1.7.tar", last modified: Mon Jun  5 15:17:06 2023, max compression
+gzip compressed data, was "dist\pycup-0.1.7.1.tar", last modified: Tue Jun  6 07:15:25 2023, max compression
```

## Comparing `pycup-0.1.7.tar` & `pycup-0.1.7.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 15:17:06.656476 pycup-0.1.7/
--rw-rw-rw-   0        0        0     6366 2023-06-05 15:17:06.655476 pycup-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     5112 2023-06-05 15:14:54.000000 pycup-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 15:17:06.641472 pycup-0.1.7/pycup/
--rw-rw-rw-   0        0        0    17161 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/GLUE.py
--rw-rw-rw-   0        0        0    38271 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/GWO.py
--rw-rw-rw-   0        0        0    33260 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/MFO.py
--rw-rw-rw-   0        0        0    14600 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/MODE.py
--rw-rw-rw-   0        0        0    26156 2023-06-05 14:09:02.000000 pycup-0.1.7/pycup/MOMFO.py
--rw-rw-rw-   0        0        0    24212 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/MOPSO.py
--rw-rw-rw-   0        0        0    14937 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/NSGA2.py
--rw-rw-rw-   0        0        0    19287 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/PESTclasses.py
--rw-rw-rw-   0        0        0    35498 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/PSO.py
--rw-rw-rw-   0        0        0    15659 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/Reslib.py
--rw-rw-rw-   0        0        0    30073 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/SCA.py
--rw-rw-rw-   0        0        0    32941 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/SOA.py
--rw-rw-rw-   0        0        0    32160 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/SSA.py
--rw-rw-rw-   0        0        0     5757 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/TOPSIS.py
--rw-rw-rw-   0        0        0    33343 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/TSA.py
--rw-rw-rw-   0        0        0    32912 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/WOA.py
--rw-rw-rw-   0        0        0      975 2023-06-05 14:17:37.000000 pycup-0.1.7/pycup/__init__.py
--rw-rw-rw-   0        0        0    10042 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/calc_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:17:06.652475 pycup-0.1.7/pycup/document/
--rw-rw-rw-   0        0        0   826264 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/document/Documentation.pdf
--rw-rw-rw-   0        0        0     4027 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/evaluation_metrics.py
--rw-rw-rw-   0        0        0    53886 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/integrate.py
--rw-rw-rw-   0        0        0     7263 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/multi_jobs.py
--rw-rw-rw-   0        0        0   125408 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/plot.py
--rw-rw-rw-   0        0        0      460 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/progress_bar.py
--rw-rw-rw-   0        0        0    10352 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/sampling.py
--rw-rw-rw-   0        0        0    19081 2023-06-05 14:17:37.000000 pycup-0.1.7/pycup/save.py
--rw-rw-rw-   0        0        0     2068 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/template.py
--rw-rw-rw-   0        0        0        0 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/test.py
--rw-rw-rw-   0        0        0     6055 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/test_functions.py
--rw-rw-rw-   0        0        0    69170 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/uncertainty_analysis_fun.py
--rw-rw-rw-   0        0        0    17048 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/utilize.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:17:06.650474 pycup-0.1.7/pycup.egg-info/
--rw-rw-rw-   0        0        0     6366 2023-06-05 15:17:06.000000 pycup-0.1.7/pycup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-06-05 15:17:06.000000 pycup-0.1.7/pycup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 15:17:06.000000 pycup-0.1.7/pycup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-05 15:17:06.000000 pycup-0.1.7/pycup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 15:17:06.000000 pycup-0.1.7/pycup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 15:17:06.656476 pycup-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-06-05 14:17:37.000000 pycup-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:15:25.190031 pycup-0.1.7.1/
+-rw-rw-rw-   0        0        0     6368 2023-06-06 07:15:25.189930 pycup-0.1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5112 2023-06-05 15:14:54.000000 pycup-0.1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 07:15:25.173926 pycup-0.1.7.1/pycup/
+-rw-rw-rw-   0        0        0    17161 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/GLUE.py
+-rw-rw-rw-   0        0        0    38271 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/GWO.py
+-rw-rw-rw-   0        0        0    32971 2023-06-05 15:19:02.000000 pycup-0.1.7.1/pycup/MFO.py
+-rw-rw-rw-   0        0        0    14600 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/MODE.py
+-rw-rw-rw-   0        0        0    25532 2023-06-06 07:13:42.000000 pycup-0.1.7.1/pycup/MOMFO.py
+-rw-rw-rw-   0        0        0    24212 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/MOPSO.py
+-rw-rw-rw-   0        0        0    14937 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/NSGA2.py
+-rw-rw-rw-   0        0        0    19287 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/PESTclasses.py
+-rw-rw-rw-   0        0        0    35498 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/PSO.py
+-rw-rw-rw-   0        0        0    15659 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/Reslib.py
+-rw-rw-rw-   0        0        0    30073 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/SCA.py
+-rw-rw-rw-   0        0        0    32941 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/SOA.py
+-rw-rw-rw-   0        0        0    32160 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/SSA.py
+-rw-rw-rw-   0        0        0     5757 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/TOPSIS.py
+-rw-rw-rw-   0        0        0    33343 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/TSA.py
+-rw-rw-rw-   0        0        0    32912 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/WOA.py
+-rw-rw-rw-   0        0        0      975 2023-06-05 14:17:37.000000 pycup-0.1.7.1/pycup/__init__.py
+-rw-rw-rw-   0        0        0    10042 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/calc_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:15:25.186508 pycup-0.1.7.1/pycup/document/
+-rw-rw-rw-   0        0        0   826264 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/document/Documentation.pdf
+-rw-rw-rw-   0        0        0     4027 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/evaluation_metrics.py
+-rw-rw-rw-   0        0        0    53886 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/integrate.py
+-rw-rw-rw-   0        0        0     7263 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/multi_jobs.py
+-rw-rw-rw-   0        0        0   125519 2023-06-06 07:11:27.000000 pycup-0.1.7.1/pycup/plot.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/progress_bar.py
+-rw-rw-rw-   0        0        0    10352 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/sampling.py
+-rw-rw-rw-   0        0        0    19081 2023-06-05 14:17:37.000000 pycup-0.1.7.1/pycup/save.py
+-rw-rw-rw-   0        0        0     2068 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/template.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/test.py
+-rw-rw-rw-   0        0        0     6055 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/test_functions.py
+-rw-rw-rw-   0        0        0    69170 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/uncertainty_analysis_fun.py
+-rw-rw-rw-   0        0        0    17048 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/utilize.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:15:25.182928 pycup-0.1.7.1/pycup.egg-info/
+-rw-rw-rw-   0        0        0     6368 2023-06-06 07:15:25.000000 pycup-0.1.7.1/pycup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-06-06 07:15:25.000000 pycup-0.1.7.1/pycup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 07:15:25.000000 pycup-0.1.7.1/pycup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-06 07:15:25.000000 pycup-0.1.7.1/pycup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 07:15:25.000000 pycup-0.1.7.1/pycup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 07:15:25.190031 pycup-0.1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      955 2023-06-06 07:13:42.000000 pycup-0.1.7.1/setup.py
```

### Comparing `pycup-0.1.7/PKG-INFO` & `pycup-0.1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycup
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.
 Home-page: https://github.com/QianyangWang/PyCUP
 Author: Qianyang Wang
 Author-email: wqy07010944@hotmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/QianyangWang/PyCUP/DOCUMENT
 Project-URL: Source, https://github.com/QianyangWang/PyCUP/pycup
```

### Comparing `pycup-0.1.7/README.md` & `pycup-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/GLUE.py` & `pycup-0.1.7.1/pycup/GLUE.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/GWO.py` & `pycup-0.1.7.1/pycup/GWO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/MFO.py` & `pycup-0.1.7.1/pycup/MFO.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,19 +191,15 @@
         Xm = np.concatenate([Xs,X],axis=0)
         fitnessM, sortIndexM = SortFitness(fitnessM)
         Xm = SortPosition(Xm, sortIndexM)
         # update the Xs (flame population)
         Xs = Xm[0:Flame_no,:]
         fitnessS = fitnessM[0:Flame_no]
 
-        """
-        Here I used the elite sample to replace the sample in X for saving, because that if 
-        fitOppo[j] < fitnessS[j] (the elite is better than the flame), it is better than any
-        of the sample in X. This will not affect the actual search process.
-        """
+
         X2file = copy.copy(X)
         fitness2file = copy.copy(fitness)
         res2file = copy.copy(res)
         if EliteOppoSwitch:
 
             EliteNumber = int(np.ceil(Xs.shape[0] * OppoFactor))
             if EliteNumber > 0:
```

### Comparing `pycup-0.1.7/pycup/MODE.py` & `pycup-0.1.7.1/pycup/MODE.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/MOMFO.py` & `pycup-0.1.7.1/pycup/MOMFO.py`

 * *Files 6% similar despite different names*

```diff
@@ -264,84 +264,63 @@
                 isCh[pIdx] = False
         archive = archive[isCh]
         arFits = arFits[isCh]
         arRes = arRes[isCh]
         return archive, arFits,arRes
 
 
-
-def initial_MV(pop, dims, ubs, lbs):
-    """
-    lhs sampling based initialization for multi-variable functions
-
-    :argument
-    pop: population size -> int
-    dims: num. parameters list -> [int, ..., int]
-    ub: upper boundaries list -> [np.array, ..., np.array]
-    lb: lower boundary list -> [np.array, ..., np.array]
-
-    :returns
-    Xs: a list of the updated samples/solutions
-    lbs: a list of upper boundaries
-    ubs: a lower boundaries
-    """
-    try:
-        Xs, lbs, ubs = eval("sampling.{}_samplingMV".format(Sampling))(pop=pop, dims=dims, ubs=ubs, lbs=lbs)
-    except:
-        raise KeyError("The selectable sampling strategies are: 'LHS','Random','Chebyshev','Circle','Logistic','Piecewise','Sine','Singer','Sinusoidal','Tent'.")
-
-    return Xs, lbs, ubs
-
-
 def run(pop, dim, lb, ub, MaxIter,n_obj,nAr,M, fun,RecordPath = None, args=()):
     """
     Main function for the algorithm
 
     :argument
     pop: population size -> int
     dim: num. parameters -> int
     ub: upper boundary -> np.array
     lb: lower boundary -> np.array
     MaxIter: num. of iterations. int
+    n_obj: number of objective functions -> int
+    nAr: archive size -> int
+    M: number of mesh grids -> int
     fun: The user defined objective function or function in pycup.test_functions. The function
          should return a fitness value and a calculation result. See pycup.test_functions for
          more information -> function variable
+    RecordPath: the path of the record file for a hot start -> str
     args: A tuple of arguments. Users can use it for obj_fun's customization. For example, the
           parameter file path and model file path can be stored in this tuple for further use.
           See the document for more details.
 
     :returns
-    GbestScore: The best fitness obtained by the algorithm.
-    GbestPositon: The sample which obtained the best fitness.
-    Curve: The optimization curve
     hs: Historical samples.
     hf: The fitness of historical samples.
     hr: The results of historical samples.
 
     Reference:
+    single objective version ->
     Mirjalili, S. (2015). Moth-flame optimization algorithm: A novel nature-inspired heuristic paradigm.
     Knowledge-Based Systems, 89, 228–249. https://doi.org/10.1016/j.knosys.2015.07.006
 
-    Notes:
-    The pseudo code in the original paper seems to has a little when updating the flame. Here we concatenate the moth
-    and flame and sort them to update the flame. By doing this, the global optimal position can always be stored in the
-    flame population.
+    bullets for multi objective modification ->
+    1. non-domination sort (used in almost all kinds of MO-algorithms)
+    2. corwding distance sort (used also in NSGA2). 1. and 2. were the criteria for sorting the flame population
+    3. archive (used also in MOPSO)
+    4. flame-based EOBL improvement (modified and proposed by Qianyang Wang in MFO, and converted to a non-domination version
+       by Qianyang Wang in MOMFO)
+
 
     Usage:
     import pycup as cp
+    from pycup.test_functions import ZDT4
 
-    def uni_fun1(X):
-        # X for example np.array([1,2,3,...,30])
-        fitness = np.sum(np.power(X,2)) + 1 # example: 1.2
-        result = fitness.reshape(1,-1) # example ([1.2,])
-        return fitness,result
-
-    lb = -100 * np.ones(30)
-    ub = 100 * np.ones(30)
-    cp.MFO.run(pop = 1000, dim = 30, lb = lb, ub = ub, MaxIter = 30, fun = uni_fun1)
+    dim = 10
+    lb = np.zeros(10)
+    ub = np.ones(10)
+    n_obj=2
+    cp.MOMFO.EliteOppoSwitch = True
+    cp.MOMFO.run(90,10,lb,ub,500,2,100,20,ZDT4)
     """
     print("Current Algorithm: MFO")
     print("Elite Opposition:{}".format(EliteOppoSwitch))
     print("Iterations: 1 (init.) + {}".format(MaxIter))
     print("Dim:{}".format(dim))
     print("Population:{}".format(pop))
     print("Lower Bnd.:{}".format(lb))
@@ -492,50 +471,54 @@
 
     :argument
     pop: population size -> int
     dim: num. parameters -> int
     ub: upper boundary -> np.array
     lb: lower boundary -> np.array
     MaxIter: num. of iterations. int
+    n_obj: number of objective functions -> int
+    nAr: archive size -> int
+    M: number of mesh grids -> int
     fun: The user defined objective function or function in pycup.test_functions. The function
          should return a fitness value and a calculation result. See pycup.test_functions for
          more information -> function variable
+    n_jobs: number of threads for multi-processing optimization -> int
+    RecordPath: the path of the record file for a hot start -> str
     args: A tuple of arguments. Users can use it for obj_fun's customization. For example, the
           parameter file path and model file path can be stored in this tuple for further use.
           See the document for more details.
 
     :returns
-    GbestScore: The best fitness obtained by the algorithm.
-    GbestPositon: The sample which obtained the best fitness.
-    Curve: The optimization curve
     hs: Historical samples.
     hf: The fitness of historical samples.
     hr: The results of historical samples.
 
     Reference:
+    single objective version ->
     Mirjalili, S. (2015). Moth-flame optimization algorithm: A novel nature-inspired heuristic paradigm.
     Knowledge-Based Systems, 89, 228–249. https://doi.org/10.1016/j.knosys.2015.07.006
 
-    Notes:
-    The pseudo code in the original paper seems to has a little when updating the flame. Here we concatenate the moth
-    and flame and sort them to update the flame. By doing this, the global optimal position can always be stored in the
-    flame population.
+    bullets for multi objective modification ->
+    1. non-domination sort (used in almost all kinds of MO-algorithms)
+    2. corwding distance sort (used also in NSGA2). 1. and 2. were the criteria for sorting the flame population
+    3. archive (used also in MOPSO)
+    4. flame-based EOBL improvement (modified and proposed by Qianyang Wang in MFO, and converted to a non-domination version
+       by Qianyang Wang in MOMFO)
+
 
     Usage:
     import pycup as cp
+    from pycup.test_functions import ZDT4
 
-    def uni_fun1(X):
-        # X for example np.array([1,2,3,...,30])
-        fitness = np.sum(np.power(X,2)) + 1 # example: 1.2
-        result = fitness.reshape(1,-1) # example ([1.2,])
-        return fitness,result
-
-    lb = -100 * np.ones(30)
-    ub = 100 * np.ones(30)
-    cp.MFO.run(pop = 1000, dim = 30, lb = lb, ub = ub, MaxIter = 30, fun = uni_fun1)
+    dim = 10
+    lb = np.zeros(10)
+    ub = np.ones(10)
+    n_obj=2
+    cp.MOMFO.EliteOppoSwitch = True
+    cp.MOMFO.runMP(90,10,lb,ub,50,2,100,20,ZDT4,5)
     """
     print("Current Algorithm: MFO")
     print("Elite Opposition:{}".format(EliteOppoSwitch))
     print("Iterations: 1 (init.) + {}".format(MaxIter))
     print("Dim:{}".format(dim))
     print("Population:{}".format(pop))
     print("Lower Bnd.:{}".format(lb))
```

### Comparing `pycup-0.1.7/pycup/MOPSO.py` & `pycup-0.1.7.1/pycup/MOPSO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/NSGA2.py` & `pycup-0.1.7.1/pycup/NSGA2.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/PESTclasses.py` & `pycup-0.1.7.1/pycup/PESTclasses.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/PSO.py` & `pycup-0.1.7.1/pycup/PSO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/Reslib.py` & `pycup-0.1.7.1/pycup/Reslib.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/SCA.py` & `pycup-0.1.7.1/pycup/SCA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/SOA.py` & `pycup-0.1.7.1/pycup/SOA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/SSA.py` & `pycup-0.1.7.1/pycup/SSA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/TOPSIS.py` & `pycup-0.1.7.1/pycup/TOPSIS.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/TSA.py` & `pycup-0.1.7.1/pycup/TSA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/WOA.py` & `pycup-0.1.7.1/pycup/WOA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/__init__.py` & `pycup-0.1.7.1/pycup/__init__.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/calc_utils.py` & `pycup-0.1.7.1/pycup/calc_utils.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/document/Documentation.pdf` & `pycup-0.1.7.1/pycup/document/Documentation.pdf`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/evaluation_metrics.py` & `pycup-0.1.7.1/pycup/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/integrate.py` & `pycup-0.1.7.1/pycup/integrate.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/multi_jobs.py` & `pycup-0.1.7.1/pycup/multi_jobs.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/plot.py` & `pycup-0.1.7.1/pycup/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2164,35 +2164,37 @@
                              'gist_rainbow', 'hsv', 'flag', 'prism'])]
     """
     if not isinstance(raw_saver, save.RawDataSaver):
         raise TypeError("The input saver object should be pycup.save.RawDataSaver.")
     fitness = np.array(raw_saver.historical_fitness)
     iterations, population = analyze_saver(raw_saver)
     if iterations > 1:
-        a = np.ones((fitness.shape[0], fitness.shape[1]))
+        a = []
+        for i in range(iterations):
+            a.append(np.ones(population[i]))
         c = np.linspace(0, iterations, iterations)
         for i in range(fitness.shape[0]):
             a[i] = a[i] * c[i]
+        a = np.concatenate(a)
+        fitness = np.concatenate(fitness)
         fig = plt.figure(figsize=figsize, dpi=dpi)
         ax = fig.add_subplot(111, projection='3d')
-        s = ax.scatter(xs=fitness[:, :, objfunid1], ys=fitness[:, :, objfunid2], zs=fitness[:, :, objfunid3], c=a,
+        s = ax.scatter(xs=fitness[:, objfunid1], ys=fitness[ :, objfunid2], zs=fitness[:, objfunid3], c=a,
                        marker=marker, s=markersize, cmap=cmap)
         bar = plt.colorbar(s, fraction=cbar_frac, pad=cbar_pad)
         bar.set_label(cbar_ttl, fontsize=cbar_ttl_size)
         bar.ax.tick_params(labelsize=cbar_lbl_size)
 
     else:
         fig = plt.figure(figsize=figsize, dpi=dpi)
         ax = fig.add_subplot(111, projection='3d')
         s = ax.scatter(xs=fitness[:, objfunid1], ys=fitness[:, objfunid2], zs=fitness[:, objfunid3], c=single_c,
                        marker=marker, s=markersize, cmap=cmap)
     ax.view_init(*view_init)
     if slim:
-        if iterations > 1:
-            fitness = np.concatenate(fitness)
         xmin = np.min(fitness[:, objfunid1], axis=0)
         ymin = np.min(fitness[:, objfunid2], axis=0)
         zmin = np.min(fitness[:, objfunid3], axis=0)
         xmax = np.max(fitness[:, objfunid1], axis=0)
         ymax = np.max(fitness[:, objfunid2], axis=0)
         zmax = np.max(fitness[:, objfunid3], axis=0)
         ax.set_xlim(xmin, xmax)
@@ -2310,15 +2312,15 @@
     cp.MOPSO.run(pop=100, dim=3, lb=lb, ub = ub, MaxIter=20,n_obj=3,nAr=300,M=50,
                        fun=mo_fun1)
 
     from pycup import plot,save
 
     path = "RawResult.rst"
     saver = save.RawDataSaver.load(path)
-    plot.plot_3d_MO_fitness_space(saver,objfunid1=0,objfunid2=1,variable_id=2)
+    plot.plot_3d_sample_fitness_space(saver,objfunid1=0,objfunid2=1,variable_id=2)
 
 
     Note:
     selectable cmaps includes [('Perceptually Uniform Sequential',
                             ['viridis', 'inferno', 'plasma', 'magma']),
          ('Sequential',     ['Blues', 'BuGn', 'BuPu',
                              'GnBu', 'Greens', 'Greys', 'Oranges', 'OrRd',
@@ -2340,35 +2342,38 @@
     """
     if not isinstance(raw_saver, save.RawDataSaver):
         raise TypeError("The input saver object should be pycup.save.RawDataSaver.")
     fitness = np.array(raw_saver.historical_fitness)
     samples = np.array(raw_saver.historical_samples)
     iterations, population = analyze_saver(raw_saver)
     if iterations > 1:
-        a = np.ones((fitness.shape[0], fitness.shape[1]))
+        a = []
+        for i in range(iterations):
+            a.append(np.ones(population[i]))
         c = np.linspace(0, iterations, iterations)
         for i in range(fitness.shape[0]):
             a[i] = a[i] * c[i]
+        a = np.concatenate(a)
+        fitness = np.concatenate(fitness)
+        samples = np.concatenate(samples)
         fig = plt.figure(figsize=figsize, dpi=dpi)
         ax = fig.add_subplot(111, projection='3d')
-        s = ax.scatter(xs=fitness[:, :, objfunid1], ys=fitness[:, :, objfunid2], zs=samples[:, :, variable_id], c=a,
+        s = ax.scatter(xs=fitness[ :, objfunid1], ys=fitness[ :, objfunid2], zs=samples[ :, variable_id], c=a,
                        marker=marker, s=markersize, cmap=cmap)
         bar = plt.colorbar(s, fraction=cbar_frac, pad=cbar_pad)
         bar.set_label(cbar_ttl, fontsize=cbar_ttl_size)
         bar.ax.tick_params(labelsize=cbar_lbl_size)
 
     else:
         fig = plt.figure(figsize=figsize, dpi=dpi)
         ax = fig.add_subplot(111, projection='3d')
         s = ax.scatter(xs=fitness[:, objfunid1], ys=fitness[:, objfunid2], zs=samples[:, variable_id], c=single_c,
                        marker=marker, s=markersize, cmap=cmap)
     ax.view_init(*view_init)
     if slim:
-        if iterations > 1:
-            fitness = np.concatenate(fitness)
         xmin = np.min(fitness[:, objfunid1], axis=0)
         ymin = np.min(fitness[:, objfunid2], axis=0)
         xmax = np.max(fitness[:, objfunid1], axis=0)
         ymax = np.max(fitness[:, objfunid2], axis=0)
         ax.set_xlim(xmin, xmax)
         ax.set_ylim(ymin, ymax)
```

### Comparing `pycup-0.1.7/pycup/sampling.py` & `pycup-0.1.7.1/pycup/sampling.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/save.py` & `pycup-0.1.7.1/pycup/save.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/template.py` & `pycup-0.1.7.1/pycup/template.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/test_functions.py` & `pycup-0.1.7.1/pycup/test_functions.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/uncertainty_analysis_fun.py` & `pycup-0.1.7.1/pycup/uncertainty_analysis_fun.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup/utilize.py` & `pycup-0.1.7.1/pycup/utilize.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/pycup.egg-info/PKG-INFO` & `pycup-0.1.7.1/pycup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycup
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.
 Home-page: https://github.com/QianyangWang/PyCUP
 Author: Qianyang Wang
 Author-email: wqy07010944@hotmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/QianyangWang/PyCUP/DOCUMENT
 Project-URL: Source, https://github.com/QianyangWang/PyCUP/pycup
```

### Comparing `pycup-0.1.7/pycup.egg-info/SOURCES.txt` & `pycup-0.1.7.1/pycup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7/setup.py` & `pycup-0.1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open(r"README.md",encoding="utf-8") as f:
   long_description = f.read()
 
 
 setup(
     name='pycup',
-  version='0.1.7',
+  version='0.1.7.1',
   description='An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Qianyang Wang',
   author_email='wqy07010944@hotmail.com',
   url='https://github.com/QianyangWang/PyCUP',
   license='MIT License',
```

