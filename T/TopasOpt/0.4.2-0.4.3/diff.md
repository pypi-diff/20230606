# Comparing `tmp/TopasOpt-0.4.2.tar.gz` & `tmp/TopasOpt-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TopasOpt-0.4.2.tar", last modified: Mon Aug 29 05:52:41 2022, max compression
+gzip compressed data, was "TopasOpt-0.4.3.tar", last modified: Tue Jun  6 11:44:23 2023, max compression
```

## Comparing `TopasOpt-0.4.2.tar` & `TopasOpt-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 05:52:41.960393 TopasOpt-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-08-29 05:52:15.000000 TopasOpt-0.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-08-29 05:52:41.960393 TopasOpt-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-08-29 05:52:15.000000 TopasOpt-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 05:52:41.960393 TopasOpt-0.4.2/TopasOpt/
--rwxr-xr-x   0 runner    (1001) docker     (121)    51437 2022-08-29 05:52:15.000000 TopasOpt-0.4.2/TopasOpt/Optimisers.py
--rw-r--r--   0 runner    (1001) docker     (121)    14739 2022-08-29 05:52:15.000000 TopasOpt-0.4.2/TopasOpt/TopasScriptGenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-08-29 05:52:15.000000 TopasOpt-0.4.2/TopasOpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28852 2022-08-29 05:52:15.000000 TopasOpt-0.4.2/TopasOpt/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 05:52:41.960393 TopasOpt-0.4.2/TopasOpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-08-29 05:52:41.000000 TopasOpt-0.4.2/TopasOpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-08-29 05:52:41.000000 TopasOpt-0.4.2/TopasOpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 05:52:41.000000 TopasOpt-0.4.2/TopasOpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-08-29 05:52:41.000000 TopasOpt-0.4.2/TopasOpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-29 05:52:41.000000 TopasOpt-0.4.2/TopasOpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-29 05:52:16.000000 TopasOpt-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-08-29 05:52:41.960393 TopasOpt-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:44:23.182844 TopasOpt-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-06 11:44:23.186843 TopasOpt-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:44:23.182844 TopasOpt-0.4.3/TopasOpt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52313 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/TopasOpt/Optimisers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/TopasOpt/TopasScriptGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/TopasOpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32339 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/TopasOpt/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:44:23.182844 TopasOpt-0.4.3/TopasOpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-06 11:44:23.000000 TopasOpt-0.4.3/TopasOpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-06 11:44:23.000000 TopasOpt-0.4.3/TopasOpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:44:23.000000 TopasOpt-0.4.3/TopasOpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-06 11:44:23.000000 TopasOpt-0.4.3/TopasOpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 11:44:23.000000 TopasOpt-0.4.3/TopasOpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-06 11:44:23.186843 TopasOpt-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:44:23.182844 TopasOpt-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/tests/test_TopasScriptGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/tests/test_docstring_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/tests/test_optimisers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/tests/test_utilities.py
```

### Comparing `TopasOpt-0.4.2/LICENSE.md` & `TopasOpt-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TopasOpt-0.4.2/PKG-INFO` & `TopasOpt-0.4.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,10 @@
-Metadata-Version: 2.1
-Name: TopasOpt
-Version: 0.4.2
-Summary: optimisation for topas Monte Carlo
-Home-page: https://github.com/ACRF-Image-X-Institute/TopasOpt
-Author: Brendan Whelan
-Author-email: bwheelz360@gmail.com
-Project-URL: Bug Tracker, https://github.com/ACRF-Image-X-Institute/TopasOpt/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # TopasOpt
 
-![](docsrc/_resources/interrogate_badge.svg) [![codecov](https://codecov.io/gh/ACRF-Image-X-Institute/TopasOpt/branch/master/graph/badge.svg?token=0FSEO19LCD)](https://codecov.io/gh/ACRF-Image-X-Institute/TopasOpt)![test](https://github.com/ACRF-Image-X-Institute/TopasOpt/actions/workflows/run_tests.yml/badge.svg) ![docs](https://github.com/ACRF-Image-X-Institute/TopasOpt/actions/workflows/build-docs.yml/badge.svg)
+![](docsrc/_resources/interrogate_badge.svg) [![codecov](https://codecov.io/gh/ACRF-Image-X-Institute/TopasOpt/branch/master/graph/badge.svg?token=0FSEO19LCD)](https://codecov.io/gh/ACRF-Image-X-Institute/TopasOpt)![test](https://github.com/ACRF-Image-X-Institute/TopasOpt/actions/workflows/run_tests.yml/badge.svg) ![docs](https://github.com/ACRF-Image-X-Institute/TopasOpt/actions/workflows/build-docs.yml/badge.svg)[![PyPI version](https://badge.fury.io/py/TopasOpt.svg)](https://badge.fury.io/py/TopasOpt)
 
 
 This code provides a framework for performing optimisation on monte carlo radiation transport 
 simulations using [TOPAS](https://www.google.com/search?channel=fs&client=ubuntu&q=topas+MC).
 
 ## Install and Requirements
 
@@ -37,13 +22,30 @@
 ## Directory Structure
 
 - **TopasOpt:** source code
 - **examples:** source code for the [worked examples](https://acrf-image-x-institute.github.io/TopasOpt/worked_examples.html) provided in the docs
 - **docsrc:** markdown/rst documentation.
 - **tests:** tests which are run through github actions
 
+## Citation
+
+This code is described in [this paper](https://aapm.onlinelibrary.wiley.com/doi/10.1002/mp.16126).
+If you use this code in your work, please cite this paper!
+
+```bibtex
+
+@article{whelan_topasopt_2022,
+	title = {{TopasOpt}: {An} open-source library for optimization with {Topas} {Monte} {Carlo}},
+	shorttitle = {{TopasOpt}},
+	journal = {Medical Physics},
+	author = {Whelan, Brendan and Loo Jr, Billy W. and Wang, Jinghui and Keall, Paul},
+	year = {2022},
+	note = {Publisher: Wiley Online Library},
+}
+
+```
```

### Comparing `TopasOpt-0.4.2/TopasOpt/Optimisers.py` & `TopasOpt-0.4.3/TopasOpt/Optimisers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 from scipy import stats
 from pathlib import Path
 import numpy as np
 import sys, os
 from bayes_opt import BayesianOptimization
 from bayes_opt import UtilityFunction
 from bayes_opt.logger import JSONLogger
-from bayes_opt.util import load_logs
+from bayes_opt.util import load_logs, NotUniqueError
 from bayes_opt.event import Events
 from sklearn.gaussian_process.kernels import Matern
 import logging
 from .utilities import bcolors, FigureSpecs, newJSONLogger, ReadInLogFile, PlotLogFile
 import stat
 from scipy.optimize import rosen
+from abc import abstractmethod
 
 ch = logging.StreamHandler()
 formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
 ch.setFormatter(formatter)
 logger = logging.getLogger(__name__)
 logger.addHandler(ch)
 logger.setLevel(logging.INFO)  # This toggles all the logging in your app
@@ -69,14 +70,16 @@
     :type BaseDirectory: string
     :param SimulationName: Specific folder for this simulation
     :type SimulationName: string
     :param OptimisationDirectory: location that TopasObjectiveFunction and GenerateTopasScript are located
     :type OptimisationDirectory: string or Path
     :param ReadMeText: If supplied, is written to a readme file in BaseDirectory
     :type ReadMeText: string, optional
+    :param G4dataLocation: location of G4data files
+    :type G4dataLocation: str
     :param TopasLocation: location of topas installation. Default is ~/topas if you follow the topas instructions.
     :type TopasLocation: string or pathlib.Path, optional
     :param ShellScriptHeader: Header to place at the start of the bash file that runs the topas model. This header
         should contain all the commands you normally perform to set up your terminal environment.
     :type ShellScriptHeader: string, optional
     :param Overwrite: if True, will automatically overwrite any existing files. If False, will ask first (safer)
     :type Overwrite: bool, optional
@@ -135,15 +138,16 @@
         self.Overwrite = Overwrite
         self.AllObjectiveFunctionValues = []
 
         if '~' in TopasLocation:
             TopasLocation = os.path.expanduser(TopasLocation)
         self.TopasLocation = Path(TopasLocation)
         self._testing_mode = False  # overwrite if True
-        if 'testing_mode' in str(self.TopasLocation):
+        self._retrospective_mode = False  # overwrite if True
+        if str(self.TopasLocation) == 'testing_mode':
             self._testing_mode = True
             logger.warning(f'Entering test mode because topas location = {self.TopasLocation}')
 
 
         # this is where we try to load the user defined model generator and objective function
         try:
             _import_from_absolute_path(Path(self.OptimisationDirectory) / 'GenerateTopasScripts.py')
@@ -269,18 +273,18 @@
                     sys.exit(1)
 
         self._CreateVariableDictionary(self.StartingValues)
 
         # make sure topas binary exists
         if not self._testing_mode:
             if not os.path.isfile(self.TopasLocation / 'bin' / 'topas'):
-                logger.error(f'{bcolors.FAIL}could not find topas binary at \n{self.TopasLocation}'
-                             f'\nPlease initialise with TopasLocation pointing to the topas installation location.'
-                             f'\nQuitting{bcolors.ENDC}')
-                sys.exit(1)
+                error = f'{bcolors.FAIL}could not find topas binary at \n{self.TopasLocation} ' \
+                        f'\nPlease initialise with TopasLocation pointing to the topas installation location.' \
+                        f'\nQuitting{bcolors.ENDC}'
+                raise FileNotFoundError(error)
 
     def _GenerateTopasModel(self, x):
         """
         Generates a topas model with the latest parameters as well as a shell script called RunAllFiles.sh to run it.
         """
 
         self.TopasScripts, self.TopasScriptNames = self.TopasScriptGenerator(self.BaseDirectory, self.Itteration, **self.VariableDict)
@@ -483,14 +487,21 @@
                     os.unlink(file_path)
                 elif os.path.isdir(file_path):
                     shutil.rmtree(file_path)
             except Exception as e:
                 logger.warning(f'Failed to delete {file_path} from results folder. Reason: {e}. continuing...')
 
     # public methods
+
+    @abstractmethod
+    def RunOptimisation(self):
+        """
+        each inheriting optimizer must supply its own RunOptimisation method
+        """
+        pass
     
     def BlackBoxFunction(self, x_new):
         """
         Called Black Box function in the spirit of bayesian optimisation, this function simply takes the most recent
         parameter guesses, and solves the model.
         """
 
@@ -647,36 +658,40 @@
 
 
 class BayesianOptimiser(TopasOptBaseClass):
     """
     Class to perform optimisation using the `Bayesian Optimisation code <https://github.com/fmfn/BayesianOptimization>`_
     Specific options are described below, the rest are described in TopasOptBaseClass
 
-    :param bayes_length_scales: Bayes-specific parameter to defined the length scales used in the gaussian process  model.  This can be supplied as one of three things:
-
-    - **None**: in this case, the default is used: length_scale=1.0
-    - **Number between 0 and 1**: in this case, the length scales for each parameter are derived as a percentage of range.
-        For instance if the user enter 0.1, all length scales will be set to 10% of the range of each variable
-    - **Array-like**: Finally, the user is free to simply specify what length scales to use for each parameter.
-        Make sure you enter them in alphabetical order as this is the order used internally by the optimizer.
+    :param bayes_length_scales: Bayes-specific parameter to defined the length scales used in the gaussian process  model.
+      This can be supplied as one of three things:
+      - **None**: in this case, the default is used: length_scale=1.0
+      - **Number between 0 and 1**: in this case, the length scales for each parameter are derived as a percentage of range.
+         For instance if the user enter 0.1, all length scales will be set to 10% of the range of each variable
+      - **Array-like**: Finally, the user is free to simply specify what length scales to use for each parameter.
+         Make sure you enter them in alphabetical order as this is the order used internally by the optimizer.
     :type bayes_length_scales: None, float, or array (optional)
     :param bayes_UCBkappa: Bayes-specific parameter . kappa value in UCB  function. A higher value=more exploration. see
         `this notebook <https://github.com/fmfn/BayesianOptimization/blob/master/examples/exploitation_vs_exploration.ipynb>`_
         for explanation
     :type bayes_UCBkappa: float, optional
     :param bayes_KappaDecayIterations: Bayes-specific parameter. Over the last N iterations, kappa will decay to be
         almost 0 (highly exploitive). For explantion of kappa decay see `here <https://github.com/fmfn/BayesianOptimization/pull/221>`_
     :type bayes_KappaDecayIterations: int, optional
     :param bayes_GP_alpha: Bayes-specific parameter. This parameter handles the smoothness of the gaussian process model.
         for a noisy objective function, increasing this value can minimise overfitting errors.
     :type bayes_GP_alpha: float, optional
+    :param custom_kernel: You can optionally [construct your own kernel](https://scikit-learn.org/stable/modules/gaussian_process.html)
+        to use in the gaussian process model
+    :type custom_kernel: instance of scikit-learn.gaussian_process.kernels.Kernel or derived classes
     """
 
     def __init__(self, bayes_length_scales=None, bayes_UCBkappa=5,
-                 bayes_KappaDecayIterations=10, bayes_GP_alpha=0.01, **kwds):
+                 bayes_KappaDecayIterations=10, bayes_GP_alpha=0.01,
+                 custom_kernel=None,**kwds):
         """
         init function for Bayesian optimiser
         """
         self.bayes_length_scales = bayes_length_scales
         self.bayes_UCBkappa = bayes_UCBkappa
         self.bayes_KappaDecayIterations = bayes_KappaDecayIterations
         self.bayes_GP_alpha = bayes_GP_alpha
@@ -684,34 +699,46 @@
 
         self.BayesOptLogLoc = Path(self.BaseDirectory) / self.SimulationName / 'logs/bayes_opt_logs.json'
         self._BayesianOptimiser__RestartMode = False  # don't change!
         self._create_p_bounds(self._optimisation_params)  # Bayesian optimiser wants bounds in a slight differnt format
         self._create_suggested_points_to_probe(self._optimisation_params)
         self._derive_bayes_length_scales(bayes_length_scales)
 
+
         # Bayesian optimisation settings:
         self._target_prediction_mean = []  # keep track of what the optimiser expects to get
         self._target_prediction_std = []  # keep track of what the optimiser expects to get
         # see here: https://github.com/fmfn/BayesianOptimization/issues/202
         self.Matern_Nu = 1.5  # see here https://scikit-learn.org/stable/modules/generated/sklearn.gaussian_process.kernels.Matern.html#sklearn.gaussian_process.kernels.Matern
         self.UCBkappa = bayes_UCBkappa  # higher kappa = more exploration. lower kappa = more exploitation
         self.n_restarts_optimizer = 20  # this controls the gaussian process fitting. 20 seems to be a good number.
         self.bayes_KappaDecayIterations = bayes_KappaDecayIterations
         self.UCBKappa_final = 0.1
         self.kappa_decay_delay = self.MaxItterations - self.bayes_KappaDecayIterations  # this many exploritive iterations will be carried out before kappa begins to decay
+        if custom_kernel is None:
+            self._kernel = Matern(length_scale=self.bayes_length_scales, nu=self.Matern_Nu)
+        else:
+            self._kernel = custom_kernel
 
         if self.kappa_decay_delay >= self.MaxItterations:
             logger.warning(f'Kappa decay requested, but since kappa_decay_delay ({self.kappa_decay_delay}) is less'
                            f'than MaxItterations ({self.MaxItterations}), decay will never occur...')
             self.kappa_decay = 1
         else:
             self.kappa_decay = (self.UCBKappa_final / self.UCBkappa) ** (
                         1 / (self.MaxItterations - self.kappa_decay_delay))
             # ^^ this is the parameter to ensure we end up with UCBKappa_final on the last iteration
 
+        # instantiate optimizer:
+        self.optimizer = BayesianOptimization(f=None, pbounds=self.pbounds, random_state=1, allow_duplicate_points=False)
+        self.optimizer.set_gp_params(normalize_y=True, kernel=self._kernel,
+                                n_restarts_optimizer=self.n_restarts_optimizer, alpha=self.bayes_GP_alpha)  # tuning of the gaussian parameters...
+        self.utility = UtilityFunction(kind="ucb", kappa=self.UCBkappa, xi=0.0, kappa_decay_delay=self.kappa_decay_delay,
+                                  kappa_decay=self.kappa_decay)
+
 
     def _derive_bayes_length_scales(self, bayes_length_scales):
         """
         Figure out what to put in to the gaussian process model kernel for length scales.
         We use the Matern Kernel which is detailed `here <https://scikit-learn.org/stable/modules/generated/sklearn.gaussian_process.kernels.Matern.html#sklearn.gaussian_process.kernels.Matern>`_
 
         :param bayes_length_scales: user input for length scales. Can be one of three things:
@@ -895,85 +922,80 @@
             plt.savefig(SaveName)
             plt.close(fig)
 
     def _update_logs_with_length_scales(self):
         """
         writes the original and optimised length scales to the end of a log file
         """
-        start_length = self.optimizer._gp.kernel.length_scale
-        final_length = self.optimizer._gp.kernel_.length_scale
-        keys = sorted(self.pbounds)
-        start_length = dict(zip(keys, start_length))
-        final_length = dict(zip(keys, final_length))
-        Entry = f'\nStarting length scales were {start_length}'
-        Entry = Entry + f'\nOptimised length scales were {final_length}'
-
-        with open(self._LogFileLoc , 'a') as f:
-            f.write(Entry)
+        try:
+            start_length = self.optimizer._gp.kernel.length_scale
+            final_length = self.optimizer._gp.kernel_.length_scale
+            keys = sorted(self.pbounds)
+            start_length = dict(zip(keys, start_length))
+            final_length = dict(zip(keys, final_length))
+            Entry = f'\nStarting length scales were {start_length}'
+            Entry = Entry + f'\nOptimised length scales were {final_length}'
+
+            with open(self._LogFileLoc, 'a') as f:
+                f.write(Entry)
+        except AttributeError:
+            pass
 
     def RunOptimisation(self):
         """
         This is the main optimisation loop.
         For explanation of the various parameters and commands, start with the
         """
 
         # set up directory structure
         if not self.__RestartMode:
             self.SetUpDirectoryStructure()
         else:
             self._setup_topas_emulator()
 
-        # instantiate optimizer:
 
-        self.optimizer = BayesianOptimization(f=None, pbounds=self.pbounds, random_state=1)
-        self.optimizer.set_gp_params(normalize_y=True, kernel=Matern(length_scale=self.bayes_length_scales, nu=self.Matern_Nu),
-                                n_restarts_optimizer=self.n_restarts_optimizer, alpha=self.bayes_GP_alpha)  # tuning of the gaussian parameters...
-        utility = UtilityFunction(kind="ucb", kappa=self.UCBkappa, xi=0.0, kappa_decay_delay=self.kappa_decay_delay,
-                                  kappa_decay=self.kappa_decay)
-        logger.warning('setting numpy to ignore underflow errors.')
-        np.seterr(under='ignore')
 
         if self.__RestartMode:
             # then load the previous log files:
             load_logs(self.optimizer, logs=[self.BayesOptLogLoc])
             bayes_opt_logger = newJSONLogger(path=str(self.BayesOptLogLoc))
             self.optimizer.subscribe(Events.OPTIMIZATION_STEP, bayes_opt_logger)
             self.optimizer._gp.fit(self.optimizer._space.params, self.optimizer._space.target)
             self.Itteration = len(self.optimizer.space.target)
             self.ItterationStart = len(self.optimizer.space.target)
-            utility._iters_counter = self.ItterationStart
+            self.utility._iters_counter = self.ItterationStart
             if self.Itteration >= self.MaxItterations-1:
                 logger.error(f'nothing to restart; max iterations is {self.MaxItterations} and have already been completed')
                 sys.exit(1)
         else:
             bayes_opt_logger = JSONLogger(path=str(self.BayesOptLogLoc))
             self.optimizer.subscribe(Events.OPTIMIZATION_STEP, bayes_opt_logger)
             # first guess is nonsense but we need the vectors to be the same length
             self._target_prediction_mean.append(0)
             self._target_prediction_std.append(0)
             target = self.BlackBoxFunction(self.VariableDict)
             self.optimizer.register(self.VariableDict, target=target)
 
         for point in range(self.Itteration, self.MaxItterations):
-            utility.update_params()
+            self.utility.update_params()
             if (self.Nsuggestions is not None) and (self.SuggestionsProbed < self.Nsuggestions):
                 # evaluate any suggested solutions first
                 next_point_to_probe = self.Suggestions[self.SuggestionsProbed]
                 self.SuggestionsProbed += 1
             else:
-                next_point_to_probe = self.optimizer.suggest(utility)
+                next_point_to_probe = self.optimizer.suggest(self.utility)
 
             NextPointValues = np.array(list(next_point_to_probe.values()))
             mean, std = self.optimizer._gp.predict(NextPointValues.reshape(1, -1), return_std=True)
             self._target_prediction_mean.append(mean[0])
             self._target_prediction_std.append(std[0])
             target = self.BlackBoxFunction(next_point_to_probe)
             try:
                 self.optimizer.register(params=next_point_to_probe, target=target)
-            except KeyError:
+            except NotUniqueError:
                 try:
                     self.RepeatedPointsProbed = self.RepeatedPointsProbed + 1
                     logger.warning(
                         f'Bayesian algorithm is attempting to probe an existing point: {NextPointValues}. Continuing for now....')
                     if self.RepeatedPointsProbed > 10:
                         logger.error('The same point has been requested more than 10 times; quitting')
                         break
```

### Comparing `TopasOpt-0.4.2/TopasOpt/TopasScriptGenerator.py` & `TopasOpt-0.4.3/TopasOpt/TopasScriptGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
             if not os.path.isfile(script):
                 logger.error(f'Could not find TopasScriptLocation at {script}. Quitting')
                 sys.exit(1)
 
         if not os.path.isdir(self.OutputDirectory):
             logger.error(f'Specified output directory does not exist: {self.OutputDirectory}')
 
-
     def _handle_include_files(self, OriginalFileLocation, line):
         """
         This function is called when an includeFile statement is found in the input topas script.
         The include file will be copied to  IncludeFileStorageDirectory, and the line updated with an
         absolute path to that location
 
         Returns: line, the updated includeFile line
@@ -179,14 +178,15 @@
             OutputPhaseSpaceFilesNames:
 
         Returns:
 
         """
         # check whether this is a dynamic or static phase space source
         UseStaticPhaseSpace = True
+        OriginalFileLocation = Path(OriginalFileLocation)
         for OutputPhaseSpace in OutputPhaseSpaceFilesNames:
             if OutputPhaseSpace in line:
                 UseStaticPhaseSpace = False
 
         line1, line2 = line.split("=", 1)  # delete everything after the first =
         OriginalFileName = line2.split('/')[-1]
         OriginalFileName = OriginalFileName.replace('"', '')
```

### Comparing `TopasOpt-0.4.2/TopasOpt/utilities.py` & `TopasOpt-0.4.3/TopasOpt/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import os, sys
 import logging
 import numpy as np
 import topas2numpy as tp
 import matplotlib.pyplot as plt
 from scipy.interpolate import RegularGridInterpolator
 from pathlib import Path
+import stat
+import glob
 # import seaborn as sns
 plt.interactive(False)
 
 
 ch = logging.StreamHandler()
 formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
 ch.setFormatter(formatter)
@@ -65,19 +67,14 @@
         super(JSONLogger, self).__init__()
         self._path = path if path[-5:] == ".json" else path + ".json"
 
 
 class WaterTankData:
     """
     Read in and analyse a series of topas scoring files in a rectangular phantom (the water tank).
-    There are two ways you might want to use this:
-
-    1. Analyse a single dose file
-    2. Analyse multiple dose files all on the same scoring grid
-
     The main attribute is the 'DoseCube' array. This is the agregate of all the input files. If you
     only put one file in, then this is simply the agregate of that single file.
     A number of plotting routines are already provided which operate on this array, but if you need to you can use
     ExtractDataFromDoseCube to generate any additional data from it.
 
     Basic use::
 
@@ -87,28 +84,37 @@
         Dose = WaterTankData(AnalysisPath, FileToAnalyse, MirrorData=True)
         Dose.Plot_DosePlanes()
         # extract some additional data from agregate dose cube, XY plane for example:
         [Xpts, Ypts] = np.meshgrid(Dose.x, Dose.y)
         Zpts = Dose.PhantomSizeZ * np.ones(Xpts.shape)
         XY_data = Dose.ExtractDataFromDoseCube(Xpts, Ypts, Zpts)
 
+    :param AnalysisPath: Location of result files
+    :type AnalysisPath: str or Path
+    :param FileToAnalyse: all result files to read in
+    :type FileToAnalyse: str, or list of strings
+    :param AbsDepthDose: if True, absolute dose instead of normalized dose is plotted
+    :type AbsDepthDose: bool
+    :param verbose: if True, various messages are printed
+    :type verbose: bool
     """
 
-    def __init__(self, AnalysisPath, FileToAnalyse, AbsDepthDose=False):
+    def __init__(self, AnalysisPath, FileToAnalyse, AbsDepthDose=False, verbose=False):
         """
         :param AnalysisPath: Path where files are located
         :type AnalysisPath: string
         :param FileToAnalyse: Can be either a single file or a list of tiles
         :type FileToAnalyse: list or string
         :param AbsDepthDose: If True, plots are in dose, if False they are normalised to Dmax
         :type AbsDepthDose: Boolean, optional
         """
 
         self.AnalysisPath = AnalysisPath
         self.FileToAnalyse = FileToAnalyse
+        self.verbose = verbose
         # the below lists all get appended to as data is read in
         self.Xangles = []
         self.Yangles = []
         self.MaxDoseAtIsoplane = []
         self.MaxDoseAtIsoplaneGauss = []
         self.BeamletWidthsManual = []
         self.BeamletWidthsGauss = []
@@ -171,15 +177,15 @@
                 if not os.path.isfile(FileLocation):
                     logging.error(f'Could not locate file: \n{FileLocation}')
             self.dose = tp.BinnedResult(FileLocation)
             # convert dose units:
             if self.dose.unit == 'Gy':
                 DoseConverter = 1e6
                 self.dose.unit = '\u03BCGy'
-                if not self.DoseUnitsWarning:
+                if not self.DoseUnitsWarning and self.verbose:
                     print(f'converting Gy to {self.dose.unit}')
                     self.DoseUnitsWarning = True
             elif self.dose.unit == 'mGy':
                 DoseConverter = 1000
                 self.dose.unit = '\u03BCGy'
                 if not self.DoseUnitsWarning:
                     print(f'converting mGy to {self.dose.unit}')
@@ -201,15 +207,15 @@
         For multifile mode, the coordinate system is only created the first time this function is called,
         otherwise it checks that the phantom dimensions are the same for subsequent files, and will cause
         an error if not
         """
         # what unit is the file in?
         if self.dose.dimensions[0].unit == 'cm':
             UnitConverter = 10
-            if not self.DistanceUnitMessage:
+            if not self.DistanceUnitMessage and self.verbose:
                 print('converting cm to mm')
                 self.DistanceUnitMessage = True
         elif self.dose.dimensions[0].unit == 'mm':
             UnitConverter = 1
         else:
             UnitConverter = 1
             logging.warning('unit could not be detected, reading in without converion')
@@ -322,15 +328,22 @@
     # Public methods:
 
     def ExtractDataFromDoseCube(self, Xpts, Ypts, Zpts):
         """
         Extract data from the dose cube at positions Xpts, Ypts, Zpts
         Each of these is an array or list, and they must be the same shape (they can be of any dimensionality as
         they are flattened inside the function). The data is returned in the same shape as the input points.
+
+        :param Xpts: x points
+        :param Ypts: y points
+        :param Zpts: z points
+        :return: InterpolatedData: numpy array of Dose at [Xpts, Ypts, Zpts]. Shape is the same
+            as the input coordinate arrays
         """
+
         assert Xpts.shape == Ypts.shape == Zpts.shape
         InputShape = Xpts.shape
         # convert to array and flatten
         Xpts = np.array(Xpts).flatten()
         Ypts = np.array(Ypts).flatten()
         Zpts = np.array(Zpts).flatten()
 
@@ -346,14 +359,16 @@
         InterpolatedData = np.reshape(InterpolatedData,InputShape)
 
         return InterpolatedData
 
     def Plot_DosePlanes(self, AddColorBar=False): # pragma: no cover
         """
         Use the DoseCube data to create a plot through each of the cardinal planes.
+
+        :param AddColorBar: adds color bar if True
         """
 
         fig, (axs1, axs2, axs3) = plt.subplots(nrows=1, ncols=3, figsize=(15, 5))
         # for generating extent in plots:
         dx = (self.x[1] - self.x[0]) / 2.
         dy = (self.y[1] - self.y[0]) / 2.
         dz = (self.z[1] - self.z[0]) / 2.
@@ -435,14 +450,17 @@
         self.integralPDD_axs.set_xlabel('Depth [mm]', fontsize=FigureSpecs.LabelFontSize)
         plt.show()
 
     def Plot_Profiles(self, dir='X', Zpoints=None): # pragma: no cover
         """
         Plot profiles through integrated data. Can choose dir='X' or dir='Y'
         You can also optionally pass multiple Z points; otherwise Z is set to the middle of the phantom
+
+        :param dir: 'X' or 'Y', controls profile direction
+        :param Zpoints: Z coordinates to plot profiles at; if None will plot through the middle of the Phantom
         """
         fig, IntProfile_axs = plt.subplots(figsize=(5, 5))
         if Zpoints is None:
             Zpoints = list([self.PhantomSizeZ])
         if not isinstance(Zpoints, list):
             Zpoints = list([Zpoints])
         if not (dir == 'X' or dir == 'Y'):
@@ -669,9 +687,75 @@
     if save_loc:
         plt.savefig(save_loc)
         plt.close(fig)
     else:
         plt.show()
 
 
+def get_all_files(PathToData, file_extension):
+    """
+    quick script to just collect all the files in the Analysis path
+    :param PathToData: folder where the files are
+    :type PathToData: pathlib.Path or string
+    :param file_extension: extension of files to return, e.g. 'dcm'
+    :type file_extension: str
+    :returns Files: list of all found files
+    """
+
+    if not file_extension[0] == '.':
+        # handles the case where the user entered 'dcm' instead of '.dcm'
+        file_extension = '.' + file_extension
+    file_extension = '*' + file_extension
+    # check that this is now in the format we require
+    if not file_extension[0:2] == '*.':
+        logger.error('please enter the file_extension parameter like this : file_extension = "jpg"')
+        sys.exit(1)
 
+    if not isinstance(PathToData,Path):
+        PathToData = Path(PathToData)
 
+    if not os.path.isdir(PathToData):
+        raise FileNotFoundError(f'invalid path supplied; {PathToData} does not exist')
+    AllFiles = glob.glob(str(PathToData / file_extension))
+    Files = []
+    for file in AllFiles:
+        head, tail = os.path.split(file)
+        Files.append(tail)
+    if not Files:
+        logging.error(f'no {file_extension} files in {PathToData}')
+
+    return Files
+
+def generate_run_all_scripts_shell_script(script_location, scripts_to_run, topas_location='~/topas38', G4_DATA='~/G4Data'):
+    """
+    generate a bash script to run a series of topas scripts
+
+    :param script_location: Directory where the scripts are stored
+    :type script_location: Path or str
+    :param scripts_to_run: a list of scripts to run
+    :type scripts_to_run: array like
+    :param topas_location: location of the topas executable
+    :type topas_location: Path or str
+    :param G4_DATA: location of the G4data
+    :type G4_DATA: Path or str
+    :return:
+    """
+    script_location = Path(script_location)
+    FileName = script_location / 'RunAllFiles.sh'
+    f = open(FileName, 'w+')
+    f.write('# !/bin/bash\n\n')
+    f.write('# This script sets up the topas environment then runs all listed files\n\n')
+    f.write('# ensure that any errors cause the script to stop executing:\n')
+    f.write('set - e\n\n')
+    f.write(f'export TOPAS_G4_DATA_DIR={str(G4_DATA)}\n')
+
+    # add in all topas scripts which need to be run:
+    for sim in scripts_to_run:
+        f.write('echo "Beginning analysis of: ' + sim.name + '"')
+        f.write('\n')
+        f.write(f'(time {str(topas_location)}/bin/topas {sim.name}) &> ../logs/{sim.name}')
+        f.write('\n')
+    f.write('\necho "All done!"\n')
+    # change file modifications:
+    st = os.stat(FileName)
+    os.chmod(FileName, st.st_mode | stat.S_IEXEC)
+    f.close()
```

### Comparing `TopasOpt-0.4.2/TopasOpt.egg-info/PKG-INFO` & `TopasOpt-0.4.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: TopasOpt
-Version: 0.4.2
+Version: 0.4.3
 Summary: optimisation for topas Monte Carlo
 Home-page: https://github.com/ACRF-Image-X-Institute/TopasOpt
 Author: Brendan Whelan
 Author-email: bwheelz360@gmail.com
 Project-URL: Bug Tracker, https://github.com/ACRF-Image-X-Institute/TopasOpt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # TopasOpt
 
-![](docsrc/_resources/interrogate_badge.svg) [![codecov](https://codecov.io/gh/ACRF-Image-X-Institute/TopasOpt/branch/master/graph/badge.svg?token=0FSEO19LCD)](https://codecov.io/gh/ACRF-Image-X-Institute/TopasOpt)![test](https://github.com/ACRF-Image-X-Institute/TopasOpt/actions/workflows/run_tests.yml/badge.svg) ![docs](https://github.com/ACRF-Image-X-Institute/TopasOpt/actions/workflows/build-docs.yml/badge.svg)
+![](docsrc/_resources/interrogate_badge.svg) [![codecov](https://codecov.io/gh/ACRF-Image-X-Institute/TopasOpt/branch/master/graph/badge.svg?token=0FSEO19LCD)](https://codecov.io/gh/ACRF-Image-X-Institute/TopasOpt)![test](https://github.com/ACRF-Image-X-Institute/TopasOpt/actions/workflows/run_tests.yml/badge.svg) ![docs](https://github.com/ACRF-Image-X-Institute/TopasOpt/actions/workflows/build-docs.yml/badge.svg)[![PyPI version](https://badge.fury.io/py/TopasOpt.svg)](https://badge.fury.io/py/TopasOpt)
 
 
 This code provides a framework for performing optimisation on monte carlo radiation transport 
 simulations using [TOPAS](https://www.google.com/search?channel=fs&client=ubuntu&q=topas+MC).
 
 ## Install and Requirements
 
@@ -37,13 +37,30 @@
 ## Directory Structure
 
 - **TopasOpt:** source code
 - **examples:** source code for the [worked examples](https://acrf-image-x-institute.github.io/TopasOpt/worked_examples.html) provided in the docs
 - **docsrc:** markdown/rst documentation.
 - **tests:** tests which are run through github actions
 
+## Citation
+
+This code is described in [this paper](https://aapm.onlinelibrary.wiley.com/doi/10.1002/mp.16126).
+If you use this code in your work, please cite this paper!
+
+```bibtex
+
+@article{whelan_topasopt_2022,
+	title = {{TopasOpt}: {An} open-source library for optimization with {Topas} {Monte} {Carlo}},
+	shorttitle = {{TopasOpt}},
+	journal = {Medical Physics},
+	author = {Whelan, Brendan and Loo Jr, Billy W. and Wang, Jinghui and Keall, Paul},
+	year = {2022},
+	note = {Publisher: Wiley Online Library},
+}
+
+```
```

### Comparing `TopasOpt-0.4.2/setup.cfg` & `TopasOpt-0.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [options]
 package_dir = 
 	= .
 packages = TopasOpt
 python_requires = >=3.8
 install_requires = 
 	numpy >= 1.9.0
-	scipy < 1.8.0
+	scipy
 	scikit-learn >= 0.18.0
 	bayesian-optimization
 	matplotlib
 	jsonpickle
 	topas2numpy
 
 [egg_info]
```

