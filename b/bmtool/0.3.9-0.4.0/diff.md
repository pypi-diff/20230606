# Comparing `tmp/bmtool-0.3.9.tar.gz` & `tmp/bmtool-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmtool-0.3.9.tar", last modified: Thu Jun  1 20:42:37 2023, max compression
+gzip compressed data, was "bmtool-0.4.0.tar", last modified: Tue Jun  6 18:06:08 2023, max compression
```

## Comparing `bmtool-0.3.9.tar` & `bmtool-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.656518 bmtool-0.3.9/
--rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.9/LICENSE
--rw-rw-rw-   0        0        0    17751 2023-06-01 20:42:37.654472 bmtool-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0    17006 2023-05-31 22:34:19.000000 bmtool-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.600814 bmtool-0.3.9/bmtool/
--rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.9/bmtool/__init__.py
--rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.9/bmtool/__main__.py
--rw-rw-rw-   0        0        0    29723 2023-06-01 20:21:45.000000 bmtool-0.3.9/bmtool/bmplot.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.641929 bmtool-0.3.9/bmtool/debug/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.9/bmtool/debug/__init__.py
--rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.9/bmtool/debug/commands.py
--rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.9/bmtool/debug/debug.py
--rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.9/bmtool/manage.py
--rw-rw-rw-   0        0        0    12528 2023-06-01 14:19:08.000000 bmtool-0.3.9/bmtool/plot_commands.py
--rw-rw-rw-   0        0        0    14900 2023-05-23 16:25:45.000000 bmtool-0.3.9/bmtool/singlecell.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.647922 bmtool-0.3.9/bmtool/util/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.9/bmtool/util/__init__.py
--rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.9/bmtool/util/commands.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.652467 bmtool-0.3.9/bmtool/util/neuron/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.9/bmtool/util/neuron/__init__.py
--rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.9/bmtool/util/neuron/celltuner.py
--rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.3.9/bmtool/util/util.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.620939 bmtool-0.3.9/bmtool.egg-info/
--rw-rw-rw-   0        0        0    17751 2023-06-01 20:42:35.000000 bmtool-0.3.9/bmtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-06-01 20:42:36.000000 bmtool-0.3.9/bmtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 20:42:35.000000 bmtool-0.3.9/bmtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-01 20:42:35.000000 bmtool-0.3.9/bmtool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2023-06-01 20:42:35.000000 bmtool-0.3.9/bmtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-01 20:42:35.000000 bmtool-0.3.9/bmtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 20:42:37.657679 bmtool-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-06-01 20:40:18.000000 bmtool-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.312708 bmtool-0.4.0/
+-rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0    17751 2023-06-06 18:06:08.312708 bmtool-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17006 2023-05-31 22:34:19.000000 bmtool-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.268740 bmtool-0.4.0/bmtool/
+-rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.4.0/bmtool/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.4.0/bmtool/__main__.py
+-rw-rw-rw-   0        0        0    29723 2023-06-01 20:21:45.000000 bmtool-0.4.0/bmtool/bmplot.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.297710 bmtool-0.4.0/bmtool/debug/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.4.0/bmtool/debug/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.4.0/bmtool/debug/commands.py
+-rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.4.0/bmtool/debug/debug.py
+-rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.4.0/bmtool/manage.py
+-rw-rw-rw-   0        0        0    12528 2023-06-01 14:19:08.000000 bmtool-0.4.0/bmtool/plot_commands.py
+-rw-rw-rw-   0        0        0    22524 2023-06-06 18:05:24.000000 bmtool-0.4.0/bmtool/singlecell.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.305706 bmtool-0.4.0/bmtool/util/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.4.0/bmtool/util/__init__.py
+-rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.4.0/bmtool/util/commands.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.309745 bmtool-0.4.0/bmtool/util/neuron/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.4.0/bmtool/util/neuron/__init__.py
+-rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.4.0/bmtool/util/neuron/celltuner.py
+-rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.4.0/bmtool/util/util.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.292734 bmtool-0.4.0/bmtool.egg-info/
+-rw-rw-rw-   0        0        0    17751 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 18:06:08.313708 bmtool-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-06-06 18:05:36.000000 bmtool-0.4.0/setup.py
```

### Comparing `bmtool-0.3.9/LICENSE` & `bmtool-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/PKG-INFO` & `bmtool-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.9
+Version: 0.4.0
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `bmtool-0.3.9/README.md` & `bmtool-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/bmtool/__main__.py` & `bmtool-0.4.0/bmtool/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/bmtool/bmplot.py` & `bmtool-0.4.0/bmtool/bmplot.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/bmtool/debug/commands.py` & `bmtool-0.4.0/bmtool/debug/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/bmtool/manage.py` & `bmtool-0.4.0/bmtool/manage.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/bmtool/plot_commands.py` & `bmtool-0.4.0/bmtool/plot_commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/bmtool/singlecell.py` & `bmtool-0.4.0/bmtool/singlecell.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,387 +1,544 @@
 import glob
 import os
 from typing import Tuple
-import random
-
+import numpy as np
 import matplotlib.pyplot as plt
+from scipy.optimize import curve_fit
 import neuron
 from neuron import h
-import numpy as np
 
-class CurrentClamp():
-    def __init__(self, template_name, post_init_function=None, record_sec="soma", record_loc="0.5", tstop=1000,
-                 inj_sec="soma", inj_loc="0.5", inj_amp=100, inj_delay=100, inj_dur=1000):
+
+def get_target_site(cell, sec=('soma', 0), loc=0.5, site=''):
+    if isinstance(sec, str):
+        sec = (sec, 0)
+    elif isinstance(sec, int):
+        if not hasattr(cell, 'all'):
+            raise ValueError("Section list named 'all' does not exist in the template.")
+        sec = ('all', sec)
+    loc = float(loc)
+    try:
+        section = next(s for i, s in enumerate(getattr(cell, sec[0])) if i == sec[1])
+        seg = section(loc)
+    except Exception as e0:
+        try:
+            section = eval("cell." + sec[0])
+            seg = section(loc)
+        except Exception as e:
+            print(e0)
+            print(e)
+            raise ValueError("Hint: Are you selecting the correct " + site + " location?")
+    return seg, section
+
+
+class CurrentClamp(object):
+    def __init__(self, template_name, post_init_function=None, record_sec='soma', record_loc=0.5,
+                 inj_sec='soma', inj_loc=0.5, inj_amp=100., inj_delay=100., inj_dur=1000., tstop=1000.):
+        """
+        template_name: str, name of the cell template located in hoc
+        post_init_function: str, function of the cell to be called after the cell has been initialized
+        record_sec: tuple, (section list name, index) to access a section in a hoc template
+            If a string of section name is specified, index default to 0
+            If an index is specified, section list name default to `all`
+        record_loc: float, location within [0, 1] of a segment in a section to record from
+        inj_sec, inj_loc: current injection site, same format as record site
+        tstop: time for simulation (ms)
+        inj_delay: current injection start time (ms)
+        inj_dur: current injection duration (ms)
+        inj_amp: current injection amplitude (pA)
+        """
         self.template_name = template_name
-        self.tstop = tstop
-        self.inj_dur = inj_dur
-        
         self.record_sec = record_sec
         self.record_loc = record_loc
         self.inj_sec = inj_sec
         self.inj_loc = inj_loc
 
-        self.inj_amp = inj_amp/1e3
-        self.cell = eval('h.'+self.template_name+'()')
+        self.tstop = max(tstop, inj_delay + inj_dur)
+        self.inj_delay = inj_delay # use x ms after start of inj to calculate r_in, etc
+        self.inj_dur = inj_dur
+        self.inj_amp = inj_amp * 1e-3 # pA to nA
+
+        self.cell = getattr(h, self.template_name)()
         if post_init_function:
             eval(f"self.cell.{post_init_function}")
-        self.cell_src = None
-        self.cell_vec = None
-        self.inj_delay = inj_delay #use x ms after start of inj to calculate r_in, etc
-
-        self.t_vec = h.Vector()
 
         self.setup()
 
     def setup(self):
-        self.t_vec.record(h._ref_t)
-
-        try:
-            inj_str = "self.cell." + self.inj_sec + "(" + self.inj_loc + ")"
-            self.cell_src = h.IClamp(eval(inj_str))
-        except TypeError:
-            try:
-                inj_str = "self.cell." + self.inj_sec + "[0](" + self.inj_loc + ")"
-                self.cell_src = h.IClamp(eval(inj_str))
-            except:
-                print("Hint: Are you selecting the correct injection location?")
-                raise
+        inj_seg, _ = get_target_site(self.cell, self.inj_sec, self.inj_loc, 'injection')
+        self.cell_src = h.IClamp(inj_seg)
         self.cell_src.delay = self.inj_delay
         self.cell_src.dur = self.inj_dur
         self.cell_src.amp = self.inj_amp
-        
-        try:
-            rec_str = "self.cell." + self.record_sec + "(" + self.record_loc + ")._ref_v"
-            self.cell_nc = h.NetCon(eval(rec_str),None,sec=eval("self.cell." + self.record_sec))
-        except TypeError:
-            try:
-                rec_str = "self.cell." + self.record_sec + "[0](" + self.record_loc + ")._ref_v"
-                self.cell_nc = h.NetCon(eval(rec_str),None,sec=eval("self.cell." + self.record_sec + '[0]'))
-            except:
-                print("Hint: Are you selecting the correct recording location?")
-                raise
-        self.cell_nc.threshold = 0
-        self.cell_vec = h.Vector()
-        self.cell_vec.record(eval(rec_str))
-
-        print(f"Injection location: {inj_str}")
-        print(f"Recording: {rec_str}")
-
-    def execute(self) -> Tuple[list,list]:
-        print("current clamp simulation running...")
-        h.tstop = int(self.tstop)
+
+        rec_seg, _ = get_target_site(self.cell, self.record_sec, self.record_loc, 'recording')
+        self.v_vec = h.Vector()
+        self.v_vec.record(rec_seg._ref_v)
+
+        self.t_vec = h.Vector()
+        self.t_vec.record(h._ref_t)
+
+        print(f'Injection location: {inj_seg}')
+        print(f'Recording: {rec_seg}._ref_v')
+
+    def execute(self) -> Tuple[list, list]:
+        print("Current clamp simulation running...")
+        h.tstop = self.tstop
         h.stdinit()
         h.run()
 
-        return (list(self.t_vec), list(self.cell_vec))
+        return self.t_vec.to_python(), self.v_vec.to_python()
+
 
 class Passive(CurrentClamp):
-    def __init__(self, template_name, tstop=1200, inj_amp=-100,inj_delay=200, inj_dur=1000, **kwargs):
-        super(Passive, self).__init__(template_name=template_name, tstop=tstop,
-                                      inj_amp=inj_amp, inj_delay=inj_delay, inj_dur=inj_dur, **kwargs)
-
-        self.cell_v_final = 0
-        self.v_t_const = 0
-
-        self.v_rest_time = 0.0
-        self.v_final_time = 0.0
-
-        self.v_rest = 0.0
-        self.r_in = 0.0
-        self.tau = 0.0
+    def __init__(self, template_name, inj_amp=-100., inj_delay=200., inj_dur=1000.,
+                 tstop=1200., method=None, **kwargs):
+        """
+        method: {'simple', 'exp2'}, optional.
+            Method to estimate membrane time constant. Default is 'simple'
+            that find the time to reach 0.632 of change. 'exp2' fits a double
+            exponential curve to the membrane potential response.
+        """
+        assert(inj_amp != 0)
+        super().__init__(template_name=template_name, tstop=tstop,
+                         inj_amp=inj_amp, inj_delay=inj_delay, inj_dur=inj_dur, **kwargs)
+        self.inj_stop = inj_delay + inj_dur
+        self.method = method
+        self.tau_methods = {'simple': self.tau_simple, 'exp2': self.tau_double_exponential}
+
+    def tau_simple(self):
+        v_t_const = self.cell_v_final - self.v_diff / np.e
+        index_v_tau = next(x for x, val in enumerate(self.v_vec_inj) if val <= v_t_const)
+        self.tau = self.t_vec[self.index_v_rest + index_v_tau] - self.v_rest_time # ms
+
+        def print_calc():
+            print()
+            print('Tau Calculation: time until 63.2% of dV')
+            print('v_rest + 0.632*(v_final-v_rest)')
+            print(f'{self.v_rest:.2f} + 0.632*({self.cell_v_final:.2f}-({self.v_rest:.2f})) = {v_t_const:.2f} (mV)')
+            print(f'Time where V = {v_t_const:.2f} (mV) is {self.v_rest_time + self.tau:.2f} (ms)')
+            print(f'{self.v_rest_time + self.tau:.2f} - {self.v_rest_time:g} = {self.tau:.2f} (ms)')
+            print()
+        return print_calc
+
+    @staticmethod
+    def double_exponential(t, a0, a1, a2, tau1, tau2):
+        return a0 + a1 * np.exp(-t / tau1) + a2 * np.exp(-t / tau2)
+
+    def tau_double_exponential(self):
+        index_v_peak = (np.sign(self.inj_amp) * self.v_vec_inj).argmax()
+        self.t_peak = self.t_vec_inj[index_v_peak]
+        self.v_peak = self.v_vec_inj[index_v_peak]
+        self.v_sag = self.v_peak - self.cell_v_final
+        self.v_max_diff = self.v_diff + self.v_sag
+        self.sag_norm = self.v_sag / self.v_max_diff
+
+        self.tau_simple()
+        p0 = (self.v_sag, -self.v_max_diff, self.t_peak, self.tau) # intial estimate
+        v0 = self.v_rest
+        def fit_func(t, a1, a2, tau1, tau2):
+            return self.double_exponential(t, v0 - a1 - a2, a1, a2, tau1, tau2)
+        bounds = ((-np.inf, -np.inf, 1e-3, 1e-3), np.inf)
+        popt, self.pcov = curve_fit(fit_func, self.t_vec_inj, self.v_vec_inj, p0=p0, bounds=bounds, maxfev=10000)
+        self.popt = np.insert(popt, 0, v0 - sum(popt[:2]))
+        self.tau = max(self.popt[-2:])
+
+        def print_calc():
+            print()
+            print('Tau Calculation: Fit a double exponential curve to the membrane potential response')
+            print('f(t) = a0 + a1*exp(-t/tau1) + a2*exp(-t/tau2)')
+            print('Constained by initial value: f(0) = a0 + a1 + a2 = v_rest')
+            print('Fit parameters: (a0, a1, a2, tau1, tau2) = (' + ', '.join(f'{x:.2f}' for x in self.popt) + ')')
+            print(f'Membrane time constant is determined from the slowest exponential term: {self.tau:.2f} (ms)')
+            print()
+            print('Sag potential: v_sag = v_peak - v_final = %.2f (mV)' % self.v_sag)
+            print('Normalized sag potential: v_sag / (v_peak - v_rest) = %.3f' % self.sag_norm)
+            print()
+        return print_calc
+
+    def double_exponential_fit(self):
+        t_vec = self.v_rest_time + self.t_vec_inj
+        v_fit = self.double_exponential(self.t_vec_inj, *self.popt)
+        return t_vec, v_fit
 
     def execute(self):
-        
-        print(f"Running passive property simulation...")
-        h.tstop = int(self.tstop)
+        print("Running simulation for passive properties...")
+        h.tstop = self.tstop
         h.stdinit()
         h.run()
 
-        index_v_rest = int(((1000/h.dt)/1000 * self.inj_delay))
-        index_v_final = int(((1000/h.dt)/1000 * (self.tstop)))
-        
-        self.v_rest = self.cell_vec[index_v_rest]
-        self.v_rest_time = index_v_rest / (1/h.dt)
-
-        self.cell_v_final = self.cell_vec[index_v_final]
-        self.v_final_time = index_v_final / (1/h.dt)
-
-        v_diff = self.v_rest - self.cell_v_final
-
-        self.v_t_const = self.v_rest - (v_diff *.632)
-
-        index_v_tau = next(x for x, val in enumerate(list(self.cell_vec)) if val < self.v_t_const) 
-        time_tau = (index_v_tau / ((1000/h.dt)/1000)) - self.inj_delay
-        self.tau = time_tau #/ 1000 (in ms)
-        self.r_in = (v_diff)/(0-self.inj_amp) * 1e6 #MegaOhms -> Ohms
-        print()
-        print(f"V Rest: {self.v_rest:.2f} (mV)")
-        print(f"Resistance: {self.r_in/1e6:.2f} (MOhms)")
-        print(f"tau: {self.tau:.2f} (ms)")
-        print()
+        self.index_v_rest = int(self.inj_delay / h.dt)
+        self.index_v_final = int(self.inj_stop / h.dt)
+        self.v_rest = self.v_vec[self.index_v_rest]
+        self.v_rest_time = self.t_vec[self.index_v_rest]
+        self.cell_v_final = self.v_vec[self.index_v_final]
+        self.v_final_time = self.t_vec[self.index_v_final]
+
+        t_idx = slice(self.index_v_rest, self.index_v_final + 1)
+        self.v_vec_inj = self.v_vec.as_numpy()[t_idx].copy()
+        self.t_vec_inj = self.t_vec.as_numpy()[t_idx].copy() - self.v_rest_time
 
-        v_rest_calc = "V_rest Calculation: Voltage taken at time " + str(self.v_rest_time) + "(ms)"
-        v_rest_calc1 = f"{self.v_rest:.2f} (mV)"
-        rin_calc = "R_in Calculation: [(dV/dI)] = (v_start-v_final)/(i_start-i_final)" 
-        rin_calc1 = "(" + str(round(self.v_rest,2)) + "-(" + str(round(self.cell_v_final,2))+"))/(0-(" + str(self.inj_amp) + "))"
-        rin_calc2 = str(round(self.v_rest-self.cell_v_final,2))+ " (mV) /" + str(0-self.inj_amp) + " (nA)"
-        rin_calc3 = str(round(((self.v_rest-self.cell_v_final)/(0-self.inj_amp)),2)) + " (MOhms)"
-
-        tau_calc = "Tau Calculation: [(s) until 63.2% change in mV]"
-        tau_calc1 = "(mV at inj_start_time (" + str(self.inj_delay) + ")) - ((mV at inj_time  - mV at inj_final (" + str(self.tstop) + ")) * 0.632)"
-        tau_calc2 = "(" + str(round(self.v_rest,2)) + ") - (" + str(round(self.v_rest,2)) +"-" +str(round(self.cell_v_final,2))+")*0.632 = " + str(round(self.v_rest - ((self.v_rest - self.cell_v_final)*0.632),2))
-        tau_calc3 = "Time where mV == " + str(round(self.v_t_const,2)) + " = " + str(self.inj_delay+self.tau) + "(ms) | (" + str(round(self.inj_delay+self.tau*1000,2)) + " - v_start_time (" + str(self.inj_delay) +"))/1000"
-        tau_calc4 = str(round(self.tau,4)) + " (ms)"
+        self.v_diff = self.cell_v_final - self.v_rest
+        self.r_in = self.v_diff / self.inj_amp # MegaOhms
 
-        print(v_rest_calc)
-        print(v_rest_calc1)
+        print_calc = self.tau_methods.get(self.method, self.tau_simple)()
+
+        print()
+        print(f'V Rest: {self.v_rest:.2f} (mV)')
+        print(f'Resistance: {self.r_in:.2f} (MOhms)')
+        print(f'Membrane time constant: {self.tau:.2f} (ms)')
         print()
-        print(rin_calc)
-        print(rin_calc1)
-        print(rin_calc2)
-        print(rin_calc3)
+        print(f'V_rest Calculation: Voltage taken at time {self.v_rest_time:.1f} (ms) is')
+        print(f'{self.v_rest:.2f} (mV)')
         print()
-        print(tau_calc)
-        print(tau_calc1)
-        print(tau_calc2) 
-        print(tau_calc3) 
-        print(tau_calc4)
-        print()  
-
-        return (list(self.t_vec), list(self.cell_vec))
-        #return (self.v_rest, self.r_in/1e6, self.tau)
-
-class FI():
-    def __init__(self,template_name, post_init_function=None,
-                 i_increment=100, i_start=0, i_stop=1050, tstart=50, tdur=1000,
-                 record_sec="soma", record_loc="0.5", inj_sec="soma", inj_loc="0.5"):
-        """ Takes in values of pA """
-        super(FI, self).__init__()
+        print('R_in Calculation: dV/dI = (v_final-v_rest)/(i_final-i_start)')
+        print(f'({self.cell_v_final:.2f} - ({self.v_rest:.2f})) / ({self.inj_amp:g} - 0)')
+        print(f'{np.sign(self.inj_amp) * self.v_diff:.2f} (mV) / {np.abs(self.inj_amp)} (nA) = {self.r_in:.2f} (MOhms)')
+        print_calc()
+
+        return self.t_vec.to_python(), self.v_vec.to_python()
+
+
+class FI(object):
+    def __init__(self, template_name, post_init_function=None,
+                 i_start=0., i_stop=1050., i_increment=100., tstart=50., tdur=1000., threshold=0.,
+                 record_sec='soma', record_loc=0.5, inj_sec='soma', inj_loc=0.5):
+        """
+        i_start: initial current injection amplitude (pA)
+        i_stop: maximum current injection amplitude (pA)
+        i_increment: amplitude increment each trial (pA)
+        tstart: current injection start time (ms)
+        tdur: current injection duration (ms)
+        """
         self.template_name = template_name
         self.post_init_function = post_init_function
-        self.i_increment = float(i_increment)/1e3
-        self.i_start = float(i_start)/1e3
-        self.i_stop = float(i_stop)/1e3
+        self.i_start = i_start * 1e-3 # pA to nA
+        self.i_stop = i_stop * 1e-3
+        self.i_increment = i_increment * 1e-3
         self.tstart = tstart
         self.tdur = tdur
+        self.tstop = tstart + tdur
+        self.threshold = threshold
 
         self.record_sec = record_sec
         self.record_loc = record_loc
         self.inj_sec = inj_sec
         self.inj_loc = inj_loc
 
-        self.tstop = tstart+tdur
         self.cells = []
         self.sources = []
         self.ncs = []
-        self.vectors = []
-        self.t_vec = h.Vector()
-        self.plenvec = []
+        self.tspk_vecs = []
+        self.nspks = []
 
-        self.amps = np.arange(self.i_start,self.i_stop,self.i_increment)
-        for _ in self.amps:
-            #Cell definition
-            cell = eval('h.'+self.template_name+'()')
+        self.ntrials = int((self.i_stop - self.i_start) // self.i_increment + 1)
+        self.amps = (self.i_start + np.arange(self.ntrials) * self.i_increment).tolist()
+        for _ in range(self.ntrials):
+            # Cell definition
+            cell = getattr(h, self.template_name)()
             if post_init_function:
                 eval(f"cell.{post_init_function}")
             self.cells.append(cell)
 
-        self.lenvec = None
-        self.ampvec = h.Vector([i*1e3 for i in self.amps])
-
-    def execute(self):
-        self.t_vec.record(h._ref_t)
+        self.setup()
 
-        for i, amp in enumerate(self.amps):
-            #Injection
-            cell = self.cells[i]
-
-            inj_str = "cell." + self.inj_sec + "(" + self.inj_loc + ")"
-            try:
-                inj_str = "cell." + self.inj_sec + "(" + self.inj_loc + ")"
-                src = h.IClamp(eval(inj_str))
-            except TypeError:
-                try:
-                    #print("Not using section " + inj_str)
-                    inj_str = "cell." + self.inj_sec + "[0](" + self.inj_loc + ")"
-                    #print("Trying " + inj_str)
-                    src = h.IClamp(eval(inj_str))
-                except:
-                    print("Hint: Are you selecting the correct injection location?")
-                    raise
+    def setup(self):
+        for cell, amp in zip(self.cells, self.amps):
+            inj_seg, _ = get_target_site(cell, self.inj_sec, self.inj_loc, 'injection')
+            src = h.IClamp(inj_seg)
             src.delay = self.tstart
             src.dur = self.tdur
             src.amp = amp
             self.sources.append(src)
 
-            #Recording
-            try:
-                rec_str = "cell." + self.record_sec + "(" + self.record_loc + ")._ref_v"
-                nc = h.NetCon(eval(rec_str),None,sec=eval("cell."+self.record_sec))
-            except TypeError:
-                try:
-                    rec_str = "cell." + self.record_sec + "[0](" + self.record_loc + ")._ref_v"
-                    nc = h.NetCon(eval(rec_str),None,sec=eval(f"cell.{self.record_sec}[0]"))
-                except:
-                    print("Hint: Are you selecting the correct recording location?")
-                    raise
-
-            nc.threshold = 0
+            rec_seg, rec_sec = get_target_site(cell, self.record_sec, self.record_loc, 'recording')
+            nc = h.NetCon(rec_seg._ref_v, None, sec=rec_sec)
+            nc.threshold = self.threshold
             spvec = h.Vector()
             nc.record(spvec)
             self.ncs.append(nc)
-            self.vectors.append(spvec)
-        
-        print(f"Injection location: {inj_str}")
-        print(f"Recording: {rec_str}")
-        print(f"Running FI curve simulation...")
-        print()
-        h.tstop = int(self.tstop)
+            self.tspk_vecs.append(spvec)
+
+        print(f'Injection location: {inj_seg}')
+        print(f'Recording: {rec_seg}._ref_v')
+
+    def execute(self):
+        print("Running simulations for FI curve...")
+        h.tstop = self.tstop
         h.stdinit()
         h.run()
 
-        self.plenvec = [len(list(i)) for i in self.vectors]
+        self.nspks = [len(v) for v in self.tspk_vecs]
+        print()
         print("Results")
-        print(f"Rates: {list(self.amps)}")
-        print(f"Spikes: {self.plenvec}")
+        print(f'Injection (nA): ' + ', '.join(f'{x:g}' for x in self.amps))
+        print(f'Number of spikes: ' + ', '.join(f'{x:d}' for x in self.nspks))
         print()
 
-        return (list(self.amps), list(self.plenvec))
+        return self.amps, self.nspks
+
+
+class ZAP(CurrentClamp):
+    def __init__(self, template_name, inj_amp=100., inj_delay=200., inj_dur=15000.,
+                 tstop=15500., fstart=0., fend=15., chirp_type=None, **kwargs):
+        """
+        fstart, fend: float, frequency at the start and end of the chirp current
+        chirp_type: {'linear', 'exponential'}, optional.
+            Type of chirp current, i.e. how frequency increase over time.
+        """
+        assert(inj_amp != 0)
+        super().__init__(template_name=template_name, tstop=tstop,
+                         inj_amp=inj_amp, inj_delay=inj_delay, inj_dur=inj_dur, **kwargs)
+        self.inj_stop = inj_delay + inj_dur
+        self.fstart = fstart
+        self.fend = fend
+        self.chirp_type = chirp_type
+        self.chirp_func = {'linear': self.linear_chirp, 'exponential': self.exponential_chirp}
+        if chirp_type=='exponential':
+            assert(fstart > 0 and fend > 0)
+
+    def linear_chirp(self, t, f0, f1):
+        return self.inj_amp * np.sin(np.pi * (2 * f0 + (f1 - f0) / t[-1] * t) * t)
+
+    def exponential_chirp(self, t, f0, f1):
+        L = np.log(f1 / f0) / t[-1]
+        return self.inj_amp * np.sin(np.pi * 2 * f0 / L * (np.exp(L * t) - 1))
+
+    def zap_current(self):
+        self.dt = dt = h.dt
+        self.index_v_rest = int(self.inj_delay / dt)
+        self.index_v_final = int(self.inj_stop / dt)
+
+        t = np.arange(int(self.tstop / dt) + 1) * dt
+        t_inj = t[:self.index_v_final - self.index_v_rest + 1]
+        f0 = self.fstart * 1e-3 # Hz to 1/ms
+        f1 = self.fend * 1e-3
+        chirp_func = self.chirp_func.get(self.chirp_type, self.linear_chirp)
+        self.zap_vec_inj = chirp_func(t_inj, f0, f1)
+        i_inj = np.zeros_like(t)
+        i_inj[self.index_v_rest:self.index_v_final + 1] = self.zap_vec_inj
+
+        self.zap_vec = h.Vector()
+        self.zap_vec.from_python(i_inj)
+        self.zap_vec.play(self.cell_src._ref_amp, dt)
+
+    def get_impedance(self, smooth=1):
+        f_idx = (self.freq > min(self.fstart, self.fend)) & (self.freq < max(self.fstart, self.fend))
+        impedance = self.impedance
+        if smooth > 1:
+            impedance = np.convolve(impedance, np.ones(smooth) / smooth, mode='same')
+        freq, impedance = self.freq[f_idx], impedance[f_idx]
+        self.peak_freq = freq[np.argmax(impedance)]
+        print(f'Resonant Peak Frequency: {self.peak_freq:.3g} (Hz)')
+        return freq, impedance
+
+    def execute(self) -> Tuple[list, list]:
+        print("ZAP current simulation running...")
+        self.zap_current()
+        h.tstop = self.tstop
+        h.stdinit()
+        h.run()
+
+        self.zap_vec.resize(self.t_vec.size())
+        self.v_rest = self.v_vec[self.index_v_rest]
+        self.v_rest_time = self.t_vec[self.index_v_rest]
+
+        t_idx = slice(self.index_v_rest, self.index_v_final + 1)
+        self.v_vec_inj = self.v_vec.as_numpy()[t_idx].copy() - self.v_rest
+        self.t_vec_inj = self.t_vec.as_numpy()[t_idx].copy() - self.v_rest_time
+
+        self.cell_v_amp_max = np.abs(self.v_vec_inj).max()
+        self.Z = np.fft.rfft(self.v_vec_inj) / np.fft.rfft(self.zap_vec_inj) # MOhms
+        self.freq = np.fft.rfftfreq(self.zap_vec_inj.size, d=self.dt * 1e-3) # ms to sec
+        self.impedance = np.abs(self.Z)
+
+        print()
+        print('Chirp current injection with frequency changing from '
+              f'{self.fstart:g} to {self.fend:g} Hz over {self.inj_dur * 1e-3:g} seconds')
+        print('Impedance is calculated as the ratio of FFT amplitude '
+              'of membrane voltage to FFT amplitude of chirp current')
+        print()
+        return self.t_vec.to_python(), self.v_vec.to_python()
 
 
 class Profiler():
-    """All in one single cell profiler
-    """
-    def __init__(self, template_dir:str=None, mechanism_dir:str=None):
+    """All in one single cell profiler"""
+    def __init__(self, template_dir: str = None, mechanism_dir: str = None, dt=None):
         self.template_dir = None
         self.mechanism_dir = None
-        
+
         if not self.template_dir:
             self.template_dir = template_dir
         if not self.mechanism_dir:
             self.mechanism_dir = mechanism_dir
         self.templates = None
 
         self.load_templates()
-    
-    def load_templates(self,hoc_template_file=None):
+
+        h.load_file("stdrun.hoc")
+        if dt is not None:
+            h.dt = dt
+            h.steps_per_ms = 1 / h.dt
+
+    def load_templates(self, hoc_template_file=None):
         if self.templates is None: # Can really only do this once
             if self.mechanism_dir != './' and self.mechanism_dir != '.' and self.mechanism_dir != '././':
                 neuron.load_mechanisms(self.mechanism_dir)
-            h_base = dir(h)
+            h_base = set(dir(h))
 
             cwd = os.getcwd()
             os.chdir(self.template_dir)
             if not hoc_template_file:
                 self.hoc_templates = glob.glob("*.hoc")
                 for hoc_template in self.hoc_templates:
                     h.load_file(str(hoc_template))
             else:
                 self.hoc_templates = [hoc_template_file]
                 h.load_file(hoc_template_file)
 
             os.chdir(cwd)
 
-            #h.load_file('biophys_components/hoc_templates/Template.hoc')
+            # h.load_file('biophys_components/hoc_templates/Template.hoc')
             h_loaded = dir(h)
 
             self.templates = [x for x in h_loaded if x not in h_base]
 
         return self.templates
-    
-    def passive_properties(self, template_name:str, post_init_function:str=None, 
-                           record_sec:str='soma', inj_sec:str='soma', plot:bool=True,
-                           **kwargs) -> Tuple[list,list]:
+
+    def passive_properties(self, template_name: str, post_init_function: str = None,
+                           record_sec: str = 'soma', inj_sec: str = 'soma', plot: bool = True,
+                           method=None, **kwargs) -> Tuple[list, list]:
         """
         Calculates passive properties for the specified cell template_name
 
         Parameters
         ==========
-        template_name:str
+        template_name: str
             name of the cell template located in hoc
-        post_init_function:str
+        post_init_function: str
             function of the cell to be called after the cell has been initialized (like insert_mechs(123))
-        record_sec:str
+        record_sec: str
             section of the cell you want to record spikes from (default: soma)
-        inj_sec:str
-            section of the cell you want to inject current (default: soma)
-        plot:bool
+        inj_sec: str
+            section of the cell you want to inject current to (default: soma)
+        plot: bool
             automatically plot the cell profile
+        method: str
+            method to estimate membrane time constant (see Passive)
         **kwargs:
             extra key word arguments for Passive()
+
+        Returns time (ms), membrane voltage (mV)
     """
         passive = Passive(template_name, post_init_function=post_init_function,
-                          record_sec=record_sec, inj_sec=inj_sec, **kwargs)
-        time_vec, amp_vec = passive.execute()
+                          record_sec=record_sec, inj_sec=inj_sec, method=method, **kwargs)
+        time, amp = passive.execute()
 
         if plot:
             plt.figure()
-            plt.plot(time_vec, amp_vec)
+            plt.plot(time, amp)
+            if passive.method == 'exp2':
+                plt.plot(*passive.double_exponential_fit(), 'r:', label='double exponential fit')
+                plt.legend()
             plt.title("Passive Cell Current Injection")
             plt.xlabel('Time (ms)')
             plt.ylabel('Membrane Potential (mV)')
             plt.show()
 
-        return (time_vec, amp_vec)
-    
-    def current_injection(self, template_name:str, post_init_function:str=None, 
-                          record_sec:str='soma', inj_sec:str='soma', plot:bool=True,
-                          **kwargs) -> Tuple[list,list]:
-        
-        ccl = CurrentClamp(template_name, post_init_function=post_init_function, 
+        return time, amp
+
+    def current_injection(self, template_name: str, post_init_function: str = None,
+                          record_sec: str = 'soma', inj_sec: str = 'soma', plot: bool = True,
+                          **kwargs) -> Tuple[list, list]:
+
+        ccl = CurrentClamp(template_name, post_init_function=post_init_function,
                            record_sec=record_sec, inj_sec=inj_sec, **kwargs)
-        time_vec, amp_vec = ccl.execute()
+        time, amp = ccl.execute()
 
         if plot:
             plt.figure()
-            plt.plot(time_vec, amp_vec)
+            plt.plot(time, amp)
             plt.title("Current Injection")
             plt.xlabel('Time (ms)')
             plt.ylabel('Membrane Potential (mV)')
             plt.show()
 
-        return (time_vec, amp_vec)
-    
-    
-    def fi_curve(self, template_name:str, post_init_function=None, 
-                 record_sec:str='soma', inj_sec:str='soma', plot:bool=True,
-                 **kwargs) -> Tuple[list,list]:
+        return time, amp
+
+    def fi_curve(self, template_name: str, post_init_function: str = None,
+                 record_sec: str = 'soma', inj_sec: str = 'soma', plot: bool = True,
+                 **kwargs) -> Tuple[list, list]:
         """
         Calculates an FI curve for the specified cell template_name
 
         Parameters
         ==========
-        template_name:str
+        template_name: str
             name of the cell template located in hoc
-        post_init_function:str
+        post_init_function: str
             function of the cell to be called after the cell has been initialized (like insert_mechs(123))
-        record_sec:str
+        record_sec: str
             section of the cell you want to record spikes from (default: soma)
-        inj_sec:str
-            section of the cell you want to inject current (default: soma)
-        plot:bool
+        inj_sec: str
+            section of the cell you want to inject current to (default: soma)
+        plot: bool
             automatically plot an fi curve
 
-        Returns the nA used, number of spikes per nA supplied
-            list(amps), list(spikes)
-
+        Returns the injection amplitudes (nA) used, number of spikes per amplitude supplied
+            list(amps), list(# of spikes)
         """
         fi = FI(template_name, post_init_function=post_init_function,
                 record_sec=record_sec, inj_sec=inj_sec, **kwargs)
-        amp_vec, spike_vec = fi.execute()
+        amp, nspk = fi.execute()
 
         if plot:
             plt.figure()
-            plt.plot(amp_vec, spike_vec)
+            plt.plot(amp, nspk)
             plt.title("FI Curve")
             plt.xlabel('Injection (nA)')
             plt.ylabel('# Spikes')
             plt.show()
 
-        return (amp_vec, spike_vec)
+        return amp, nspk
+
+    def impedance_amplitude_profile(self, template_name: str, post_init_function: str = None,
+                                    record_sec: str = 'soma', inj_sec: str = 'soma', plot: bool = True,
+                                    chirp_type=None, smooth: int = 9, **kwargs) -> Tuple[list, list]:
+        """
+        chirp_type: str
+            Type of chirp current (see ZAP)
+        smooth: int
+            Window size for smoothing the impedance in frequency domain
+        **kwargs:
+            extra key word arguments for ZAP()
+        """
+        zap = ZAP(template_name, post_init_function=post_init_function,
+                  record_sec=record_sec, inj_sec=inj_sec, chirp_type=chirp_type, **kwargs)
+        time, amp = zap.execute()
+
+        if plot:
+            plt.figure()
+            plt.plot(time, amp)
+            plt.title("ZAP Response")
+            plt.xlabel('Time (ms)')
+            plt.ylabel('Membrane Potential (mV)')
+
+            plt.figure()
+            plt.plot(time, zap.zap_vec)
+            plt.title('ZAP Current')
+            plt.xlabel('Time (ms)')
+            plt.ylabel('Current Injection (nA)')
+
+            plt.figure()
+            plt.plot(*zap.get_impedance(smooth=smooth))
+            plt.title('Impedance Amplitude Profile')
+            plt.xlabel('Frequency (Hz)')
+            plt.ylabel('Impedance (MOhms)')
+            plt.show()
 
+        return time, amp
 
-#Example usage
-#profiler = Profiler('./temp/templates', './temp/mechanisms/modfiles')
-#profiler.passive_properties('Cell_Cf')
-#profiler.fi_curve('Cell_Cf')
-#profiler.current_injection('Cell_Cf', post_init_function="insert_mechs(123)", inj_amp=300, inj_delay=100)
+# Example usage
+# profiler = Profiler('./temp/templates', './temp/mechanisms/modfiles')
+# profiler.passive_properties('Cell_Cf')
+# profiler.fi_curve('Cell_Cf')
+# profiler.current_injection('Cell_Cf', post_init_function="insert_mechs(123)", inj_amp=300, inj_delay=100)
```

### Comparing `bmtool-0.3.9/bmtool/util/commands.py` & `bmtool-0.4.0/bmtool/util/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/bmtool/util/neuron/celltuner.py` & `bmtool-0.4.0/bmtool/util/neuron/celltuner.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/bmtool/util/util.py` & `bmtool-0.4.0/bmtool/util/util.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/bmtool.egg-info/PKG-INFO` & `bmtool-0.4.0/bmtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.9
+Version: 0.4.0
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `bmtool-0.3.9/bmtool.egg-info/SOURCES.txt` & `bmtool-0.4.0/bmtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.9/setup.py` & `bmtool-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bmtool",
-    version="0.3.9",
+    version="0.4.0",
     author="Tyler Banks",
     author_email="tbanks@mail.missouri.edu",
     description="BMTool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tjbanks/bmtool",
     download_url='',
```

