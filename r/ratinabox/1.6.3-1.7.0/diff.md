# Comparing `tmp/ratinabox-1.6.3.tar.gz` & `tmp/ratinabox-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.6.3.tar", last modified: Thu May  4 12:25:12 2023, max compression
+gzip compressed data, was "ratinabox-1.7.0.tar", last modified: Tue Jun  6 19:29:57 2023, max compression
```

## Comparing `ratinabox-1.6.3.tar` & `ratinabox-1.7.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.861111 ratinabox-1.6.3/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.6.3/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-05-04 12:25:12.861244 ratinabox-1.6.3/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    26607 2023-04-24 16:38:06.000000 ratinabox-1.6.3/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.6.3/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.854160 ratinabox-1.6.3/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    43226 2023-05-04 11:27:59.000000 ratinabox-1.6.3/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    32568 2023-04-27 09:08:29.000000 ratinabox-1.6.3/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    83295 2023-05-04 11:28:06.000000 ratinabox-1.6.3/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.6.3/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3874 2023-04-27 09:08:29.000000 ratinabox-1.6.3/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.856412 ratinabox-1.6.3/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-23 10:24:42.000000 ratinabox-1.6.3/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-23 10:24:42.000000 ratinabox-1.6.3/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-23 10:24:42.000000 ratinabox-1.6.3/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.6.3/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.6.3/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3402 2023-04-24 16:38:06.000000 ratinabox-1.6.3/ratinabox/contribs/SuccessorFeatures.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-23 10:24:42.000000 ratinabox-1.6.3/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7522 2023-04-24 16:38:06.000000 ratinabox-1.6.3/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.6.3/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.857519 ratinabox-1.6.3/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.6.3/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.6.3/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.6.3/ratinabox/data/rat.png
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.6.3/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.6.3/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    34484 2023-05-03 14:00:43.000000 ratinabox-1.6.3/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.854950 ratinabox-1.6.3/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-05-04 12:25:12.000000 ratinabox-1.6.3/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      907 2023-05-04 12:25:12.000000 ratinabox-1.6.3/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-05-04 12:25:12.000000 ratinabox-1.6.3/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-05-04 12:25:12.000000 ratinabox-1.6.3/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-05-04 12:25:12.000000 ratinabox-1.6.3/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-05-04 12:25:12.861568 ratinabox-1.6.3/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.6.3/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.860995 ratinabox-1.6.3/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.6.3/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.6.3/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.6.3/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.6.3/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.689907 ratinabox-1.7.0/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.7.0/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27991 2023-06-06 19:29:57.690044 ratinabox-1.7.0/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27271 2023-06-06 19:12:00.000000 ratinabox-1.7.0/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.7.0/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.682410 ratinabox-1.7.0/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    43768 2023-05-25 16:57:08.000000 ratinabox-1.7.0/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    32568 2023-04-27 09:08:29.000000 ratinabox-1.7.0/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    88673 2023-06-06 19:27:47.000000 ratinabox-1.7.0/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.7.0/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3986 2023-05-25 16:50:19.000000 ratinabox-1.7.0/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.685087 ratinabox-1.7.0/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-23 10:24:42.000000 ratinabox-1.7.0/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-23 10:24:42.000000 ratinabox-1.7.0/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-23 10:24:42.000000 ratinabox-1.7.0/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.7.0/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.7.0/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3402 2023-04-24 16:38:06.000000 ratinabox-1.7.0/ratinabox/contribs/SuccessorFeatures.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    56348 2023-06-06 18:34:59.000000 ratinabox-1.7.0/ratinabox/contribs/TaskEnvironment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-23 10:24:42.000000 ratinabox-1.7.0/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7522 2023-04-24 16:38:06.000000 ratinabox-1.7.0/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.7.0/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.686185 ratinabox-1.7.0/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.7.0/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.7.0/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.7.0/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.7.0/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.7.0/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    34824 2023-06-06 13:51:08.000000 ratinabox-1.7.0/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.683367 ratinabox-1.7.0/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27991 2023-06-06 19:29:57.000000 ratinabox-1.7.0/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      945 2023-06-06 19:29:57.000000 ratinabox-1.7.0/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-06-06 19:29:57.000000 ratinabox-1.7.0/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       91 2023-06-06 19:29:57.000000 ratinabox-1.7.0/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-06-06 19:29:57.000000 ratinabox-1.7.0/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      979 2023-06-06 19:29:57.690381 ratinabox-1.7.0/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.7.0/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.689776 ratinabox-1.7.0/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.7.0/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.7.0/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.7.0/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.7.0/tests/test_neurons.py
```

### Comparing `ratinabox-1.6.3/LICENSE` & `ratinabox-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/PKG-INFO` & `ratinabox-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.6.3
+Version: 1.7.0
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: gymnasium
 License-File: LICENSE
 
 # RatInABox 
 ![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox) [![Downloads](https://static.pepy.tech/badge/ratinabox)](https://pepy.tech/project/ratinabox)
 
 `RatInABox` (see [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3)) is a toolkit for generating locomotion trajectories and complementary neural data for spatially and/or velocity selective cell types in complex continuous environments. 
 
@@ -56,14 +57,16 @@
 * **Biological**:   Simulate large populations of spatially and/or velocity modulated cell types. Neurons can be rate based or spiking. The random motion model is fitted to match real rodent motion. 
 * **Flexible**:     Simulate environments in 1D or 2D with arbitrarily wall arrangements.  Combine premade or bespoke `Neurons` classes into arbitrary deep networks (examples given).
 * **Fast**:         Simulating 1 minute of exploration in a 2D environment with 100 place cells (dt=10 ms) take just 2 seconds on a laptop (no GPU needed).
 * **Precise**:      No more prediscretised positions, tabular state spaces, or jerky movement policies. It's all continuous. 
 * **Easy**:         Sensible default parameters mean you can have realisitic simulation data to work with in ~10 lines of code.
 * **Visual**        Plot or animate trajectories, firing rate timeseries', spike rasters, receptive fields, heat maps, velocity histograms...using the plotting functions ([summarised here](./demos/list_of_plotting_fuctions.md)). 
 
+## Announcement about support for OpenAI's `gymnasium` <img src=".images/readme/gymnasium_logo.svg" width=25> API
+A new wrapper contributed by [@SynapticSage](https://github.com/SynapticSage) allows `RatInABox` to natively support OpenAI's [`gymnasium`](https://gymnasium.farama.org) API for standardised and multiagent reinforment learning. This can be used to flexibly integrate `RatInABox` with other RL libraries such as Stable-Baselines3 etc. and to build non-trivial tasks with objectives and time dependent rewards. Check it out [here](https://github.com/TomGeorge1234/RatInABox/blob/dev/ratinabox/contribs/TaskEnv_example_files/TaskEnvironment_basics.md).
 
 ## Get started 
 Many [demos](./demos/) are provided. Reading through the [example scripts](#example-scripts) (one simple and one extensive, duplicated at the bottom of the readme) these should be enough to get started. We also provide numerous interactive jupyter scripts as more in-depth case studies; for example one where `RatInABox` is used for [reinforcement learning](./demos/reinforcement_learning_example.ipynb), another for [neural decoding](./demos/decoding_position_example.ipynb) of position from firing rate. Jupyter scripts reproducing all figures in the [paper](./demos/paper_figures.ipynb) and [readme](./demos/readme_figures.ipynb) are also provided. All [demos](./demos/) can be run on Google Colab [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](./demos/)
 
 ## Installing and Importing
 **Requirements** are minimal (`python3`, `numpy`, `scipy` and `matplotlib`, listed in `setup.cfg`) and will be installed automatically.
```

### Comparing `ratinabox-1.6.3/README.md` & `ratinabox-1.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 * **Biological**:   Simulate large populations of spatially and/or velocity modulated cell types. Neurons can be rate based or spiking. The random motion model is fitted to match real rodent motion. 
 * **Flexible**:     Simulate environments in 1D or 2D with arbitrarily wall arrangements.  Combine premade or bespoke `Neurons` classes into arbitrary deep networks (examples given).
 * **Fast**:         Simulating 1 minute of exploration in a 2D environment with 100 place cells (dt=10 ms) take just 2 seconds on a laptop (no GPU needed).
 * **Precise**:      No more prediscretised positions, tabular state spaces, or jerky movement policies. It's all continuous. 
 * **Easy**:         Sensible default parameters mean you can have realisitic simulation data to work with in ~10 lines of code.
 * **Visual**        Plot or animate trajectories, firing rate timeseries', spike rasters, receptive fields, heat maps, velocity histograms...using the plotting functions ([summarised here](./demos/list_of_plotting_fuctions.md)). 
 
+## Announcement about support for OpenAI's `gymnasium` <img src=".images/readme/gymnasium_logo.svg" width=25> API
+A new wrapper contributed by [@SynapticSage](https://github.com/SynapticSage) allows `RatInABox` to natively support OpenAI's [`gymnasium`](https://gymnasium.farama.org) API for standardised and multiagent reinforment learning. This can be used to flexibly integrate `RatInABox` with other RL libraries such as Stable-Baselines3 etc. and to build non-trivial tasks with objectives and time dependent rewards. Check it out [here](https://github.com/TomGeorge1234/RatInABox/blob/dev/ratinabox/contribs/TaskEnv_example_files/TaskEnvironment_basics.md).
 
 ## Get started 
 Many [demos](./demos/) are provided. Reading through the [example scripts](#example-scripts) (one simple and one extensive, duplicated at the bottom of the readme) these should be enough to get started. We also provide numerous interactive jupyter scripts as more in-depth case studies; for example one where `RatInABox` is used for [reinforcement learning](./demos/reinforcement_learning_example.ipynb), another for [neural decoding](./demos/decoding_position_example.ipynb) of position from firing rate. Jupyter scripts reproducing all figures in the [paper](./demos/paper_figures.ipynb) and [readme](./demos/readme_figures.ipynb) are also provided. All [demos](./demos/) can be run on Google Colab [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](./demos/)
 
 ## Installing and Importing
 **Requirements** are minimal (`python3`, `numpy`, `scipy` and `matplotlib`, listed in `setup.cfg`) and will be installed automatically.
```

### Comparing `ratinabox-1.6.3/ratinabox/Agent.py` & `ratinabox-1.7.0/ratinabox/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -485,15 +485,14 @@
             dataset = os.path.join(
                 os.path.join(
                     os.path.abspath(os.path.join(ratinabox.__file__, os.pardir)),
                     "data",
                 ),
                 dataset + ".npz",
             )
-            print(dataset)
             try:
                 data = np.load(dataset)
             except FileNotFoundError:
                 print(
                     f"IMPORT FAILED. No datafile found at {dataset}. Please try a different one. For now the default inbuilt random policy will be used."
                 )
                 return
@@ -573,17 +572,17 @@
         Args:
             • t_start: start time in seconds (default = self.history['t'][0])
             • t_end: end time in seconds (default = self.history["t"][-1])
             • framerate: frames per second (default = None --> step=0 so, just whatever the data frequency (1/Ag.dt) is)
         """
 
         t = np.array(self.history["t"])
-        t_start = (t_start or t[0])
+        t_start = t_start or t[0]
         startid = np.nanargmin(np.abs(t - (t_start)))
-        t_end = (t_end or t[-1])
+        t_end = t_end or t[-1]
         endid = np.nanargmin(np.abs(t - (t_end)))
         if framerate is None:
             skiprate = 1
         else:
             skiprate = max(1, int((1 / framerate) / self.dt))
 
         return slice(startid, endid, skiprate)
@@ -636,15 +635,14 @@
             if color is None:
                 color = "#7b699a"
         else:
             agent_list = self.Environment.Agents
         replot_env = True
         for i, self_ in enumerate(agent_list):
             t_end = t_end or self_.history["t"][-1]
-            print("t_end:", t_end)
             slice = self_.get_history_slice(
                 t_start=t_start, t_end=t_end, framerate=framerate
             )
             time = np.array(self_.history["t"])[slice]
             trajectory = np.array(self_.history["pos"])[slice]
             if color is None:
                 color_list = [f"C{i}"] * len(time)
@@ -690,30 +688,43 @@
                 # rect = 0.5, 0.4, 0.4, 0.4 # What should these values be?
                 # newax = fig.add_axes(rect, anchor='NE', zorder=1)
                 # newax.axis('off')
                 # newax.imshow(rat)
 
             if self_.Environment.dimensionality == "1D":
                 if fig is None and ax is None:
-                    fig, ax = plt.subplots(figsize=(3, 1.5))
+                    w, h = ratinabox.MOUNTAIN_PLOT_WIDTH_MM / 25, 2
+                    dw, dh = 1, 1
+                    fig = plt.figure(figsize=(w + dw, h + dh))
+                    ax = fig.add_axes(
+                        [
+                            dw / (2 * (w + dw)),
+                            dh / (2 * (h + dh)),
+                            w / (w + dw),
+                            h / (h + dh),
+                        ]
+                    )
+                    # fig = plt.figure
+                    # fig, ax = plt.subplots(figsize=(3, 1.5))
                 ax.scatter(
                     time / 60, trajectory, alpha=alpha, linewidth=0, c=color_list, s=5
                 )
                 ax.spines["left"].set_position(("data", t_start / 60))
                 if axis_labels == True:
                     ax.set_xlabel("Time / min")
                     ax.set_ylabel("Position / m")
                 ax.set_xlim([t_start / 60, t_end / 60])
                 if xlim is not None:
                     ax.set_xlim(right=xlim)
 
                 ax.set_ylim(bottom=0, top=self_.Environment.extent[1])
-                ax.spines["right"].set_color(None)
-                ax.spines["top"].set_color(None)
+                ax.spines["right"].set_visible(False)
+                ax.spines["top"].set_visible(False)
                 ax.set_xticks([t_start / 60, t_end / 60])
+                ax.set_xticklabels([round(t_start / 60, 2), round(t_end / 60, 2)])
                 ex = self_.Environment.extent
                 ax.set_yticks([ex[1]])
                 if background_color is not None:
                     ax.set_facecolor(background_color)
                     fig.patch.set_facecolor(background_color)
 
         ratinabox.utils.save_figure(fig, "trajectory", save=autosave)
@@ -868,17 +879,17 @@
             fig, ax = plt.subplots()
         n, bins, patches = ax.hist(
             speeds, bins=np.linspace(0, 1.2, 100), color=color, alpha=0.8, density=True
         )
         ax.set_xlabel(r"Speed  / $ms^{-1}$")
         ax.set_yticks([])
         ax.set_xlim(left=0, right=8 * std)
-        ax.spines["left"].set_color(None)
-        ax.spines["right"].set_color(None)
-        ax.spines["top"].set_color(None)
+        ax.spines["left"].set_visible(False)
+        ax.spines["right"].set_visible(False)
+        ax.spines["top"].set_visible(False)
 
         ratinabox.utils.save_figure(fig, "speed_histogram", save=autosave)
 
         if return_data == True:
             return fig, ax, n, bins, patches
         else:
             return fig, ax
@@ -912,17 +923,17 @@
             bins=np.linspace(-2000, 2000, 100),
             color=color,
             alpha=0.8,
             density=False,
         )
         ax.set_yticks([])
         ax.set_xlim(-5 * std, 5 * std)
-        ax.spines["left"].set_color(None)
-        ax.spines["right"].set_color(None)
-        ax.spines["top"].set_color(None)
+        ax.spines["left"].set_visible(False)
+        ax.spines["right"].set_visible(False)
+        ax.spines["top"].set_visible(False)
         ax.set_xlabel(r"Rotational velocity / $^{\circ} s^{-1}$")
 
         ratinabox.utils.save_figure(fig, "rotational_velocity_histogram", save=autosave)
 
         if return_data == True:
             return fig, ax, n, bins, patches
         return fig, ax
```

### Comparing `ratinabox-1.6.3/ratinabox/Environment.py` & `ratinabox-1.7.0/ratinabox/Environment.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/Neurons.py` & `ratinabox-1.7.0/ratinabox/Neurons.py`

 * *Files 4% similar despite different names*

```diff
@@ -427,15 +427,15 @@
                             norm_by_bincount=True,
                         )
                         im = ax_.imshow(
                             rate_map,
                             extent=ex,
                             cmap="inferno",
                             interpolation="bicubic",
-                            zorder=1,
+                            zorder=0,
                         )
                     ims.append(im)
                     vmin, vmax = (
                         min(vmin, np.min(rate_map)),
                         max(vmax, np.max(rate_map)),
                     )
                 for im in ims:
@@ -449,17 +449,19 @@
 
             if spikes is True:
                 for i, ax_ in enumerate(axes):
                     pos_where_spiked = pos[spike_data[chosen_neurons[i], :]]
                     ax_.scatter(
                         pos_where_spiked[:, 0],
                         pos_where_spiked[:, 1],
-                        s=2,
+                        s=3,
                         linewidth=0,
                         alpha=0.7,
+                        zorder=1.2,
+                        color=(self.color or "C1"),
                     )
 
         # PLOT 1D
         elif self.Agent.Environment.dimensionality == "1D":
             if method == "groundtruth":
                 rate_maps = rate_maps[chosen_neurons, :]
                 x = self.Agent.Environment.flattened_discrete_coords[:, 0]
@@ -598,15 +600,15 @@
             animate_,
             interval=1000 * dt,
             frames=int((t_end - t_start) / (dt * speed_up)),
             blit=False,
             fargs=(fig, ax, chosen_neurons, t_start, t_end, dt, speed_up),
         )
 
-        ratinabox.utils.save_animation(anim, "rat_timeseries", save=autosave)
+        ratinabox.utils.save_animation(anim, "rate_timeseries", save=autosave)
 
         return anim
 
     def return_list_of_neurons(self, chosen_neurons="all"):
         """Returns a list of indices corresponding to neurons.
 
         Args:
@@ -850,37 +852,45 @@
 
 
 class GridCells(Neurons):
     """The GridCells class defines a population of GridCells. This class is a subclass of Neurons() and inherits it properties/plotting functions.
 
     Must be initialised with an Agent and a 'params' dictionary.
 
-    GridCells defines a set of 'n' grid cells with random orientations, grid scales and offsets (these can be set non-randomly of coursse). Grids are modelled as the rectified sum of three cosine waves at 60 degrees to each other.
+    GridCells defines a set of 'n' grid cells with random orientations, grid scales and offsets (these can be set non-randomly of course). Grids are modelled as the rectified sum of three cosine waves at 60 degrees to each other.
+
+    To initialise grid cells you specify three things: (i) params['gridscale'], (ii) params['orientation'] and (iii) params['phase_offset']. These are all sampled from a distribution (specified as, e.g. params['phase_offset_distribution']) and then used to calculate the firing rate of each grid cell. For each of these there quantities the value you specify parameterises the distribution from which it is sampled. For example params['gridscale':0.45,'gridscale_distribution':'uniform'] will pull gridscales from a uniform distribution between 0 and 0.45m. The 'delta' distribution means a constant will be taken. For all three of these you can optionally just pass an array of length GridCells.n (in which case the corresponding distribution parameter is ignored). This array is set a the value for each grid cell.
 
     List of functions:
         • get_state()
+        • set_phase_offsets()
+
 
     default_params = {
             "n": 10,
-            "gridscale": 0.45,
-            "random_orientations": True,
-            "random_gridscales": True,
-            "random_phase_offsets": True,
+            "gridscale": 0.45, 
+            "gridscale_distribution": "uniform",
+            "orientation": None, 
+            "orientation_distribution": "uniform",
+            "phase_offset": True,
+            "phase_offset_distribution": "uniform",
             "min_fr": 0,
             "max_fr": 1,
             "name": "GridCells",
         }
     """
 
     default_params = {
         "n": 10,
-        "gridscale": 0.45,
-        "random_orientations": True,
-        "random_gridscales": True,
-        "random_phase_offsets": True,
+        "gridscale": 0.50, 
+        "gridscale_distribution": "rayleigh",
+        "orientation": None, 
+        "orientation_distribution": "uniform",
+        "phase_offset": True,
+        "phase_offset_distribution": "uniform",
         "min_fr": 0,
         "max_fr": 1,
         "name": "GridCells",
     }
 
     def __init__(self, Agent, params={}):
         """Initialise GridCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
@@ -889,40 +899,82 @@
             params (dict, optional). Defaults to {}."""
 
         self.Agent = Agent
 
         self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
+        # deprecation warnings
+        if ("random_gridscales" in self.params) or ("random_orientations" in self.params) or ("random_phase_offsets" in self.params):
+            warnings.warn("the GridCell API has changed slightly, 'random_gridscales', 'random_orientations' and 'random_phase_offsets' are no longer accepted as parameters. Please use 'gridscale','gridscale_distribution','orientation','orientation_distribution','phase_offset' and 'phase_offset_distribution' instead. See docstring or 1.7.0 release notes for instructions.")
+
+        # Initialise the gridscales
+        if hasattr(self.params["gridscale"],"__len__"):
+            self.gridscales = np.array(self.params["gridscale"])
+            self.params['n'] = len(self.gridscales)
+        else: 
+            if self.params['gridscale_distribution'] == "uniform":
+                self.gridscales = np.random.uniform(0, self.params["gridscale"], self.params["n"])
+            elif self.params['gridscale_distribution'] == "rayleigh":
+                self.gridscales = np.random.rayleigh(scale=self.params["gridscale"], size=self.params["n"])
+            elif self.params['gridscale_distribution'] == "delta":
+                self.gridscales = np.ones(self.params["n"]) * self.params["gridscale"]
+            else:
+                raise ValueError("gridscale distribution not recognised")
+        
+        # Initialise Neurons parent class
         super().__init__(Agent, self.params)
 
+
+        #Initialise phase offsets for each grid cell
+        if hasattr(self.params["phase_offset"],"__len__") and len(np.array(self.params['phase_offset']).shape) == 2:
+            self.phase_offsets = np.array(self.params["phase_offset"])
+            assert len(self.phase_offsets) == self.params["n"], "number of phase offsets supplied incompatible with number of neurons"
+        else:
+            if self.params['phase_offset_distribution'] == "uniform":
+                self.phase_offsets = np.random.uniform(0, 2*np.pi, size=(self.params["n"],2))
+            elif self.params['phase_offset_distribution'] == "delta":
+                phase_offset = self.params["phase_offset"] or np.array([0,0])
+                self.phase_offsets = np.ones((self.params["n"],2)) * np.array(phase_offset)
+            elif self.params['phase_offset_distribution'] == "grid":
+                self.phase_offsets = self.set_phase_offsets_on_grid()
+            else:
+                raise ValueError("phase offset distribution not recognised")
+        
+        #Initialise orientations for each grid cell
+        if hasattr(self.params["orientation"],"__len__"):
+            self.orientations = np.array(self.params["orientation"])
+            assert len(self.orientations) == self.params["n"], "number of orientations supplied incompatible with number of neurons"
+        else:
+            if self.params['orientation_distribution'] == "uniform":
+                self.orientations = np.random.uniform(0, 2*np.pi, size=(self.params["n"],))
+            elif self.params['orientation_distribution'] == "delta":
+                orientation = self.params["orientation"] or 0
+                self.orientations = np.ones(self.params["n"]) * orientation
+            else:
+                raise ValueError("orientation distribution not recognised")
+        
+
         # Initialise grid cells
         assert (
             self.Agent.Environment.dimensionality == "2D"
         ), "grid cells only available in 2D"
-        if self.random_phase_offsets == True:
-            self.phase_offsets = np.random.uniform(0, self.gridscale, size=(self.n, 2))
-        else:
-            self.phase_offsets = self.set_phase_offsets()
+
         w = []
         for i in range(self.n):
             w1 = np.array([1, 0])
-            if self.random_orientations == True:
-                w1 = utils.rotate(w1, np.random.uniform(0, 2 * np.pi))
+            w1 = utils.rotate(w1, self.orientations[i])
             w2 = utils.rotate(w1, np.pi / 3)
             w3 = utils.rotate(w1, 2 * np.pi / 3)
             w.append(np.array([w1, w2, w3]))
         self.w = np.array(w)
-        if self.random_gridscales == True:
-            self.gridscales = np.random.rayleigh(scale=self.gridscale, size=self.n)
-        else:
-            self.gridscales = np.full(self.n, fill_value=self.gridscale)
+
         if ratinabox.verbose is True:
             print(
-                "GridCells successfully initialised. You can also manually set their gridscale (GridCells.gridscales), offsets (GridCells.phase_offset) and orientations (GridCells.w1, GridCells.w2,GridCells.w3 give the cosine vectors)"
+                "GridCells successfully initialised. You can also manually set their gridscale (GridCells.gridscales), offsets (GridCells.phase_offsets) and orientations (GridCells.w1, GridCells.w2,GridCells.w3 give the cosine vectors)"
             )
         return
 
     def get_state(self, evaluate_at="agent", **kwargs):
         """Returns the firing rate of the grid cells.
         By default position is taken from the Agent and used to calculate firing rates. This can also by passed directly (evaluate_at=None, pos=pass_array_of_positions) or you can use all the positions in the environment (evaluate_at="all").
 
@@ -936,16 +988,17 @@
         else:
             pos = kwargs["pos"]
         pos = np.array(pos)
         pos = pos.reshape(-1, pos.shape[-1])
 
         # grid cells are modelled as the thresholded sum of three cosines all at 60 degree offsets
         # vectors to grids cells "centred" at their (random) phase offsets
+        origin = self.gridscales.reshape(-1,1)*self.phase_offsets/(2*np.pi)
         vecs = utils.get_vectors_between(
-            self.phase_offsets, pos
+            origin, pos
         )  # shape = (N_cells,N_pos,2)
         w1 = np.tile(np.expand_dims(self.w[:, 0, :], axis=1), reps=(1, pos.shape[0], 1))
         w2 = np.tile(np.expand_dims(self.w[:, 1, :], axis=1), reps=(1, pos.shape[0], 1))
         w3 = np.tile(np.expand_dims(self.w[:, 2, :], axis=1), reps=(1, pos.shape[0], 1))
         gridscales = np.tile(
             np.expand_dims(self.gridscales, axis=1), reps=(1, pos.shape[0])
         )
@@ -956,66 +1009,70 @@
         firingrate[firingrate < 0] = 0
 
         firingrate = (
             firingrate * (self.max_fr - self.min_fr) + self.min_fr
         )  # scales from being between [0,1] to [min_fr, max_fr]
         return firingrate
 
-    def set_phase_offsets(self):
-        """Set non-random phase_offsets. Most offsets (cell number: x*y) are grid-like, while the remainings (cell number: n - x*y) are random."""
+    def set_phase_offsets_on_grid(self):
+        """Set non-random phase_offsets. Most offsets (n_on_grid, the largest square numer before self.n) will tile a grid of 0 to 2pi in x and 0 to 2pi in y, while the remainings (cell number: n - n_on_grid) are random."""
         n_x = int(np.sqrt(self.n))
         n_y = self.n // n_x
         n_remaining = self.n - n_x * n_y
 
-        dx = self.gridscale / n_x
-        dy = self.gridscale / n_y
+        dx = 2*np.pi / n_x
+        dy = 2*np.pi / n_y
 
         grid = np.mgrid[
-            (0 + dx / 2) : (self.gridscale - dx / 2) : (n_x * 1j),
-            (0 + dy / 2) : (self.gridscale - dy / 2) : (n_y * 1j),
+            (0 + dx / 2) : (2*np.pi - dx / 2) : (n_x * 1j),
+            (0 + dy / 2) : (2*np.pi - dy / 2) : (n_y * 1j),
         ]
         grid = grid.reshape(2, -1).T
-        remaining = np.random.uniform(0, self.gridscale, size=(n_remaining, 2))
+        remaining = np.random.uniform(0, 2*np.pi, size=(n_remaining, 2))
 
         all_offsets = np.vstack([grid, remaining])
 
         return all_offsets
 
 
 class BoundaryVectorCells(Neurons):
     """The BoundaryVectorCells class defines a population of Boundary Vector Cells. This class is a subclass of Neurons() and inherits it properties/plotting functions.
 
     Must be initialised with an Agent and a 'params' dictionary.
 
     BoundaryVectorCells defines a set of 'n' BVCs cells with random orientations preferences, distance preferences  (these can be set non-randomly of course). We use the model described firstly by Hartley et al. (2000) and more recently de Cothi and Barry (2000).
 
+    Distance preferences of each BVC are drawn fro ma random distribution which can be one of "uniform" (default), "rayleigh", "normal", and "delta" and parameterised by "wall_pref_dist".
+
     BVCs can have allocentric (mec,subiculum) OR egocentric (ppc, retrosplenial cortex) reference frames.
 
     List of functions:
         • get_state()
         • boundary_vector_preference_function()
 
     default_params = {
             "n": 10,
             "reference_frame": "allocentric",
             "pref_wall_dist": 0.15,
+            "pref_wall_dist_distribution": "uniform",
             "angle_spread_degrees": 11.25,
             "xi": 0.08,  # as in de cothi and barry 2020
             "beta": 12,
             "dtheta":2, #angular resolution in degrees
             "min_fr": 0,
             "max_fr": 1,
             "name": "BoundaryVectorCells",
         }
     """
 
     default_params = {
         "n": 10,
         "reference_frame": "allocentric",
-        "pref_wall_dist": 0.15,
+        "pref_wall_dist": 0.25,
+        "pref_wall_dist_distribution": "uniform",
         "angle_spread_degrees": 11.25,
         "xi": 0.08,
         "beta": 12,
         "dtheta": 2,
         "min_fr": 0,
         "max_fr": 1,
         "name": "BoundaryVectorCells",
@@ -1055,18 +1112,37 @@
             test_angles.append(2 * np.pi * i * self.dtheta / 360)
         self.test_directions = np.array(test_directions)
         self.test_angles = np.array(test_angles)
         self.sigma_angles = np.array(
             [(self.angle_spread_degrees / 360) * 2 * np.pi] * self.n
         )
         self.tuning_angles = np.random.uniform(0, 2 * np.pi, size=self.n)
-        self.tuning_distances = np.random.rayleigh(
-            scale=self.pref_wall_dist,
-            size=self.n,
-        )
+
+        # define tuning distances from specific distribution in params dict
+        if self.pref_wall_dist_distribution == "rayleigh":
+            self.tuning_distances = np.random.rayleigh(
+                scale=self.pref_wall_dist, size=self.n
+            )
+        elif self.pref_wall_dist_distribution == "uniform":
+            self.tuning_distances = np.random.uniform(
+                low=0, high=self.pref_wall_dist * 2, size=self.n
+            )
+        elif self.pref_wall_dist_distribution == "normal":
+            lower, upper = 0, self.Agent.Environment.scale
+            mu, sigma = self.pref_wall_dist, self.pref_wall_dist / 2
+            self.tuning_distances = scipy.stats.truncnorm.rvs(
+                (lower - mu) / sigma,
+                (upper - mu) / sigma,
+                scale=sigma,
+                loc=mu,
+                size=self.n,
+            )
+        elif self.pref_wall_dist_distribution == "delta":
+            self.tuning_distances = self.pref_wall_dist * np.ones(self.n)
+
         self.sigma_distances = self.tuning_distances / beta + xi
 
         # calculate normalising constants for BVS firing rates in the current environment. Any extra walls you add from here onwards you add will likely push the firingrate up further.
         locs = self.Agent.Environment.discretise_environment(dx=0.04)
         locs = locs.reshape(-1, locs.shape[-1])
         self.cell_fr_norm = np.ones(self.n)
         self.cell_fr_norm = np.max(self.get_state(evaluate_at=None, pos=locs), axis=1)
@@ -1476,24 +1552,24 @@
 
     List of functions:
         • get_state()
 
     default_params = {
             "min_fr": 0,
             "max_fr": 1,
-            "n":1,
+            "n":10,
             "angle_spread_degrees":30,
             "name": "HeadDirectionCells",
         }
     """
 
     default_params = {
         "min_fr": 0,
         "max_fr": 1,
-        "n": 4,
+        "n": 10,
         "angular_spread_degrees": 45,  # width of HDC preference function (degrees)
         "name": "HeadDirectionCells",
     }
 
     def __init__(self, Agent, params={}):
         """Initialise HeadDirectionCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
         Args:
@@ -1838,15 +1914,15 @@
         else:
             V = np.zeros((self.n, kwargs["pos"].shape[0]))
 
         for inputlayer in self.inputs.values():
             w = inputlayer["w"]
             if evaluate_at == "last":
                 I = inputlayer["layer"].firingrate
-            else:  # kick can down the road let input layer decide how to evaluate the firingrate
+            else:  # kick can down the road let input layer decide how to evaluate the firingrate. this is core to feedforward layer as this recursive call will backprop through the upstraem layers until it reaches a "core" (e.g. place cells) layer which will then evaluate the firingrate. 
                 I = inputlayer["layer"].get_state(evaluate_at, **kwargs)
             inputlayer["I_temp"] = I
             V += np.matmul(w, I)
 
         biases = self.biases
         if biases.shape != V.shape:
             biases = biases.reshape((-1, 1))
```

### Comparing `ratinabox-1.6.3/ratinabox/README.md` & `ratinabox-1.7.0/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/__init__.py` & `ratinabox-1.7.0/ratinabox/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # rcParams['font.family'] = 'sans-serif'
     # rcParams['font.sans-serif'] = 'Helvetica'
     rcParams["text.color"] = darkgrey
     rcParams["axes.labelcolor"] = darkgrey
     rcParams["xtick.color"] = darkgrey
     rcParams["ytick.color"] = darkgrey
     # FIGURE
-    rcParams["figure.dpi"] = 150
+    rcParams["figure.dpi"] = 200
     rcParams["figure.figsize"] = [1, 1]  # 2 x 2 inches
     rcParams["figure.titlesize"] = "medium"
     # AXES
     rcParams["axes.labelsize"] = 8
     rcParams["axes.labelpad"] = 3
     rcParams["axes.titlepad"] = 3
     rcParams["axes.titlesize"] = 8
@@ -82,14 +82,17 @@
     # BOXPLOTS
     rcParams["boxplot.flierprops.linewidth"] = 1
     rcParams["boxplot.meanprops.linewidth"] = 1
     rcParams["boxplot.medianprops.linewidth"] = 1
     rcParams["boxplot.boxprops.linewidth"] = 1
     rcParams["boxplot.whiskerprops.linewidth"] = 1
     rcParams["boxplot.capprops.linewidth"] = 1
+    # SAVEFIG
+    rcParams["savefig.facecolor"] = [1, 1, 1, 0]
+    rcParams["savefig.edgecolor"] = [1, 1, 1, 0]
     # COLORSCHEME
     rcParams["axes.prop_cycle"] = cycler(
         "color",
         [
             "#7b699a",
             "#37738f",
             "#2eb37f",
```

### Comparing `ratinabox-1.6.3/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.7.0/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.7.0/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.7.0/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/contribs/README.md` & `ratinabox-1.7.0/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.7.0/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/contribs/SuccessorFeatures.py` & `ratinabox-1.7.0/ratinabox/contribs/SuccessorFeatures.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.7.0/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.7.0/ratinabox/contribs/ValueNeuron.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/data/README.md` & `ratinabox-1.7.0/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/data/rat.png` & `ratinabox-1.7.0/ratinabox/data/rat.png`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/data/sargolini.npz` & `ratinabox-1.7.0/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/data/tanni.npz` & `ratinabox-1.7.0/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/ratinabox/utils.py` & `ratinabox-1.7.0/ratinabox/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from datetime import datetime
 from scipy import stats as stats
 import ratinabox
 
 """OTHER USEFUL FUNCTIONS"""
 """Geometry functions"""
 
+
 def get_perpendicular(a=None):
     """Given 2-vector, a, returns its perpendicular
     Args:
         a (array, optional): 2-vector direction. Defaults to None.
     Returns:
         array: perpendicular to a
     """
@@ -497,18 +498,26 @@
     Returns:
         fig, ax: _description_
     """
     c = color or "C1"
     c = np.array(matplotlib.colors.to_rgb(c))
     fc = 0.3 * c + (1 - 0.3) * np.array([1, 1, 1])  # convert rgb+alpha to rgb
 
-    NbyX = overlap * NbyX / (np.max(np.abs(NbyX)) if norm_by=="max" else norm_by)
+    NbyX = overlap * NbyX / (np.max(np.abs(NbyX)) if norm_by == "max" else norm_by)
     if fig is None and ax is None:
-        fig, ax = plt.subplots()
-        fig.set_size_inches(width / 25, len(NbyX) * shift / 25)
+        w, h = width / 25, len(NbyX) * shift / 25
+        # fig, ax = plt.subplots()
+        # fig.set_size_inches(w,h)
+
+        # new way: adds extra space for captions etc. within figure frame
+        dw, dh = 1, 1  # extra space for captions
+        fig = plt.figure(figsize=(w + dw, h + dh))
+        ax = fig.add_axes(
+            [dw / (2 * (w + dw)), dh / (2 * (h + dh)), w / (w + dw), h / (h + dh)]
+        )
 
     zorder = 1
     for i in range(len(NbyX)):
         ax.plot(X, NbyX[i] + i + 1, c=c, zorder=zorder)
         zorder -= 0.01
         ax.fill_between(
             X, NbyX[i] + i + 1, i + 1, color=fc, zorder=zorder, alpha=0.8, linewidth=0
@@ -516,17 +525,17 @@
         zorder -= 0.01
     ax.spines["left"].set_bounds(1, len(NbyX))
     ax.spines["bottom"].set_position(("outward", 1))
     ax.spines["left"].set_position(("outward", 1))
     ax.set_yticks([1, len(NbyX)])
     ax.set_ylim(1 - 0.5, len(NbyX) + 1.1 * overlap)
     ax.set_xticks(np.arange(max(X + 0.1)))
-    ax.spines["left"].set_color(None)
-    ax.spines["right"].set_color(None)
-    ax.spines["top"].set_color(None)
+    ax.spines["left"].set_visible(False)
+    ax.spines["right"].set_visible(False)
+    ax.spines["top"].set_visible(False)
     ax.set_yticks([])
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     ax.set_ylim()
     if xlim is not None:
         ax.set_xlim(right=xlim)
 
@@ -628,15 +637,15 @@
                 if os.path.isfile(f"{path}.{filetype}"):
                     path = f"{path_}_{i}"
                     i += 1
                 elif i >= 100:
                     break
                 else:
                     break
-            fig.save(f"{path}.{filetype}")
+            fig.save(f"{path}.{filetype}", dpi=300)
 
     print(f"{file_type} saved to {os.path.abspath(path)}.{save_types}")
 
     return path
 
 
 def save_animation(*args, **kwargs):
```

### Comparing `ratinabox-1.6.3/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.7.0/ratinabox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.6.3
+Version: 1.7.0
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: gymnasium
 License-File: LICENSE
 
 # RatInABox 
 ![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox) [![Downloads](https://static.pepy.tech/badge/ratinabox)](https://pepy.tech/project/ratinabox)
 
 `RatInABox` (see [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3)) is a toolkit for generating locomotion trajectories and complementary neural data for spatially and/or velocity selective cell types in complex continuous environments. 
 
@@ -56,14 +57,16 @@
 * **Biological**:   Simulate large populations of spatially and/or velocity modulated cell types. Neurons can be rate based or spiking. The random motion model is fitted to match real rodent motion. 
 * **Flexible**:     Simulate environments in 1D or 2D with arbitrarily wall arrangements.  Combine premade or bespoke `Neurons` classes into arbitrary deep networks (examples given).
 * **Fast**:         Simulating 1 minute of exploration in a 2D environment with 100 place cells (dt=10 ms) take just 2 seconds on a laptop (no GPU needed).
 * **Precise**:      No more prediscretised positions, tabular state spaces, or jerky movement policies. It's all continuous. 
 * **Easy**:         Sensible default parameters mean you can have realisitic simulation data to work with in ~10 lines of code.
 * **Visual**        Plot or animate trajectories, firing rate timeseries', spike rasters, receptive fields, heat maps, velocity histograms...using the plotting functions ([summarised here](./demos/list_of_plotting_fuctions.md)). 
 
+## Announcement about support for OpenAI's `gymnasium` <img src=".images/readme/gymnasium_logo.svg" width=25> API
+A new wrapper contributed by [@SynapticSage](https://github.com/SynapticSage) allows `RatInABox` to natively support OpenAI's [`gymnasium`](https://gymnasium.farama.org) API for standardised and multiagent reinforment learning. This can be used to flexibly integrate `RatInABox` with other RL libraries such as Stable-Baselines3 etc. and to build non-trivial tasks with objectives and time dependent rewards. Check it out [here](https://github.com/TomGeorge1234/RatInABox/blob/dev/ratinabox/contribs/TaskEnv_example_files/TaskEnvironment_basics.md).
 
 ## Get started 
 Many [demos](./demos/) are provided. Reading through the [example scripts](#example-scripts) (one simple and one extensive, duplicated at the bottom of the readme) these should be enough to get started. We also provide numerous interactive jupyter scripts as more in-depth case studies; for example one where `RatInABox` is used for [reinforcement learning](./demos/reinforcement_learning_example.ipynb), another for [neural decoding](./demos/decoding_position_example.ipynb) of position from firing rate. Jupyter scripts reproducing all figures in the [paper](./demos/paper_figures.ipynb) and [readme](./demos/readme_figures.ipynb) are also provided. All [demos](./demos/) can be run on Google Colab [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](./demos/)
 
 ## Installing and Importing
 **Requirements** are minimal (`python3`, `numpy`, `scipy` and `matplotlib`, listed in `setup.cfg`) and will be installed automatically.
```

### Comparing `ratinabox-1.6.3/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.7.0/ratinabox.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ratinabox.egg-info/top_level.txt
 ratinabox/contribs/FieldOfViewNeurons.py
 ratinabox/contribs/PhasePrecessingPlaceCells.py
 ratinabox/contribs/PlaneWaveNeurons.py
 ratinabox/contribs/README.md
 ratinabox/contribs/STDPFeedForwardLayer.py
 ratinabox/contribs/SuccessorFeatures.py
+ratinabox/contribs/TaskEnvironment.py
 ratinabox/contribs/ThetaSequenceAgent.py
 ratinabox/contribs/ValueNeuron.py
 ratinabox/contribs/__init__.py
 ratinabox/data/README.md
 ratinabox/data/__init__.py
 ratinabox/data/rat.png
 ratinabox/data/sargolini.npz
```

### Comparing `ratinabox-1.6.3/setup.cfg` & `ratinabox-1.7.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.6.3
+version = 1.7.0
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
@@ -27,14 +27,17 @@
 	shapely
 python_requires = >=3.7
 include_package_data = False
 
 [options.extras_require]
 test = 
 	pytest
+	scikit-learn
+gymnasium = 
+	pettingzoo >= 1.23.0
 
 [options.package_data]
 ratinabox = data/*
 * = README.md
 
 [egg_info]
 tag_build =
```

### Comparing `ratinabox-1.6.3/tests/test_advanced.py` & `ratinabox-1.7.0/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.3/tests/test_environment.py` & `ratinabox-1.7.0/tests/test_environment.py`

 * *Files identical despite different names*

