# Comparing `tmp/hsmm_mvpy-0.1.0a2.tar.gz` & `tmp/hsmm_mvpy-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.1.0a2.tar", last modified: Thu May  4 10:17:52 2023, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0b0.tar", last modified: Tue Jun  6 12:33:32 2023, max compression
```

## Comparing `hsmm_mvpy-0.1.0a2.tar` & `hsmm_mvpy-0.1.0b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 10:17:52.635035 hsmm_mvpy-0.1.0a2/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0a2/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22533 2023-05-04 10:17:52.635035 hsmm_mvpy-0.1.0a2/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    20167 2023-05-04 09:20:47.000000 hsmm_mvpy-0.1.0a2/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      849 2023-05-04 10:17:42.000000 hsmm_mvpy-0.1.0a2/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-05-04 10:17:52.635035 hsmm_mvpy-0.1.0a2/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 10:17:52.635035 hsmm_mvpy-0.1.0a2/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 10:17:52.635035 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      171 2022-09-28 08:31:43.000000 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57128 2023-05-04 06:34:27.000000 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     8910 2023-05-02 16:12:55.000000 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    36660 2023-05-04 07:49:35.000000 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    20999 2023-05-03 22:23:27.000000 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 10:17:52.635035 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22533 2023-05-04 10:17:52.000000 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      343 2023-05-04 10:17:52.000000 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-05-04 10:17:52.000000 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       86 2023-05-04 10:17:52.000000 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-05-04 10:17:52.000000 hsmm_mvpy-0.1.0a2/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b0/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    23787 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    21421 2023-06-06 10:06:52.000000 hsmm_mvpy-0.1.0b0/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      844 2023-06-06 12:33:16.000000 hsmm_mvpy-0.1.0b0/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      171 2022-09-28 08:31:43.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    56649 2023-06-06 12:11:24.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    10494 2023-05-30 15:57:35.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    40133 2023-06-06 09:51:30.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    21011 2023-06-06 10:51:18.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    23787 2023-06-06 12:33:32.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      343 2023-06-06 12:33:32.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-06 12:33:32.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       83 2023-06-06 12:33:32.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-06 12:33:32.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.1.0a2/LICENSE.md` & `hsmm_mvpy-0.1.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0a2/PKG-INFO` & `hsmm_mvpy-0.1.0b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm_mvpy
-Version: 0.1.0a2
+Version: 0.1.0b0
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -37,30 +37,31 @@
 Project-URL: Bug Tracker, https://github.com/GWeindel/hmp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-HMP
+HsMM MVpy
 ==========
 
 ![](plots/general_illustration.png)
 
-hmp is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HsMM-MVPA) of electro-encephalographic (EEG) data based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
+HsMM MVpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HMP) of neural time-series (e.g. EEG) based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
 
-As a summary of the method, an HsMM-MVPA analysis parses the EEG into a number of significant cognitive event (called bumps) separated by flat period reflecting the ongoing stage initiated by a bump. Hence any reaction time can then be described by the number of bumps and stage estimated using hsmm_mvpy. The important aspect of HsMM-MVPA is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of cognitive events on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in the EEG (or MEG) signal:
-- Describing an experiment or a clinical sample in terms of processes detected in the EEG signal
+As a summary of the method, an HMP model parses the reaction time into a number of successive stages determined based on patterns in a neural time-serie. Hence any reaction time can then be described by a number of stage  and their duration estimated using hsmm_mvpy. The important aspect of HMP is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of stages on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in a signal:
+- Describing an experiment or a clinical sample in terms of stages detected in the EEG signal
 - Describing experimental effects based on a particular stage duration
-- Estimating the effect of trial-wise manipuations (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
-- Time-lock EEG signal to the onset of a given bump and perform classical ERPs or time-freauency analysis based on the events that are the estimated bumps
-- And many more (e.g. evidence accumulation models on decision stage, classification based on the number of events in the signal,...)
+- Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
+- Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
+- And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
+**Important note** The current tutorials are based on the latest (unstable) version not yet available through _pip_, installing through github is therefore recommended.
 
 The package is available through *pip* with the command ```pip install hsmm_mvpy```. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
@@ -68,103 +69,101 @@
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
 
-For the cutting edge version (not recommended) you can clone the repository using *git*
+For the cutting edge version you can clone the repository using *git*
 
 Open a terminal and type:
 
     $ git clone https://github.com/gweindel/hsmm_mvpy.git
    
 Then move to the clone repository and run 
     
     $ pip install -e .
 
+
 ## To get started
 To get started with the code:
 - Check the demo below 
 - Inspect the tutorials in the tutorials repository
     - Load EEG data (tutorial 1)
-    - Estimating a given number of bumps (tutorial 2)
-    - Test for the number of bumps that best explains the data (tutorial 3)
+    - Estimating a HMP with given number of stages (tutorial 2)
+    - Test for the number of stages that best explains the data (tutorial 3)
     - Testing differences across conditions (tutorial 4)
 
-To further learn about the method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)). The following list also contains a non-exhaustive list of papers published using the HsMM-MVPA method:
+To further learn about the method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)). The following list also contains a non-exhaustive list of papers published using HMP:
 - Berberyan, H. S., van Maanen, L., van Rijn, H., & Borst, J. (2021). EEG-based identification of evidence accumulation stages in decision-making. Journal of Cognitive Neuroscience, 33(3), 510-527. [link](https://doi.org/10.1162/jocn_a_01663)
 - Van Maanen, L., Portoles, O., & Borst, J. P. (2021). The discovery and interpretation of evidence accumulation stages. Computational brain & behavior, 4(4), 395-415. [link](https://link.springer.com/article/10.1007/s42113-021-00105-2)
 - Portoles, O., Blesa, M., van Vugt, M., Cao, M., & Borst, J. P. (2022). Thalamic bursts modulate cortical synchrony locally to switch between states of global functional connectivity in a cognitive task. PLoS computational biology, 18(3), e1009407. [link](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009407)
 
 ## Demo on simulated data
 
 The following section will quickly walk you through an example usage in simulated data (using [MNE](https://mne.tools/dev/auto_examples/simulation/index.html)'s simulation functions and tutorials)
 
 First we load the libraries necessary for the demo on simulated data
 
 ### Importing libraries
 
-
-
 ```python
 ## Importing these packages is specific for this simulation case
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from scipy.stats import gamma
 
 ## Importing HMP
 import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
-    <frozen importlib._bootstrap>:241: RuntimeWarning: scipy._lib.messagestream.MessageStream size changed, may indicate binary incompatibility. Expected 56 from C header, got 64 from PyObject
-
-
 ### Simulating data
 
-In the following code block we simulate 30 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HsM models. All these four sources are defined by a localization, an activation amplitude and a distribution (here gamma with shape and scale parameters) for the onsets of the bumps on each trial. The simulation functions are based on the [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
+In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HMP models. All these four sources are defined by a localization, an activation amplitude and a distribution (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
 _If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
 ```python
 cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
 n_trials = 50 #Number of trials to simulate
 
-##### Here we define the sources of the brain activity (bump) for each trial
-frequency = 10.#Frequency of the bump defining its duration, half-sine of 10Hz = 50ms
-amplitude = np.array([.1e-6,.1e-6,.1e-6,.1e-6,1e-20]) #Amplitude of the bump in Volt, defining signal to noise ratio
+##### Here we define the sources of the brain activity (event) for each trial
+frequency = 10.#Frequency of the event defining its duration, half-sine of 10Hz = 50ms
+amplitude = .5e-6 #Amplitude of the event in Volt, defining signal to noise ratio
 shape = 2 #shape of the gamma distribution
-means = np.array([60,150, 200, 100, 80])/shape #Mean duration of the stages separating bumps, in ms
+means = np.array([60, 150, 200, 100, 80])/shape #Mean duration of the stages in ms
 names = ['bankssts-rh','posteriorcingulate-lh','parahippocampal-lh',\
          'pericalcarine-rh','postcentral-lh']#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
 sources = []
-for source in zip(names, amplitude, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
-    sources.append([source[0], frequency, source[1], gamma(shape, scale=source[2])])
+for source in zip(names, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
+    sources.append([source[0], frequency, amplitude, gamma(shape, scale=source[1])])
 
 # Function used to generate the data
-file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', overwrite=False)
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True)
 #Recovering sampling frequency of the simulated dataset
 sfreq = simulations.simulation_sfreq()
 #load electrode position, specific to the simulations
 positions = simulations.simulation_positions()
 ```
 
-    ./dataset_README_raw.fif exists no new simulation performed
+    Simulating ./dataset_README_raw.fif
+    ./dataset_README_raw.fif simulated
+
 
 
 ### Creating the event structure and plotting the raw data
 
 
-To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 0 signal the onset of the stimulus and 5 the onset of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
+To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 1 signal the onset of the stimulus and 6 the moment of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
 
 
 ```python
 #Recovering the events to epoch the data (in the number of trials defined above)
 generating_events = np.load(file[1])
 resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
 event_id = {'stimulus':1}#trigger 1 = stimulus
@@ -177,149 +176,206 @@
 raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
 raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
 
     Using qt as 2D backend.
     Channels marked as bad:
     none
+    
 ![png](README_files/README_7_1.png)
 
 
-### Recovering number of sources as well as actual by-trial variation
 
-To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth
+### Recovering number of stages as well as actual by-trial variation
+
+To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of stages or sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth.
 
 
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
-#Recover the actual time of the simulated bumps
+#Recover the actual time of the simulated events
 random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
            (n_trials, number_of_sources))
 ```
 
-## Demo of the HsMM Code for a single participant in a single condition based on the simulated data
+## Demo for a single participant in a single condition based on the simulated data
 
 First we read the EEG data as we would for a single participant:
 
 
 ```python
 # Reading the data
-eeg_data = hmp.utils.read_mne_EEG(file[0], event_id, resp_id, sfreq, 
+eeg_data = hmp.utils.read_mne_data(file[0], event_id=event_id, resp_id=resp_id, sfreq=sfreq, 
             events_provided=events, verbose=False)
 
 ```
 
-    Processing participant ./dataset_README_raw.fif
-    Reading 0 ... 142583  =      0.000 ...   237.395 secs...
-    Creating epochs based on following event ID :[1 6]
-    N trials without response event: 0
-    Applying reaction time trim to keep RTs between 0.001 and 5 seconds
-    50 RTs kept of 50 clean epochs
+    Processing participant ./dataset_README_raw.fif's continuous eeg
+    Reading 0 ... 153075  =      0.000 ...   254.864 secs...
     50 trials were retained for participant ./dataset_README_raw.fif
-    End sampling frequency is 600.614990234375 Hz
 
 
 The package uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
 ```python
 #example of usage of xarray
 print(eeg_data)
 eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
     .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 843)
+    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 711)
     Coordinates:
       * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
       * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 836 837 838 839 840 841 842
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 704 705 706 707 708 709 710
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 2.469e-06...
-        event        (participant, epochs) <U8 'stimulus' 'stimulus' ... 'stimulus'
+        data         (participant, epochs, electrodes, samples) float64 1.96e-06 ...
     Attributes:
         sfreq:    600.614990234375
         offset:   0
 
 
 
     
-![png](README_files/README_13_1.png)
+![png](README_files/README_12_1.png)
     
 
 
+
 Next we transform the data as in Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) including standardization of individual variances (not in this case as we have only one simulated participant), z-scoring and spatial principal components analysis (PCA). 
 
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
-hsmm_dat = hmp.utils.transform_data(eeg_data.data, apply_standard=False, n_comp=4)
+hmp_data = hmp.utils.transform_data(eeg_data, apply_standard=False, n_comp=4)
 ```
 
-# Estimating an HsMM model
+Once the data is in the expected format, we can initialize an HMP
+
+
+```python
+init = hmp.models.hmp(hmp_data, eeg_data, event_width=50, cpus=cpus)#Initialization of the model
+```
+
+# HMP model
+
+We are looking for stages in the data (**Hidden Markov**) and assume that transitions between stages are signaled by a template in the data (**pattern analysis**). By default we use the same template as Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet'.apa.org/doi/10.1037/rev0000030)), a 10 Hz half-sine, resulting in a 50ms duration bump-like shape:
 
-We can directly fit an HsMM model without giving any info on the number of bumps (see tutorial 2 for the explanation of the following cell)
 
 
 ```python
-%%time
-init = hmp.models.hsmm(hsmm_dat, eeg_data, bump_width=50, cpus=cpus)#Initialization of the model
-estimates = init.fit(step=10, verbose=False)
+plt.plot(init.template,'x');
 ```
 
 
-      0%|          | 0/360 [00:00<?, ?it/s]
+    
+![png](README_files/README_18_0.png)
+    
+
+
+This pattern is assumed to be present in multiple electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
+
+
+
+```python
+epoch = 0 #illustrating the first trial
+hmp_data.unstack().sel(component=[0,1,2], epochs=epoch).squeeze().plot.line(hue='component');
+plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k')#overlaying the simulated stage transition times
+```
+
+
+    
+![png](README_files/README_20_1.png)
+    
+
 
 
-    CPU times: user 645 ms, sys: 1.6 ms, total: 647 ms
-    Wall time: 646 ms
+The by-trial onset of this transition event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
+
+
+```python
+T = 350
+plt.plot(np.linspace(0,T,1001),gamma.pdf(np.linspace(0,T,1001), 2, scale=50)) 
+plt.xlabel('t');
+```
+
+
+    
+![png](README_files/README_22_0.png)
+    
+
+
+And this is then the full explanation of an HMP model: Looking for a transition event across several electrodes and trials that signals a transition to the next stage and which onset is expected to follow a probability distribution (in this case a gamma).
+
+# Estimating an HMP model
+
+We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for the explanation of the following cell)
+
+
+
+```python
+estimates = init.fit(step=20, verbose=True)
+```
+
+
+    Transition event 2 found around sample 137
+    Transition event 3 found around sample 258
+    Transition event 4 found around sample 330
+    Estimating 4 events model
+    Parameters estimated for 4 events model
 
 
 ### Visualizing results of the fit
 
-In the previous cell we initiated an HsMM model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 bumps and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit
+In the previous cell we initiated an HMP model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 Transition events and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit.
+
+We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
+
 
-We can directly take a look to the topologies and latencies of the bumps by calling ```hmp.visu.plot_topo_timecourse```
+We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
 
 
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
                                positions, init,#position of the electrodes and initialized model
                                magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
                                times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
 
     
-![png](README_files/README_21_0.png)
+![png](README_files/README_27_0.png)
     
 
 
-This shows us the electrode activity on the scalp as well as the average time of occurence of the bump based on the stage distributions.
+This shows us the electrode activity on the scalp as well as the average time of occurence of the events based on the stage distributions.
 
-As we are estimating the bump onsets on a by-trial basis we can look at the by-trial variation in stage duration.
+As we are estimating the event onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
 
 ```python
-bump_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('bump')#computing predicted bump times
-ax = hmp.visu.plot_latencies_average(bump_times_estimates, init.bump_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
+event_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('event')#computing predicted event times
+ax = hmp.visu.plot_latencies_average(event_times_estimates, init.event_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
-![png](README_files/README_23_0.png)
+![png](README_files/README_29_0.png)
     
 
 
-For the same reason we can also inspect the probability distribution of bump onsets:
+For the same reason we can also inspect the probability distribution of event onsets:
+
 
 
 ```python
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)), survival=True)
 ```
 
@@ -328,118 +384,119 @@
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_25_1.png)
+![png](README_files/README_31_1.png)
     
 
 
 
     
-![png](README_files/README_25_2.png)
+![png](README_files/README_31_2.png)
     
 
 
-As HsMM-MVPA selected those bumps onset per trial we can also look at the predicted bump onsets for a single trial
+As HMP estimated stage onset per trial we can also look at the predicted stage onsets for a given trial.
 
 
 ```python
-hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 1)), 
+hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 0)), 
                             xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 ```
 
 
 
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_27_1.png)
+![png](README_files/README_33_1.png)
     
 
 
-This then shows the likeliest bump location in time for the first trial!
+This then shows the likeliest stage onset location in time for the first trial!
 
 ## Comparing with ground truth
 
-As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HsMM-MVpy. As in the beginning, this code is specific to the case where you simulate data.
+As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP-MVpy. As in the beginning, this code is specific to the case where you simulate data.
 
 
 ```python
 colors = sns.color_palette(None, number_of_sources)
-# plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(params=1)*2+np.concatenate([[0],np.repeat(init.bump_width_samples,number_of_sources-1)]), color=colors,s=50)
-plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(parameter=1)*2, color=colors,s=50)
+plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.prod(axis=1), color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
 plt.title('Actual vs estimated stage durations')
 plt.xlabel('Simulated stage duration')
 plt.ylabel('Estimated stage duration')
 plt.show()
 
 ```
 
 
     
-![png](README_files/README_30_0.png)
+![png](README_files/README_35_0.png)
     
 
 
 Or also overlay actual bumps onset with predicted one
 
 
+
 ```python
-hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated bump onsets',
+hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated event onsets',
         times_to_display = np.mean(np.cumsum(random_source_times,axis=1),axis=0))
 ```
 
 
     
-![png](README_files/README_32_0.png)
+![png](README_files/README_37_0.png)
     
 
 
-We see that the HsMM-MVpy package recovers the exact average location of the bumps defined in the simulated data
+We see that the HSMM-MVpy package recovers the exact average location of the bumps defined in the simulated data.
 
-We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HsMM model
+We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HMP model
 
 
 ```python
 fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
 i = 0
 
-for bump in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
-    sns.regplot(x=random_source_times[:,i].T, y=bump, ax=ax[i], color=colors[i])
-    ax[i].plot([np.min(bump), np.max(bump)], [np.min(bump), np.max(bump)],'--', color='k')
+for event in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
+    sns.regplot(x=random_source_times[:,i].T, y=event, ax=ax[i], color=colors[i])
+    ax[i].plot([np.min(event), np.max(event)], [np.min(event), np.max(event)],'--', color='k')
     ax[i].set_ylabel(f'Estimated by-trial stage duration for stage {i+1}')
     ax[i].set_xlabel(f'Simulated by-trial stage duration for stage {i+1}')
     i+= 1
 ```
 
 
     
-![png](README_files/README_35_0.png)
+![png](README_files/README_39_0.png)
     
 
 
 We see that every stage gets nicely recovered even on a by-trial basis!
 
 # Beyond summary statistics for EEG analysis
 
-Now the purpose, apart from determining the number and timecourse of important EEG events in the Rreaction time, is also to use the by-trial information.
+Now the purpose, apart from determining the number and time course of important EEG events in the reaction time, is also to use the by-trial information.
 
 We illustrate this by first plotting the traditional event-related potentials (i.e. taking the average of given electrodes across the different time points) with cherry-picked electrodes.
 
 
+
 ```python
 import seaborn as sns
 import pandas as pd
 
 data = eeg_data.stack({'trial_x_participant':['participant','epochs']}).data.dropna('trial_x_participant', how="all")
 fig, ax = plt.subplots(1,1, figsize=(20,5), sharey=True)
 
@@ -453,25 +510,25 @@
 plt.xlim(0,500)
 plt.ylim(-3e-6,3e-6);
 
 ```
 
 
     
-![png](README_files/README_38_0.png)
+![png](README_files/README_41_0.png)
     
 
 
-Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to trqditional ERPs with very clear signal in the beginning of a trial (as events are more in sync) and summed and blurried in later stages of the reaction times (as event are off sync).
+Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to traditional ERPs with very clear signal in the beginning of a trial (as events are more in phase) and summed and blurried in later stages of the reaction times (as event are off phase).
 
-Now things can get better if we first parse, by-trial, the signal into the different stages based on the HsMM estimates:
+Now things can get better if we first parse, by-trial, the signal into the different stages based on the HMP estimates:
 
 
 ```python
-BRP_times = init.compute_times(init, estimates.dropna('bump'), fill_value=0, add_rt=True)
+BRP_times = init.compute_times(init, estimates.dropna('event'), fill_value=0, add_rt=True)
 
 fig, ax = plt.subplots(1,number_of_sources, figsize=(20,5), sharey=True, sharex=True)
 ax[0].set_ylabel('Volt')
 for stage in range(number_of_sources):
     BRP = hmp.utils.event_times(data, BRP_times,'EEG 016',stage=stage)
     df = pd.DataFrame(BRP).melt(var_name='Time')
     sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkgreen')
@@ -482,21 +539,23 @@
     df = pd.DataFrame(BRP).melt(var_name='Time')
     sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkblue') 
     plt.xlim(0,100)
 ```
 
 
     
-![png](README_files/README_40_0.png)
+![png](README_files/README_43_0.png)
     
 
 
+
 In this case we clearly see at each stage the half-sin (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sin). Note that the end of the stages tend to be noisier because less trial are defining the average signal (also why the confidence interval grows).
 
 
 ### Follow-up
 
-For examples on how to use the package when the number of bumps are unkown, or to compare stage durations across conditions see the tutorial notebooks:
+For examples on how to use the package when the number of transition events/stages is unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
-- Estimating a given number of bumps (tutorial 2)
-- Test for the number of bumps that best explains the data (tutorial 3)
+- Estimating a given number of events (tutorial 2)
+- Test for the number of events that best explains the data (tutorial 3)
 - Testing differences across conditions (tutorial 4)
+
```

### Comparing `hsmm_mvpy-0.1.0a2/README.md` & `hsmm_mvpy-0.1.0b0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-HMP
+HsMM MVpy
 ==========
 
 ![](plots/general_illustration.png)
 
-hmp is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HsMM-MVPA) of electro-encephalographic (EEG) data based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
+HsMM MVpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HMP) of neural time-series (e.g. EEG) based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
 
-As a summary of the method, an HsMM-MVPA analysis parses the EEG into a number of significant cognitive event (called bumps) separated by flat period reflecting the ongoing stage initiated by a bump. Hence any reaction time can then be described by the number of bumps and stage estimated using hsmm_mvpy. The important aspect of HsMM-MVPA is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of cognitive events on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in the EEG (or MEG) signal:
-- Describing an experiment or a clinical sample in terms of processes detected in the EEG signal
+As a summary of the method, an HMP model parses the reaction time into a number of successive stages determined based on patterns in a neural time-serie. Hence any reaction time can then be described by a number of stage  and their duration estimated using hsmm_mvpy. The important aspect of HMP is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of stages on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in a signal:
+- Describing an experiment or a clinical sample in terms of stages detected in the EEG signal
 - Describing experimental effects based on a particular stage duration
-- Estimating the effect of trial-wise manipuations (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
-- Time-lock EEG signal to the onset of a given bump and perform classical ERPs or time-freauency analysis based on the events that are the estimated bumps
-- And many more (e.g. evidence accumulation models on decision stage, classification based on the number of events in the signal,...)
+- Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
+- Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
+- And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
+**Important note** The current tutorials are based on the latest (unstable) version not yet available through _pip_, installing through github is therefore recommended.
 
 The package is available through *pip* with the command ```pip install hsmm_mvpy```. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
@@ -25,103 +26,101 @@
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
 
-For the cutting edge version (not recommended) you can clone the repository using *git*
+For the cutting edge version you can clone the repository using *git*
 
 Open a terminal and type:
 
     $ git clone https://github.com/gweindel/hsmm_mvpy.git
    
 Then move to the clone repository and run 
     
     $ pip install -e .
 
+
 ## To get started
 To get started with the code:
 - Check the demo below 
 - Inspect the tutorials in the tutorials repository
     - Load EEG data (tutorial 1)
-    - Estimating a given number of bumps (tutorial 2)
-    - Test for the number of bumps that best explains the data (tutorial 3)
+    - Estimating a HMP with given number of stages (tutorial 2)
+    - Test for the number of stages that best explains the data (tutorial 3)
     - Testing differences across conditions (tutorial 4)
 
-To further learn about the method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)). The following list also contains a non-exhaustive list of papers published using the HsMM-MVPA method:
+To further learn about the method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)). The following list also contains a non-exhaustive list of papers published using HMP:
 - Berberyan, H. S., van Maanen, L., van Rijn, H., & Borst, J. (2021). EEG-based identification of evidence accumulation stages in decision-making. Journal of Cognitive Neuroscience, 33(3), 510-527. [link](https://doi.org/10.1162/jocn_a_01663)
 - Van Maanen, L., Portoles, O., & Borst, J. P. (2021). The discovery and interpretation of evidence accumulation stages. Computational brain & behavior, 4(4), 395-415. [link](https://link.springer.com/article/10.1007/s42113-021-00105-2)
 - Portoles, O., Blesa, M., van Vugt, M., Cao, M., & Borst, J. P. (2022). Thalamic bursts modulate cortical synchrony locally to switch between states of global functional connectivity in a cognitive task. PLoS computational biology, 18(3), e1009407. [link](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009407)
 
 ## Demo on simulated data
 
 The following section will quickly walk you through an example usage in simulated data (using [MNE](https://mne.tools/dev/auto_examples/simulation/index.html)'s simulation functions and tutorials)
 
 First we load the libraries necessary for the demo on simulated data
 
 ### Importing libraries
 
-
-
 ```python
 ## Importing these packages is specific for this simulation case
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from scipy.stats import gamma
 
 ## Importing HMP
 import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
-    <frozen importlib._bootstrap>:241: RuntimeWarning: scipy._lib.messagestream.MessageStream size changed, may indicate binary incompatibility. Expected 56 from C header, got 64 from PyObject
-
-
 ### Simulating data
 
-In the following code block we simulate 30 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HsM models. All these four sources are defined by a localization, an activation amplitude and a distribution (here gamma with shape and scale parameters) for the onsets of the bumps on each trial. The simulation functions are based on the [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
+In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HMP models. All these four sources are defined by a localization, an activation amplitude and a distribution (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
 _If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
 ```python
 cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
 n_trials = 50 #Number of trials to simulate
 
-##### Here we define the sources of the brain activity (bump) for each trial
-frequency = 10.#Frequency of the bump defining its duration, half-sine of 10Hz = 50ms
-amplitude = np.array([.1e-6,.1e-6,.1e-6,.1e-6,1e-20]) #Amplitude of the bump in Volt, defining signal to noise ratio
+##### Here we define the sources of the brain activity (event) for each trial
+frequency = 10.#Frequency of the event defining its duration, half-sine of 10Hz = 50ms
+amplitude = .5e-6 #Amplitude of the event in Volt, defining signal to noise ratio
 shape = 2 #shape of the gamma distribution
-means = np.array([60,150, 200, 100, 80])/shape #Mean duration of the stages separating bumps, in ms
+means = np.array([60, 150, 200, 100, 80])/shape #Mean duration of the stages in ms
 names = ['bankssts-rh','posteriorcingulate-lh','parahippocampal-lh',\
          'pericalcarine-rh','postcentral-lh']#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
 sources = []
-for source in zip(names, amplitude, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
-    sources.append([source[0], frequency, source[1], gamma(shape, scale=source[2])])
+for source in zip(names, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
+    sources.append([source[0], frequency, amplitude, gamma(shape, scale=source[1])])
 
 # Function used to generate the data
-file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', overwrite=False)
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True)
 #Recovering sampling frequency of the simulated dataset
 sfreq = simulations.simulation_sfreq()
 #load electrode position, specific to the simulations
 positions = simulations.simulation_positions()
 ```
 
-    ./dataset_README_raw.fif exists no new simulation performed
+    Simulating ./dataset_README_raw.fif
+    ./dataset_README_raw.fif simulated
+
 
 
 ### Creating the event structure and plotting the raw data
 
 
-To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 0 signal the onset of the stimulus and 5 the onset of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
+To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 1 signal the onset of the stimulus and 6 the moment of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
 
 
 ```python
 #Recovering the events to epoch the data (in the number of trials defined above)
 generating_events = np.load(file[1])
 resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
 event_id = {'stimulus':1}#trigger 1 = stimulus
@@ -134,149 +133,206 @@
 raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
 raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
 
     Using qt as 2D backend.
     Channels marked as bad:
     none
+    
 ![png](README_files/README_7_1.png)
 
 
-### Recovering number of sources as well as actual by-trial variation
 
-To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth
+### Recovering number of stages as well as actual by-trial variation
+
+To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of stages or sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth.
 
 
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
-#Recover the actual time of the simulated bumps
+#Recover the actual time of the simulated events
 random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
            (n_trials, number_of_sources))
 ```
 
-## Demo of the HsMM Code for a single participant in a single condition based on the simulated data
+## Demo for a single participant in a single condition based on the simulated data
 
 First we read the EEG data as we would for a single participant:
 
 
 ```python
 # Reading the data
-eeg_data = hmp.utils.read_mne_EEG(file[0], event_id, resp_id, sfreq, 
+eeg_data = hmp.utils.read_mne_data(file[0], event_id=event_id, resp_id=resp_id, sfreq=sfreq, 
             events_provided=events, verbose=False)
 
 ```
 
-    Processing participant ./dataset_README_raw.fif
-    Reading 0 ... 142583  =      0.000 ...   237.395 secs...
-    Creating epochs based on following event ID :[1 6]
-    N trials without response event: 0
-    Applying reaction time trim to keep RTs between 0.001 and 5 seconds
-    50 RTs kept of 50 clean epochs
+    Processing participant ./dataset_README_raw.fif's continuous eeg
+    Reading 0 ... 153075  =      0.000 ...   254.864 secs...
     50 trials were retained for participant ./dataset_README_raw.fif
-    End sampling frequency is 600.614990234375 Hz
 
 
 The package uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
 ```python
 #example of usage of xarray
 print(eeg_data)
 eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
     .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 843)
+    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 711)
     Coordinates:
       * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
       * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 836 837 838 839 840 841 842
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 704 705 706 707 708 709 710
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 2.469e-06...
-        event        (participant, epochs) <U8 'stimulus' 'stimulus' ... 'stimulus'
+        data         (participant, epochs, electrodes, samples) float64 1.96e-06 ...
     Attributes:
         sfreq:    600.614990234375
         offset:   0
 
 
 
     
-![png](README_files/README_13_1.png)
+![png](README_files/README_12_1.png)
     
 
 
+
 Next we transform the data as in Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) including standardization of individual variances (not in this case as we have only one simulated participant), z-scoring and spatial principal components analysis (PCA). 
 
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
-hsmm_dat = hmp.utils.transform_data(eeg_data.data, apply_standard=False, n_comp=4)
+hmp_data = hmp.utils.transform_data(eeg_data, apply_standard=False, n_comp=4)
 ```
 
-# Estimating an HsMM model
+Once the data is in the expected format, we can initialize an HMP
+
+
+```python
+init = hmp.models.hmp(hmp_data, eeg_data, event_width=50, cpus=cpus)#Initialization of the model
+```
+
+# HMP model
+
+We are looking for stages in the data (**Hidden Markov**) and assume that transitions between stages are signaled by a template in the data (**pattern analysis**). By default we use the same template as Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet'.apa.org/doi/10.1037/rev0000030)), a 10 Hz half-sine, resulting in a 50ms duration bump-like shape:
 
-We can directly fit an HsMM model without giving any info on the number of bumps (see tutorial 2 for the explanation of the following cell)
 
 
 ```python
-%%time
-init = hmp.models.hsmm(hsmm_dat, eeg_data, bump_width=50, cpus=cpus)#Initialization of the model
-estimates = init.fit(step=10, verbose=False)
+plt.plot(init.template,'x');
 ```
 
 
-      0%|          | 0/360 [00:00<?, ?it/s]
+    
+![png](README_files/README_18_0.png)
+    
+
+
+This pattern is assumed to be present in multiple electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
+
+
+
+```python
+epoch = 0 #illustrating the first trial
+hmp_data.unstack().sel(component=[0,1,2], epochs=epoch).squeeze().plot.line(hue='component');
+plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k')#overlaying the simulated stage transition times
+```
+
+
+    
+![png](README_files/README_20_1.png)
+    
+
 
 
-    CPU times: user 645 ms, sys: 1.6 ms, total: 647 ms
-    Wall time: 646 ms
+The by-trial onset of this transition event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
+
+
+```python
+T = 350
+plt.plot(np.linspace(0,T,1001),gamma.pdf(np.linspace(0,T,1001), 2, scale=50)) 
+plt.xlabel('t');
+```
+
+
+    
+![png](README_files/README_22_0.png)
+    
+
+
+And this is then the full explanation of an HMP model: Looking for a transition event across several electrodes and trials that signals a transition to the next stage and which onset is expected to follow a probability distribution (in this case a gamma).
+
+# Estimating an HMP model
+
+We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for the explanation of the following cell)
+
+
+
+```python
+estimates = init.fit(step=20, verbose=True)
+```
+
+
+    Transition event 2 found around sample 137
+    Transition event 3 found around sample 258
+    Transition event 4 found around sample 330
+    Estimating 4 events model
+    Parameters estimated for 4 events model
 
 
 ### Visualizing results of the fit
 
-In the previous cell we initiated an HsMM model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 bumps and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit
+In the previous cell we initiated an HMP model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 Transition events and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit.
+
+We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
+
 
-We can directly take a look to the topologies and latencies of the bumps by calling ```hmp.visu.plot_topo_timecourse```
+We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
 
 
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
                                positions, init,#position of the electrodes and initialized model
                                magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
                                times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
 
     
-![png](README_files/README_21_0.png)
+![png](README_files/README_27_0.png)
     
 
 
-This shows us the electrode activity on the scalp as well as the average time of occurence of the bump based on the stage distributions.
+This shows us the electrode activity on the scalp as well as the average time of occurence of the events based on the stage distributions.
 
-As we are estimating the bump onsets on a by-trial basis we can look at the by-trial variation in stage duration.
+As we are estimating the event onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
 
 ```python
-bump_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('bump')#computing predicted bump times
-ax = hmp.visu.plot_latencies_average(bump_times_estimates, init.bump_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
+event_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('event')#computing predicted event times
+ax = hmp.visu.plot_latencies_average(event_times_estimates, init.event_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
-![png](README_files/README_23_0.png)
+![png](README_files/README_29_0.png)
     
 
 
-For the same reason we can also inspect the probability distribution of bump onsets:
+For the same reason we can also inspect the probability distribution of event onsets:
+
 
 
 ```python
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)), survival=True)
 ```
 
@@ -285,118 +341,119 @@
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_25_1.png)
+![png](README_files/README_31_1.png)
     
 
 
 
     
-![png](README_files/README_25_2.png)
+![png](README_files/README_31_2.png)
     
 
 
-As HsMM-MVPA selected those bumps onset per trial we can also look at the predicted bump onsets for a single trial
+As HMP estimated stage onset per trial we can also look at the predicted stage onsets for a given trial.
 
 
 ```python
-hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 1)), 
+hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 0)), 
                             xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 ```
 
 
 
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_27_1.png)
+![png](README_files/README_33_1.png)
     
 
 
-This then shows the likeliest bump location in time for the first trial!
+This then shows the likeliest stage onset location in time for the first trial!
 
 ## Comparing with ground truth
 
-As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HsMM-MVpy. As in the beginning, this code is specific to the case where you simulate data.
+As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP-MVpy. As in the beginning, this code is specific to the case where you simulate data.
 
 
 ```python
 colors = sns.color_palette(None, number_of_sources)
-# plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(params=1)*2+np.concatenate([[0],np.repeat(init.bump_width_samples,number_of_sources-1)]), color=colors,s=50)
-plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(parameter=1)*2, color=colors,s=50)
+plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.prod(axis=1), color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
 plt.title('Actual vs estimated stage durations')
 plt.xlabel('Simulated stage duration')
 plt.ylabel('Estimated stage duration')
 plt.show()
 
 ```
 
 
     
-![png](README_files/README_30_0.png)
+![png](README_files/README_35_0.png)
     
 
 
 Or also overlay actual bumps onset with predicted one
 
 
+
 ```python
-hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated bump onsets',
+hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated event onsets',
         times_to_display = np.mean(np.cumsum(random_source_times,axis=1),axis=0))
 ```
 
 
     
-![png](README_files/README_32_0.png)
+![png](README_files/README_37_0.png)
     
 
 
-We see that the HsMM-MVpy package recovers the exact average location of the bumps defined in the simulated data
+We see that the HSMM-MVpy package recovers the exact average location of the bumps defined in the simulated data.
 
-We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HsMM model
+We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HMP model
 
 
 ```python
 fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
 i = 0
 
-for bump in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
-    sns.regplot(x=random_source_times[:,i].T, y=bump, ax=ax[i], color=colors[i])
-    ax[i].plot([np.min(bump), np.max(bump)], [np.min(bump), np.max(bump)],'--', color='k')
+for event in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
+    sns.regplot(x=random_source_times[:,i].T, y=event, ax=ax[i], color=colors[i])
+    ax[i].plot([np.min(event), np.max(event)], [np.min(event), np.max(event)],'--', color='k')
     ax[i].set_ylabel(f'Estimated by-trial stage duration for stage {i+1}')
     ax[i].set_xlabel(f'Simulated by-trial stage duration for stage {i+1}')
     i+= 1
 ```
 
 
     
-![png](README_files/README_35_0.png)
+![png](README_files/README_39_0.png)
     
 
 
 We see that every stage gets nicely recovered even on a by-trial basis!
 
 # Beyond summary statistics for EEG analysis
 
-Now the purpose, apart from determining the number and timecourse of important EEG events in the Rreaction time, is also to use the by-trial information.
+Now the purpose, apart from determining the number and time course of important EEG events in the reaction time, is also to use the by-trial information.
 
 We illustrate this by first plotting the traditional event-related potentials (i.e. taking the average of given electrodes across the different time points) with cherry-picked electrodes.
 
 
+
 ```python
 import seaborn as sns
 import pandas as pd
 
 data = eeg_data.stack({'trial_x_participant':['participant','epochs']}).data.dropna('trial_x_participant', how="all")
 fig, ax = plt.subplots(1,1, figsize=(20,5), sharey=True)
 
@@ -410,25 +467,25 @@
 plt.xlim(0,500)
 plt.ylim(-3e-6,3e-6);
 
 ```
 
 
     
-![png](README_files/README_38_0.png)
+![png](README_files/README_41_0.png)
     
 
 
-Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to trqditional ERPs with very clear signal in the beginning of a trial (as events are more in sync) and summed and blurried in later stages of the reaction times (as event are off sync).
+Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to traditional ERPs with very clear signal in the beginning of a trial (as events are more in phase) and summed and blurried in later stages of the reaction times (as event are off phase).
 
-Now things can get better if we first parse, by-trial, the signal into the different stages based on the HsMM estimates:
+Now things can get better if we first parse, by-trial, the signal into the different stages based on the HMP estimates:
 
 
 ```python
-BRP_times = init.compute_times(init, estimates.dropna('bump'), fill_value=0, add_rt=True)
+BRP_times = init.compute_times(init, estimates.dropna('event'), fill_value=0, add_rt=True)
 
 fig, ax = plt.subplots(1,number_of_sources, figsize=(20,5), sharey=True, sharex=True)
 ax[0].set_ylabel('Volt')
 for stage in range(number_of_sources):
     BRP = hmp.utils.event_times(data, BRP_times,'EEG 016',stage=stage)
     df = pd.DataFrame(BRP).melt(var_name='Time')
     sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkgreen')
@@ -439,21 +496,23 @@
     df = pd.DataFrame(BRP).melt(var_name='Time')
     sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkblue') 
     plt.xlim(0,100)
 ```
 
 
     
-![png](README_files/README_40_0.png)
+![png](README_files/README_43_0.png)
     
 
 
+
 In this case we clearly see at each stage the half-sin (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sin). Note that the end of the stages tend to be noisier because less trial are defining the average signal (also why the confidence interval grows).
 
 
 ### Follow-up
 
-For examples on how to use the package when the number of bumps are unkown, or to compare stage durations across conditions see the tutorial notebooks:
+For examples on how to use the package when the number of transition events/stages is unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
-- Estimating a given number of bumps (tutorial 2)
-- Test for the number of bumps that best explains the data (tutorial 3)
+- Estimating a given number of events (tutorial 2)
+- Test for the number of events that best explains the data (tutorial 3)
 - Testing differences across conditions (tutorial 4)
+
```

### Comparing `hsmm_mvpy-0.1.0a2/pyproject.toml` & `hsmm_mvpy-0.1.0b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.1.0-alpha2"
+version = "0.1.0-beta"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
@@ -19,16 +19,16 @@
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies=["mne >=1.0.0",
 "numpy",
 "xarray",
 "scikit-learn",
+"statsmodels",
 "seaborn",
 "scipy",
 "netcdf4",
-"xskillscore",
-"more_itertools"]
+"xskillscore"]
 
 [project.urls]
 "Homepage" = "https://github.com/GWeindel/hmp"
 "Bug Tracker" = "https://github.com/GWeindel/hmp/issues"
```

### Comparing `hsmm_mvpy-0.1.0a2/src/hsmm_mvpy/models.py` & `hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,51 +4,63 @@
 
 import numpy as np
 import xarray as xr
 import multiprocessing as mp
 import itertools
 import math
 import time#Just for speed testing
-from warnings import warn
+from warnings import warn, filterwarnings, resetwarnings
 from scipy.stats import gamma as sp_gamma
 import matplotlib.pyplot as plt
 from tqdm.auto import tqdm
 default_colors =  ['cornflowerblue','indianred','orange','darkblue','darkgreen','gold', 'brown']
 
 
-class hsmm:
+class hmp:
     
-    def __init__(self, data, eeg_data=None, sfreq=None, offset=0, cpus=1, bump_width=50, shape=2, estimate_magnitudes=True, estimate_parameters=True, template=None, min_duration=None):
+    def __init__(self, data, eeg_data=None, sfreq=None, offset=0, cpus=1, event_width=50, shape=2, estimate_magnitudes=True, estimate_parameters=True, template=None, location=None, distribution='gamma'):
         '''
-        HSMM calculates the probability of data summing over all ways of 
-        placing the n bumps to break the trial into n + 1 flats.
+        HMP calculates the probability of data summing over all ways of 
+        placing the n events to break the trial into n + 1 stages.
 
         Parameters
         ----------
         data : ndarray
             2D ndarray with n_samples * components 
         sfreq : int
             Sampling frequency of the signal (initially 100)
-        bump_width : int
-            width of bumps in milliseconds, originally 5 samples
-        min_duration : float
+        event_width : int
+            width of events in milliseconds, originally 5 samples
+        location : float
             Minimum stage duration in milliseconds. 
         '''
+        if distribution == 'gamma':
+            from scipy.stats import gamma as sp_dist
+        elif distribution == 'lognormal':
+            from scipy.stats import lognorm as sp_dist
+        elif distribution == 'wald':
+            from scipy.stats import invgauss as sp_dist
+        elif distribution == 'weibull':
+            from scipy.stats import weibull_min as sp_dist
+        else:
+            raise ValueError(f'Unknown Distribution {distribution}')
+        self.cdf = sp_dist.cdf
+            
         if sfreq is None:
             sfreq = eeg_data.sfreq
         if offset is None:
             offset = eeg_data.offset
         self.sfreq = sfreq
         self.steps = 1000/self.sfreq
         self.shape = float(shape)
-        self.bump_width = bump_width
-        self.bump_width_samples = int(np.round(self.bump_width / self.steps))
-        if min_duration is None:
-            self.min_duration = int(self.bump_width_samples/2)
-        else: self.min_duration =  int(np.round(min_duration / self.steps))
+        self.event_width = event_width
+        self.event_width_samples = int(np.round(self.event_width / self.steps))
+        if location is None:
+            self.location = int(np.round(self.event_width_samples/2))
+        else: self.location =  int(np.round(location / self.steps))
         durations = data.unstack().sel(component=0).swap_dims({'epochs':'trials'})\
             .stack(trial_x_participant=['participant','trials']).dropna(dim="trial_x_participant",\
             how="all").groupby('trial_x_participant').count(dim="samples").cumsum().squeeze()
         if durations.trial_x_participant.count() > 1:
             dur_dropped_na = durations.dropna("trial_x_participant")
             starts = np.roll(dur_dropped_na.data, 1)
             starts[0] = 0
@@ -56,330 +68,345 @@
         else: 
             dur_dropped_na = durations
             starts = np.array([0])
             ends = np.array([dur_dropped_na.data-1 -offset])
         self.starts = starts
         self.ends = ends
         self.durations =  self.ends-self.starts+1
+        self.max_events = self.compute_max_events()
         if durations.trial_x_participant.count() > 1:
             self.named_durations =  durations.dropna("trial_x_participant") - durations.dropna("trial_x_participant").shift(trial_x_participant=1, fill_value=0)
             self.coords = durations.reset_index('trial_x_participant').coords
         else: 
             self.named_durations = durations
             self.coords = durations.coords
         self.mean_d = self.durations.mean()
         self.n_trials = durations.trial_x_participant.count().values
             
         self.cpus = cpus
         self.n_samples, self.n_dims = np.shape(data.data.T)
         if template is None:
-            self.template = self.bump_shape()
+            self.template = self.event_shape()
         else: self.template = template
-        self.bumps = self.cross_correlation(data.data.T)#adds bump morphology
+        self.events = self.cross_correlation(data.data.T)#adds event morphology
         self.max_d = self.durations.max()
         self.estimate_magnitudes = estimate_magnitudes
         self.estimate_parameters = estimate_parameters
         if self.max_d > 500:#FFT conv from scipy faster in this case
             from scipy.signal import fftconvolve
             self.convolution = fftconvolve
         else:
             self.convolution = np.convolve
     
-    def bump_shape(self):
+    def event_shape(self):
         '''
-        Computes the template of a half-sine (bump) with given frequency f and sampling frequency
+        Computes the template of a half-sine (event) with given frequency f and sampling frequency
         '''
-        bump_idx = np.arange(self.bump_width_samples)*self.steps+self.steps/2
-        bump_frequency = 1000/(self.bump_width*2)#gives bump frequency given that bumps are defined as half-sines
-        template = np.sin(2*np.pi*bump_idx/1000*bump_frequency)#bump morph based on a half sine with given bump width and sampling frequency
+        event_idx = np.arange(self.event_width_samples)*self.steps+self.steps/2
+        event_frequency = 1000/(self.event_width*2)#gives event frequency given that events are defined as half-sines
+        template = np.sin(2*np.pi*event_idx/1000*event_frequency)#event morph based on a half sine with given event width and sampling frequency
         template = template/np.sum(template**2)#Weight normalized
         return template
             
     def cross_correlation(self,data):
         '''
         This function puts on each sample the correlation of that sample and the next 
-        x samples (depends on sampling frequency and bump size) with a half sine on time domain.
+        x samples (depends on sampling frequency and event size) with a half sine on time domain.
         
         Parameters
         ----------
         data : ndarray
             2D ndarray with n_samples * components
         Returns
         -------
         bumbs : ndarray
             a 2D ndarray with samples * PC components where cell values have
-            been correlated with bump morphology
+            been correlated with event morphology
         '''
         from scipy.signal import fftconvolve
-        bumps = np.zeros(data.shape)
+        events = np.zeros(data.shape)
         for trial in range(self.n_trials):#avoids confusion of gains between trials
             for dim in np.arange(self.n_dims):
-                bumps[self.starts[trial]:self.ends[trial]+1,dim] = \
+                events[self.starts[trial]:self.ends[trial]+1,dim] = \
                     fftconvolve(data[self.starts[trial]:self.ends[trial]+1, dim], \
                         self.template, mode='full')\
                         [len(self.template)-1:self.durations[trial]+len(self.template)+1]
-        return bumps
+        return events
 
-    def fit_single(self, n_bumps=None, magnitudes=None, parameters=None, threshold=1, verbose=True,
-            starting_points=1, parameters_to_fix=None, magnitudes_to_fix=None, method='random', multiple_n_bumps=None):
+    def fit_single(self, n_events=None, magnitudes=None, parameters=None, threshold=1, verbose=True,
+            starting_points=1, parameters_to_fix=None, magnitudes_to_fix=None, method='random', multiple_n_events=None):
         '''
-        Fit HsMM for a single n_bumps model
+        Fit HMP for a single n_events model
+        
         Parameters
         ----------
-        n_bumps : int
-            how many bumps are estimated
+        n_events : int
+            how many events are estimated
         magnitudes : ndarray
-            2D ndarray n_bumps * components, initial conditions for bumps magnitudes
+            2D ndarray n_events * components, initial conditions for events magnitudes
         parameters : list
             list of initial conditions for Gamma distribution scale parameter. If parameters are estimated, the list provided is used as starting point,
             if parameters are fixed, parameters estimated will be the same as the one provided. When providing a list, stage need to be in the same order
             _n_th gamma parameter is  used for the _n_th stage
         threshold : float
-            threshold for the HsMM algorithm, 0 skips HsMM
+            threshold for the HMP algorithm, 0 skips HMP
         '''
         import pandas as pd 
+        if n_events is None:
+            raise ValueError('The fit_single() function needs to be provided with a number of expected transition events. Look at function fit() if you want to fit a model without assuming a particular number of events.')
         if verbose:
             if parameters is None:
-                print(f'Estimating {n_bumps} bumps model with {starting_points} starting point(s)')
+                print(f'Estimating {n_events} events model with {starting_points} starting point(s)')
             else:
-                print(f'Estimating {n_bumps} bumps model')
-        if n_bumps is None and parameters is not None:
-            n_bumps = len(parameters)-1
+                print(f'Estimating {n_events} events model')
+        if n_events is None and parameters is not None:
+            n_events = len(parameters)-1
         if self.estimate_magnitudes == False:#Don't need to manually fix mags if not estimated
-            magnitudes_to_fix = np.arange(n_bumps)
+            magnitudes_to_fix = np.arange(n_events)
         if self.estimate_parameters == False:#Don't need to manually fix pars if not estimated
-            parameters_to_fix = np.arange(n_bumps+1)            
+            parameters_to_fix = np.arange(n_events+1)            
         #Formatting parameters
         if isinstance(parameters, (xr.DataArray,xr.Dataset)):
             parameters = parameters.dropna(dim='stage').values
         if isinstance(magnitudes, (xr.DataArray,xr.Dataset)):
-            magnitudes = magnitudes.dropna(dim='bump').values  
+            magnitudes = magnitudes.dropna(dim='event').values  
         if isinstance(magnitudes, np.ndarray):
             magnitudes = magnitudes.copy()
         if isinstance(parameters, np.ndarray):
             parameters = parameters.copy()          
         if parameters_to_fix is None: parameters_to_fix=[]
         if magnitudes_to_fix is None: magnitudes_to_fix=[]
         if starting_points > 0:#Initialize with equally spaced option
             if parameters is None:
-                parameters = np.tile([self.shape, (np.mean(self.durations))/(n_bumps+1)/self.shape], (n_bumps+1,1))
+                parameters = np.tile([self.shape, ((np.mean(self.durations))/(n_events+1)-self.location)/self.shape], (n_events+1,1))
             initial_p = parameters
             
             if magnitudes is None:
-                magnitudes = np.zeros((n_bumps,self.n_dims), dtype=np.float64)
+                magnitudes = np.zeros((n_events,self.n_dims), dtype=np.float64)
             initial_m = magnitudes
         
         if starting_points > 1:
+            filterwarnings("ignore", category=RuntimeWarning)#Error in the generation of random see GH issue #38
             parameters = [initial_p]
             magnitudes = [initial_m]
             if method == 'random':
                 for sp in np.arange(starting_points):
-                    proposal_p = self.gen_random_stages(n_bumps, np.mean(self.durations))
-                    proposal_m = np.zeros((n_bumps,self.n_dims), dtype=np.float64)#Mags are NOT random but always 0
+                    proposal_p = self.gen_random_stages(n_events, self.mean_d)
+                    proposal_m = np.zeros((n_events,self.n_dims), dtype=np.float64)#Mags are NOT random but always 0
                     proposal_p[parameters_to_fix] = initial_p[parameters_to_fix]
                     proposal_m[magnitudes_to_fix] = initial_m[magnitudes_to_fix]
                     parameters.append(proposal_p)
                     magnitudes.append(proposal_m)
             elif method == 'grid':
-                parameters = self.grid_search(n_bumps+1, iter_limit=starting_points, method='grid')
-                magnitudes = np.zeros((len(parameters), n_bumps, self.n_dims), dtype=np.float64)
+                parameters = self._grid_search(n_events+1, iter_limit=starting_points, method='grid')
+                magnitudes = np.zeros((len(parameters), n_events, self.n_dims), dtype=np.float64)
             else:
                 raise ValueError('Unknown starting point method requested, use "random" or "grid"')
             with mp.Pool(processes=self.cpus) as pool:
                 estimates = pool.starmap(self.EM, 
-                    zip(itertools.repeat(n_bumps), magnitudes, parameters, itertools.repeat(1),\
+                    zip(itertools.repeat(n_events), magnitudes, parameters, itertools.repeat(1),\
                     itertools.repeat(magnitudes_to_fix),itertools.repeat(parameters_to_fix),))   
             lkhs_sp = [x[0] for x in estimates]
             mags_sp = [x[1] for x in estimates]
             pars_sp = [x[2] for x in estimates]
             eventprobs_sp = [x[3] for x in estimates]
             max_lkhs = np.where(lkhs_sp == np.max(lkhs_sp))[0][0]
             lkh = lkhs_sp[max_lkhs]
             mags = mags_sp[max_lkhs]
             pars = pars_sp[max_lkhs]
             eventprobs = eventprobs_sp[max_lkhs]
+            resetwarnings()
             
         elif starting_points==1:#informed starting point
-            lkh, mags, pars, eventprobs = self.EM(n_bumps, initial_m, initial_p,\
+            lkh, mags, pars, eventprobs = self.EM(n_events, initial_m, initial_p,\
                                         threshold, magnitudes_to_fix, parameters_to_fix)
 
         else:#uninitialized    
             if np.any(parameters)== None:
-                parameters = np.tile([self.shape, (self.mean_d)/self.shape], (n_bumps+1,1))
+                parameters = np.tile([self.shape, (self.mean_d)/self.shape], (n_events+1,1))
             if np.any(magnitudes)== None:
-                magnitudes = np.zeros((n_bumps, self.n_dims), dtype=np.float64)
-            lkh, mags, pars, eventprobs = self.EM(n_bumps, magnitudes, parameters,\
+                magnitudes = np.zeros((n_events, self.n_dims), dtype=np.float64)
+            lkh, mags, pars, eventprobs = self.EM(n_events, magnitudes, parameters,\
                                         threshold, magnitudes_to_fix, parameters_to_fix)
-        if multiple_n_bumps is not None and len(pars) != multiple_n_bumps+1:#align all dimensions
-            pars = np.concatenate((pars, np.tile(np.nan, (multiple_n_bumps+1-len(pars),2))))
+        if multiple_n_events is not None and len(pars) != multiple_n_events+1:#align all dimensions
+            pars = np.concatenate((pars, np.tile(np.nan, (multiple_n_events+1-len(pars),2))))
             mags = np.concatenate((mags, np.tile(np.nan, 
-                (multiple_n_bumps-len(mags), np.shape(mags)[1]))),axis=0)
+                (multiple_n_events-len(mags), np.shape(mags)[1]))),axis=0)
             eventprobs = np.concatenate((eventprobs, np.tile(np.nan, (np.shape(eventprobs)[0],\
-                    np.shape(eventprobs)[1], multiple_n_bumps-np.shape(eventprobs)[2]))),axis=2)
-            n_bumps = multiple_n_bumps
+                    np.shape(eventprobs)[1], multiple_n_events-np.shape(eventprobs)[2]))),axis=2)
+            n_events = multiple_n_events
             # print(np.shape(eventprobs))
         
         xrlikelihoods = xr.DataArray(lkh , name="likelihoods")
         xrparams = xr.DataArray(pars, dims=("stage",'parameter'), name="parameters")
-        xrmags = xr.DataArray(mags, dims=("bump","component"), name="magnitudes")
+        xrmags = xr.DataArray(mags, dims=("event","component"), name="magnitudes")
         part, trial = self.coords['participant'].values, self.coords['trials'].values
-        if n_bumps>0:
+        if n_events>0:
             n_samples, n_participant_x_trials,_ = np.shape(eventprobs)
         else:
             n_samples, n_participant_x_trials = np.shape(eventprobs)
-        if n_participant_x_trials >1 and n_bumps >0:
-            xreventprobs = xr.Dataset({'eventprobs': (('bump', 'trial_x_participant','samples'), 
+        if n_participant_x_trials >1 and n_events >0:
+            xreventprobs = xr.Dataset({'eventprobs': (('event', 'trial_x_participant','samples'), 
                                          eventprobs.T)},
-                         {'bump':np.arange(n_bumps),
+                         {'event':np.arange(n_events),
                           'samples':np.arange(n_samples),
                         'trial_x_participant':  pd.MultiIndex.from_arrays([part,trial],
                                 names=('participant','trials'))})
-            xreventprobs = xreventprobs.transpose('trial_x_participant','samples','bump')
-        elif n_bumps == 0:
+            xreventprobs = xreventprobs.transpose('trial_x_participant','samples','event')
+        elif n_events == 0:
             xreventprobs = xr.Dataset({'eventprobs': (('trial_x_participant','samples'), 
                                          eventprobs.T)},
                          {'samples':np.arange(n_samples),
                         'trial_x_participant':  pd.MultiIndex.from_arrays([part,trial],
                                 names=('participant','trials'))})
             xreventprobs = xreventprobs.transpose('trial_x_participant','samples')
 
         elif n_participant_x_trials == 1: 
-            xreventprobs = xr.Dataset({'eventprobs': (('bump', 'trial_x_participant','samples'), 
+            xreventprobs = xr.Dataset({'eventprobs': (('event', 'trial_x_participant','samples'), 
                                          eventprobs.T)},
-                         {'bump':np.arange(n_bumps),
+                         {'event':np.arange(n_events),
                           'samples':np.arange(n_samples)})
-            xreventprobs = xreventprobs.transpose('trial_x_participant','samples','bump')
+            xreventprobs = xreventprobs.transpose('trial_x_participant','samples','event')
         estimated = xr.merge((xrlikelihoods, xrparams, xrmags, xreventprobs))
 
         if verbose:
-            print(f"Parameters estimated for {n_bumps} bumps model")
+            print(f"Parameters estimated for {n_events} events model")
         return estimated
     
-    def EM(self, n_bumps, magnitudes, parameters,  threshold, magnitudes_to_fix=None, parameters_to_fix=None, max_iteration = 1e3):
+    def EM(self, n_events, magnitudes, parameters,  threshold, magnitudes_to_fix=None, parameters_to_fix=None, max_iteration = 1e3):
         '''
         Expectation maximization function underlying fit
         ''' 
-        null_stages = np.where(parameters[:,1]*self.shape<(self.min_duration/self.shape))[0]
+        null_stages = np.where(parameters[:,1]<0)[0]
         wrong_shape = np.where(parameters[:,0]!=self.shape)[0]
         if len(null_stages)>0:
-            raise ValueError(f'Wrong scale parameter input, provided scale parameter(s) {null_stages} should be higher than minimum duration of {self.min_duration} but have value {parameters[null_stages,:].prod(axis=1)}')
+            raise ValueError(f'Wrong scale parameter input, provided scale parameter(s) {null_stages} should be positive but have value {parameters[null_stages,:].prod(axis=1)}')
         if len(wrong_shape)>0:
             raise ValueError(f'Wrong shape parameter input, provided parameter(s) {wrong_shape} shape is {parameters[wrong_shape,0]} but expected  expected {self.shape}')
         initial_parameters =  np.copy(parameters)
         initial_magnitudes = np.copy(magnitudes)
         
-        lkh, eventprobs = self.estim_probs(magnitudes, parameters, n_bumps)
+        lkh, eventprobs = self.estim_probs(magnitudes, parameters, n_events)
         means = np.zeros((self.max_d, self.n_trials, self.n_dims), dtype=np.float64)
         for trial in range(self.n_trials):
-            means[:self.durations[trial],trial,:] = self.bumps[self.starts[trial]:self.ends[trial]+1,:]
+            means[:self.durations[trial],trial,:] = self.events[self.starts[trial]:self.ends[trial]+1,:]
             #Reorganize samples crosscorrelated with template on trial basis
-        if threshold == 0 or n_bumps==0:
+        if threshold == 0 or n_events==0:
             lkh_prev = lkh
             magnitudes_prev = initial_magnitudes
             parameters_prev = initial_parameters
             eventprobs_prev = eventprobs
         else:
-            lkh_prev = -np.inf
-            for bump in range(n_bumps):
+            for event in range(n_events):
                 for comp in range(self.n_dims):
-                    magnitudes[bump,comp] = np.mean(np.sum( \
-                        eventprobs[:,:,bump]*means[:,:,comp], axis=0))
-            parameters = self.gamma_parameters(eventprobs, n_bumps)
-            magnitudes_prev = magnitudes.copy()
-            parameters_prev = parameters.copy()
-            eventprobs_prev = eventprobs.copy()
+                    magnitudes[event,comp] = np.mean(np.sum( \
+                        eventprobs[:,:,event]*means[:,:,comp], axis=0))
+            parameters = self.scale_parameters(eventprobs, n_events)
+            null_stages = np.where(parameters[:,1]<0)[0]
+            if len(null_stages) == 0: 
+                lkh_prev = -np.inf
+                magnitudes_prev = magnitudes.copy()
+                parameters_prev = parameters.copy()
+                eventprobs_prev = eventprobs.copy()
+            else:#Corner case in simulations
+                lkh_prev = lkh
+                magnitudes_prev = initial_magnitudes
+                parameters_prev = initial_parameters
+                eventprobs_prev = eventprobs
         i = 0
         while lkh - lkh_prev > threshold and i < max_iteration:#Expectation-Maximization algorithm
             #As long as new run gives better likelihood, go on  
             lkh_prev = lkh.copy()
             magnitudes_prev = magnitudes.copy()
             parameters_prev = parameters.copy()
             eventprobs_prev = eventprobs.copy()
             #Magnitudes from Expectation
-            for bump in range(n_bumps):
+            for event in range(n_events):
                 for comp in range(self.n_dims):
-                    magnitudes[bump,comp] = np.mean(np.sum( \
-                        eventprobs[:,:,bump]*means[:,:,comp], axis=0))
+                    magnitudes[event,comp] = np.mean(np.sum( \
+                        eventprobs[:,:,event]*means[:,:,comp], axis=0))
                     # Scale cross-correlation with likelihood of the transition
                     # sum by-trial these scaled activation for each transition events
                     # average across trials
 
             magnitudes[magnitudes_to_fix,:] = initial_magnitudes[magnitudes_to_fix,:].copy()
             #Parameters from Expectation
-            parameters = self.gamma_parameters(eventprobs, n_bumps)
+            parameters = self.scale_parameters(eventprobs, n_events)
             parameters[parameters_to_fix, :] = initial_parameters[parameters_to_fix,:].copy()
-            lkh, eventprobs = self.estim_probs(magnitudes, parameters, n_bumps)
+            lkh, eventprobs = self.estim_probs(magnitudes, parameters, n_events)
             i += 1
+        null_probs = np.where(eventprobs_prev<-1e-10)[0]
+        if len(null_probs)>0:
+            warn('Negative probabilities found after estimation, this likely refers to several events overlapping events. In case of simulated data ensure that events are enoughly separated (i.e. location parameter). In the case of real data this error is not expected, please report to the maintainers')
         if i == max_iteration:
             warn(f'Convergence failed, estimation hitted the maximum number of iteration ({int(max_iteration)})', RuntimeWarning)
         return lkh_prev, magnitudes_prev, parameters_prev, eventprobs_prev
 
-    def estim_probs(self, magnitudes, parameters, n_bumps, lkh_only=False):
+    def estim_probs(self, magnitudes, parameters, n_events, lkh_only=False):
         '''
         
         Returns
         -------
         likelihood : float
             Summed log probabilities
         eventprobs : ndarray
-            Probabilities with shape max_samples*n_trials*n_bumps
+            Probabilities with shape max_samples*n_trials*n_events
         '''
-        n_stages = n_bumps+1
-        gains = np.zeros((self.n_samples, n_bumps), dtype=np.float64)
+        n_stages = n_events+1
+        gains = np.zeros((self.n_samples, n_events), dtype=np.float64)
         for i in range(self.n_dims):
             # computes the gains, i.e. how much the congruence between the pattern shape
             # and the data given the magnitudes of the sensors
-            gains = gains + self.bumps[:,i][np.newaxis].T * magnitudes[:,i]
+            gains = gains + self.events[:,i][np.newaxis].T * magnitudes[:,i]
         gains = np.exp(gains)
-        probs = np.zeros([self.max_d,self.n_trials,n_bumps], dtype=np.float64) # prob per trial
-        probs_b = np.zeros([self.max_d,self.n_trials,n_bumps], dtype=np.float64)# Sample and state reversed
+        probs = np.zeros([self.max_d,self.n_trials,n_events], dtype=np.float64) # prob per trial
+        probs_b = np.zeros([self.max_d,self.n_trials,n_events], dtype=np.float64)# Sample and state reversed
         for trial in np.arange(self.n_trials):
             # Following assigns gain per trial to variable probs 
             probs[:self.durations[trial],trial,:] = \
                 gains[self.starts[trial]:self.ends[trial]+1,:] 
-            # Same but samples and bumps are reversed, this allows to compute
+            # Same but samples and events are reversed, this allows to compute
             # fwd and bwd in the same way in the following steps
             probs_b[:self.durations[trial],trial,:] = \
                 gains[self.starts[trial]:self.ends[trial]+1,:][::-1,::-1]
 
         pmf = np.zeros([self.max_d, n_stages], dtype=np.float64) # Gamma pmf for each stage parameters
         for stage in range(n_stages):
-            if stage < n_stages-1:
-                location = self.min_duration
+            if n_stages-1 > stage > 0:
+                location = self.location
             else:
                 location = 0
-            pmf[:,stage] = self.gamma_EEG(parameters[stage,0], parameters[stage,1], location)
+            pmf[:,stage] = self.distribution_pmf(parameters[stage,0], parameters[stage,1], location)
         pmf_b = pmf[:,::-1] # Stage reversed gamma pmf, same order as prob_b
 
-        if n_bumps > 0:
-            forward = np.zeros((self.max_d, self.n_trials, n_bumps), dtype=np.float64)
-            backward = np.zeros((self.max_d, self.n_trials, n_bumps), dtype=np.float64)
+        if n_events > 0:
+            forward = np.zeros((self.max_d, self.n_trials, n_events), dtype=np.float64)
+            backward = np.zeros((self.max_d, self.n_trials, n_events), dtype=np.float64)
             # Computing forward and backward helper variable
             #  when stage = 0:
             forward[:,:,0] = np.tile(pmf[:,0][np.newaxis].T,\
                 (1,self.n_trials))*probs[:,:,0] #first stage transition is p(B) * p(d)
             backward[:,:,0] = np.tile(pmf_b[:,0][np.newaxis].T,\
-                        (1,self.n_trials)) #Reversed gamma (i.e. last stage) without probs as last bump ends at time T
+                        (1,self.n_trials)) #Reversed gamma (i.e. last stage) without probs as last event ends at time T
 
-            for bump in np.arange(1,n_bumps):#Following stage transitions integrate previous transitions
-                add_b = backward[:,:,bump-1]*probs_b[:,:,bump-1]#Next stage in back
+            for event in np.arange(1,n_events):#Following stage transitions integrate previous transitions
+                add_b = backward[:,:,event-1]*probs_b[:,:,event-1]#Next stage in back
                 for trial in np.arange(self.n_trials):
-                    # convolution between gamma * gains at previous bump and bump
-                    forward[:,trial,bump] = self.convolution(forward[:,trial,bump-1], pmf[:,bump])[:self.max_d]
+                    # convolution between gamma * gains at previous event and event
+                    forward[:,trial,event] = self.convolution(forward[:,trial,event-1], pmf[:,event])[:self.max_d]
                     # same but backwards
-                    backward[:,trial,bump] = self.convolution(add_b[:,trial], pmf_b[:, bump])[:self.max_d]
-                forward[:,:,bump] = forward[:,:,bump]*probs[:,:,bump]
-                # print(forward[:self.min_duration+10, 0, 0])
-                # print(backward[:self.min_duration+10, -1, -1])
+                    backward[:,trial,event] = self.convolution(add_b[:,trial], pmf_b[:, event])[:self.max_d]
+                forward[:,:,event] = forward[:,:,event]*probs[:,:,event]
             #re-arranging backward to the expected variable
             backward = backward[:,:,::-1]#undoes stage inversion
             for trial in np.arange(self.n_trials):#Undoes sample inversion
                 backward[:self.durations[trial],trial,:] = \
                     backward[:self.durations[trial],trial,:][::-1]
             eventprobs = forward * backward
+            eventprobs[eventprobs < 1e-10] = 0 #floating point precision error
             likelihood = np.sum(np.log(eventprobs[:,:,0].sum(axis=0)))#sum over max_samples to avoid 0s in log
             eventprobs = eventprobs / eventprobs.sum(axis=0)
             #conversion to probabilities, divide each trial and state by the sum of the likelihood of the n points in a trial
         else:
             forward = np.zeros((self.max_d, self.n_trials), dtype=np.float64)
             backward = np.zeros((self.max_d, self.n_trials), dtype=np.float64)
             forward[:,:] = np.tile(pmf[:,0][np.newaxis].T,\
@@ -388,353 +415,323 @@
                         (1,self.n_trials))
             for trial in np.arange(self.n_trials):#Undoes sample inversion
                 backward[:self.durations[trial],trial] = \
                     backward[:self.durations[trial],trial][::-1]
             eventprobs = forward * backward
             likelihood = np.sum(np.log(eventprobs[:,:].sum(axis=0)))#sum over max_samples to avoid 0s in log
             eventprobs = eventprobs / eventprobs.sum(axis=0)
+
         if lkh_only:
             return likelihood
         else:
             return [likelihood, eventprobs]
 
-    def gamma_EEG(self, a, scale, location):
+    def distribution_pmf(self, shape, scale, location):
         '''
-        Returns PMF of gamma dist with shape = a and scale, on a range from 0 to max_length 
+        Returns PMF of gamma or lognormal dist with shape and scale, on a range from 0 to max_length 
         
         Parameters
         ----------
         a : float
             shape parameter
         scale : float
             scale parameter      
         Returns
         -------
         p : ndarray
-            probabilties for a gamma with given parameters, normalized to 1
+            probabilty mass function for a gamma with given parameters
         '''
-        # print(location)
-        p = sp_gamma.cdf(np.arange(self.max_d), a, scale=scale, loc=location)
-        # print(p[:self.min_duration+1])
+        if scale == 0:
+            warn('Convergence failed: one stage has been found to be null')
+        p = self.cdf(np.arange(self.max_d), shape, scale=scale, loc=location)
+        #Location is in fact +1 as np.arange starts from 0
         p = np.diff(p, prepend=0)#going to pmf
-        # p = np.concatenate([np.zeros(location),np.diff(p,prepend=0)[location-2:]])
-        # p = 
-        # print(p[:self.min_duration+1])#going to pmf
         return p
     
-    def gamma_parameters(self, eventprobs, n_bumps):
+    def scale_parameters(self, eventprobs, n_events):
         '''
         Used for the re-estimation in the EM procdure. The likeliest location of 
-        the bump is computed from eventprobs. The flats are then taken as the 
-        distance between the bumps
+        the event is computed from eventprobs. The scale parameters are then taken as the average 
+        distance between the events corrected for (eventual) location
         Parameters
         ----------
         eventprobs : ndarray
-            [samples(max_d)*n_trials*n_bumps] = [max_d*trials*nTransition events]
+            [samples(max_d)*n_trials*n_events] = [max_d*trials*nTransition events]
         durations : ndarray
             1D array of trial length
         mags : ndarray
-            2D ndarray components * nTransition events, initial conditions for bumps magnitudes
+            2D ndarray components * nTransition events, initial conditions for events magnitudes
         shape : float
             shape parameter for the gamma, defaults to 2  
         Returns
         -------
         params : ndarray
             shape and scale for the gamma distributions
         '''
-        averagepos = np.arange(self.max_d)@eventprobs.mean(axis=1)
-        params = np.zeros((n_bumps+1,2), dtype=np.float64)
+        averagepos = np.concatenate([np.arange(1,self.max_d+1)@eventprobs.mean(axis=1),
+                                     [self.mean_d]])#Durations
+        params = np.zeros((n_events+1,2), dtype=np.float64)
         params[:,0] = self.shape
-        params[:-1,1] = np.diff(averagepos, prepend=0)
-        params[-1,1] = self.mean_d-averagepos[-1]
-        # params[:,1] += self.min_duration
+        params[:,1] = np.diff(averagepos, prepend=0)
+        # params[[0.-1],1] += self.location
+        params[0,1] -= .5#Event following starts half-sample before position
+        params[-1,1] += .5# Last event terminates half-sample earlier
         params[:,1] = params[:,1]/params[:,0]
         return params
     
-    def __multi_cpu_dispatch(self, list_n_bumps, list_mags, list_pars, threshold=1, verbose=False):
+    def __multi_cpu_dispatch(self, list_n_events, list_mags, list_pars, threshold=1, verbose=False):
         if self.cpus > 1:
-            if len(list_n_bumps) == 1:
-                list_n_bumps = itertools.repeat(list_n_bumps)
+            if len(list_n_events) == 1:
+                list_n_events = itertools.repeat(list_n_events)
             with mp.Pool(processes=self.cpus) as pool:
-                bump_loo_results = pool.starmap(self.fit_single, 
-                    zip(list_n_bumps, list_mags, list_pars,
+                event_loo_results = pool.starmap(self.fit_single, 
+                    zip(list_n_events, list_mags, list_pars,
                         itertools.repeat(threshold),itertools.repeat(verbose)))
         else:
-            bump_loo_results = []
-            for bump_tmp, flat_tmp in zip(list_mags, list_pars):
-                n_bump = len(bump_loo_results)+1
-                bump_loo_results.append(self.fit_single(n_bump, bump_tmp, flat_tmp, 0, False))
-        return bump_loo_results
-    
-    def iterative_fit(self, likelihoods, fitted=None, parameters=None, magnitudes=None):
-        if fitted is not None:
-            parameters = fitted.parameters.values
-            magnitudes = fitted.magnitudes.values
-        parameters = parameters.copy()
-        magnitudes = magnitudes.copy()
-        n_bumps_max = len(magnitudes)
-        magnitudes = magnitudes.copy()
-        n_bumps = len(likelihoods)
-        pars_n_bumps = []
-        mags_n_bumps = []
-        for n_bump in range(1, n_bumps+1):
-            temp_par = parameters.copy()
-            bump_idx = np.sort(np.argsort(likelihoods)[::-1][:n_bump])#sort the index of highest likelihood bumps
-            print(n_bump)
-            print(bump_idx)
-            bump_mags = magnitudes[bump_idx,:].copy()
-            print(bump_mags)
-
-            bump_pars = np.tile(self.shape, (n_bump+1,2))
-            bump_pars[:-1,1] = temp_par[bump_idx,1]
-            bump_pars[-1,1] = temp_par[-1,1]
-            bump_pars[:,1] = np.diff(bump_pars[:,1], prepend=0)
-            pars_n_bumps.append(bump_pars)
-            mags_n_bumps.append(bump_mags)
-        bump_loo_results = self.__multi_cpu_dispatch(np.arange(1,n_bumps+1), mags_n_bumps, 
-                             pars_n_bumps, 1, False)
-        bests = xr.concat(bump_loo_results, dim="n_bumps")
-        bests = bests.assign_coords({"n_bumps": np.arange(1,n_bumps+1)})
-        return bests
-    
+            event_loo_results = []
+            for event_tmp, flat_tmp in zip(list_mags, list_pars):
+                n_event = len(event_loo_results)+1
+                event_loo_results.append(self.fit_single(n_event, event_tmp, flat_tmp, 0, False))
+        return event_loo_results
+        
     def loo_loglikelihood(self, estimates):
-        bump_loo_results = [estimates.copy()]
-        n_bumps = bump_loo_results[0].dropna('bump').bump.max().values
-        list_values_n_bumps = [n_bumps]
-        print(bump_loo_results[0].parameters.values)  
+        event_loo_results = [estimates.copy()]
+        n_events = event_loo_results[0].dropna('event').event.max().values
+        list_values_n_events = [n_events]
+        print(event_loo_results[0].parameters.values)  
         i = 0
-        while n_bumps  > 0:
-            print(f'Estimating all solutions for {n_bumps} number of bumps')
-            temp_best = bump_loo_results[i]#previous bump solution
-            temp_best = temp_best.dropna('bump')
+        while n_events  > 0:
+            print(f'Estimating all solutions for {n_events} number of events')
+            temp_best = event_loo_results[i]#previous event solution
+            temp_best = temp_best.dropna('event')
             temp_best = temp_best.dropna('stage')
-            n_bumps_list = np.arange(n_bumps+1)#all bumps from previous solution
+            n_events_list = np.arange(n_events+1)#all events from previous solution
             flats = temp_best.parameters.values
             print(flats)
-            bumps_temp, flats_temp = [], []
-            for bump in np.arange(n_bumps+1):#creating all possible solutions
-                bumps_temp.append(temp_best.magnitudes.sel(bump = np.array(list(set(n_bumps_list) - set([bump])))).values)
-                flat = bump + 1 #one more flat than bumps
+            events_temp, flats_temp = [], []
+            for event in np.arange(n_events+1):#creating all possible solutions
+                events_temp.append(temp_best.magnitudes.sel(event = np.array(list(set(n_events_list) - set([event])))).values)
+                flat = event + 1 #one more flat than events
                 temp = flats[:,1].copy()
                 temp[flat-1] += temp[flat]
                 temp = np.delete(temp, flat)
                 flats_temp.append(np.reshape(np.concatenate([np.repeat(self.shape, len(temp)), temp]), (2, len(temp))).T)
 
-            bump_loo_likelihood_temp = self.__multi_cpu_dispatch(np.repeat(n_bumps,n_bumps+1), bumps_temp, 
+            event_loo_likelihood_temp = self.__multi_cpu_dispatch(np.repeat(n_events,n_events+1), events_temp, 
                      flats_temp, 0, False)
-            print([[x.likelihoods.values, x.parameters.values[:,1],'---------------------------------------\n'] for x in bump_loo_likelihood_temp])
+            print([[x.likelihoods.values, x.parameters.values[:,1],'---------------------------------------\n'] for x in event_loo_likelihood_temp])
             print('---------------------------------------\n')
-            models = xr.concat(bump_loo_likelihood_temp, dim="iteration")
-            bump_loo_results.append(models.sel(iteration=[np.where(models.likelihoods == models.likelihoods.max())[0][0]]).squeeze('iteration'))
-            n_bumps = bump_loo_results[-1].dropna('bump').bump.max().values
-            list_values_n_bumps.append(n_bumps)
+            models = xr.concat(event_loo_likelihood_temp, dim="iteration")
+            event_loo_results.append(models.sel(iteration=[np.where(models.likelihoods == models.likelihoods.max())[0][0]]).squeeze('iteration'))
+            n_events = event_loo_results[-1].dropna('event').event.max().values
+            list_values_n_events.append(n_events)
             i += 1
-        lkh = [x.likelihoods for x in bump_loo_results]
+        lkh = [x.likelihoods for x in event_loo_results]
         return lkh
 
 
-    def backward_estimation(self,max_bumps=None, min_bumps=0, max_fit=None, max_starting_points=1, method="random", threshold=1):
+    def backward_estimation(self,max_events=None, min_events=0, max_fit=None, max_starting_points=1, method="random", threshold=1):
         '''
-        First read or estimate max_bump solution then estimate max_bump - 1 solution by 
-        iteratively removing one of the bump and pick the one with the highest 
+        First read or estimate max_event solution then estimate max_event - 1 solution by 
+        iteratively removing one of the event and pick the one with the highest 
         likelihood
         
         Parameters
         ----------
         max_fit : xarray
-            To avoid re-estimating the model with maximum number of bumps it can be provided 
+            To avoid re-estimating the model with maximum number of events it can be provided 
             with this arguments, defaults to None
         max_starting_points: int
-            how many random starting points iteration to try for the model estimating the maximal number of bumps
+            how many random starting points iteration to try for the model estimating the maximal number of events
         
         '''
-        if max_bumps is None and max_fit is None:
-            max_bumps = self.compute_max_bumps()
+        if max_events is None and max_fit is None:
+            max_events = self.compute_max_events()
         if not max_fit:
             if max_starting_points >0:
-                print(f'Estimating all solutions for maximal number of bumps ({max_bumps}) with 1 pre-defined starting point and {max_starting_points-1} {method} starting points')
-            bump_loo_results = [self.fit_single(max_bumps, starting_points=max_starting_points, method=method, verbose=False)]
+                print(f'Estimating all solutions for maximal number of events ({max_events}) with 1 pre-defined starting point and {max_starting_points-1} {method} starting points')
+            event_loo_results = [self.fit_single(max_events, starting_points=max_starting_points, method=method, verbose=False)]
         else:
-            bump_loo_results = [max_fit]
-        max_bumps = bump_loo_results[0].bump.max().values+1
+            event_loo_results = [max_fit]
+        max_events = event_loo_results[0].event.max().values+1
         i = 0
-        for n_bumps in np.arange(max_bumps-1,min_bumps,-1):
-            print(f'Estimating all solutions for {n_bumps} number of bumps')
-            temp_best = bump_loo_results[i]#previous bump solution
-            temp_best = temp_best.dropna('bump')
+        for n_events in np.arange(max_events-1,min_events,-1):
+            print(f'Estimating all solutions for {n_events} number of events')
+            temp_best = event_loo_results[i]#previous event solution
+            temp_best = temp_best.dropna('event')
             temp_best = temp_best.dropna('stage')
-            n_bumps_list = np.arange(n_bumps+1)#all bumps from previous solution
+            n_events_list = np.arange(n_events+1)#all events from previous solution
             flats = temp_best.parameters.values
-            bumps_temp,flats_temp = [],[]
-            for bump in np.arange(n_bumps+1):#creating all possible solutions
-                bumps_temp.append(temp_best.magnitudes.sel(bump = np.array(list(set(n_bumps_list) - set([bump])))).values)
-                flat = bump + 1 #one more flat than bumps
+            events_temp,flats_temp = [],[]
+            for event in np.arange(n_events+1):#creating all possible solutions
+                events_temp.append(temp_best.magnitudes.sel(event = np.array(list(set(n_events_list) - set([event])))).values)
+                flat = event + 1 #one more flat than events
                 temp = np.copy(flats[:,1])
                 temp[flat-1] = temp[flat-1] + temp[flat]
                 temp = np.delete(temp, flat)
                 flats_temp.append(np.reshape(np.concatenate([np.repeat(self.shape, len(temp)), temp]), (2, len(temp))).T)
             if self.cpus > 1:
                 with mp.Pool(processes=self.cpus) as pool:
-                    bump_loo_likelihood_temp = pool.starmap(self.fit_single, 
-                        zip(itertools.repeat(n_bumps), bumps_temp, flats_temp,
+                    event_loo_likelihood_temp = pool.starmap(self.fit_single, 
+                        zip(itertools.repeat(n_events), events_temp, flats_temp,
                             itertools.repeat(threshold),itertools.repeat(False),itertools.repeat(1),\
                             itertools.repeat([]),itertools.repeat([]),\
-                            itertools.repeat('random'),itertools.repeat(max_bumps)))
+                            itertools.repeat('random'),itertools.repeat(max_events)))
             else:
                 raise ValueError('For loop not yet written use cpus >1')
-            models = xr.concat(bump_loo_likelihood_temp, dim="iteration")
-            bump_loo_results.append(models.sel(iteration=[np.where(models.likelihoods == models.likelihoods.max())[0][0]]).squeeze('iteration'))
+            models = xr.concat(event_loo_likelihood_temp, dim="iteration")
+            event_loo_results.append(models.sel(iteration=[np.where(models.likelihoods == models.likelihoods.max())[0][0]]).squeeze('iteration'))
             i+=1
-        bests = xr.concat(bump_loo_results, dim="n_bumps")
-        bests = bests.assign_coords({"n_bumps": np.arange(max_bumps,min_bumps,-1)})
+        bests = xr.concat(event_loo_results, dim="n_events")
+        bests = bests.assign_coords({"n_events": np.arange(max_events,min_events,-1)})
         #bests = bests.squeeze('iteration')
         return bests
 
-    def compute_max_bumps(self):
+    def compute_max_events(self):
         '''
-        Compute the maximum possible number of bumps given bump width and mean or minimum reaction time
+        Compute the maximum possible number of events given event width and mean or minimum reaction time
         '''
-        return int(np.min(self.durations)//(self.min_duration+1))
+        return int(np.min(self.durations)//(self.event_width_samples))
 
-    def bump_times(self, eventprobs, mean=True):
+    def event_times(self, eventprobs, mean=True):
         '''
-        Compute bump onset times based on bump probabilities
+        Compute event onset times based on event probabilities
         Parameters
         ----------
         a : float
             shape parameter
         b : float
             scale parameter
         max_length : int
             maximum length of the trials        
         Returns
         -------
         d : ndarray
             density for a gamma with given parameters
         '''
-        warn('This method is deprecated and will be removed in future version, use compute_times() instead', DeprecationWarning, stacklevel=2)
-        eventprobs = eventprobs.dropna('bump', how="all")
+        # warn('This method is deprecated and will be removed in future version, use compute_times() instead', DeprecationWarning, stacklevel=2)
+        eventprobs = eventprobs.dropna('event', how="all")
         eventprobs = eventprobs.dropna('trial_x_participant', how="all")
-        onsets = np.empty((len(eventprobs.trial_x_participant),len(eventprobs.bump)+1))
+        onsets = np.empty((len(eventprobs.trial_x_participant),len(eventprobs.event)+1))*np.nan
         i = 0
         for trial in eventprobs.trial_x_participant.dropna('trial_x_participant', how="all").values:
-            onsets[i, :len(eventprobs.bump)] = np.arange(self.max_d) @ eventprobs.sel(trial_x_participant=trial).data
+            onsets[i, :len(eventprobs.event)] = np.arange(self.max_d) @ eventprobs.sel(trial_x_participant=trial).data
             onsets[i, -1] = self.ends[i] - self.starts[i]
             i += 1
         if mean:
             return np.mean(onsets, axis=0)
         else:
             return onsets
 
     @staticmethod        
     def compute_times(init, estimates, duration=False, fill_value=None, mean=False, cumulative=False, add_rt=False):
         '''
-        Compute the likeliest onset times for each bump
+        Compute the likeliest onset times for each event
 
         Parameters
         ----------
         estimates :
-            Estimated instance of an hsmm model
+            Estimated instance of an HMP model
         init : 
-            Initialized HsMM object  
+            Initialized HMP object  
         duration : bool
             Whether to compute onset times (False) or stage duration (True)
         fill_value : float | ndarray
             What value to fill for the first onset/duration
 
         Returns
         -------
         times : xr.DataArray
-            Transition event onset or stage duration with trial_x_participant*bump dimensions
+            Transition event onset or stage duration with trial_x_participant*event dimensions
         '''
 
         eventprobs = estimates.eventprobs
-        times = xr.dot(eventprobs, eventprobs.samples, dims='samples')#Most likely bump location
+        times = xr.dot(eventprobs, eventprobs.samples, dims='samples')#Most likely event location
         n = len(times[0,:].values[np.isfinite(times[0,:].values)])
         if duration:
             fill_value=0
         if fill_value != None:            
             added = xr.DataArray(np.repeat(fill_value,len(times.trial_x_participant))[np.newaxis,:],
-                                 coords={'bump':[0], 
+                                 coords={'event':[0], 
                                          'trial_x_participant':times.trial_x_participant})
-            times = times.assign_coords(bump=times.bump+1)
+            times = times.assign_coords(event=times.event+1)
             times = times.combine_first(added)
         if add_rt:             
             rts = init.named_durations
-            rts = rts.assign_coords(bump=int(times.bump.max().values+1))
-            rts = rts.expand_dims(dim="bump")
-            times = xr.concat([times, rts], dim='bump')
+            rts = rts.assign_coords(event=int(times.event.max().values+1))
+            rts = rts.expand_dims(dim="event")
+            times = xr.concat([times, rts], dim='event')
         if duration:
-            #adding reaction time and treating it as the last bump
-            times = times.rename({'bump':'stage'})
+            #adding reaction time and treating it as the last event
+            times = times.rename({'event':'stage'})
             if not cumulative:
                 times = times.diff(dim='stage')
         if mean:
             times = times.mean('trial_x_participant')
         return times
    
     @staticmethod
-    def compute_topologies(electrodes, estimated, bump_width_samples, extra_dim=False):
-        shifted_times = estimated.eventprobs.shift(samples=bump_width_samples//2+1, fill_value=0).copy()#Shifts to compute electrode topology at the peak of the bump
+    def compute_topologies(electrodes, estimated, event_width_samples, extra_dim=False):
+        shifted_times = estimated.eventprobs.shift(samples=event_width_samples//2+1, fill_value=0).copy()#Shifts to compute electrode topology at the peak of the event
         if extra_dim:
             return xr.dot(electrodes.rename({'epochs':'trials'}).\
                       stack(trial_x_participant=['participant','trials']).data.fillna(0), \
                       shifted_times.fillna(0), dims=['samples']).mean('trial_x_participant').\
-                      transpose(extra_dim,'bump','electrodes')
+                      transpose(extra_dim,'event','electrodes')
         else:
             return xr.dot(electrodes.rename({'epochs':'trials'}).\
                       stack(trial_x_participant=['participant','trials']).data.fillna(0), \
                       shifted_times.fillna(0), dims=['samples']).mean('trial_x_participant').\
-                      transpose('bump','electrodes')
+                      transpose('event','electrodes')
     
-    def gen_random_stages(self, n_bumps, mean_d):
+    def gen_random_stages(self, n_events, mean_d):
         '''
         Returns random stage duration between 0 and mean RT by iteratively drawind sample from a 
         uniform distribution between the last stage duration (equal to 0 for first iteration) and 1.
         Last stage is equal to 1-previous stage duration.
         The stages are then scaled to the mean RT
         Parameters
         ----------
-        n_bumps : int
-            how many bumps
+        n_events : int
+            how many events
         mean_d : float
             scale parameter
         Returns
         -------
         random_stages : ndarray
             random partition between 0 and mean_d
         '''
-        random_stages = np.array([[self.shape,(x*mean_d/self.shape)+self.min_duration/self.shape] for x in np.random.beta(2, 2, n_bumps+1)])
+        random_stages = np.array([[self.shape,x*mean_d/self.shape] for x in np.random.beta(2, 2, n_events+1)])
         return random_stages
     
-    def grid_search(self, n_stages, n_points=None, verbose=True, start_time=0, end_time=None, iter_limit=np.inf, step=1, offset=None, method='slide'):
+    def _grid_search(self, n_stages, n_points=None, verbose=True, start_time=0, end_time=None, iter_limit=np.inf, step=1, offset=None, method='slide'):
         '''
         This function decomposes the mean RT into a grid with points. Ideal case is to have a grid with one sample = one search point but the number
         of possibilities badly scales with the length of the RT and the number of stages. Therefore the iter_limit is used to select an optimal number
         of points in the grid with a given spacing. After having defined the grid, the function then generates all possible combination of 
-        bump placements within this grid. It is faster than using random points (both should converge) but depending on the mean RT and the number 
-        of bumps to look for, the number of combination can be really large. 
+        event placements within this grid. It is faster than using random points (both should converge) but depending on the mean RT and the number 
+        of events to look for, the number of combination can be really large. 
         
         Parameters
         ----------
         n_stages : int
-            how many bump to look for
+            how many event to look for
         iter_limit : int
             How much is too much
 
         Returns
         -------
         parameters : ndarray
             3D array with numper of possibilities * n_stages * 2 (gamma parameters)
         '''
         from itertools import combinations_with_replacement, permutations  
         from math import comb as binomcoeff
         import more_itertools as mit
         if offset is None:
-            offset = self.min_duration
+            offset = 1
         start_time = int(start_time)
         if end_time is None:
             end_time = int(self.mean_d)
         duration = end_time-start_time
         if n_points is None:
             n_points = duration//step
             duration = step*n_points
@@ -766,113 +763,113 @@
             if method == 'grid':
                 return parameters
             else:
                 return parameters[np.argsort(parameters[:,0,1]),:,:]
         else:
             raise ValueError(f'No combination found given length of the data {self.mean_d}, number of events {n_stages} and a max iteration of {iter_limit}')
     
-    def sliding_bump(self, n_bumps=None, colors=default_colors, figsize=(12,3), verbose=True, method=None, plot_deriv=False, magnitudes=None, step=1):
+    def sliding_event(self, n_events=None, colors=default_colors, figsize=(12,3), verbose=True, method=None, plot_deriv=False, magnitudes=None, step=1):
         '''
-        This method outputs the likelihood and estimated parameters of a 1 bump model with each sample, from 0 to the mean 
+        This method outputs the likelihood and estimated parameters of a 1 event model with each sample, from 0 to the mean 
         epoch duration. The parameters and likelihoods that are returned are 
-        Take the highest likelihood, place a bump by excluding bump width space around it, follow with the next one
+        Take the highest likelihood, place a event by excluding event width space around it, follow with the next one
         '''
         
         from itertools import cycle
         
         mean_d = int(self.mean_d)
-        init_n_bumps = n_bumps
-        # if n_bumps == None:
-        #     n_bumps = self.max_bumps
-        parameters = self.grid_search(2, verbose=verbose, step=step)#Looking for all possibilities with one bump
+        init_n_events = n_events
+        # if n_events == None:
+        #     n_events = self.max_events
+        parameters = self._grid_search(2, verbose=verbose, step=step)#Looking for all possibilities with one event
         if magnitudes is None:
             magnitudes = np.zeros((len(parameters),1, self.n_dims), dtype=np.float64)
         else:
             magnitudes = np.tile(magnitudes, (len(parameters),1, self.n_dims))
-            method = 'single_bump'
+            method = 'single_event'
         lkhs_init, mags_init, pars_init, _ = \
-            self.estimate_single_bump(magnitudes, parameters, [0,1], [], 1)
+            self.estimate_single_event(magnitudes, parameters, [0,1], [], 1)
         if verbose:
             _, ax = plt.subplots(figsize=figsize, dpi=300)
             ax.plot(pars_init[:,0,1]*self.shape, lkhs_init, '-', color='k')
         if method == 'derivative':
             deriv = np.gradient(lkhs_init)
-            bump_idx = np.where(np.diff(np.sign(deriv)) < 0)[0]
-            n_bumps = len(bump_idx)
+            event_idx = np.where(np.diff(np.sign(deriv)) < 0)[0]
+            n_events = len(event_idx)
             cycol = cycle(colors)
-            colors = [next(cycol) for x in range(n_bumps)]
-            pars = np.zeros((len(bump_idx)+1, 2), dtype=np.float64)
-            pars[:len(bump_idx), :] = pars_init[:, 0, :][bump_idx, :]
-            pars[len(bump_idx),:] = np.array([self.shape, mean_d/self.shape])#last stage defined as rt
-            mags = mags_init[:, :, :][bump_idx]
-            lkhs = lkhs_init[bump_idx]
+            colors = [next(cycol) for x in range(n_events)]
+            pars = np.zeros((len(event_idx)+1, 2), dtype=np.float64)
+            pars[:len(event_idx), :] = pars_init[:, 0, :][event_idx, :]
+            pars[len(event_idx),:] = np.array([self.shape, mean_d/self.shape])#last stage defined as rt
+            mags = mags_init[:, :, :][event_idx]
+            lkhs = lkhs_init[event_idx]
             if verbose:
-                for bump in range(len(bump_idx)):
-                    ax.plot(np.array(pars)[bump,1]*self.shape, lkhs[bump], 'o', color=colors[bump], label='Likelihood of Transition event %s'%(bump+1))
+                for event in range(len(event_idx)):
+                    ax.plot(np.array(pars)[event,1]*self.shape, lkhs[event], 'o', color=colors[event], label='Likelihood of Transition event %s'%(event+1))
                 plt.ylabel('Log-likelihood')
                 plt.xlabel('Sample number')
                 plt.legend()
                 plt.show()
                 if plot_deriv:
                     _, ax = plt.subplots(figsize=figsize, dpi=300)
                     plt.plot(pars_init[:,0,1]*self.shape, np.gradient(lkhs_init), '-', color='k')
                     plt.hlines(0, 0, mean_d)
                     plt.show()
             
         elif method == 'estimation':
-            if n_bumps is None:
-                n_bumps = self.compute_max_bumps()
+            if n_events is None:
+                n_events = self.compute_max_events()
             lkhs_sp, mags_sp, pars_sp, eventprobs_sp = \
-                self.estimate_single_bump(np.zeros((len(parameters),1,self.n_dims), dtype=np.float64), \
+                self.estimate_single_event(np.zeros((len(parameters),1,self.n_dims), dtype=np.float64), \
                 parameters, [], [], 1)
             lkhs_sp_sorting = lkhs_sp.copy()
             mags_sp_sorting = mags_sp.copy()
             pars_sp_sorting = pars_sp.copy()
             group_color = np.empty(len(lkhs_sp),dtype=str)
             max_lkhs = []
-            for bump in range(n_bumps):
-                if not np.isnan(lkhs_sp_sorting).all():#Avoids problem if n_bumps > actual bumps
+            for event in range(n_events):
+                if not np.isnan(lkhs_sp_sorting).all():#Avoids problem if n_events > actual events
                     max_lkh = np.where(lkhs_sp_sorting == np.nanmax(lkhs_sp_sorting))[0][0]
                     max_lkhs.append(max_lkh)
                     gamma_max = pars_sp[max_lkh,0,1] 
-                    neighbors = np.where(abs(pars_sp[:,0,1]-gamma_max) <= (self.bump_width_samples/2)/self.shape)[0]
+                    neighbors = np.where(abs(pars_sp[:,0,1]-gamma_max) <= (self.event_width_samples/2)/self.shape)[0]
                     group = np.concatenate([[max_lkh], neighbors])
                     if verbose:
-                        ax.plot(np.array(pars_sp)[group,0,1]*self.shape, lkhs_sp_sorting[group], 'o', color=colors[bump])
+                        ax.plot(np.array(pars_sp)[group,0,1]*self.shape, lkhs_sp_sorting[group], 'o', color=colors[event])
                     lkhs_sp_sorting[group] = np.nan
                     pars_sp_sorting[group, :, :] = np.nan
 
-            if np.isnan(lkhs_sp_sorting).all() and init_n_bumps != None and verbose:
-                print(f'The number of requested bumps exceeds the number of convergence points found in the parameter space, bumps {bump} to {n_bumps} were not found') 
+            if np.isnan(lkhs_sp_sorting).all() and init_n_events != None and verbose:
+                print(f'The number of requested events exceeds the number of convergence points found in the parameter space, events {event} to {n_events} were not found') 
 
             if not np.isnan(lkhs_sp_sorting).all() and verbose:#plot remaining points if all where not handled before
                 ax.plot(pars_sp_sorting[:,0,1]*self.shape, lkhs_sp_sorting, 'o', color='gray', label='Not attributed')
                 ax.legend()
             if verbose: 
                 ax.set_xlabel('sample #')
                 ax.set_ylabel('Loglikelihood')
                 plt.show()
-            pars = np.tile(np.nan, (n_bumps+1, 2))
+            pars = np.tile(np.nan, (n_events+1, 2))
             pars[:len(max_lkhs), :] = pars_sp[max_lkhs, 0, :]
             order = np.argsort(pars[:len(max_lkhs),1])#sorted index based on first stage duration
             pars[:len(max_lkhs), :] = pars[order, :]
             mags = mags_sp[max_lkhs][order]
             max_lkhs = np.array(max_lkhs)[order]
             pars[len(max_lkhs),:] = np.array([self.shape, mean_d/self.shape])#last stage defined as rt
-            lkhs = np.repeat(np.nan, n_bumps)
+            lkhs = np.repeat(np.nan, n_events)
             lkhs[:len(max_lkhs)] = lkhs_sp[max_lkhs]
         elif method is None:
             #pars, mags, lkhs = pars_init, mags_init, lkhs_init
             plt.ylabel('Log-likelihood')
             plt.xlabel('Sample number')
             plt.show()
         else:
             return pars, mags[:, 0, :], lkhs
 
-    def estimate_single_bump(self, magnitudes, parameters, parameters_to_fix, magnitudes_to_fix, threshold):
+    def estimate_single_event(self, magnitudes, parameters, parameters_to_fix, magnitudes_to_fix, threshold):
         if self.cpus >1:
             if np.shape(magnitudes) == 2:
                 magnitudes = np.tile(magnitudes, (len(parameters), 1, 1))
             with mp.Pool(processes=self.cpus) as pool:
                 estimates = pool.starmap(self.EM, 
                     zip(itertools.repeat(1), magnitudes, parameters, 
                         itertools.repeat(threshold), itertools.repeat(magnitudes_to_fix), 
@@ -883,178 +880,152 @@
                 estimates.append(self.EM(1, mags, pars, threshold, magnitudes_to_fix, parameters_to_fix))
         lkhs_sp = np.array([x[0] for x in estimates])
         mags_sp = np.array([x[1] for x in estimates])
         pars_sp = np.array([x[2] for x in estimates])
         eventprobs_sp = np.array([x[3] for x in estimates])
         return lkhs_sp, mags_sp, pars_sp, eventprobs_sp
     
-    def fit(self, step=1, verbose=True, figsize=(12,3), end=None, stdev=None, threshold=1, bwd=False, trace=False):
+    def fit(self, step=1, verbose=True, figsize=(12,3), end=None, stdev=None, threshold=1, trace=False):
         '''
         '''
         if end is None:
-            end = int(self.mean_d)
+            end = self.mean_d
+        n_points = int(end//step)
         if threshold is None:
-            threshold = stdev/np.sqrt(self.n_trials)*self.n_dims
+            threshold = (stdev/np.sqrt(self.n_trials))
             print(threshold)
-        # else:
-        #     print(f'Using {threshold} as threshold for event separation') 
-        n_points = int(end//step)
         end = step*(n_points)#Rounding up to step size  
-        lkh = np.repeat(-np.inf, n_points+1)
-        pars, mags = np.zeros((n_points-1,2)),np.zeros((n_points-1, self.n_dims))
-        new_pars, new_mags = pars.copy(), mags.copy()
+        lkh = -np.inf
+        pars = np.zeros((n_points-1,2))
+        pars[:,0] = self.shape
+        pars[0,1] = 0.5#initialize with one event
+        mags = np.zeros((n_points-1, self.n_dims))
         pbar = tqdm(total = end)
-        n_bumps, i, j, time = 1,0,0,0
-        #Adding an initial bump as threshold might miss the difference with 0
-        pars[:n_bumps] = np.array([self.shape, (self.min_duration)/self.shape])
+        n_events, j, time = 1,1,0
+        last_stage = end
         if trace:
             all_pars, all_mags, all_mags_prop, all_pars_prop, all_diffs = [],[],[],[],[]
-        previous_bump = np.zeros(self.n_dims)
-        while time < end-self.min_duration*2:
-            prev_time = time
-            if j == 0:
-                # print(pars[:n_bumps])
-                # print(mags[:n_bumps])
-                # print((np.round(pars[:n_bumps].prod(axis=1).sum())))
-                next_pars = self.grid_search(2, verbose=False, start_time=\
-                    (np.round(pars[:n_bumps].prod(axis=1).sum())), step=step, end_time=end)#next steps in parameter space
-                next_mags = np.zeros(self.n_dims)#reinitialisze mags
-            if j < len(next_pars):
-                pars_prop = np.concatenate([pars[:n_bumps], next_pars[j]])
-                mags_prop = np.concatenate([mags[:n_bumps], [next_mags]])
-                # print(mags_prop)
-                # print(pars_prop[:n_bumps+2].prod(axis=1).cumsum())
-                # print(pars_prop)
-
-                # next_pars[j, 1, 1] = end/self.shape-np.sum(pars_prop[:n_bumps+1, 1])
-                lkh[i], new_mags[:n_bumps+1], new_pars[:n_bumps+2], _ = \
-                    self.EM(n_bumps+1, mags_prop, pars_prop, 1, [], [])
-                # print(new_pars[:n_bumps+2].prod(axis=1).cumsum())
-                
-                diffs = mags[n_bumps-1]  -  new_mags[n_bumps]
-                if trace:
-                    all_mags_prop.append(mags_prop.copy())
-                    all_pars_prop.append(pars_prop.copy())
-                    all_mags.append(new_mags[:n_bumps+1].copy())
-                    all_pars.append(new_pars[:n_bumps+2].copy())
-                    all_diffs.append(diffs)
-                # print(diffs)
-                if np.any(np.abs(diffs)  > threshold):#valid iteration
-                    # print(new_mags[n_bumps])
-                    # print(f'Times = {np.round(pars[:n_bumps].prod(axis=1).cumsum())}')
-
-                    time = new_pars[:n_bumps+1].prod(axis=1).sum()+j*step
-                    if time < end-step*2-self.min_duration:
-                        j = 0
-                        n_bumps += 1
-                        # print(pars[:n_bumps+1])
-                        pars[:n_bumps], mags[:n_bumps] = new_pars[:n_bumps].copy(), new_mags[:n_bumps].copy()
-                        # print(pars[:n_bumps])
-                        if verbose:
-                            print(f'Transition event {n_bumps} found around sample {int(np.round(np.sum(pars[:n_bumps,:].prod(axis=1))))} (step {i}): Transition event samples = {np.round(pars[:n_bumps].prod(axis=1).cumsum())}')
-                    else:
-                        j += 1
-                    # print(f'Times = {np.round(pars[:n_bumps].prod(axis=1).cumsum())}')
-
-                else:
-                    # if np.all(np.any(new_mags[n_bumps] > threshold)) :
-                    pars[:n_bumps,:] = new_pars[:n_bumps,:]
-                    mags[:n_bumps] = new_mags[:n_bumps]
-                    next_mags = new_mags[n_bumps]
-                    # else:
-                    #     next_mags = np.zeros(self.n_dims)#reinitialisze mags
-                    j += 1
-
-                i += 1
-                time = pars[:n_bumps].prod(axis=1).sum()+j*step
-                pbar.update(int(np.round(time-prev_time)))
-            else:
-                break
-        pbar.update(int(np.round(end-time)))
-        mags = mags[:n_bumps, :]
-        pars = pars[:n_bumps+1, :]
-        pars[-1, :] = np.concatenate([[self.shape], [self.mean_d/self.shape-np.sum(pars[:-1, 1])]])
-        fit = self.fit_single(len(pars)-1, parameters=pars, magnitudes=mags, verbose=verbose)
+        pars_accepted, mags_accepted = pars.copy(), mags.copy()
+        pars_prop = pars_accepted[:n_events+2].copy()#cumulative
+        pars_prop[n_events,1] = step*j/self.shape
+        last_stage = end/self.shape - np.sum(pars_prop[:n_events+1,1])
+        pars_prop[n_events+1,1] = last_stage
+        while last_stage*self.shape > self.location+step:
+            prev_n_events, prev_lkh, prev_time = n_events, lkh, time
+            mags_prop = mags_accepted[:n_events+1].copy()
+            lkh, mags[:n_events+1], pars[:n_events+2], _ = \
+                self.EM(n_events+1, mags_prop, pars_prop.copy(), 1, [], [])
+            diffs = np.diff(mags[:n_events+1], axis=0)
+            if np.all(np.any(np.abs(diffs) > threshold, axis=1)):
+                n_events += 1
+                pars_accepted = pars[:n_events+2].copy()
+                mags_accepted = mags[:n_events+2].copy()
+                mags_accepted[n_events] =  np.zeros(self.n_dims)
+                j = 0
+                if verbose:
+                    print(f'Transition event {n_events} found around sample {int(np.round(np.sum(pars_accepted[:n_events,:].prod(axis=1))))}')#: Transition event samples = {np.round(pars[:n_events].prod(axis=1).cumsum())+self.location*np.arange(n_events)}')
+            if trace:
+                all_mags_prop.append(mags_prop.copy())
+                all_pars_prop.append(pars_prop.copy())
+                all_mags.append(mags_accepted[:n_events].copy())
+                all_pars.append(pars_accepted[:n_events+1].copy())
+                all_diffs.append(diffs)
+            j += 1
+            pars_prop = pars_accepted[:n_events+2].copy()#cumulative
+            pars_prop[n_events,1] = step*j/self.shape
+            last_stage = end/self.shape - np.sum(pars_prop[:n_events+1,1])
+            pars_prop[n_events+1,1] = last_stage
+            time = np.sum(pars_prop[:n_events,1])*self.shape + \
+                self.location*n_events + step*j/self.shape
+            pbar.update(int(np.round(time-prev_time+1)))
+        # pbar.update(int(np.round(end-prev_time)+self.location+step))
+        mags = mags_accepted[:n_events, :]
+        pars = pars_accepted[:n_events+1, :]
+        if n_events > 1: 
+            fit = self.fit_single(n_events, parameters=pars, magnitudes=mags, verbose=verbose)
+        else:
+            warn('Failed to find more than two stages, returning 2 stage model with default starting values')
+            fit = self.fit_single(n_events)
         if trace:
-            all_pars_aligned = np.tile(np.nan, (i+1, np.max([len(x) for x in all_pars]), 2))
-            all_pars_prop_aligned = np.tile(np.nan, (i+1, np.max([len(x) for x in all_pars_prop]), 2))
-            all_mags_aligned = np.tile(np.nan, (i+1, np.max([len(x) for x in all_mags]), self.n_dims))
-            all_mags_prop_aligned = np.tile(np.nan, (i+1, np.max([len(x) for x in all_mags_prop]), self.n_dims))
-            all_diffs_aligned = np.tile(np.nan, (i+1, self.n_dims))
+            all_pars_aligned = np.tile(np.nan, (len(all_pars)+1, np.max([len(x) for x in all_pars]), 2))
+            all_pars_prop_aligned = np.tile(np.nan, (len(all_pars_prop)+1, np.max([len(x) for x in all_pars_prop]), 2))
+            all_mags_aligned = np.tile(np.nan, (len(all_mags)+1, np.max([len(x) for x in all_mags]), self.n_dims))
+            all_mags_prop_aligned = np.tile(np.nan, (len(all_mags_prop)+1, np.max([len(x) for x in all_mags_prop]), self.n_dims))
+            all_diffs_aligned = np.tile(np.nan, (len(all_diffs)+1, np.max([len(x) for x in all_diffs]), self.n_dims))
             for iteration, _i in enumerate(zip(all_pars, all_mags, all_mags_prop, all_pars_prop, all_diffs)):
                 all_pars_aligned[iteration, :len(_i[0]), :] = _i[0]
                 all_mags_aligned[iteration, :len(_i[1]), :] = _i[1]
                 all_mags_prop_aligned[iteration, :len(_i[2]), :] = _i[2]
                 all_pars_prop_aligned[iteration, :len(_i[3]), :] = _i[3]
-                all_diffs_aligned[iteration, :] = _i[4]
-            traces = xr.Dataset({'parameters_accepted': (('iteration', 'stage','parameter'), 
+                all_diffs_aligned[iteration, :len(_i[4]), :] = _i[4]
+            traces = xr.Dataset({'parameters_accepted': (('iteration', 'stage_acc','parameter_acc'), 
                                          all_pars_aligned),
-                                'magnitudes_accepted': (('iteration', 'bump','component'), 
+                                'magnitudes_accepted': (('iteration', 'event_acc','component_acc'), 
                                          all_mags_aligned),
                                 'parameters_proposed': (('iteration', 'stage','parameter'), 
                                          all_pars_prop_aligned),
-                                'magnitudes_proposed': (('iteration', 'bump', 'component'), 
+                                'magnitudes_proposed': (('iteration', 'event', 'component'), 
                                          all_mags_prop_aligned),
-                                'difference_magnitudes':(('iteration', 'component'), 
+                                'difference_magnitudes':(('iteration','diffs', 'component'), 
                                          all_diffs_aligned)})
             return fit, traces
         else:
             return fit
     
-    def bwd_fit(self, step=1, verbose=True, figsize=(12,3), end=None, threshold=None, bwd=True):
+    def _bwd_fit(self, step=1, verbose=True, figsize=(12,3), end=None, threshold=None, bwd=True):
         '''
         '''
         if threshold is None:
             threshold = .05*self.n_dims
         if end is None:
             end = int(self.mean_d)
         n_points = int(end//step)
         lkh = np.repeat(-np.inf, n_points*3)
         pars, mags = np.zeros((n_points-1,2)),np.zeros((n_points-1, self.n_dims))
         new_pars, new_mags = pars.copy(), mags.copy()
         pbar = tqdm(total = n_points-1)
-        n_bumps, i,j = 0,1,0
-        bump_width = self.bump_width_samples / self.shape
+        n_events, i,j = 0,1,0
+        event_width = self.event_width_samples / self.shape
         all_diffs = []
-        while pars[-n_bumps:].prod(axis=1).sum() < self.mean_d:
+        while pars[-n_events:].prod(axis=1).sum() < self.mean_d:
             if bwd:
-                index = range(-n_bumps-2,0)
+                index = range(-n_events-2,0)
             else:
-                index = range(0,n_bumps+2)[::-1]
+                index = range(0,n_events+2)[::-1]
             if j == 0:
                 print(np.round(pars[index[1:]].prod(axis=1).sum()))
-                next_pars = self.grid_search(2, verbose=False, start_time=(np.round(pars[index[:n_bumps]].prod(axis=1).sum())), step=step, end_time=end)#next steps in parameter space
+                next_pars = self._grid_search(2, verbose=False, start_time=(np.round(pars[index[:n_events]].prod(axis=1).sum())), step=step, end_time=end)#next steps in parameter space
                 if bwd:
                     next_pars = next_pars[:,::-1,:]
                     
                 next_mags = np.zeros(self.n_dims)#reinitialisze mags
             if j < len(next_pars):
                 pars_prop = np.concatenate([pars[index[2:]], next_pars[j]])
                 mags_prop = np.concatenate([mags[index[2:]], [next_mags]])
                 print(mags_prop)
                 print(pars_prop)
-                # next_pars[j, 1, 1] = end/self.shape-np.sum(pars_prop[:n_bumps+1, 1])
+                # next_pars[j, 1, 1] = end/self.shape-np.sum(pars_prop[:n_events+1, 1])
                 lkh[i], new_mags[index[1:],:], new_pars[index,:], _ = \
-                    self.EM(n_bumps+1, mags_prop.copy(), pars_prop.copy(), 1, [], [])
+                    self.EM(n_events+1, mags_prop.copy(), pars_prop.copy(), 1, [], [])
                 print(new_mags[index[1:],:])
                 print(new_pars[index,:])
 
                 diffs = np.sum(np.diff(new_mags[index[1:]],axis=0, prepend=0)**2,axis=1)
                 all_diffs.append(diffs[-1])
                 print(diffs)
-                # print(f'Times = {np.round(pars[:n_bumps].prod(axis=1).cumsum())}')
+                # print(f'Times = {np.round(pars[:n_events].prod(axis=1).cumsum())}')
                 if (diffs > threshold).all() and np.all(new_mags[index[1:]][-1]>0):#valid iteration
                     j = 0
-                    n_bumps += 1
+                    n_events += 1
                     pars[index], mags[index] = new_pars[index], new_mags[index]
                     if verbose:
-                        print(f'Transition event {n_bumps} found around time {np.round(np.sum(pars[index[1:]].prod(axis=1)))} (step {i})')
+                        print(f'Transition event {n_events} found around time {np.round(np.sum(pars[index[1:]].prod(axis=1)))} (step {i})')
                     print(f'New pars : {pars[index[0]]}')
-                    print(int((pars[-n_bumps,1] - np.sum(pars_prop[index[1:],1]))*self.shape))
-                    pbar.update(int((np.sum(pars[-n_bumps:,1]) - np.sum(pars_prop[-n_bumps:,1]))*self.shape))
+                    print(int((pars[-n_events,1] - np.sum(pars_prop[index[1:],1]))*self.shape))
+                    pbar.update(int((np.sum(pars[-n_events:,1]) - np.sum(pars_prop[-n_events:,1]))*self.shape))
                 else:
                     pbar.update(1)
                     j += 1
                 i += 1
             else:
                 break
         all_diffs = np.array(all_diffs)
@@ -1076,26 +1047,26 @@
             ax.set_xlabel('Sample number')
             plt.show()
         print(mags)
         print(pars)
         fit = self.fit_single(len(pars)-1, parameters=pars, magnitudes=mags)
         return fit, lkh    
     
-    def bump_gain_plot(self, lkh, pars, mags, colors=default_colors, figsize=(12,3)):
+    def event_gain_plot(self, lkh, pars, mags, colors=default_colors, figsize=(12,3)):
         
         from itertools import cycle
-        n_bumps = len(mags)
+        n_events = len(mags)
         _, ax = plt.subplots(figsize=figsize, dpi=300)
         cycol = cycle(colors)
-        colors = [next(cycol) for x in range(n_bumps)]
-        parameters = self.grid_search(2, verbose=True)
-        for bump in range(n_bumps):
-            bump_lkh = np.zeros(len(parameters))
+        colors = [next(cycol) for x in range(n_events)]
+        parameters = self._grid_search(2, verbose=True)
+        for event in range(n_events):
+            event_lkh = np.zeros(len(parameters))
             iteration = 0
-            print(mags[bump,:])
-            for pars_bump in parameters:
-                bump_lkh[iteration], _, _, _ = \
-                    self.EM(1,  np.array([mags[bump,:]]), pars_bump,1, [0], [0,1])
+            print(mags[event,:])
+            for pars_event in parameters:
+                event_lkh[iteration], _, _, _ = \
+                    self.EM(1,  np.array([mags[event,:]]), pars_event,1, [0], [0,1])
                 iteration += 1
-            ax.plot(parameters[:,0,1], bump_lkh, color=colors[bump])
+            ax.plot(parameters[:,0,1], event_lkh, color=colors[event])
         plt.show()
```

### Comparing `hsmm_mvpy-0.1.0a2/src/hsmm_mvpy/simulations.py` & `hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/simulations.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 '''
 
 import os.path as op
 import os
 import numpy as np
 import mne
 from mne.datasets import sample
+from warnings import warn
+
 
 def available_sources():
     '''
     list available sources for sample subject in MNE
     '''
     data_path = sample.data_path()
     subjects_dir = op.join(data_path, 'subjects')
@@ -44,17 +46,17 @@
     bump_idx = np.arange(bump_width_samples)*steps+steps/2
     bump_frequency = 1000/(bump_width*2)#gives bump frequency given that bumps are defined as half-sines
     template = np.sin(2*np.pi*bump_idx/1000*bump_frequency)#bump morph based on a half sine with given bump width and sampling frequency
     template = template/np.sum(template**2)#Weight normalized
     return template
 
 
-def simulate(sources, n_trials, n_jobs, file, n_subj=1, path='./', overwrite=False, verbose=False): 
+def simulate(sources, n_trials, n_jobs, file, data_type='eeg', n_subj=1, path='./', overwrite=False, verbose=False, noise=True, times=None, location=1): 
     '''
-    Simulates EEG n_trials using MNE's tools based on the specified sources
+    Simulates n_trials of EEG and/or MEG using MNE's tools based on the specified sources
     
     Parameters
     ----------
     sources : list
         2D or 3D list with dimensions (n_subjects *) sources * source_parameters
         Source parameters should contain :
         - the name of the source (see the output of available_source())
@@ -63,20 +65,30 @@
         - the duration of the preceding stage as a scipy.stats distribution (e.g. scipy.stats.gamma(a, scale))
     n_trials: int
         Number of trials
     n_jobs: int
         Number of jobs to use with MNE's function (multithreading)
     file: str
         Name of the file to be saved (number of the subject will be added)
+    data_type: str
+        Whether to simulate "eeg" or "meg"
+    n_subj: int
+        How many subjects to simulate
     path: str
         path where to save the data
     overwrite: bool
         Whether to overwrite existing file
     verbose: bool
         Whether to display MNE's output
+    noise: bool
+        Adding noise to the simulated sources
+    times: ndarray
+        Deterministic simulation of event transitions times. Format is n_sources X n_trials
+    location: float
+        value in ms to add after a simulated event and before another one
     
     Returns
     -------
     generating_events: ndarray
         Times of the simulated bumps used to test for accurate recovery compared to estimation
     files: list
         list of file names (file + number of subject)
@@ -85,27 +97,39 @@
     if len(np.shape(sources)) == 2:
         sources = [sources]#If only one subject
     if np.shape(sources)[0] != n_subj:
         raise ValueError('Number of subject is not coherent with the sources provided')
     #Infer max duration of a trial from the specified sources
     percentiles = np.empty(len(sources[0]))
     for source in range(len(sources[0])):
-        stage_dur_fun = sources[0][source][-1]
-        percentiles[source] = np.percentile(stage_dur_fun.rvs(size=n_trials), q=99)
+        if times is None:
+            stage_dur_fun = sources[0][source][-1]
+            percentiles[source] = np.percentile(stage_dur_fun.rvs(size=n_trials), q=99)
+        else:
+            percentiles[source] = np.max(times[:,source])
     max_trial_length = np.sum(percentiles)+1000
     # Following code and comments largely comes from MNE examples (e.g. \
     # https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html)
     # It loads the data, info structure and forward solution for one example subject,
     # Note that all 'subject' will use this forward solution
     data_path = sample.data_path()
     subjects_dir = op.join(data_path, 'subjects')
     subject = 'sample'
     # First, we get an info structure from the test subject.
     evoked_fname = op.join(data_path, 'MEG', subject, 'sample_audvis-ave.fif')
     info = mne.io.read_info(evoked_fname, verbose=verbose)
+    if data_type == 'eeg':
+        picked_type = mne.pick_types(info, meg=False, eeg=True)
+    elif data_type == 'meg':
+        picked_type = mne.pick_types(info, meg=True, eeg=False)
+    elif data_type == 'eeg/meg':
+        picked_type = mne.pick_types(info, meg=True, eeg=False)
+    else:
+        raise ValueError(f'Invalid data type {data_type}, expected "eeg", "meg" or "eeg/meg"')
+    info = mne.pick_info(info, picked_type)
     tstep = 1. / info['sfreq']
     # To simulate sources, we also need a source space. It can be obtained from the
     # forward solution of the sample subject.
     fwd_fname = op.join(data_path, 'MEG', subject,'sample_audvis-meg-eeg-oct-6-fwd.fif')
     fwd = mne.read_forward_solution(fwd_fname, verbose=verbose)
     src = fwd['src']
     
@@ -116,15 +140,15 @@
         files_subj = []
         source_simulator = mne.simulation.SourceSimulator(src, tstep=tstep, first_samp=0, \
                     duration=(2+1*n_trials+3)*max_trial_length*tstep)
         if n_subj == 1: subj_file = file + f'_raw.fif'
         else: subj_file = file + f'_{subj}_raw.fif'
         if subj_file in os.listdir(path) and not overwrite:
             subj_file = path+subj_file
-            print(f'{subj_file} exists no new simulation performed')
+            warn(f'{subj_file} exists no new simulation performed', UserWarning)
             files_subj.append(subj_file)
             files_subj.append(subj_file.split('.fif')[0]+'_generating_events.npy')
             files.append(files_subj)
         else:
             subj_file = path+subj_file
             print(f'Simulating {subj_file}')
             sources_subj = sources[subj]
@@ -133,54 +157,66 @@
             stim_onsets =  2000+max_trial_length * np.arange(n_trials)#2000 = offset of first stim
             events[:,0] = stim_onsets#last event 
             events[:,2] = 1#trigger 1 = stimulus 
 
             #Fake source, actually stimulus onset
             selected_label = mne.read_labels_from_annot(
                     subject, regexp=sources_subj[0][0], subjects_dir=subjects_dir, verbose=verbose)[0]
-            label = mne.label.select_sources(
-                    subject, selected_label, location='center', extent=10,# Extent in mm of the region.
-                    subjects_dir=subjects_dir)
+            label = mne.label.select_sources(subject, selected_label, subjects_dir=subjects_dir)
             source_time_series = np.array([1e-99])#stim trigger
             source_simulator.add_data(label, source_time_series, events)
             source_simulator.add_data(label, source_time_series, events)
 
             trigger = 2
             random_source_times = []
             generating_events = events
             for source in sources_subj:
                 selected_label = mne.read_labels_from_annot(
                     subject, regexp=source[0], subjects_dir=subjects_dir, verbose=verbose)[0]
-                label = mne.label.select_sources(
-                    subject, selected_label, location='center', extent=10,# Extent in mm of the region.
-                    subjects_dir=subjects_dir)
-
+                label = mne.label.select_sources(subject, selected_label, subjects_dir=subjects_dir, location='random', extent=1)
+                #last two parameters ensure sources that are different enough
                 # Define the time course of the activity for each source of the region to
                 # activate
                 bump_duration = int(((1/source[1])/2)*info['sfreq'])
-                source_time_series = bump_shape(((1000/source[1])/2),bump_duration,1000/info['sfreq'])* source[2]
+                source_time_series = bump_shape(((1000/source[1])/2),bump_duration,1000/info['sfreq'])*source[2]
+
                 #adding source event
                 events = events.copy()
-                rand_i = np.round(source[-1].rvs(size=n_trials)/(tstep*1000),decimals=0)+1#+1 as bump is next sample after stage
+                if times is None:
+                    rand_i = np.round(source[-1].rvs(size=n_trials)/(tstep*1000),decimals=0)
+                else:
+                    rand_i = times[:,trigger-2]
+                if len(sources_subj)+1 > trigger > 2:
+                    rand_i += location/(tstep*1000)
+                else:
+                    rand_i += 1
+                if 0 in rand_i:
+                    warn("0 stage duration found, add a location parameter to avoid this case", UserWarning)
                 random_source_times.append(rand_i) #varying event 
                 events[:, 0] = events[:,0] + random_source_times[-1] # Events sample.
                 events[:, 2] = trigger  # All events have the sample id.
                 trigger += 1
                 generating_events = np.concatenate([generating_events, events])
 
                 #add these events
                 source_simulator.add_data(label, source_time_series, events)
 
             generating_events = generating_events[generating_events[:, 0].argsort()]
             # Project the source time series to sensor space and add some noise. The source
             # simulator can be given directly to the simulate_raw function.
             raw = mne.simulation.simulate_raw(info, source_simulator, forward=fwd, n_jobs=n_jobs,verbose=verbose)
-            raw = raw.pick_types(meg=False, eeg=True, stim=True)
-            cov = mne.make_ad_hoc_cov(raw.info, verbose=verbose)
-            mne.simulation.add_noise(raw, cov, iir_filter=[0.2, -0.2, 0.04], verbose=verbose)
+            if data_type == 'eeg':
+                raw = raw.pick_types(meg=False, eeg=True, stim=True)
+            elif data_type == 'meg':
+                raw = raw.pick_types(meg=True, eeg=False, stim=True)
+            elif data_type == 'eeg/meg':
+                raw = raw.pick_types(meg=True, eeg=True, stim=True)
+            if noise:
+                cov = mne.make_ad_hoc_cov(raw.info, verbose=verbose)
+                mne.simulation.add_noise(raw, cov, iir_filter=[0.2, -0.2, 0.04], verbose=verbose)
             raw.save(subj_file, overwrite=True)
             files_subj.append(subj_file)
             np.save(subj_file.split('.fif')[0]+'_generating_events.npy', generating_events)
             files_subj.append(subj_file.split('.fif')[0]+'_generating_events.npy')
             files.append(files_subj)
             print(f'{subj_file} simulated')
     if n_subj == 1:
```

### Comparing `hsmm_mvpy-0.1.0a2/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,49 +3,62 @@
 '''
 
 import numpy as np
 import scipy.stats as stats
 import xarray as xr
 import multiprocessing as mp
 import itertools
+import pandas as pd
 import warnings
 from warnings import warn, filterwarnings
 
-
-filterwarnings('ignore', 'Degrees of freedom <= 0 for slice.', )#weird warning, likely due to nan in xarray, not important but better fix it later  
-
-def read_mne_EEG(pfiles, event_id, resp_id, sfreq=None, subj_idx=None, events_provided=None, verbose=True,
-                 tmin=-.2, tmax=5, offset_after_resp = 0, high_pass=.5, pick_channels = 'eeg', baseline=(None, 0),\
-                 low_pass = 30, upper_limit_RT=5, lower_limit_RT=0.001, reject_threshold=None):
+def read_mne_EEG(pfiles, event_id=None, resp_id=None, epoched=False, sfreq=None, 
+                 subj_idx=None, metadata = None, events_provided=None, rt_col='response',
+                 verbose=True, tmin=-.2, tmax=5, offset_after_resp = 0, 
+                 high_pass=.5, low_pass = None, pick_channels = 'eeg', baseline=(None, 0),
+                 upper_limit_RT=5, lower_limit_RT=0.001, reject_threshold=None):
+    warn('This method is deprecated and will be removed in future version, use read_mne_data instead', DeprecationWarning, stacklevel=2)
+    return read_mne_data(pfiles, event_id, resp_id, epoched, sfreq, 
+                 subj_idx, metadata, events_provided, rt_col,
+                 verbose, tmin, tmax, offset_after_resp, 
+                 high_pass, low_pass, pick_channels, baseline,
+                 upper_limit_RT, lower_limit_RT, reject_threshold)
+
+def read_mne_data(pfiles, event_id=None, resp_id=None, epoched=False, sfreq=None, 
+                 subj_idx=None, metadata=None, events_provided=None, rt_col='rt', rts=None,
+                 verbose=True, tmin=-.2, tmax=5, offset_after_resp = 0, 
+                 high_pass=.5, low_pass = None, pick_channels = 'eeg', baseline=(None, 0),
+                 upper_limit_RT=5, lower_limit_RT=0.001, reject_threshold=None, scale=1):
     ''' 
-    Reads EEG data format (.fif or .bdf) using MNE's integrated function .
+    Reads EEG/MEG data format (.fif or .bdf) using MNE's integrated function .
     
     Notes: 
-    - Only EEG data are selected (other channel types are discarded)
+    - Only EEG or MEG data are selected (other channel types are discarded)
     - All times are expressed on the second scale.
     - If multiple files in pfiles the data of the group is read and seqentially processed.
-    - Reaction Times are only computed if response trigger is in the epoch window (determined by tmin and tmax)
+    - For non epoched data: Reaction Times are only computed if response trigger is in the epoch window (determined by tmin and tmax)
     
     Procedure:
-    1) the data is filtered with filters specified in low_pass and high_pass. Parameters of the filter are
+    if data not already epoched:
+        0.1) the data is filtered with filters specified in low_pass and high_pass. Parameters of the filter are
         determined by MNE's filter function.
-    2) if no events is provided, detect events in stumulus channel and keep events with id in event_id and resp_id.
-    3) eventual downsampling is performed if sfreq is lower than the data's sampling frequency. The event structure is
+        0.2) if no events is provided, detect events in stumulus channel and keep events with id in event_id and resp_id.
+        0.3) eventual downsampling is performed if sfreq is lower than the data's sampling frequency. The event structure is
         passed at the resample() function of MNE to ensure that events are approriately timed after downsampling.
-    4) epochs are created based on stimulus onsets (event_id) and tmin and tmax. Epoching removes any epoch where a 
+        0.4) epochs are created based on stimulus onsets (event_id) and tmin and tmax. Epoching removes any epoch where a 
         'BAD' annotiation is present and all epochs where an electrode exceeds reject_threshold. Epochs are baseline 
-        corrected from tmin to stimulus onset (time 0).
-    5) Reaction times (RT) are computed based on the sample difference between onset of stimulus and response triggers. 
+        corrected from tmin to stimulus onset (time 0).)
+    1) Reaction times (RT) are computed based on the sample difference between onset of stimulus and response triggers. 
         If no response event happens after a stimulus or if RT > upper_limit_RT & < upper_limit_RT, RT is 0.
-    6) all the non-rejected epochs with positive RTs are cropped to stimulus onset to stimulus_onset + RT.
+    2) all the non-rejected epochs with positive RTs are cropped to stimulus onset to stimulus_onset + RT.
     
     Parameters
     ----------
     pfiles : str or list
-        list of EEG files to read154,
+        list of EEG files to read,
     event_id : dict
         Dictionary containing the correspondance of named condition [keys] and event code [values]
     resp_id : dict
         Dictionary containing the correspondance of named response [keys] and event code [values]
     sfreq : float
         Desired sampling frequency
     to_merge_id: dict
@@ -74,136 +87,173 @@
         Time values to compute the baseline and substract to epoch data (usually some time before stimulus onset)
     upper_limit_RT : float
         Upper limit for RTs. Longer RTs are discarded
     lower_limit_RT : float
         Lower limit for RTs. Shorter RTs are discarded
     reject_threshold : float
         Rejection threshold to apply when creating epochs, expressed in microvolt
-    
+    scale: float
+        Scale to apply to the RT data (e.g. 1000 if ms)
         
     Returns
     -------
     epoch_data : xarray
         Returns an xarray Dataset with all the data, events, electrodes, participant. 
         All eventual participant/electrodes naming and epochs index are kept. 
         The choosen sampling frequnecy is stored as attribute.
     '''
     import mne
-    tstep = 1/sfreq
+    dict_datatype = {False:'continuous', True:'epoched'}
     epoch_data = [] 
     if isinstance(pfiles,str):#only one participant
         pfiles = [pfiles]
     if not subj_idx:
         subj_idx = ["S"+str(x) for x in np.arange(len(pfiles))]
+    if isinstance(subj_idx,str):
+        subj_idx = [subj_idx]
     y = 0
+    metadata_i = None
     for participant in pfiles:
-        print(f'Processing participant {participant}')
-        if '.fif' in participant:
-            data = mne.io.read_raw_fif(participant, preload=False, verbose=verbose)
-        elif '.bdf' in participant:
-            data = mne.io.read_raw_bdf(participant, preload=False, verbose=verbose)
-        else:
-            raise ValueError(f'Unknown EEG file format for participant {participant}')
-        # Loading events (in our case one event = one trial)
-        if sfreq is None: 
-            sfreq = data.info['sfreq']
-        if events_provided is None:
-            try:
-                events = mne.find_events(data, verbose=verbose, min_duration = 1 / data.info['sfreq'])
-            except:
-                events = mne.events_from_annotations(data, verbose=verbose)
-            if events[0,1] > 0:#bug from some stim channel, should be 0 otherwise indicates offset in the trggers
-                print(f'Correcting event values as trigger channel has offset {np.unique(events[:,1])}')
-                events[:,2] = events[:,2]-events[:,1]#correction on event value                
-            events_values = np.concatenate([np.array([x for x in event_id.values()]), np.array([x for x in resp_id.values()])])
-            events = np.array([list(x) for x in events if x[2] in events_values])#only keeps events with stim or response
-        else:
-            if len(np.shape(events_provided)) == 2:
-                events_provided = events_provided[np.newaxis]
-            events = events_provided[y]
-
-        if isinstance(pick_channels, list):
-               try:
-                    data = data.pick_channels(pick_channels)
-               except:
-                    raise ValueError('incorrect electrode pick specified')
-        elif pick_channels == 'eeg':
-                data = data.pick_types(meg=False, eeg=True, stim=False, eog=False, misc=False, exclude='bads') 
-        else:
-             raise ValueError('incorrect electrode pick specified')
-    
-
-        data.load_data()
-        data.filter(high_pass, low_pass, fir_design='firwin', verbose=verbose)#Filtering out frequency outside range .5 and 30Hz, as study by Anderson et al.
-
-        if sfreq < data.info['sfreq']:#Downsampling
-            print(f'Downsampling to {sfreq} Hz')
-            data, events = data.resample(sfreq, events=events)#100 Hz is the standard used for previous applications of HsMM
-        
-        print(f'Creating epochs based on following event ID :{np.unique(events[:,2])}')
+        if metadata_i is not None:
+            metadata = None#avoids confusion of metadata infered for prev_subj
+        print(f"Processing participant {participant}'s {dict_datatype[epoched]} {pick_channels}")
+
+        # loading data
+        if epoched == False:# performs epoching on raw data
+            if '.fif' in participant:
+                data = mne.io.read_raw_fif(participant, preload=False, verbose=verbose)
+            elif '.bdf' in participant:
+                data = mne.io.read_raw_bdf(participant, preload=False, verbose=verbose)
+            else:
+                raise ValueError(f'Unknown EEG file format for participant {participant}')
+            data = _pick_channels(pick_channels,data, stim=True)
+            if sfreq is None: 
+                sfreq = data.info['sfreq']
+
+            if 'response' not in list(resp_id.keys())[0]:
+                resp_id = {f'response/{k}': v for k, v in resp_id.items()}
+            if events_provided is None:
+                try:
+                    events = mne.find_events(data, verbose=verbose, min_duration = 1 / data.info['sfreq'])
+                except:
+                    events = mne.events_from_annotations(data, verbose=verbose)
+                if events[0,1] > 0:#bug from some stim channel, should be 0 otherwise indicates offset in the trggers
+                    print(f'Correcting event values as trigger channel has offset {np.unique(events[:,1])}')
+                    events[:,2] = events[:,2]-events[:,1]#correction on event value                
+                events_values = np.concatenate([np.array([x for x in event_id.values()]), np.array([x for x in resp_id.values()])])
+                events = np.array([list(x) for x in events if x[2] in events_values])#only keeps events with stim or response
+                events_stim = np.array([list(x) for x in events if x[2] in event_id.values()])#only stim
+            else:
+                if len(np.shape(events_provided)) == 2:
+                    events_provided = events_provided[np.newaxis]
+                events = events_provided[y]
+
+            data.load_data()
+            data.filter(high_pass, low_pass, fir_design='firwin', verbose=verbose)
+
+            if sfreq < data.info['sfreq']:#Downsampling
+                print(f'Downsampling to {sfreq} Hz')
+                data, events = data.resample(sfreq, events=events)
+            combined =  {**event_id, **resp_id}#event_id | resp_id 
+            stim = list(event_id.keys())
             
-        offset_after_resp_samples = int(offset_after_resp/tstep)
-        metadata, meta_events, event_id = mne.epochs.make_metadata(
-            events=events, event_id= event_id,
-            tmin=tmin, tmax=tmax, sfreq=data.info['sfreq'])
-        epochs = mne.Epochs(data, meta_events, event_id, tmin, tmax, proj=False,
-                        baseline=baseline, preload=True,
-                        verbose=verbose,detrend=1, on_missing = 'warn', event_repeated='drop',
-                        metadata=metadata, reject_by_annotation=True, reject=reject_threshold)
-        data_epoch = epochs.get_data()
-
-        valid_epochs_idx = [x for x in np.arange(len(epochs.drop_log)) if epochs.drop_log[x] == ()]
-        correct_stim_timing  = np.array([list(x) for x in events if x[2] in event_id.values()])[valid_epochs_idx,0]
-        stim_events = np.array([x for x in np.arange(len(events)) if events[x,0] in correct_stim_timing])
-        rts=[]#reaction times
-        trigger = []
-        without_rt = 0
-        for i in stim_events:
-            if any(x in resp_id.values() for x in events[i:,2]) and events[i+1,2] in resp_id.values():
-                rts.append(events[i+1,0] - events[i,0] )
+            if verbose:
+                print(f'Creating epochs based on following event ID :{np.unique(events[:,2])}')
 
+            offset_after_resp_samples = int(offset_after_resp*sfreq)
+            if metadata is None:
+                metadata_i, meta_events, event_id = mne.epochs.make_metadata(
+                    events=events, event_id=combined, tmin=tmin, tmax=tmax,
+                    sfreq=data.info["sfreq"], row_events=stim, keep_first=["response"])
+                metadata_i = metadata_i[["event_name","response"]]#only keep event_names and rts
+            epochs = mne.Epochs(data, meta_events, event_id, tmin, tmax, proj=False,
+                    baseline=baseline, preload=True, picks=pick_channels,
+                    verbose=verbose, detrend=1, on_missing = 'warn', event_repeated='drop',
+                    metadata=metadata_i, reject_by_annotation=True, reject=reject_threshold)
+            epochs.metadata.rename({'response':'rt'}, axis=1, inplace=True)
+            rts = epochs.metadata.rt
+        else:
+            if '.fif' in participant:
+                epochs = mne.read_epochs(participant, preload=True, verbose=verbose)
+                if sfreq is None: 
+                    sfreq = epochs.info['sfreq']
+                elif sfreq  < epochs.info['sfreq']:
+                    if verbose:
+                        print(f'Resampling data at {sfreq}')
+                    epochs = epochs.resample(sfreq)
             else:
-                rts.append(0)
-                without_rt += 1
-        print(f'N trials without response event: {without_rt}')
-        rts = np.array(rts)
-        print(f'Applying reaction time trim to keep RTs between {lower_limit_RT} and {upper_limit_RT} seconds')
-        rts[rts > sfreq*upper_limit_RT] = 0 #removes RT above x sec
-        rts[rts < sfreq*lower_limit_RT] = 0 #removes RT below x sec, important as determines max bumps
-        print(f'{len(rts[rts > 0])} RTs kept of {len(stim_events)} clean epochs')
-        triggers = epochs.metadata["event_name"].reset_index(drop=True)
-        cropped_data_epoch = np.empty([len(rts[rts> 0]), len(epochs.ch_names), max(rts)+offset_after_resp_samples])
+                raise ValueError('Incorrect file format')
+            _pick_channels(pick_channels,epochs, stim=False)
+            if metadata is not None and not isinstance(metadata, pd.DataFrame):
+                raise ValueError('Metadata should be a pandas data-frame as generated by mne')
+            metadata = epochs.metadata#accounts for dropped epochs
+        offset_after_resp_samples = np.rint(offset_after_resp*sfreq).astype(int)
+        valid_epoch_index = [x for x,y in enumerate(epochs.drop_log) if len(y) == 0]
+        data_epoch = epochs.get_data()#preserves index
+        if isinstance(metadata, pd.DataFrame):
+            if len(metadata) > len(data_epoch):#assumes metadata contains rejected epochs
+                metadata = metadata.iloc[valid_epoch_index]
+                metadata.reset_index(drop=True, inplace=True)
+            try:
+                rts = metadata[rt_col]/scale
+            except:
+                raise ValueError(f'Expected column named {rt_col} in the provided metadata file, alternative names can be passed through the rt_col parameter')
+        elif rts is None:
+            raise ValueError(f'Expected either a metadata Dataframe or an array of Reaction Times')
+        rts_arr = np.array(rts)
+        if verbose:
+            print(f'Applying reaction time trim to keep RTs between {lower_limit_RT} and {upper_limit_RT} seconds')
+        rts_arr[rts_arr > upper_limit_RT] = 0 #removes RT above x sec
+        rts_arr[rts_arr < lower_limit_RT] = 0 #removes RT below x sec, important as determines max events
+        rts_arr[np.isnan(rts_arr)] = 0#too long trial
+        rts_arr = np.rint(rts_arr*sfreq).astype(int)
+        if verbose:
+            print(f'{len(rts_arr[rts_arr > 0])} RTs kept of {len(rts_arr)} clean epochs')
+        triggers = epochs.metadata.iloc[:,0].values#assumes first col is trigger
+        cropped_data_epoch = np.empty([len(rts_arr[rts_arr>0]), len(epochs.ch_names), max(rts_arr)+offset_after_resp_samples])
         cropped_data_epoch[:] = np.nan
         cropped_trigger = []
         epochs_idx = []
         j = 0
-        for i in np.arange(len(data_epoch)):
-            if rts[i] > 0:
+        time0 = epochs.time_as_index(0)[0]
+        for i in range(len(data_epoch)):
+            if rts_arr[i] > 0:
                 cropped_trigger.append(triggers[i])
             #Crops the epochs to time 0 (stim onset) up to RT
-                cropped_data_epoch[j,:,:rts[i]+offset_after_resp_samples] = \
-                (data_epoch[i,:,epochs.time_as_index(0)[0]:\
-                epochs.time_as_index(0)[0]+int(rts[i])+offset_after_resp_samples])
-                epochs_idx.append(valid_epochs_idx[j])
+                cropped_data_epoch[j,:,:rts_arr[i]+offset_after_resp_samples] = \
+                (data_epoch[i,:,time0:time0+rts_arr[i]+offset_after_resp_samples])
+                epochs_idx.append(valid_epoch_index[i])#Keeps trial number
                 j += 1
         x = 0
-        while np.isnan(cropped_data_epoch[-1]).all():#Weird bug I guess it is perhps due to too long epoch?
+        while np.isnan(cropped_data_epoch[-1]).all():#Weird bug I guess it is perhps due to too long last epoch? update: cannot reproduce
             cropped_data_epoch = cropped_data_epoch[:-1]
             x += 1
         if x > 0:
             print(f'RTs > 0 longer than expected ({x})')
         print(f'{len(cropped_data_epoch)} trials were retained for participant {participant}')
-        print(f'End sampling frequency is {sfreq} Hz')
-        epoch_data.append(hsmm_data_format(cropped_data_epoch, cropped_trigger, epochs.info['sfreq'], offset_after_resp_samples, epochs=[int(x) for x in epochs_idx], electrodes = epochs.ch_names))
+        if verbose:
+            print(f'End sampling frequency is {sfreq} Hz')
+        epoch_data.append(hmp_data_format(cropped_data_epoch, cropped_trigger, epochs.info['sfreq'], offset_after_resp_samples, epochs=[int(x) for x in epochs_idx], electrodes = epochs.ch_names, metadata = metadata))
         y += 1
-        
     epoch_data = xr.concat(epoch_data, dim = xr.DataArray(subj_idx, dims='participant'),
                           fill_value={'event':'', 'data':np.nan})
     return epoch_data
 
+def _pick_channels(pick_channels,data,stim=True):
+    if isinstance(pick_channels, list):
+        try:
+            data = data.pick_channels(pick_channels)
+        except:
+            raise ValueError('incorrect electrode pick specified')
+    elif pick_channels == 'eeg':
+            data = data.pick_types(meg=False, eeg=True, stim=stim, eog=False, misc=False, exclude='bads') 
+    else:
+         raise ValueError('incorrect electrode pick specified')
+    return data
+
 def parsing_epoched_eeg(data, rts, conditions, sfreq, start_time=0, offset_after_resp=0.1):
     '''
     Function to parse epochs and crop them to start_time (usually stimulus onset so 0) up to the reaction time of the trial.
     The returned object is a xarray Dataset allowing further processing using built-in methods
 
     Importantly 
     1) if you are considering some lower or upper limit on the RTs you should replace values outside of these ranges
@@ -283,18 +333,18 @@
     j = 0
     for epoch in np.arange(len(data)):
         #Crops the epochs up to RT
         cropped_data_epoch[j,:,:rts[epoch]+offset_after_resp_samples] = \
         (data[epoch,:,:rts[epoch]+offset_after_resp_samples])
         j += 1
     print(f'Totaling {len(cropped_data_epoch)} valid trials')
-    data_xr = hsmm_data_format(cropped_data_epoch, conditions, sfreq, offset_after_resp_samples, epochs=epochs, electrodes = electrode_columns)
+    data_xr = hmp_data_format(cropped_data_epoch, conditions, sfreq, offset_after_resp_samples, epochs=epochs, electrodes = electrode_columns)
     return data_xr
 
-def hsmm_data_format(data, events, sfreq, offset=0, participants=[], epochs=None, electrodes=None):
+def hmp_data_format(data, events, sfreq, offset=0, participants=[], epochs=None, electrodes=None, metadata=None):
     '''
     Converting 3D matrix with dimensions (participant) * trials * electrodes * sample into xarray Dataset
     
     Parameters
     ----------
     data : ndarray
         4/3D matrix with dimensions (participant) * trials * electrodes * sample  
@@ -322,37 +372,40 @@
         electrodes = np.arange(n_electrodes)
     if epochs is None:
          epochs = np.arange(n_epochs)
     if len(participants) < 2:
         data = xr.Dataset(
                 {
                     "data": (["epochs", "electrodes", "samples"],data),
-                    "event": (["epochs"], events),
                 },
                 coords={
                     "epochs" :epochs,
                     "electrodes":  electrodes,
                     "samples": np.arange(n_samples)
                 },
                 attrs={'sfreq':sfreq,'offset':offset}
                 )
     else:
         data = xr.Dataset(
                 {
                     "data": (['participant',"epochs", "electrodes", "samples"],data),
-                    "event": (['participant',"epochs"], events),
                 },
                 coords={
                     'participant':participants,
                     "epochs" :epochs,
                     "electrodes":  electrodes,
                     "samples": np.arange(n_samples)
                 },
                 attrs={'sfreq':sfreq,'offset':offset}
                 )
+    if metadata is not None:
+        metadata = metadata.to_xarray()
+        metadata = metadata.rename_dims({'index':'epochs'})
+        metadata = metadata.rename_vars({'index':'epochs'})
+        data = data.merge(metadata)
     return data
 
 def standardize(x):
     '''
     Scaling variances to mean variance of the group
     '''
     return ((x.data / x.data.std(dim=...))*x.mean_std)
@@ -400,15 +453,15 @@
         data = data.expand_dims("participant")
     data = data.stack(all_samples=['participant','epochs',"samples"]).dropna(dim="all_samples")
     return data #xr.Dataset({'data':data, 'durations':durations})
     #return data, durations
 
 def transform_data(data, subjects_variable="participant", apply_standard=True,  apply_zscore=True, method='pca', n_comp=None, return_weights=False):
     '''
-    Adapts EEG epoched data (in xarray format) to the expected data format for hsmms. 
+    Adapts EEG epoched data (in xarray format) to the expected data format for hmps. 
     First this code can apply standardization of individual variances (if apply_standard=True).
     Second, a spatial PCA on the average variance-covariance matrix is performed (if method='pca', more methods in development)
     Third,stacks the data going from format [participant * epochs * samples * electrodes] to [samples * electrodes]
     Last, performs z-scoring on each epoch and for each principal component (PC)
     
     
     Parameters
@@ -435,14 +488,16 @@
     pca_data : xarray.Dataset
         loadings of the PCA, used to retrieve electrode space
     pca.explained_variance_ : ndarray
         explained variance for each component
     means : xarray.DataArray
         means of the electrodes before PCA/zscore
     '''
+    if isinstance(data, xr.DataArray):
+        raise ValueError('Expected a xarray Dataset with data and event as DataArrays, check the data format')
     if apply_standard:
         mean_std = data.groupby(subjects_variable).std(dim=...).data.mean()
         data = data.assign(mean_std=mean_std.data)
         data = data.groupby(subjects_variable).map(standardize)
     if method == 'pca':
         from sklearn.decomposition import PCA
         var_cov_matrices = []
@@ -490,234 +545,234 @@
         data = stack_data(data)
     if return_weights:
         return data, pca_data, pca.explained_variance_, means
     else:
         return data
     
 
-def LOOCV(data, subject, n_bumps, initial_fit, sfreq, bump_width=50):
+def LOOCV(data, subject, n_events, initial_fit, sfreq, event_width=50):
     '''
-    Performs Leave-one-out cross validation, removes one participant from data, estimate n_bumps HsMM parameters, 
+    Performs Leave-one-out cross validation, removes one participant from data, estimate n_events HMP parameters, 
     compute the likelihood of the data from the left out participant with the estimated parameters. The model is fit
     using initial fit as starting points for magnitudes and parameters
     
     
     Parameters
     ----------
     data : xarray.Dataset
         xarray data from transform_data() 
     subject : str
         name of the subject to remove
-    n_bumps : int 
-        How many bumps in the model
+    n_events : int 
+        How many events in the model
     initial_fit : xarray.Dataset
-        Fit of the model with the same number of bumps and all participants
+        Fit of the model with the same number of events and all participants
     sfreq : float
         Sampling frequency of the data
-    bump_width : float
-        length of the bumps in milliseconds
+    event_width : float
+        length of the events in milliseconds
     
     Returns
     -------
     likelihood : float
         likelihood computed for the left-out participant
     subject : str
         name of the subject to remove
     '''
-    # warn('This method is deprecated and will be removed in future version, use loocv() instead', DeprecationWarning, stacklevel=2) 
-    from hsmm_mvpy.models import hsmm
-    #Looping over possible number of bumps
+    # wc 
+    from hsmm_mvpy.models import hmp
+    #Looping over possible number of events
     subjects_idx = data.participant.values
     likelihoods_loo = []
     #Extracting data without left out subject
     stacked_loo = stack_data(data.sel(participant= subjects_idx[subjects_idx!=subject],drop=False))
-    #Fitting the HsMM using previous estimated parameters as initial parameters
-    model_loo = hsmm(stacked_loo, sfreq=sfreq, bump_width=bump_width)
-    fit = model_loo.fit_single(n_bumps, initial_fit.magnitudes.dropna('bump').values, initial_fit.parameters, 1, verbose=False)
+    #Fitting the HMP using previous estimated parameters as initial parameters
+    model_loo = hmp(stacked_loo, sfreq=sfreq, event_width=event_width)
+    fit = model_loo.fit_single(n_events, initial_fit.magnitudes.dropna('event').values, initial_fit.parameters, 1, verbose=False)
     #Evaluating likelihood for left out subject
     #Extracting data of left out subject
     stacked_left_out = stack_data(data.sel(participant=subject, drop=False))
-    model_left_out = hsmm(stacked_left_out, sfreq=sfreq, bump_width=bump_width)
-    likelihood = model_left_out.estim_probs(fit.magnitudes.dropna('bump').values, fit.parameters, n_bumps,True)
+    model_left_out = hmp(stacked_left_out, sfreq=sfreq, event_width=event_width)
+    likelihood = model_left_out.estim_probs(fit.magnitudes.dropna('event').values, fit.parameters, n_events,True)
     return likelihood, subject
 
-def loocv_estimation(data, subject, sfreq, bump_width):
+def loocv_estimation(data, subject, sfreq, event_width):
     '''
-    Performs Leave-one-out cross validation, removes one participant from data, estimate n_bumps HsMM parameters, 
+    Performs Leave-one-out cross validation, removes one participant from data, estimate n_events HMP parameters, 
     compute the likelihood of the data from the left out participant with the estimated parameters. The model is fit
     using initial fit as starting points for magnitudes and parameters
     
     
     Parameters
     ----------
     data : xarray
         xarray data from transform_data() 
     subject : str
         name of the subject to remove
     sfreq : float
         Sampling frequency of the data
-    bump_width : float
-        length of the bumps in milliseconds
+    event_width : float
+        length of the events in milliseconds
     
     Returns
     -------
     likelihood : float
         likelihood computed for the left-out participant
     subject : str
         name of the subject to remove
     '''    
     print(f'Leaving out participant #{subject}')
-    from hsmm_mvpy.models import hsmm
-    #Looping over possible number of bumps
+    from hsmm_mvpy.models import hmp
+    #Looping over possible number of events
     subjects_idx = data.participant.values
     likelihoods_loo = []
     #Extracting data without left out subject
     stacked_loo = stack_data(data.sel(participant= subjects_idx[subjects_idx!=subject],drop=False))
-    #Fitting the HsMM using previous estimated parameters as initial parameters
-    model_loo = hsmm(stacked_loo, sfreq=sfreq, bump_width=bump_width, cpus=1)
-    parameters, magnitudes, likelihoods = model_loo.sliding_bump(verbose=False)
+    #Fitting the HMP using previous estimated parameters as initial parameters
+    model_loo = hmp(stacked_loo, sfreq=sfreq, event_width=event_width, cpus=1)
+    parameters, magnitudes, likelihoods = model_loo.sliding_event(verbose=False)
     estimates = model_loo.iterative_fit(likelihoods=likelihoods, parameters=parameters, magnitudes=magnitudes)
     #Evaluating likelihood for left out subject
     #Extracting data of left out subject
     stacked_left_out = stack_data(data.sel(participant=subject, drop=False))
-    model_left_out = hsmm(stacked_left_out, sfreq=sfreq, bump_width=bump_width, cpus=1)
-    n_bumps = int(estimates.dropna('n_bumps',how='all').n_bumps.max())
-    for n_bump in range(1,n_bumps+1):
-        likelihoods_loo.append( model_left_out.calc_EEG_50h(estimates.sel(n_bumps=n_bump).magnitudes.dropna('bump').values, estimates.sel(n_bumps=n_bump).parameters.dropna('stage').values, n_bump, True))
+    model_left_out = hmp(stacked_left_out, sfreq=sfreq, event_width=event_width, cpus=1)
+    n_events = int(estimates.dropna('n_events',how='all').n_events.max())
+    for n_event in range(1,n_events+1):
+        likelihoods_loo.append( model_left_out.calc_EEG_50h(estimates.sel(n_events=n_event).magnitudes.dropna('event').values, estimates.sel(n_events=n_event).parameters.dropna('stage').values, n_event, True))
     return likelihoods_loo, subject
 
-def loocv(stacked_data,sfreq, max_bump, cpus=1, bump_width=50):
+def loocv(stacked_data,sfreq, max_event, cpus=1, event_width=50):
     '''
-    Performs Leave-one-out cross validation, removes one participant from data, estimate n_bumps HsMM parameters, 
+    Performs Leave-one-out cross validation, removes one participant from data, estimate n_events HMP parameters, 
     compute the likelihood of the data from the left out participant with the estimated parameters. The model is fit
     using initial fit as starting points for magnitudes and parameters
     
     
     Parameters
     ----------
     data : xarray.Dataset
         xarray data from transform_data() 
     initial_fit : xarray.Dataset
-        Fit of the model with the same number of bumps and all participants
+        Fit of the model with the same number of events and all participants
     sfreq : float
         Sampling frequency of the data
-    bump_width : float
-        length of the bumps in milliseconds
+    event_width : float
+        length of the events in milliseconds
     
     Returns
     -------
     loocv
     '''
     unstacked_data = stacked_data.unstack()
-    #Looping over possible number of bumps
+    #Looping over possible number of events
     participants = unstacked_data.participant.data
     likelihoods_loo = []
     loocv = []
     if cpus>1:
         import multiprocessing
         with multiprocessing.Pool(processes=cpus) as pool:
             loo = pool.starmap(loocv_estimation, 
-                zip(itertools.repeat(unstacked_data), participants, itertools.repeat(sfreq), itertools.repeat(bump_width)))
+                zip(itertools.repeat(unstacked_data), participants, itertools.repeat(sfreq), itertools.repeat(event_width)))
         loocv.append(loo)
     else:
         loo = []
         for participant in participants:
-            loo.append(loocv_estimation(unstacked_data, participant,sfreq, bump_width))
+            loo.append(loocv_estimation(unstacked_data, participant,sfreq, event_width))
         loocv.append(loo)
-    loocv_arr = np.tile(np.nan, (max_bump, len(participants)))
+    loocv_arr = np.tile(np.nan, (max_event, len(participants)))
     par_arr = np.repeat(np.nan, len(participants))
     for idx, values in enumerate(loocv[0]):
         par_arr[idx] = np.array(values[-1])
         values = np.array(values[:-1][0])
         loocv_arr[:len(values), idx] = values 
-    loocv = xr.DataArray(loocv_arr, coords={"n_bump":np.arange(1,max_bump+1),
+    loocv = xr.DataArray(loocv_arr, coords={"n_event":np.arange(1,max_event+1),
                                                            "participants":par_arr}, name="loo_likelihood")
     return loocv
 
 
 def loocv_mp(init, stacked_data, bests, func=LOOCV, cpus=2, verbose=True):
     '''
     multiprocessing wrapper for LOOCV()
     
     Parameters
     ----------
-    init : hsmm.model
-        initialized hsmm model
+    init : hmp.model
+        initialized hmp model
     data : xarray.Dataset
         xarray data from transform_data() , can also be a subset, e.g. based on conditions
     bests : xarray.Dataset
-        Fit from all possible n bump solution
+        Fit from all possible n event solution
     
     Returns
     -------
     loocv
     '''
     # warn('This method is deprecated and will be removed in future version, use loocv() instead', DeprecationWarning, stacklevel=2) 
     unstacked_data = stacked_data.unstack()
     import multiprocessing
     import itertools
     participants = unstacked_data.participant.data
     likelihoods_loo = []
     loocv = []
-    for n_bumps in bests.n_bumps.values:
+    for n_events in bests.n_events.values:
         if verbose:
-            print(f'LOOCV for model with {n_bumps} bump(s)')
+            print(f'LOOCV for model with {n_events} event(s)')
         with multiprocessing.Pool(processes=cpus) as pool:
             loo = pool.starmap(func, 
-                zip(itertools.repeat(unstacked_data), participants, itertools.repeat(n_bumps), 
-                    itertools.repeat(bests.sel(n_bumps=n_bumps)), itertools.repeat(init.sfreq)))
+                zip(itertools.repeat(unstacked_data), participants, itertools.repeat(n_events), 
+                    itertools.repeat(bests.sel(n_events=n_events)), itertools.repeat(init.sfreq)))
         loocv.append(loo)
 
-    loocv = xr.DataArray(np.array(loocv)[:,:,0].astype(np.float64), coords={"n_bump":np.arange(1,bests.n_bumps.max().values+1),
+    loocv = xr.DataArray(np.array(loocv)[:,:,0].astype(np.float64), coords={"n_event":np.arange(1,bests.n_events.max().values+1)[::-1],
                                                            "participants":np.array(loocv)[0,:,1]}, name="loo_likelihood")
     return loocv
 
 def reconstruct(magnitudes, PCs, eigen, means):
     '''
     Reconstruct electrode activity from PCA
     
     Parameters
     ----------
     magnitudes :  
-        2D or 3D ndarray with [n_components * n_bumps] can also contain several estimations [estimation * n_components * n_bumps]
+        2D or 3D ndarray with [n_components * n_events] can also contain several estimations [estimation * n_components * n_events]
     PCs : 
         2D ndarray with PCA loadings [channels x n_components]
     eigen : 
         PCA eigenvalues of the covariance matrix of data [n_components]
     means : 
         Grand mean [channels]
         
     Returns
     -------
     electrodes : ndarray
-        a 2D ndarray with [electrodes * bumps]
+        a 2D ndarray with [electrodes * events]
     '''
     if len(np.shape(magnitudes))==2:
         magnitudes = np.array([magnitudes])
-    n_iter, n_comp, n_bumps = np.shape(magnitudes)
+    n_iter, n_comp, n_events = np.shape(magnitudes)
     list_electrodes = []
     for iteration in np.arange(n_iter): 
         #electrodes = np.array(magnitudes[iteration].T * 
-        electrodes =  np.array(magnitudes[iteration, ].T * np.tile(np.sqrt(eigen[:n_comp]).T, (n_bumps,1))) @ np.array(PCs[:,:n_comp]).T
-        list_electrodes.append(electrodes + np.tile(means,(n_bumps,1)))#add means for each electrode
+        electrodes =  np.array(magnitudes[iteration, ].T * np.tile(np.sqrt(eigen[:n_comp]).T, (n_events,1))) @ np.array(PCs[:,:n_comp]).T
+        list_electrodes.append(electrodes + np.tile(means,(n_events,1)))#add means for each electrode
     return np.array(list_electrodes)
 
 def stage_durations(times):
     '''
-    Returns the stage durations from the bump onset times by substracting each stage to the previous
+    Returns the stage durations from the event onset times by substracting each stage to the previous
     
     Parameters
     ----------
     times : ndarray
-        2D ndarray with [n_trials * n_bumps]
+        2D ndarray with [n_trials * n_events]
     
     Returns
     -------
     times : ndarray
-        2D ndarray with [n_trials * n_bumps]
+        2D ndarray with [n_trials * n_events]
     '''
     times = np.diff(times, axis=1, prepend=0)
     return times
 
 def save_fit(data, filename):
     '''
     Save fit
@@ -740,82 +795,85 @@
     '''
     eventprobs = eventprobs.unstack()
     eventprobs.to_dataframe().to_csv(filename)
     print(f"Saved at {filename}")
 
 def event_times(data, times, electrode, stage):
     '''
-    Event times parses the single trial EEG signal of a given electrode in a given stage, from bump onset to the next one. If requesting the last
-    stage it is defined as the onset of the last bump until the response of the participants.
+    Event times parses the single trial EEG signal of a given electrode in a given stage, from event onset to the next one. If requesting the last
+    stage it is defined as the onset of the last event until the response of the participants.
 
     Parameters
     ----------
     data : xr.Dataset
-        HsMM EEG data (untransformed but with trial and participant stacked)
+        HMP EEG data (untransformed but with trial and participant stacked)
     times : xr.DataArray
         Onset times as computed using onset_times()
     electrode : str
         Electrode to pick for the parsing of the signal
     stage : float | ndarray
         Which stage to parse the signal into
 
     Returns
     -------
     brp_data : ndarray
         Matrix with trial_x_participant * samples with sample dimension given by the maximum stage duration
     '''
 
-    brp_data = np.tile(np.nan, (len(data.trial_x_participant), int(round(max(times.sel(bump=stage+1).data- times.sel(bump=stage).data)))+1))
+    brp_data = np.tile(np.nan, (len(data.trial_x_participant), int(round(max(times.sel(event=stage+1).data- times.sel(event=stage).data)))+1))
     i=0
     for trial, trial_dat in data.groupby('trial_x_participant'):
-        trial_time = slice(times.sel(bump=stage, trial_x_participant=trial), \
-                                                 times.sel(bump=stage+1, trial_x_participant=trial))
+        trial_time = slice(times.sel(event=stage, trial_x_participant=trial), \
+                                                 times.sel(event=stage+1, trial_x_participant=trial))
         trial_elec = trial_dat.sel(electrodes = electrode, samples=trial_time).squeeze()
         try:
             brp_data[i, :len(trial_elec)] = trial_elec
         except:
             brp_data[i, :1] = trial_elec
             
         i += 1
 
     return brp_data    
     
-def condition_selection(hsmm_data, eeg_data, condition_string):
-    unstacked = hsmm_data.unstack().where(eeg_data.event.str.contains(condition_string),drop=True)
+def condition_selection(hmp_data, eeg_data, condition_string, variable='event'):
+    unstacked = hmp_data.unstack().where(eeg_data[variable].str.contains(condition_string),drop=True)
     stacked = stack_data(unstacked)
     return stacked
 
+def load_data(path):
+    return xr.load_dataset(path)
+
     
-def participant_selection(hsmm_data, eeg_data, participant):
-    unstacked = hsmm_data.unstack().sel(participant = participant)
+def participant_selection(hmp_data, eeg_data, participant):
+    unstacked = hmp_data.unstack().sel(participant = participant)
     stacked = stack_data(unstacked)
     return stacked
 
-def bootstrapping(init, hsmm_data, general_run, positions, eeg_data, iterations, threshold=1, verbose=True, plots=True, cpus=1):
-    from hsmm_mvpy.models import hsmm
+def bootstrapping(init, hmp_data, general_run, positions, eeg_data, iterations, threshold=1, verbose=True, plots=True, cpus=1):
+    from hsmm_mvpy.models import hmp
     from hsmm_mvpy.visu import plot_topo_timecourse
     import xskillscore as xs
     fitted_mags = general_run.magnitudes.values[np.unique(np.where(np.isfinite(general_run.magnitudes))[0]),:]#remove NAs
-    mags_boot_mat = np.tile(np.nan, (iterations, init.compute_max_bumps(), init.n_dims))
-    pars_boot_mat = np.tile(np.nan, (iterations, init.compute_max_bumps()+1, 2))
+    mags_boot_mat = np.tile(np.nan, (iterations, init.compute_max_events(), init.n_dims))
+    pars_boot_mat = np.tile(np.nan, (iterations, init.compute_max_events()+1, 2))
 
     for i in range(iterations):
-        bootstapped = xs.resample_iterations(hsmm_data.unstack(), iterations=1, dim='epochs')
-        hsmm_data_boot = stack_data(bootstapped.squeeze())
-        init_boot = hsmm(hsmm_data_boot, sfreq=eeg_data.sfreq, bump_width=50, cpus=15)
+        bootstapped = xs.resample_iterations(hmp_data.unstack(), iterations=1, dim='epochs')
+        hmp_data_boot = stack_data(bootstapped.squeeze())
+        init_boot = hmp(hmp_data_boot, sfreq=eeg_data.sfreq, event_width=50, cpus=15)
         estimates_boot = init_boot.fit(verbose=verbose, threshold=1)
         mags_boot_mat[i, :len(estimates_boot.magnitudes),:] = estimates_boot.magnitudes
         pars_boot_mat[i, :len(estimates_boot.parameters),:] = estimates_boot.parameters
         if plots:
             plot_topo_timecourse(eeg_data, estimates_boot, positions, init_boot)
 
     all_pars_aligned = np.tile(np.nan, (iterations, np.max([len(x) for x in pars_boot_mat]), 2))
     all_mags_aligned = np.tile(np.nan, (iterations, np.max([len(x) for x in mags_boot_mat]), init.n_dims))
     for iteration, _i in enumerate(zip(pars_boot_mat, mags_boot_mat)):
         all_pars_aligned[iteration, :len(_i[0]), :] = _i[0]
         all_mags_aligned[iteration, :len(_i[1]), :] = _i[1]
 
     booted = xr.Dataset({'parameters': (('iteration', 'stage','parameter'), 
                                  all_pars_aligned),
-                        'magnitudes': (('iteration', 'bump','component'), 
+                        'magnitudes': (('iteration', 'event','component'), 
                                  all_mags_aligned)})
     return booted
```

### Comparing `hsmm_mvpy-0.1.0a2/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/visu.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,38 +8,38 @@
 default_colors =  ['cornflowerblue','indianred','orange','darkblue','darkgreen','gold']
 
 def plot_topo_timecourse(electrodes, estimated, channel_position, init, time_step=1, ydim=None,
                         figsize=None, dpi=100, magnify=1, times_to_display=None, cmap='Spectral_r',
                         ylabels=[], max_time = None, vmin=None, vmax=None, title=False, ax=False, 
                         sensors=False, skip_electrodes_computation=False):
     '''
-    Plotting the bump topologies at the average time of the end of the previous stage.
+    Plotting the event topologies at the average time of the end of the previous stage.
     
     Parameters
     ----------
     electrodes : ndarray | xr.Dataarray 
-        a 2D or 3D matrix of electrode activity with electrodes and bump as dimension (+ eventually a varying dimension) OR
-        the original EEG data in HsMM format
+        a 2D or 3D matrix of electrode activity with electrodes and event as dimension (+ eventually a varying dimension) OR
+        the original EEG data in HMP format
     estimated : ndarray
-        a 1D or 2D matrix of times with bump as dimension OR directly the results from a fitted hsmm 
+        a 1D or 2D matrix of times with event as dimension OR directly the results from a fitted hmp 
     channel_position : ndarray
         Either a 2D array with dimension electrode and [x,y] storing electrode location in meters or an info object from
         the mne package containning digit. points for electrode location
     init : float
-        initialized HsMM object
+        initialized HMP object
     time_step : float
         What unit to multiply all the times with, if you want to go on the second or millisecond scale you can provide 
         1/sf or 1000/sf where sf is the sampling frequency of the data
     figsize : list | tuple | ndarray
         Length and heigth of the matplotlib plot
     dpi : float
         DPI of the  matplotlib plot
     magnify : float
-        How much should the bumps be enlarged, useful to zoom on topologies, providing any other value than 1 will 
-        however change the displayed size of the bump
+        How much should the events be enlarged, useful to zoom on topologies, providing any other value than 1 will 
+        however change the displayed size of the event
     times_to_display : ndarray
         Times to display (e.g. Reaction time or any other relevant time) in the time unit of the fitted data
     cmap : str
         Colormap of matplotlib
     ylabels : dict
         dictonary with {label_name : label_values}
     max_time : float
@@ -63,52 +63,52 @@
     '''
     
     from mne.viz import plot_topomap
     from mpl_toolkits.axes_grid1.inset_locator import inset_axes
     return_ax = True
     if times_to_display is None:
         times_to_display = init.mean_d*time_step
-    if 'bump' in estimated:
+    if 'event' in estimated:
         #This is to keep backward compatibility but supplyng externally computed electrodes and times will probably be
         # DEPRECATED
-        if ydim is None and 'n_bumps' in estimated.dims:
-            if estimated.n_bumps.count() > 1:
-                ydim = 'n_bumps'
+        if ydim is None and 'n_events' in estimated.dims:
+            if estimated.n_events.count() > 1:
+                ydim = 'n_events'
         if ydim is not None and not skip_electrodes_computation:
-            electrodes = init.compute_topologies(electrodes, estimated, init.bump_width_samples, ydim).data
+            electrodes = init.compute_topologies(electrodes, estimated, init.event_width_samples, ydim).data
         elif not skip_electrodes_computation:
-            electrodes = init.compute_topologies(electrodes, estimated, init.bump_width_samples).data
+            electrodes = init.compute_topologies(electrodes, estimated, init.event_width_samples).data
         electrodes[electrodes == 0] = np.nan
         times = init.compute_times(init, estimated, mean=True).data
     else:#assumes times already computed
         times = estimated
     if len(np.shape(electrodes)) == 2:
         electrodes = electrodes[np.newaxis]
     n_iter = np.shape(electrodes)[0]
     if isinstance(ax, bool):
         if figsize == None:
             figsize = (12, 1*n_iter)
         fig, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
         return_ax = False
-    bump_size = init.bump_width_samples*time_step*magnify
+    event_size = init.event_width_samples*time_step*magnify
     yoffset =.25*magnify
     axes = []
     if n_iter == 1:
         times = [times]
     times = np.array(times, dtype=object)
     for iteration in np.arange(n_iter):
         times_iteration = times[iteration]*time_step
         electrodes_ = electrodes[iteration,:,:]
-        n_bump = int(sum(np.isfinite(electrodes_[:,0])))
-        electrodes_ = electrodes_[:n_bump,:]
-        for bump in np.arange(n_bump):
-            # if np.sum(electrodes_[bump,:]) != 0:
-            axes.append(ax.inset_axes([times_iteration[bump],iteration-yoffset,
-                                       (bump_size),yoffset*2], transform=ax.transData))
-            plot_topomap(electrodes_[bump,:], channel_position, axes=axes[-1], show=False,
+        n_event = int(sum(np.isfinite(electrodes_[:,0])))
+        electrodes_ = electrodes_[:n_event,:]
+        for event in np.arange(n_event):
+            # if np.sum(electrodes_[event,:]) != 0:
+            axes.append(ax.inset_axes([times_iteration[event],iteration-yoffset,
+                                       (event_size),yoffset*2], transform=ax.transData))
+            plot_topomap(electrodes_[event,:], channel_position, axes=axes[-1], show=False,
                          cmap=cmap, vlim=(vmin, vmax), sensors=sensors)
     if isinstance(ylabels, dict):
         ax.set_yticks(np.arange(len(list(ylabels.values())[0])),
                       [str(x) for x in list(ylabels.values())[0]])
         ax.set_ylabel(str(list(ylabels.keys())[0]))
     else:
         ax.set_yticks([])
@@ -129,22 +129,22 @@
     if return_ax:
         ax.set_ylim(0-yoffset, n_iter-1+yoffset)
         return ax
     else:
         plt.show()    
 
 
-def plot_LOOCV(loocv_estimates, pvals=True, test='t-test', figsize=(16,5), indiv=True, ax=False, mean=False):
+def plot_loocv(loocv_estimates, pvals=True, test='t-test', figsize=(16,5), indiv=True, ax=False, mean=False):
     '''
     Plotting the LOOCV results
     
     Parameters
     ----------
     loocv_estimates : ndarray or xarra.DataArray
-        results from a call to hsmm.utils.loocv()
+        results from a call to hmp.utils.loocv()
     pvals : bool
         Whether to display the pvalue with the associated test
     test : str
         which statistical test to compute for the difference in LOOCV-likelihood (one sample t-test or sign test)
     figsize : list | tuple | ndarray
         Length and heigth of the matplotlib plot
     indiv : bool
@@ -166,68 +166,68 @@
         else:
             raise ValueError('Expected sign or t-test argument to test parameter')
     if isinstance(ax, bool):
         fig, ax = plt.subplots(1,2, figsize=figsize)
         return_ax = False
     else:
         return_ax = True
-    loocv_estimates = loocv_estimates.dropna('n_bump', how='all')
+    loocv_estimates = loocv_estimates.dropna('n_event', how='all')
     if mean:
         alpha = .2#for the indiv plot
         means = np.nanmean(loocv_estimates.data,axis=1)
         ax[0].errorbar(x=np.arange(len(means))+1, y=means, \
                  yerr= np.nanstd(loocv_estimates.data,axis=1)/np.sqrt(len(loocv_estimates.participants))*1.96, marker='o', color='k')
     else:
         alpha=1
     if indiv:
         for loo in loocv_estimates.T:
-            ax[0].plot(np.arange(loocv_estimates.n_bump.max())+1,loo, alpha=alpha)
+            ax[0].plot(loocv_estimates.n_event,loo, alpha=alpha)
     ax[0].set_ylabel('LOOCV Loglikelihood')
-    ax[0].set_xlabel('Number of bumps')
-    ax[0].set_xticks(ticks=np.arange(1,loocv_estimates.n_bump.max()+1))
+    ax[0].set_xlabel('Number of events')
+    ax[0].set_xticks(ticks=loocv_estimates.n_event)
     total_sub = len(loocv_estimates.participants)
     diffs, diff_bin, labels = [],[],[]
-    for n_bump in np.arange(2,loocv_estimates.n_bump.max()+1):
-        diffs.append(loocv_estimates.sel(n_bump=n_bump).data - loocv_estimates.sel(n_bump=n_bump-1).data)
+    for n_event in np.arange(2,loocv_estimates.n_event.max()+1):
+        diffs.append(loocv_estimates.sel(n_event=n_event).data - loocv_estimates.sel(n_event=n_event-1).data)
         diff_bin.append([1 for x in diffs[-1] if x > 0])
-        labels.append(str(n_bump-1)+'->'+str(n_bump))
+        labels.append(str(n_event-1)+'->'+str(n_event))
         if pvals:
             pvalues = []
             if test == 'sign':
                 diff_tmp = np.array(diffs)
                 diff_tmp[np.isnan(diff_tmp)] = -np.inf 
                 pvalues.append((sign_test(diff_tmp[-1])))
             elif test == 't-test':
                 pvalues.append((ttest_1samp(diffs[-1], 0, alternative='greater')))
-            mean = np.nanmean(loocv_estimates.sel(n_bump=n_bump).data)
-            ax[1].text(x=n_bump-2, y=0, s=str(int(np.nansum(diff_bin[-1])))+'/'+str(len(diffs[-1]))+':'+str(np.around(pvalues[-1][-1],3)))
+            mean = np.nanmean(loocv_estimates.sel(n_event=n_event).data)
+            ax[1].text(x=n_event-2, y=0, s=str(int(np.nansum(diff_bin[-1])))+'/'+str(len(diffs[-1]))+':'+str(np.around(pvalues[-1][-1],3)))
     ax[1].plot(diffs,'.-', alpha=.3)
-    ax[1].set_xticks(ticks=np.arange(0,loocv_estimates.n_bump.max()-1), labels=labels)
-    ax[1].hlines(0,0,len(np.arange(2,loocv_estimates.n_bump.max())),color='k')
+    ax[1].set_xticks(ticks=np.arange(0,loocv_estimates.n_event.max()-1), labels=labels)
+    ax[1].hlines(0,0,len(np.arange(2,loocv_estimates.n_event.max())),color='k')
     ax[1].set_ylabel('Change in likelihood')
     ax[1].set_xlabel('')
     if return_ax:
         return ax
     else:
         plt.tight_layout()
         plt.show()
 
-def plot_latencies_average(times, bump_width, time_step=1, labels=[], colors=default_colors,
+def plot_latencies_average(times, event_width, time_step=1, labels=[], colors=default_colors,
     figsize=None, errs='ci', max_time=None, times_to_display=None):
     '''
     REDUNDANT WITH plot_latencies() WILL BE DEPRECATED
     Plots the average of stage latencies with choosen errors bars
 
     Parameters
     ----------
     times : ndarray
-        2D or 3D numpy array, Either trials * bumps or conditions * trials * bumps
-    bump_width : float
-        Display size of the bump in time unit given sampling frequency, if drawing a fitted object using hsmm_mvpy you 
-        can provide the bump_width_sample of fitted hsmm (e.g. init.bump_width_sample)
+        2D or 3D numpy array, Either trials * events or conditions * trials * events
+    event_width : float
+        Display size of the event in time unit given sampling frequency, if drawing a fitted object using hsmm_mvpy you 
+        can provide the event_width_sample of fitted hmp (e.g. init.event_width_sample)
     time_step : float
         What unit to multiply all the times with, if you want to go on the second or millisecond scale you can provide 
         1/sf or 1000/sf where sf is the sampling frequency of the data
     labels : tuples | list
         labels to draw on the y axis
     colors : ndarray
         array of colors for the different stages
@@ -288,15 +288,15 @@
 def plot_distribution(times, colors=default_colors, xlims=False, figsize=(8, 3), survival=False):
     '''
     Plots the distribution of each stage latencies
 
     Parameters
     ----------
     times : ndarray
-        2D or 3D numpy array, Either trials * bumps or conditions * trials * bumps
+        2D or 3D numpy array, Either trials * events or conditions * trials * events
     colors : ndarray
         array of colors for the different stages
     xlims : tuple | list
         lower and upper limit of the x (time) axis
     figsize : list | tuple | ndarray
         Length and heigth of the matplotlib plot
     survival : bool
@@ -330,26 +330,26 @@
         else:
             ax.vlines(times_to_display*time_step, yoffset-1.1, yoffset+1.1, ls='--')
             ax.set_xlim(-1*time_step, times_to_display*time_step+(times_to_display*time_step)/15)
     if max_time:
         ax.set_xlim(-1*time_step, max_time)
     return ax
 
-def plot_latencies_gamma(gammas, bump_width=0, time_step=1, labels=[''], colors=default_colors, 
+def plot_latencies_gamma(gammas, event_width=0, time_step=1, labels=[''], colors=default_colors, 
                          figsize=False, times_to_display=None, max_time=None, kind='bar', legend=False):
     '''
     Plots the average of stage latencies based on the estimated scale parameter of the gamma distributions
 
     Parameters
     ----------
     gammas : ndarray
-        instance of hsmm.hsmm.parameters
-    bump_width : float
-        Size of the bump in time unit given sampling frequency, if drawing a fitted object using hsmm_mvpy you 
-        can provide the bump_width_sample of fitted hsmm (e.g. init.bump_width_sample)
+        instance of hmp.hmp.parameters
+    event_width : float
+        Size of the event in time unit given sampling frequency, if drawing a fitted object using hsmm_mvpy you 
+        can provide the event_width_sample of fitted hmp (e.g. init.event_width_sample)
     time_step : float
         What unit to multiply all the times with, if you want to go on the second or millisecond scale you can provide 
         1/sf or 1000/sf where sf is the sampling frequency of the data
     labels : tuples | list
         labels to draw on the y axis
     colors : ndarray
         array of colors for the different stages
@@ -396,26 +396,26 @@
     axs.spines.top.set_visible(False)
     # Only show ticks on the left and bottom spines
     axs.yaxis.set_ticks_position('left')
     if legend:
         axs.legend()
     return axs
 
-def plot_latencies(times, bump_width, time_step=1, labels=[], colors=default_colors,
+def plot_latencies(times, event_width, time_step=1, labels=[], colors=default_colors,
     figsize=False, errs='ci',  max_time=None, times_to_display=None, kind='bar', legend=False):
     '''
     Plots the average of stage latencies with choosen errors bars
 
     Parameters
     ----------
     times : ndarray
-        2D or 3D numpy array, Either trials * bumps or conditions * trials * bumps
-    bump_width : float
-        Display size of the bump in time unit given sampling frequency, if drawing a fitted object using hsmm_mvpy you 
-        can provide the bump_width_sample of fitted hsmm (e.g. init.bump_width_sample)
+        2D or 3D numpy array, Either trials * events or conditions * trials * events
+    event_width : float
+        Display size of the event in time unit given sampling frequency, if drawing a fitted object using hsmm_mvpy you 
+        can provide the event_width_sample of fitted hmp (e.g. init.event_width_sample)
     time_step : float
         What unit to multiply all the times with, if you want to go on the second or millisecond scale you can provide 
         1/sf or 1000/sf where sf is the sampling frequency of the data
     labels : tuples | list
         labels to draw on the y axis
     colors : ndarray
         array of colors for the different stages
@@ -473,17 +473,17 @@
     axs.yaxis.set_ticks_position('left')
     axs.xaxis.set_ticks_position('bottom')
     if legend:
         axs.legend()
     return axs
 
 def plot_iterations(iterations, eeg_data, init, positions, dims):
-    from hsmm_mvpy.models import hsmm
+    from hsmm_mvpy.models import hmp
     for iteration in iterations.iteration[:-1]:
-        selected = init.fit_single(iterations.sel(iteration=iteration)[dims[0]].dropna(dim='bump').bump[-1].values+1,\
-            magnitudes = iterations.sel(iteration=iteration)[dims[0]].dropna(dim='bump'),\
+        selected = init.fit_single(iterations.sel(iteration=iteration)[dims[0]].dropna(dim='event').event[-1].values+1,\
+            magnitudes = iterations.sel(iteration=iteration)[dims[0]].dropna(dim='event'),\
             parameters = iterations.sel(iteration=iteration)[dims[1]].dropna(dim='stage'),\
             threshold=0, verbose=False)
 
         #Visualizing
         plot_topo_timecourse(eeg_data, selected, positions,  init, magnify=1, sensors=False)
```

### Comparing `hsmm_mvpy-0.1.0a2/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.1.0a2
+Version: 0.1.0b0
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -37,30 +37,31 @@
 Project-URL: Bug Tracker, https://github.com/GWeindel/hmp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-HMP
+HsMM MVpy
 ==========
 
 ![](plots/general_illustration.png)
 
-hmp is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HsMM-MVPA) of electro-encephalographic (EEG) data based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
+HsMM MVpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HMP) of neural time-series (e.g. EEG) based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
 
-As a summary of the method, an HsMM-MVPA analysis parses the EEG into a number of significant cognitive event (called bumps) separated by flat period reflecting the ongoing stage initiated by a bump. Hence any reaction time can then be described by the number of bumps and stage estimated using hsmm_mvpy. The important aspect of HsMM-MVPA is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of cognitive events on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in the EEG (or MEG) signal:
-- Describing an experiment or a clinical sample in terms of processes detected in the EEG signal
+As a summary of the method, an HMP model parses the reaction time into a number of successive stages determined based on patterns in a neural time-serie. Hence any reaction time can then be described by a number of stage  and their duration estimated using hsmm_mvpy. The important aspect of HMP is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of stages on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in a signal:
+- Describing an experiment or a clinical sample in terms of stages detected in the EEG signal
 - Describing experimental effects based on a particular stage duration
-- Estimating the effect of trial-wise manipuations (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
-- Time-lock EEG signal to the onset of a given bump and perform classical ERPs or time-freauency analysis based on the events that are the estimated bumps
-- And many more (e.g. evidence accumulation models on decision stage, classification based on the number of events in the signal,...)
+- Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
+- Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
+- And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
+**Important note** The current tutorials are based on the latest (unstable) version not yet available through _pip_, installing through github is therefore recommended.
 
 The package is available through *pip* with the command ```pip install hsmm_mvpy```. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
@@ -68,103 +69,101 @@
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
 
-For the cutting edge version (not recommended) you can clone the repository using *git*
+For the cutting edge version you can clone the repository using *git*
 
 Open a terminal and type:
 
     $ git clone https://github.com/gweindel/hsmm_mvpy.git
    
 Then move to the clone repository and run 
     
     $ pip install -e .
 
+
 ## To get started
 To get started with the code:
 - Check the demo below 
 - Inspect the tutorials in the tutorials repository
     - Load EEG data (tutorial 1)
-    - Estimating a given number of bumps (tutorial 2)
-    - Test for the number of bumps that best explains the data (tutorial 3)
+    - Estimating a HMP with given number of stages (tutorial 2)
+    - Test for the number of stages that best explains the data (tutorial 3)
     - Testing differences across conditions (tutorial 4)
 
-To further learn about the method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)). The following list also contains a non-exhaustive list of papers published using the HsMM-MVPA method:
+To further learn about the method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)). The following list also contains a non-exhaustive list of papers published using HMP:
 - Berberyan, H. S., van Maanen, L., van Rijn, H., & Borst, J. (2021). EEG-based identification of evidence accumulation stages in decision-making. Journal of Cognitive Neuroscience, 33(3), 510-527. [link](https://doi.org/10.1162/jocn_a_01663)
 - Van Maanen, L., Portoles, O., & Borst, J. P. (2021). The discovery and interpretation of evidence accumulation stages. Computational brain & behavior, 4(4), 395-415. [link](https://link.springer.com/article/10.1007/s42113-021-00105-2)
 - Portoles, O., Blesa, M., van Vugt, M., Cao, M., & Borst, J. P. (2022). Thalamic bursts modulate cortical synchrony locally to switch between states of global functional connectivity in a cognitive task. PLoS computational biology, 18(3), e1009407. [link](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009407)
 
 ## Demo on simulated data
 
 The following section will quickly walk you through an example usage in simulated data (using [MNE](https://mne.tools/dev/auto_examples/simulation/index.html)'s simulation functions and tutorials)
 
 First we load the libraries necessary for the demo on simulated data
 
 ### Importing libraries
 
-
-
 ```python
 ## Importing these packages is specific for this simulation case
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from scipy.stats import gamma
 
 ## Importing HMP
 import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
-    <frozen importlib._bootstrap>:241: RuntimeWarning: scipy._lib.messagestream.MessageStream size changed, may indicate binary incompatibility. Expected 56 from C header, got 64 from PyObject
-
-
 ### Simulating data
 
-In the following code block we simulate 30 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HsM models. All these four sources are defined by a localization, an activation amplitude and a distribution (here gamma with shape and scale parameters) for the onsets of the bumps on each trial. The simulation functions are based on the [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
+In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HMP models. All these four sources are defined by a localization, an activation amplitude and a distribution (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
 _If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
 ```python
 cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
 n_trials = 50 #Number of trials to simulate
 
-##### Here we define the sources of the brain activity (bump) for each trial
-frequency = 10.#Frequency of the bump defining its duration, half-sine of 10Hz = 50ms
-amplitude = np.array([.1e-6,.1e-6,.1e-6,.1e-6,1e-20]) #Amplitude of the bump in Volt, defining signal to noise ratio
+##### Here we define the sources of the brain activity (event) for each trial
+frequency = 10.#Frequency of the event defining its duration, half-sine of 10Hz = 50ms
+amplitude = .5e-6 #Amplitude of the event in Volt, defining signal to noise ratio
 shape = 2 #shape of the gamma distribution
-means = np.array([60,150, 200, 100, 80])/shape #Mean duration of the stages separating bumps, in ms
+means = np.array([60, 150, 200, 100, 80])/shape #Mean duration of the stages in ms
 names = ['bankssts-rh','posteriorcingulate-lh','parahippocampal-lh',\
          'pericalcarine-rh','postcentral-lh']#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
 sources = []
-for source in zip(names, amplitude, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
-    sources.append([source[0], frequency, source[1], gamma(shape, scale=source[2])])
+for source in zip(names, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
+    sources.append([source[0], frequency, amplitude, gamma(shape, scale=source[1])])
 
 # Function used to generate the data
-file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', overwrite=False)
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True)
 #Recovering sampling frequency of the simulated dataset
 sfreq = simulations.simulation_sfreq()
 #load electrode position, specific to the simulations
 positions = simulations.simulation_positions()
 ```
 
-    ./dataset_README_raw.fif exists no new simulation performed
+    Simulating ./dataset_README_raw.fif
+    ./dataset_README_raw.fif simulated
+
 
 
 ### Creating the event structure and plotting the raw data
 
 
-To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 0 signal the onset of the stimulus and 5 the onset of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
+To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 1 signal the onset of the stimulus and 6 the moment of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
 
 
 ```python
 #Recovering the events to epoch the data (in the number of trials defined above)
 generating_events = np.load(file[1])
 resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
 event_id = {'stimulus':1}#trigger 1 = stimulus
@@ -177,149 +176,206 @@
 raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
 raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
 
     Using qt as 2D backend.
     Channels marked as bad:
     none
+    
 ![png](README_files/README_7_1.png)
 
 
-### Recovering number of sources as well as actual by-trial variation
 
-To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth
+### Recovering number of stages as well as actual by-trial variation
+
+To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of stages or sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth.
 
 
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
-#Recover the actual time of the simulated bumps
+#Recover the actual time of the simulated events
 random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
            (n_trials, number_of_sources))
 ```
 
-## Demo of the HsMM Code for a single participant in a single condition based on the simulated data
+## Demo for a single participant in a single condition based on the simulated data
 
 First we read the EEG data as we would for a single participant:
 
 
 ```python
 # Reading the data
-eeg_data = hmp.utils.read_mne_EEG(file[0], event_id, resp_id, sfreq, 
+eeg_data = hmp.utils.read_mne_data(file[0], event_id=event_id, resp_id=resp_id, sfreq=sfreq, 
             events_provided=events, verbose=False)
 
 ```
 
-    Processing participant ./dataset_README_raw.fif
-    Reading 0 ... 142583  =      0.000 ...   237.395 secs...
-    Creating epochs based on following event ID :[1 6]
-    N trials without response event: 0
-    Applying reaction time trim to keep RTs between 0.001 and 5 seconds
-    50 RTs kept of 50 clean epochs
+    Processing participant ./dataset_README_raw.fif's continuous eeg
+    Reading 0 ... 153075  =      0.000 ...   254.864 secs...
     50 trials were retained for participant ./dataset_README_raw.fif
-    End sampling frequency is 600.614990234375 Hz
 
 
 The package uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
 ```python
 #example of usage of xarray
 print(eeg_data)
 eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
     .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 843)
+    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 711)
     Coordinates:
       * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
       * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 836 837 838 839 840 841 842
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 704 705 706 707 708 709 710
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 2.469e-06...
-        event        (participant, epochs) <U8 'stimulus' 'stimulus' ... 'stimulus'
+        data         (participant, epochs, electrodes, samples) float64 1.96e-06 ...
     Attributes:
         sfreq:    600.614990234375
         offset:   0
 
 
 
     
-![png](README_files/README_13_1.png)
+![png](README_files/README_12_1.png)
     
 
 
+
 Next we transform the data as in Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) including standardization of individual variances (not in this case as we have only one simulated participant), z-scoring and spatial principal components analysis (PCA). 
 
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
-hsmm_dat = hmp.utils.transform_data(eeg_data.data, apply_standard=False, n_comp=4)
+hmp_data = hmp.utils.transform_data(eeg_data, apply_standard=False, n_comp=4)
 ```
 
-# Estimating an HsMM model
+Once the data is in the expected format, we can initialize an HMP
+
+
+```python
+init = hmp.models.hmp(hmp_data, eeg_data, event_width=50, cpus=cpus)#Initialization of the model
+```
+
+# HMP model
+
+We are looking for stages in the data (**Hidden Markov**) and assume that transitions between stages are signaled by a template in the data (**pattern analysis**). By default we use the same template as Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet'.apa.org/doi/10.1037/rev0000030)), a 10 Hz half-sine, resulting in a 50ms duration bump-like shape:
 
-We can directly fit an HsMM model without giving any info on the number of bumps (see tutorial 2 for the explanation of the following cell)
 
 
 ```python
-%%time
-init = hmp.models.hsmm(hsmm_dat, eeg_data, bump_width=50, cpus=cpus)#Initialization of the model
-estimates = init.fit(step=10, verbose=False)
+plt.plot(init.template,'x');
 ```
 
 
-      0%|          | 0/360 [00:00<?, ?it/s]
+    
+![png](README_files/README_18_0.png)
+    
+
+
+This pattern is assumed to be present in multiple electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
+
+
+
+```python
+epoch = 0 #illustrating the first trial
+hmp_data.unstack().sel(component=[0,1,2], epochs=epoch).squeeze().plot.line(hue='component');
+plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k')#overlaying the simulated stage transition times
+```
+
+
+    
+![png](README_files/README_20_1.png)
+    
+
 
 
-    CPU times: user 645 ms, sys: 1.6 ms, total: 647 ms
-    Wall time: 646 ms
+The by-trial onset of this transition event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
+
+
+```python
+T = 350
+plt.plot(np.linspace(0,T,1001),gamma.pdf(np.linspace(0,T,1001), 2, scale=50)) 
+plt.xlabel('t');
+```
+
+
+    
+![png](README_files/README_22_0.png)
+    
+
+
+And this is then the full explanation of an HMP model: Looking for a transition event across several electrodes and trials that signals a transition to the next stage and which onset is expected to follow a probability distribution (in this case a gamma).
+
+# Estimating an HMP model
+
+We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for the explanation of the following cell)
+
+
+
+```python
+estimates = init.fit(step=20, verbose=True)
+```
+
+
+    Transition event 2 found around sample 137
+    Transition event 3 found around sample 258
+    Transition event 4 found around sample 330
+    Estimating 4 events model
+    Parameters estimated for 4 events model
 
 
 ### Visualizing results of the fit
 
-In the previous cell we initiated an HsMM model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 bumps and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit
+In the previous cell we initiated an HMP model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 Transition events and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit.
+
+We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
+
 
-We can directly take a look to the topologies and latencies of the bumps by calling ```hmp.visu.plot_topo_timecourse```
+We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
 
 
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
                                positions, init,#position of the electrodes and initialized model
                                magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
                                times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
 
     
-![png](README_files/README_21_0.png)
+![png](README_files/README_27_0.png)
     
 
 
-This shows us the electrode activity on the scalp as well as the average time of occurence of the bump based on the stage distributions.
+This shows us the electrode activity on the scalp as well as the average time of occurence of the events based on the stage distributions.
 
-As we are estimating the bump onsets on a by-trial basis we can look at the by-trial variation in stage duration.
+As we are estimating the event onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
 
 ```python
-bump_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('bump')#computing predicted bump times
-ax = hmp.visu.plot_latencies_average(bump_times_estimates, init.bump_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
+event_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('event')#computing predicted event times
+ax = hmp.visu.plot_latencies_average(event_times_estimates, init.event_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
-![png](README_files/README_23_0.png)
+![png](README_files/README_29_0.png)
     
 
 
-For the same reason we can also inspect the probability distribution of bump onsets:
+For the same reason we can also inspect the probability distribution of event onsets:
+
 
 
 ```python
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)), survival=True)
 ```
 
@@ -328,118 +384,119 @@
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_25_1.png)
+![png](README_files/README_31_1.png)
     
 
 
 
     
-![png](README_files/README_25_2.png)
+![png](README_files/README_31_2.png)
     
 
 
-As HsMM-MVPA selected those bumps onset per trial we can also look at the predicted bump onsets for a single trial
+As HMP estimated stage onset per trial we can also look at the predicted stage onsets for a given trial.
 
 
 ```python
-hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 1)), 
+hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 0)), 
                             xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 ```
 
 
 
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_27_1.png)
+![png](README_files/README_33_1.png)
     
 
 
-This then shows the likeliest bump location in time for the first trial!
+This then shows the likeliest stage onset location in time for the first trial!
 
 ## Comparing with ground truth
 
-As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HsMM-MVpy. As in the beginning, this code is specific to the case where you simulate data.
+As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP-MVpy. As in the beginning, this code is specific to the case where you simulate data.
 
 
 ```python
 colors = sns.color_palette(None, number_of_sources)
-# plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(params=1)*2+np.concatenate([[0],np.repeat(init.bump_width_samples,number_of_sources-1)]), color=colors,s=50)
-plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(parameter=1)*2, color=colors,s=50)
+plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.prod(axis=1), color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
 plt.title('Actual vs estimated stage durations')
 plt.xlabel('Simulated stage duration')
 plt.ylabel('Estimated stage duration')
 plt.show()
 
 ```
 
 
     
-![png](README_files/README_30_0.png)
+![png](README_files/README_35_0.png)
     
 
 
 Or also overlay actual bumps onset with predicted one
 
 
+
 ```python
-hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated bump onsets',
+hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated event onsets',
         times_to_display = np.mean(np.cumsum(random_source_times,axis=1),axis=0))
 ```
 
 
     
-![png](README_files/README_32_0.png)
+![png](README_files/README_37_0.png)
     
 
 
-We see that the HsMM-MVpy package recovers the exact average location of the bumps defined in the simulated data
+We see that the HSMM-MVpy package recovers the exact average location of the bumps defined in the simulated data.
 
-We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HsMM model
+We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HMP model
 
 
 ```python
 fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
 i = 0
 
-for bump in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
-    sns.regplot(x=random_source_times[:,i].T, y=bump, ax=ax[i], color=colors[i])
-    ax[i].plot([np.min(bump), np.max(bump)], [np.min(bump), np.max(bump)],'--', color='k')
+for event in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
+    sns.regplot(x=random_source_times[:,i].T, y=event, ax=ax[i], color=colors[i])
+    ax[i].plot([np.min(event), np.max(event)], [np.min(event), np.max(event)],'--', color='k')
     ax[i].set_ylabel(f'Estimated by-trial stage duration for stage {i+1}')
     ax[i].set_xlabel(f'Simulated by-trial stage duration for stage {i+1}')
     i+= 1
 ```
 
 
     
-![png](README_files/README_35_0.png)
+![png](README_files/README_39_0.png)
     
 
 
 We see that every stage gets nicely recovered even on a by-trial basis!
 
 # Beyond summary statistics for EEG analysis
 
-Now the purpose, apart from determining the number and timecourse of important EEG events in the Rreaction time, is also to use the by-trial information.
+Now the purpose, apart from determining the number and time course of important EEG events in the reaction time, is also to use the by-trial information.
 
 We illustrate this by first plotting the traditional event-related potentials (i.e. taking the average of given electrodes across the different time points) with cherry-picked electrodes.
 
 
+
 ```python
 import seaborn as sns
 import pandas as pd
 
 data = eeg_data.stack({'trial_x_participant':['participant','epochs']}).data.dropna('trial_x_participant', how="all")
 fig, ax = plt.subplots(1,1, figsize=(20,5), sharey=True)
 
@@ -453,25 +510,25 @@
 plt.xlim(0,500)
 plt.ylim(-3e-6,3e-6);
 
 ```
 
 
     
-![png](README_files/README_38_0.png)
+![png](README_files/README_41_0.png)
     
 
 
-Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to trqditional ERPs with very clear signal in the beginning of a trial (as events are more in sync) and summed and blurried in later stages of the reaction times (as event are off sync).
+Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to traditional ERPs with very clear signal in the beginning of a trial (as events are more in phase) and summed and blurried in later stages of the reaction times (as event are off phase).
 
-Now things can get better if we first parse, by-trial, the signal into the different stages based on the HsMM estimates:
+Now things can get better if we first parse, by-trial, the signal into the different stages based on the HMP estimates:
 
 
 ```python
-BRP_times = init.compute_times(init, estimates.dropna('bump'), fill_value=0, add_rt=True)
+BRP_times = init.compute_times(init, estimates.dropna('event'), fill_value=0, add_rt=True)
 
 fig, ax = plt.subplots(1,number_of_sources, figsize=(20,5), sharey=True, sharex=True)
 ax[0].set_ylabel('Volt')
 for stage in range(number_of_sources):
     BRP = hmp.utils.event_times(data, BRP_times,'EEG 016',stage=stage)
     df = pd.DataFrame(BRP).melt(var_name='Time')
     sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkgreen')
@@ -482,21 +539,23 @@
     df = pd.DataFrame(BRP).melt(var_name='Time')
     sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkblue') 
     plt.xlim(0,100)
 ```
 
 
     
-![png](README_files/README_40_0.png)
+![png](README_files/README_43_0.png)
     
 
 
+
 In this case we clearly see at each stage the half-sin (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sin). Note that the end of the stages tend to be noisier because less trial are defining the average signal (also why the confidence interval grows).
 
 
 ### Follow-up
 
-For examples on how to use the package when the number of bumps are unkown, or to compare stage durations across conditions see the tutorial notebooks:
+For examples on how to use the package when the number of transition events/stages is unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
-- Estimating a given number of bumps (tutorial 2)
-- Test for the number of bumps that best explains the data (tutorial 3)
+- Estimating a given number of events (tutorial 2)
+- Test for the number of events that best explains the data (tutorial 3)
 - Testing differences across conditions (tutorial 4)
+
```

