# Comparing `tmp/aggregate-0.9.6.5.tar.gz` & `tmp/aggregate-0.9.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aggregate-0.9.6.5.tar", last modified: Tue Dec 20 09:24:14 2022, max compression
+gzip compressed data, was "aggregate-0.9.6.8.tar", last modified: Sun Jan  1 16:01:35 2023, max compression
```

## Comparing `aggregate-0.9.6.5.tar` & `aggregate-0.9.6.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-12-20 09:24:14.027011 aggregate-0.9.6.5/
--rw-rw-rw-   0        0        0     1522 2018-09-01 02:28:07.000000 aggregate-0.9.6.5/LICENSE
--rw-rw-rw-   0        0        0     1925 2022-12-20 09:24:14.026011 aggregate-0.9.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     3945 2022-11-29 09:45:51.000000 aggregate-0.9.6.5/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-20 09:24:14.017512 aggregate-0.9.6.5/aggregate/
--rw-rw-rw-   0        0        0     2415 2022-12-18 17:28:23.000000 aggregate-0.9.6.5/aggregate/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:24:14.025005 aggregate-0.9.6.5/aggregate/agg/
--rw-rw-rw-   0        0        0    19396 2022-11-11 12:19:04.000000 aggregate-0.9.6.5/aggregate/agg/test_suite.agg
--rw-rw-rw-   0        0        0    35610 2022-12-18 09:02:54.000000 aggregate-0.9.6.5/aggregate/bounds.py
--rw-rw-rw-   0        0        0       72 2022-12-18 09:00:15.000000 aggregate-0.9.6.5/aggregate/constants.py
--rw-rw-rw-   0        0        0   167278 2022-12-19 11:49:01.000000 aggregate-0.9.6.5/aggregate/distributions.py
--rw-rw-rw-   0        0        0    41475 2022-12-07 10:21:53.000000 aggregate-0.9.6.5/aggregate/parser.py
--rw-rw-rw-   0        0        0   275255 2022-12-19 15:44:03.000000 aggregate-0.9.6.5/aggregate/portfolio.py
--rw-rw-rw-   0        0        0    22855 2022-12-18 09:05:54.000000 aggregate-0.9.6.5/aggregate/spectral.py
--rw-rw-rw-   0        0        0    39339 2022-12-13 17:05:18.000000 aggregate-0.9.6.5/aggregate/underwriter.py
--rw-rw-rw-   0        0        0   113339 2022-12-19 10:37:48.000000 aggregate-0.9.6.5/aggregate/utilities.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:24:14.023514 aggregate-0.9.6.5/aggregate.egg-info/
--rw-rw-rw-   0        0        0     1925 2022-12-20 09:24:13.000000 aggregate-0.9.6.5/aggregate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2022-12-20 09:24:13.000000 aggregate-0.9.6.5/aggregate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-20 09:24:13.000000 aggregate-0.9.6.5/aggregate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2022-12-20 09:24:13.000000 aggregate-0.9.6.5/aggregate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-12-20 09:24:13.000000 aggregate-0.9.6.5/aggregate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-20 09:24:14.027011 aggregate-0.9.6.5/setup.cfg
--rw-rw-rw-   0        0        0     3369 2022-12-14 09:54:54.000000 aggregate-0.9.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-01 16:01:35.764093 aggregate-0.9.6.8/
+-rw-rw-rw-   0        0        0     1522 2018-09-01 02:28:07.000000 aggregate-0.9.6.8/LICENSE
+-rw-rw-rw-   0        0        0     2042 2023-01-01 16:01:35.764093 aggregate-0.9.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5928 2022-12-30 19:21:00.000000 aggregate-0.9.6.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-01-01 16:01:35.751214 aggregate-0.9.6.8/aggregate/
+-rw-rw-rw-   0        0        0     2517 2022-12-30 20:29:49.000000 aggregate-0.9.6.8/aggregate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-01 16:01:35.761083 aggregate-0.9.6.8/aggregate/agg/
+-rw-rw-rw-   0        0        0    19396 2022-11-11 12:19:04.000000 aggregate-0.9.6.8/aggregate/agg/test_suite.agg
+-rw-rw-rw-   0        0        0    35610 2022-12-18 09:02:54.000000 aggregate-0.9.6.8/aggregate/bounds.py
+-rw-rw-rw-   0        0        0      242 2022-12-31 09:18:18.000000 aggregate-0.9.6.8/aggregate/constants.py
+-rw-rw-rw-   0        0        0   166912 2022-12-31 09:17:25.000000 aggregate-0.9.6.8/aggregate/distributions.py
+-rw-rw-rw-   0        0        0    39486 2022-12-27 14:35:04.000000 aggregate-0.9.6.8/aggregate/parser.py
+-rw-rw-rw-   0        0        0   263041 2023-01-01 06:29:14.000000 aggregate-0.9.6.8/aggregate/portfolio.py
+-rw-rw-rw-   0        0        0    25292 2023-01-01 06:44:02.000000 aggregate-0.9.6.8/aggregate/spectral.py
+-rw-rw-rw-   0        0        0    35245 2023-01-01 06:51:11.000000 aggregate-0.9.6.8/aggregate/underwriter.py
+-rw-rw-rw-   0        0        0   114035 2022-12-31 09:21:47.000000 aggregate-0.9.6.8/aggregate/utilities.py
+drwxrwxrwx   0        0        0        0 2023-01-01 16:01:35.760083 aggregate-0.9.6.8/aggregate.egg-info/
+-rw-rw-rw-   0        0        0     2042 2023-01-01 16:01:35.000000 aggregate-0.9.6.8/aggregate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-01-01 16:01:35.000000 aggregate-0.9.6.8/aggregate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-01 16:01:35.000000 aggregate-0.9.6.8/aggregate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-01-01 16:01:35.000000 aggregate-0.9.6.8/aggregate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-01-01 16:01:35.000000 aggregate-0.9.6.8/aggregate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-01 16:01:35.764093 aggregate-0.9.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     3402 2023-01-01 16:01:21.000000 aggregate-0.9.6.8/setup.py
```

### Comparing `aggregate-0.9.6.5/LICENSE` & `aggregate-0.9.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aggregate-0.9.6.5/PKG-INFO` & `aggregate-0.9.6.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aggregate
-Version: 0.9.6.5
+Version: 0.9.6.8
 Summary: aggregate - working with compound probability distributions
 Author: Stephen J. Mildenhall
 Author-email: steve@convexrisk.com
 Maintainer: Stephen J. Mildenhall
 Maintainer-email: steve@convexrisk.com
 License: BSD
 Project-URL: Documentation, https://aggregate.readthedocs.io/en/latest/
@@ -13,28 +13,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Education
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Education
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 aggregate: a powerful aggregate distribution modeling library in Python
 ========================================================================
 
 What is it?
 -----------
 
-**aggregate** is a Python package providing an expressive language and fast,
-accurate computations to make working with aggregate (compound) probability
-distributions easy and intuitive. It allows students and practitioners to
-use realistic real-world distributions that reflect the underlying
-frequency and severity generating processes. It has applications in
-insurance, risk management, actuarial science, and related areas.
+``aggregate`` solves insurance, risk management, and actuarial problems using realistic models that reflect underlying frequency and severity.
+It delivers the speed and accuracy of parametric distributions to situations that usually require simulation, making it as easy to work with an aggregate (compound) probability distribution as the lognormal.
+``aggregate`` includes an expressive language called DecL to describe aggregate distributions and is implemented in Python under an open source BSD-license.
+
 
 Documentation
 -------------
 
 https://aggregate.readthedocs.io/
```

### Comparing `aggregate-0.9.6.5/aggregate/__init__.py` & `aggregate-0.9.6.8/aggregate/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     FigureManager, tweedie_convert, tweedie_density,\
     power_variance_family, \
     iman_conover, rearrangement_algorithm_max_VaR, \
     mu_sigma_from_mean_cv, \
     make_corr_matrix, random_corr_matrix, \
     LoggerManager, knobble_fonts, approximate_work, \
     partial_e, partial_e_numeric, moms_analytic, qd, \
-    sEngFormatter, mv, picks_work, GCN, lognorm_approx
+    sEngFormatter, mv, picks_work, GCN, lognorm_approx, \
+    integral_by_doubling
 from . spectral import Distortion
 from . distributions import Frequency, Severity, Aggregate
 from . portfolio import Portfolio, make_awkward
 from . underwriter import Underwriter, build, debug_build
 from . bounds import Bounds, plot_max_min, plot_lee
 from . constants import *
 
@@ -30,15 +31,15 @@
 __project__ = 'aggregate'
 __author__ = "Stephen J. Mildenhall"
 __copyright__ = "2018-2022, Convex Risk LLC"
 __license__ = "BSD 3-Clause New License"
 __email__ = "steve@convexrisk.com"
 __status__ = "alpha"
 # only need to change here, feeds conf.py (docs) and setup.py (build)
-__version__ = "0.9.6.5"
+__version__ = "0.9.6.8"
 
 # set up
 from pathlib import Path
 base_dir = Path.home() / 'aggregate'
 base_dir.mkdir(exist_ok=True)
 
 for p in ['cases', 'parser', 'temp', 'generated']:
@@ -53,14 +54,9 @@
 
 # as a default turn off all logging
 logger_level(30)
 knobble_fonts()
 
 # module level doc-string
 __doc__ = """
-**aggregate** is a Python package providing an expressive language and fast, accurate computations
-to make working with aggregate (compound) probability distributions
-easy and intuitive. It allows students and practitioners to work with realistic
-real-world distributions that reflect the underlying frequency and severity
-generating processes. It has applications in insurance, risk management, actuarial
-science, and related areas.
+:mod:`aggregate` solves insurance, risk management, and actuarial problems using realistic models that reflect underlying frequency and severity. It makes working with an aggregate (compound) probability distribution as easy as the lognormal, delivering the speed and accuracy of parametric distributions to situations that usually require simulation. :mod:`aggregate` includes an expressive language called DecL to describe aggregate distributions and is implemented in Python under an open source BSD-license.
 """
```

### Comparing `aggregate-0.9.6.5/aggregate/agg/test_suite.agg` & `aggregate-0.9.6.8/aggregate/agg/test_suite.agg`

 * *Files identical despite different names*

### Comparing `aggregate-0.9.6.5/aggregate/bounds.py` & `aggregate-0.9.6.8/aggregate/bounds.py`

 * *Files identical despite different names*

### Comparing `aggregate-0.9.6.5/aggregate/distributions.py` & `aggregate-0.9.6.8/aggregate/distributions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 import inspect
 import itertools
 import logging
 import matplotlib.ticker as ticker
 from matplotlib import pyplot as plt
 import numpy as np
 from numpy.linalg import inv
+from numpy.random import PCG64
 import pandas as pd
 from scipy.integrate import quad
 import scipy.stats as ss
 from scipy import interpolate
 from scipy.optimize import newton
-from IPython.core.display import display
 from scipy.special import kv, gammaln, hyp1f1
 from scipy.optimize import broyden2, newton_krylov
 from scipy.optimize.nonlin import NoConvergence
 from scipy.interpolate import interp1d
 from textwrap import fill
 
 from .constants import *
-from .utilities import sln_fit, sgamma_fit, ft, ift, \
+from .utilities import sln_fit, sgamma_fit, ln_fit, gamma_fit, ft, ift, \
     axiter_factory, estimate_agg_percentile, suptitle_and_tight, \
     MomentAggregator, xsden_to_meancv, round_bucket, make_ceder_netter, MomentWrangler, \
     make_mosaic_figure, nice_multiple, xsden_to_meancvskew, \
-    pprint_ex, approximate_work, moms_analytic, picks_work, GCN
+    pprint_ex, approximate_work, moms_analytic, picks_work, \
+    integral_by_doubling
 
 from .spectral import Distortion
 
 logger = logging.getLogger(__name__)
 
 
 class Frequency(object):
@@ -503,15 +504,15 @@
             if self.agg_density is None:
                 raise ValueError('Update Aggregate before asking for density_df')
 
             # really convenient to have p=p_total to be consistent with Portfolio objects
             self._density_df = pd.DataFrame(dict(loss=self.xs, p_total=self.agg_density))
             self._density_df['p'] = self._density_df.p_total
             # remove the fuzz, same method as Portfolio.remove_fuzz
-            eps = np.finfo(np.float).eps
+            eps = np.finfo(float).eps
             # may not have a severity, remember...
             self._density_df.loc[:, self._density_df.select_dtypes(include=['float64']).columns] = \
                 self._density_df.select_dtypes(include=['float64']).applymap(lambda x: 0 if abs(x) < eps else x)
 
             # we spend a lot of time computing sev exactly, so don't want to flush that away
             # with remove fuzz...hence add here
             self._density_df['p_sev'] = self.sev_density
@@ -586,15 +587,15 @@
         * both programs: agg is gcn for the agg program applied to the requested occ output
 
 
 
         ``_apply_reins_work``
         """
         if self.occ_reins is None and self.agg_reins is None:
-            logger.warning('Asking for reinsurance_df, but no reinsurance specified. Returning None.')
+            logger.log(WL, 'Asking for reinsurance_df, but no reinsurance specified. Returning None.')
             return None
 
         if self._reinsurance_df is None:
             self._reinsurance_df = \
                 pd.DataFrame({'loss': self.xs,
                               'p_sev_gross': self.sev_density_gross if
                               self.sev_density_gross is not None else self.sev_density,
@@ -637,20 +638,23 @@
         bit0 = self.reinsurance_audit_df.loc['occ'].xs('ex', axis=1, level=1)
         bit = self.reinsurance_audit_df.loc['occ'].xs('cv', axis=1, level=1)
         bit1 = pd.DataFrame(index=bit.index)
         bit1['ceded'] = [self.n if i == 'gup' else self.n * self.sev.sf(i)
                          for i in bit1.index.get_level_values('attach')]
         bit2 = pd.DataFrame(index=bit.index)
         # i = (share, layer, attach)
+        bit3 = bit0['ceded']
+        bit3 = bit3.iloc[:] / bit0['subject'].iloc[-1]
+        # TODO: not sure total cession is correct
         bit2['ceded'] = [v.ceded if i[-1] == 'gup' else v.ceded / self.sev.sf(i[-1] / i[0])
                          for i, v in bit0[['ceded']].iterrows()]
         ans = pd.concat((
             bit0 * self.n,
-            bit, bit1, bit2),
-            axis=1, keys=['ex', 'cv', 'en', 'severity'],
+            bit, bit1, bit2, bit3),
+            axis=1, keys=['ex', 'cv', 'en', 'severity', 'pct'],
             names=['stat', 'view'])
         return ans 
 
     @property
     def reinsurance_report_df(self):
         """
         Create and return a dataframe with the reinsurance report.
@@ -671,14 +675,15 @@
 
     def reinsurance_occ_plot(self, axs=None):
         """
         Plots for occurrence reinsurance: occurrence log density and aggregate quantile plot.
         """
         if axs is None:
             fig, axs = plt.subplots(1, 2, figsize=(2 * FIG_W, FIG_H), constrained_layout=True)
+            self.figure = fig
         ax0, ax1 = axs.flat
 
         self.occ_reins_df.filter(regex='p_[scn]').rename(columns=lambda x: x[2:]).plot(ax=ax0, logy=True)
         # TODO: better limit
         xl = ax0.get_xlim()
         l = self.spec['exp_limit']
         if type(l) != float:
@@ -913,15 +918,22 @@
         self.xs = None
         self.bs = 0
         self.log2 = 0
         # self.ex = 0 --> est_m
         self.est_m = 0
         self.est_cv = 0
         self.est_sd = 0
+        self.est_var = 0
         self.est_skew = 0
+        self.est_sev_m = 0
+        self.est_sev_cv = 0
+        self.est_sev_sd = 0
+        self.est_sev_var = 0
+        self.est_sev_skew = 0
+
         self.note = note
         self.program = ''  # can be set externally
         self.en = None     # this is for a sublayer e.g. for limit profile
         self.n = 0         # this is total frequency
         self.attachment = None
         self.limit = None
         self.agg_density = None
@@ -1092,14 +1104,20 @@
         self.n = ma.tot_freq_1
         self.agg_m = self.statistics_total_df.loc['mixed', 'agg_m']
         self.agg_cv = self.statistics_total_df.loc['mixed', 'agg_cv']
         self.agg_skew = self.statistics_total_df.loc['mixed', 'agg_skew']
         # variance and sd come up in exam questions
         self.agg_sd = self.agg_m * self.agg_cv
         self.agg_var = self.agg_sd * self.agg_sd
+        # severity exact moments
+        self.sev_m, self.sev_cv, self.sev_skew = self.statistics_total_df.loc['mixed',
+                                                                                          ['sev_m', 'sev_cv', 'sev_skew']]
+        self.sev_sd = self.sev_m * self.sev_cv
+        self.sev_var = self.sev_sd * self.sev_sd
+
         # finally, need a report_ser series for Portfolio to consolidate
         self.report_ser = ma.stats_series(self.name, np.max(self.limit), 0.999, remix=True)
         self._middle_q = None
         self._q = None
 
     def __repr__(self):
         """
@@ -1277,15 +1295,15 @@
 
         :param x:
         :return:
         """
         ix = self.density_df.index.get_loc(x, 'nearest')
         return self.density_df.iat[ix, 0]
 
-    def update(self, log2=13, bs=0, recommend_p=0.999, debug=False, **kwargs):
+    def update(self, log2=16, bs=0, recommend_p=0.999, debug=False, **kwargs):
         """
         Convenience function, delegates to update_work. Avoids having to pass xs. Also
         aliased as easy_update for backward compatibility.
 
         :param log2:
         :param bs:
         :param recommend_p: p value passed to recommend_bucket. If > 1 converted to 1 - 10**-p in rec bucket.
@@ -1294,15 +1312,15 @@
         :return:
         """
         # guess bucket and update
         if bs == 0:
             bs = round_bucket(self.recommend_bucket(log2, p=recommend_p))
         xs = np.arange(0, 1 << log2, dtype=float) * bs
         if 'approximation' not in kwargs:
-            if self.n > 100:
+            if self.n > 10000:
                 kwargs['approximation'] = 'slognorm'
             else:
                 kwargs['approximation'] = 'exact'
         return self.update_work(xs, debug=debug, **kwargs)
 
     # for backwards compatibility
     easy_update = update
@@ -1339,30 +1357,32 @@
         self.discretization_calc = discretization_calc
         self.normalize = normalize
         self.approximation = approximation
         self.padding = padding
         self.xs = xs
         self.bs = xs[1]
         # WHOA! WTF
-        self.log2 = int(np.log(len(xs)) / np.log(2))
+        self.log2 = int(np.log2(len(xs)))
 
         if type(tilt_vector) == float:
             tilt_vector = np.exp(-tilt_vector * np.arange(2**self.log2))
 
         # make the severity vector: a claim count weighted average of the severities
         if approximation == 'exact' or force_severity:
             wts = self.statistics_df.freq_1 / self.statistics_df.freq_1.sum()
+            if self.en.sum() == 0:
+                self.en = self.statistics_df.freq_1.values
             self.sev_density = np.zeros_like(xs)
             beds = self.discretize(sev_calc, discretization_calc, normalize)
             for temp, w, a, l, n in zip(beds, wts, self.attachment, self.limit, self.en):
                 self.sev_density += temp * w
 
             # adjust for picks if necessary
             if self.sev_pick_attachments is not None:
-                logger.warning('Adjusting for picks.')
+                logger.log(WL, 'Adjusting for picks.')
                 self.sev_density = self.picks(self.sev_pick_attachments, self.sev_pick_losses)
 
         if force_severity == 'yes':
             # only asking for severity (used by plot)
             return
 
         # deal with per occ reinsurance
@@ -1372,15 +1392,15 @@
             if self.sev_density_gross is not None:
                 # make the function an involution...
                 self.sev_density = self.sev_density_gross
             self.apply_occ_reins(debug)
 
         if approximation == 'exact':
             if self.n > 100:
-                logger.warning(f'Claim count {self.n} is high; consider an approximation ')
+                logger.info(f'Claim count {self.n} is high; consider an approximation ')
 
             if self.n == 0:
                 # for dynamics, it is helpful to have a zero risk return zero appropriately
                 # z = ft(self.sev_density, padding, tilt_vector)
                 self.agg_density = np.zeros_like(self.xs)
                 self.agg_density[0] = 1
                 # extreme idleness...but need to make sure it is the right shape and type
@@ -1402,24 +1422,37 @@
 
                 # NOW have to apply agg reinsurance to this line
                 self.apply_agg_reins(debug)
 
         else:
             # regardless of request if skew == 0 have to use normal
             # must check there is no per occ reinsurance... it won't work
-            assert self.occ_reins is None
+            if self.occ_reins is not None:
+                raise ValueError('Per occ reinsurance not supported with approximation')
+            if not np.isfinite(self.agg_cv):
+                raise ValueError('Cannot fit a distribution with infinite second moment.')
+            if self.agg_skew < 0:
+                logger.log(WL, 'Negative skewness, ignoring and fitting unshifted distribution.')
 
             if self.agg_skew == 0:
                 self.fzapprox = ss.norm(scale=self.agg_m * self.agg_cv, loc=self.agg_m)
             elif approximation == 'slognorm':
-                shift, mu, sigma = sln_fit(self.agg_m, self.agg_cv, self.agg_skew)
-                self.fzapprox = ss.lognorm(sigma, scale=np.exp(mu), loc=shift)
+                if np.isfinite(self.agg_skew) and self.agg_skew > 0:
+                    shift, mu, sigma = sln_fit(self.agg_m, self.agg_cv, self.agg_skew)
+                    self.fzapprox = ss.lognorm(sigma, scale=np.exp(mu), loc=shift)
+                else:
+                    mu, sigma = ln_fit(self.agg_m, self.agg_cv)
+                    self.fzapprox = ss.lognorm(sigma, scale=np.exp(mu))
             elif approximation == 'sgamma':
-                shift, alpha, theta = sgamma_fit(self.agg_m, self.agg_cv, self.agg_skew)
-                self.fzapprox = ss.gamma(alpha, scale=theta, loc=shift)
+                if np.isfinite(self.agg_skew) and self.agg_skew > 0:
+                    shift, alpha, theta = sgamma_fit(self.agg_m, self.agg_cv, self.agg_skew)
+                    self.fzapprox = ss.gamma(alpha, scale=theta, loc=shift)
+                else:
+                    alpha, theta = gamma_fit(self.agg_m, self.agg_cv)
+                    self.fzapprox = ss.gamma(alpha, scale=theta)
             else:
                 raise ValueError(f'Invalid approximation {approximation} option passed to CAgg density. '
                                  'Allowable options are: exact | slogorm | sgamma')
 
             ps = self.fzapprox.pdf(xs)
             self.agg_density = ps / np.sum(ps)
             self.ftagg_density = ft(self.agg_density, padding, tilt_vector)
@@ -1430,101 +1463,106 @@
         # originally...irritating no freq cv or sev cv
         # cols = ['name', 'limit', 'attachment', 'el', 'freq_1', 'sev_1', 'agg_m', 'agg_cv', 'agg_skew']
         cols = ['name', 'limit', 'attachment', 'el', 'freq_1', 'freq_cv', 'freq_skew',
                 'sev_1', 'sev_cv', 'sev_skew', 'agg_m', 'agg_cv', 'agg_skew']
         self.audit_df = pd.concat((self.statistics_df[cols],
                                    self.statistics_total_df.loc[['mixed'], cols]),
                                   axis=0)
-        # add empirical stats
+        # add empirical sev stats
         if self.sev_density is not None:
             _m, _cv, _sk = xsden_to_meancvskew(self.xs, self.sev_density)
         else:
             _m = np.nan
             _cv = np.nan
             _sk = np.nan
         self.audit_df.loc['mixed', 'emp_sev_1'] = _m
         self.audit_df.loc['mixed', 'emp_sev_cv'] = _cv
         self.audit_df.loc['mixed', 'emp_sev_skew'] = _sk
+        self.est_sev_m, self.est_sev_cv, self.est_sev_skew = _m, _cv, _sk
+        self.est_sev_sd = self.est_sev_m * self.est_sev_cv
+        self.est_sev_var = self.est_sev_sd * self.est_sev_sd
+        # add empirical agg stats
         _m, _cv, _sk = xsden_to_meancvskew(self.xs, self.agg_density)
         self.audit_df.loc['mixed', 'emp_agg_1'] = _m
+        self.audit_df.loc['mixed', 'emp_agg_cv'] = _cv
+        self.audit_df.loc['mixed', 'emp_agg_skew'] = _sk
         self.est_m = _m
         self.est_cv = _cv
         self.est_sd = _m * _cv
+        self.est_var = self.est_sd ** 2
         self.est_skew = _sk
-        self.audit_df.loc['mixed', 'emp_agg_cv'] = _cv
-        self.audit_df.loc['mixed', 'emp_agg_skew'] = _sk
 
         # invalidate stored functions
         self._cdf = None
 
-    def update_efficiently(self, xs, padding=1, approximation='exact', sev_calc='discrete',
-                           discretization_calc='survival', normalize=True):
-        """
-        Compute the density with absolute minimum overhead. Called by port.update_efficiently
-        Started with code for update and removed frills
-        No tilting!
-
-        :param xs:  range of x values used to discretize
-        :param padding: for FFT calculation
-        :param approximation: exact = perform frequency / severity convolution using FFTs. slognorm or
-          sgamma apply shifted lognormal or shifted gamma approximations.
-        :param sev_calc:   discrete = suitable for fft, continuous = for rv_histogram cts version
-        :param discretization_calc: use survival, distribution or both (=max(cdf, sf)) which is most accurate calc
-        :param normalize:  if True, normalize the density to sum to 1. For thick tail distributions, this may not
-          be appropriate and should be set to False.
-        :return:
-        """
-
-        self.xs = xs
-        self.bs = xs[1]
-        self.log2 = int(np.log(len(xs)) / np.log(2))
-        tilt_vector = None
-
-        # make the severity vector: a claim count weighted average of the severities
-        if approximation == 'exact':
-            wts = self.statistics_df.freq_1 / self.statistics_df.freq_1.sum()
-            self.sev_density = np.zeros_like(xs)
-            beds = self.discretize(sev_calc, discretization_calc, normalize)
-            for temp, w, a, l, n in zip(beds, wts, self.attachment, self.limit, self.en):
-                self.sev_density += temp * w
-
-        if approximation == 'exact':
-            if self.n == 0:
-                # for dynamics it is helpful to have a zero risk return zero appropriately
-                # z = ft(self.sev_density, padding, tilt_vector)
-                self.agg_density = np.zeros_like(self.xs)
-                self.agg_density[0] = 1
-                # extreme idleness...but need to make sure it is the right shape and type
-                self.ftagg_density = ft(self.agg_density, padding, tilt_vector)
-            else:
-                # usual calculation...this is where the magic happens!
-                z = ft(self.sev_density, padding, tilt_vector)
-                self.ftagg_density = self.mgf(self.n, z)
-                self.agg_density = np.real(ift(self.ftagg_density, padding, tilt_vector))
-        else:
-            # regardless of request if skew == 0 have to use normal
-            if self.agg_skew == 0:
-                self.fzapprox = ss.norm(scale=self.agg_m * self.agg_cv, loc=self.agg_m)
-            elif approximation == 'slognorm':
-                shift, mu, sigma = sln_fit(self.agg_m, self.agg_cv, self.agg_skew)
-                self.fzapprox = ss.lognorm(sigma, scale=np.exp(mu), loc=shift)
-            elif approximation == 'sgamma':
-                shift, alpha, theta = sgamma_fit(self.agg_m, self.agg_cv, self.agg_skew)
-                self.fzapprox = ss.gamma(alpha, scale=theta, loc=shift)
-            else:
-                raise ValueError(f'Invalid approximation {approximation} option passed to CAgg density. '
-                                 'Allowable options are: exact | slogorm | sgamma')
-
-            ps = self.fzapprox.pdf(xs)
-            self.agg_density = ps / np.sum(ps)
-            self.ftagg_density = ft(self.agg_density, padding, tilt_vector)
-
-        # invalidate stored functions
-        self._cdf = None
-        self.verbose_audit_df = None
+    # def update_efficiently(self, xs, padding=1, approximation='exact', sev_calc='discrete',
+    #                        discretization_calc='survival', normalize=True):
+    #     """
+    #     Compute the density with absolute minimum overhead. Called by port.update_efficiently
+    #     Started with code for update and removed frills
+    #     No tilting!
+    #
+    #     :param xs:  range of x values used to discretize
+    #     :param padding: for FFT calculation
+    #     :param approximation: exact = perform frequency / severity convolution using FFTs. slognorm or
+    #       sgamma apply shifted lognormal or shifted gamma approximations.
+    #     :param sev_calc:   discrete = suitable for fft, continuous = for rv_histogram cts version
+    #     :param discretization_calc: use survival, distribution or both (=max(cdf, sf)) which is most accurate calc
+    #     :param normalize:  if True, normalize the density to sum to 1. For thick tail distributions, this may not
+    #       be appropriate and should be set to False.
+    #     :return:
+    #     """
+    #
+    #     self.xs = xs
+    #     self.bs = xs[1]
+    #     self.log2 = int(np.log(len(xs)) / np.log(2))
+    #     tilt_vector = None
+    #
+    #     # make the severity vector: a claim count weighted average of the severities
+    #     if approximation == 'exact':
+    #         wts = self.statistics_df.freq_1 / self.statistics_df.freq_1.sum()
+    #         self.sev_density = np.zeros_like(xs)
+    #         beds = self.discretize(sev_calc, discretization_calc, normalize)
+    #         for temp, w, a, l, n in zip(beds, wts, self.attachment, self.limit, self.en):
+    #             self.sev_density += temp * w
+    #
+    #     if approximation == 'exact':
+    #         if self.n == 0:
+    #             # for dynamics it is helpful to have a zero risk return zero appropriately
+    #             # z = ft(self.sev_density, padding, tilt_vector)
+    #             self.agg_density = np.zeros_like(self.xs)
+    #             self.agg_density[0] = 1
+    #             # extreme idleness...but need to make sure it is the right shape and type
+    #             self.ftagg_density = ft(self.agg_density, padding, tilt_vector)
+    #         else:
+    #             # usual calculation...this is where the magic happens!
+    #             z = ft(self.sev_density, padding, tilt_vector)
+    #             self.ftagg_density = self.mgf(self.n, z)
+    #             self.agg_density = np.real(ift(self.ftagg_density, padding, tilt_vector))
+    #     else:
+    #         # regardless of request if skew == 0 have to use normal
+    #         if self.agg_skew == 0:
+    #             self.fzapprox = ss.norm(scale=self.agg_m * self.agg_cv, loc=self.agg_m)
+    #         elif approximation == 'slognorm':
+    #             shift, mu, sigma = sln_fit(self.agg_m, self.agg_cv, self.agg_skew)
+    #             self.fzapprox = ss.lognorm(sigma, scale=np.exp(mu), loc=shift)
+    #         elif approximation == 'sgamma':
+    #             shift, alpha, theta = sgamma_fit(self.agg_m, self.agg_cv, self.agg_skew)
+    #             self.fzapprox = ss.gamma(alpha, scale=theta, loc=shift)
+    #         else:
+    #             raise ValueError(f'Invalid approximation {approximation} option passed to CAgg density. '
+    #                              'Allowable options are: exact | slogorm | sgamma')
+    #
+    #         ps = self.fzapprox.pdf(xs)
+    #         self.agg_density = ps / np.sum(ps)
+    #         self.ftagg_density = ft(self.agg_density, padding, tilt_vector)
+    #
+    #     # invalidate stored functions
+    #     self._cdf = None
+    #     self.verbose_audit_df = None
 
     def picks(self, attachments, layer_loss_picks, debug=False):
         """
         Adjust the computed severity to hit picks targets in layers defined by a.
         Delegates work to ``utilities.picks_work``. See that function for details.
 
         """
@@ -1657,14 +1695,22 @@
         if self.occ_kind == 'ceded to':
             self.sev_density = self.sev_density_ceded
         elif self.occ_kind == 'net of':
             self.sev_density = self.sev_density_net
         else:
             raise ValueError(f'Unexpected kind of occ reinsurace, {self.occ_kind}')
 
+        # see impact on severity moments
+        _m2, _cv2, _sk2 = xsden_to_meancvskew(self.xs, self.sev_density)
+        self.est_sev_m = _m2
+        self.est_sev_cv = _cv2
+        self.est_sev_sd = _m2 * _cv2
+        self.est_sev_var = self.est_sev_sd ** 2
+        self.est_sev_skew = _sk2
+
     def apply_agg_reins(self, debug=False, padding=1, tilt_vector=None):
         """
         Apply the entire agg reins structure and save output
         For by layer detail create reins_audit_df
         Makes sev_density_gross, sev_density_net and sev_density_ceded, and updates sev_density to the requested view.
 
         Treatment in stats?
@@ -1702,14 +1748,15 @@
         # see impact on moments
         _m2, _cv2, _sk2 = xsden_to_meancvskew(self.xs, self.agg_density)
         # self.audit_df.loc['mixed', 'emp_agg_1'] = _m
         # old_m = self.ex
         self.est_m = _m2
         self.est_cv = _cv2
         self.est_sd = _m2 * _cv2
+        self.est_var = self.est_sd ** 2
         self.est_skew = _sk2
         # self.audit_df.loc['mixed', 'emp_agg_cv'] = _cv
         # invalidate quantile function
 
         logger.info(f'Applying agg reins to {self.name}\tOld mean and cv= {_m:,.3f}\t{_m:,.3f}\n'
                     f'New mean and cv = {_m2:,.3f}\t{_cv2:,.3f}')
 
@@ -2378,40 +2425,145 @@
                 if n == log2:
                     rbr = rb
                 print(f'Recommended bucket size with {2 ** n} buckets: {rb:,.3f}')
             if self.bs != 0:
                 print(f'Bucket size set with {N} buckets at {self.bs:,.3f}')
             return rbr
 
-    # def q_old(self, p):
-    #     """
-    #     Return lowest quantile, appropriate for discrete bucketing.
-    #     quantile guaranteed to be in the index
-    #     nearest does not work because you always want to pick rounding up
-    #
-    #     Definition 2.1 (Quantiles)
-    #
-    #     :math:`x(α) = qα(X) = inf\{x ∈ R : P[X ≤ x] ≥ α\}` is the lower α-quantile of X
-    #
-    #     :math:`x(α) = qα(X) = inf\{x ∈ R : P[X ≤ x] > α\}` is the upper α-quantile of X.
-    #
-    #     We use the x-notation if the dependence on X is evident, otherwise the q-notion.
-    #     Acerbi and Tasche (2002)
-    #
-    #     :param p:
-    #     :return:
-    #     """
-    #     if self._q is None:
-    #         self._q = interpolate.interp1d(self.density_df.F, self.density_df.loss, kind='linear')
-    #     l = float(self._q(p))
-    #     # find next nearest index value if not an exact match (this is slightly faster and more robust
-    #     # than l/bs related math)
-    #     l1 = self.density_df.index.get_loc(l, 'bfill')
-    #     l1 = self.density_df.index[l1]
-    #     return l1
+    def aggregate_error_analysis(self, log2, bs2_from=None, **kwargs):
+        """
+        Analysis of aggregate error across a range of bucket sizes. If ``bs2_from
+        is None`` use recommend_bucket plus/mins 3. Note: if distribution does
+        not have a second moment, you must enter bs2_from.
+
+        :param log2:
+        :param bs2_from: lower bound on bs to use, in log2 terms; estimate using
+          ``recommend_bucket`` if not input.
+        :param kwargs: passed to ``update``
+
+        """
+        # copy of self, updating alters the internal state of an object
+        cself = Aggregate(**self.spec)
+
+        if bs2_from is None:
+            if cself.agg_cv == np.inf:
+                raise ValueError('Distribution must have variance to guess bucket size. '
+                                 'Input bs2_from')
+            bs = self.recommend_bucket(log2)
+            bs = round_bucket(bs)
+            bs2 = int(np.log2(bs))
+            bss = 2. ** np.arange(bs2 - 3, bs2 + 4)
+        else:
+            bss = 2. ** np.arange(bs2_from, bs2_from + 7)
+
+        # analytic aggregate mean
+        m = cself.agg_m
+        # aggregate analysis
+        agg_ans = []
+        for bs in bss:
+            cself.update(bs=bs, log2=log2, approximation='exact', **kwargs)
+            agg_ans.append([bs, m, cself.est_m,
+                            cself.est_m - m, cself.est_m / m - 1])
+
+        agg_df = pd.DataFrame(agg_ans,
+                              columns=['bs', 'agg_m', 'est_m',
+                                       'abs_m', 'rel_m', ])
+        m = cself.sev_m
+        agg_df['rel_h'] = agg_df.bs / 2 / m
+        agg_df['rel_total'] = agg_df.rel_h * np.sign(agg_df.rel_m) + agg_df.rel_m
+        agg_df = agg_df.set_index('bs')
+        agg_df.columns = agg_df.columns.str.split('_', expand=True)
+        agg_df.columns.names = ['view', 'stat']
+        return agg_df
+
+    def severity_error_analysis(self, sev_calc='round', discretization_calc='survival',
+                                normalize=True):
+        """
+        Analysis of severity component errors, uses the current bs in self.
+        Gives detailed, component by component, error analysis of severities.
+        Includes discretization error (bs large relative to mean) and
+        truncation error (tail integral large).
+
+        Total S shows the aggregate not severity. Generally about self.n * (1 - sum_p)
+        (per Feller).
+
+        """
+        truncation_point = self.bs * (1 << self.log2)
+        wts = self.en / self.n
+        beds = self.discretize(sev_calc=sev_calc,
+                               discretization_calc=discretization_calc,
+                               normalize=normalize)
+        sev_ans = []
+        total_row = len(self.sevs)
+        for i, (s, wt, en, bed) in enumerate(zip(self.sevs, wts, self.en, beds)):
+            if len(self.sevs) == 1:
+                i = self.name
+            # exact
+            m = self.statistics.loc[('sev', 'ex1'), i]
+            # estimated
+            em, _ = xsden_to_meancv(self.xs, bed)
+            sev_ans.append([s.long_name,
+                            s.limit, s.attachment,
+                            truncation_point,
+                            s.sf(truncation_point), bed.sum(),
+                            wt, en,
+                            m, 0,
+                            m, em
+                            ])
+        # the total
+        m = self.sev_m
+        sev_ans.append(['total',
+                        self.limit.max(), self.attachment.min(),
+                        truncation_point,
+                        self.sf(truncation_point), self.density_df.p_sev.sum(),
+                        1, self.n,
+                        m, 0.,
+                        m, self.est_sev_m
+                        ])
+
+        sev_df = pd.DataFrame(sev_ans,
+                              columns=['name',
+                                       'limit', 'attachment',
+                                       'trunc',
+                                       'S', 'sum_p',
+                                       'wt', 'en',
+                                       'agg_mean', 'agg_wt',
+                                       'mean', 'est_mean'
+                                       ],
+                              index=range(total_row + 1))
+        sev_df['agg_mean'] *= sev_df['en']
+        sev_df['agg_wt'] = sev_df['agg_mean'] / \
+            sev_df.loc[0:total_row-1, 'agg_mean'].sum()
+        sev_df['abs'] = sev_df['est_mean'] - sev_df['mean']
+        sev_df['rel'] = sev_df['abs'] / sev_df['mean']
+        sev_df['trunc_error'] = \
+            [integral_by_doubling(s.sf, truncation_point) for s in self.sevs] + \
+            [integral_by_doubling(self.sev.sf, truncation_point)]
+        sev_df['rel_trunc_error'] = sev_df.trunc_error / sev_df['mean']
+        sev_df['h_error'] = self.bs / 2
+        sev_df['rel_h_error'] = self.bs / 2 / sev_df['mean']
+
+        # compute discretization_err_2 (was a separate function in development)
+        xs = np.hstack((self.xs - self.bs / 2, self.xs[-1] + self.bs / 2))
+        ans = []
+        for s in self.sevs:
+            # density at xs
+            f = s.pdf(xs)
+            # derv of f = -S''
+            df = np.gradient(f, self.bs)
+            # integral to quadratic adjustment term approx to S
+            ans.append(np.sum(df) * self.bs ** 3 / 24)
+        ans = pd.Series(ans)
+
+        sev_df['h2_adj'] = np.hstack((ans, 0.))
+        sev_df.loc[total_row, 'h2_adj'] = \
+            sev_df.loc[0:total_row - 1, ['wt', 'h2_adj']].prod(1).sum()
+        sev_df['rel_h2_adj'] = sev_df['h2_adj'] / sev_df['mean']
+
+        return sev_df
 
     def q(self, p, kind='lower'):
         """
         Compute quantile, returning element in the index. Exact same code from Portfolio.q.
 
         :param p:
         :param kind: lower, middle reproduces middle_q, upper
@@ -2475,126 +2627,14 @@
         l = float(self._sev_linear_quantile_function(p))
         # because we are not interpolating the returned value must (should) be in the index...
         if l not in self.density_df.index:
             logger.error(f'Unexpected weirdness in {self.name} severity quantile...computed {p}th percentile as {l} '
                          'which is not in the index but is expected to be. Make sure bs has nice binary expansion!')
         return l
 
-    # def careful_q(self, p):
-    #     """
-    #     Careful calculation of q handling jumps (based of SRM_Examples Noise class originally).
-    #     Note this is automatically vectorized and returns and array whereas q isn't.
-    #     It doesn't necessarily return an element of the index.
-    #
-    #     Just for reference here is code to illustrate the problem. This code is used in Vig_0_Audit.ipynb. ::
-    #
-    #         uw = agg.Underwriter()
-    #
-    #         def plot_eg_agg(b, e, w, n=32, axs=None, x_range=1):
-    #             '''
-    #             makes a tricky distribution function with a poss isolated jump
-    #             creates an agg object and checks the quantile function is correct
-    #
-    #             mass at w
-    #
-    #             '''
-    #
-    #             if axs is None:
-    #                 f, axs0 = plt.subplots(2,3, figsize=(9,6))
-    #                 axs = iter(axs0.flatten())
-    #
-    #             tm = np.linspace(0, 1, 33)
-    #             tf = lambda x : f'{32*x:.0f}'
-    #
-    #             def pretty(axis, ticks, formatter):
-    #                 maj = ticks[::4]
-    #                 mnr = [i for i in ticks if i not in maj]
-    #                 labels = [formatter(i) for i in maj]
-    #                 axis.set_ticks(maj)
-    #                 axis.set_ticks(mnr, True)
-    #                 axis.set_ticklabels(labels)
-    #                 axis.grid(True, 'major', lw=0.707, c='lightblue')
-    #                 axis.grid(True, 'minor', lw=0.35, c='lightblue')
-    #
-    #             # make the distribution
-    #             xs = np.linspace(0, x_range, n+1)
-    #             Fx = np.zeros_like(xs)
-    #             Fx[b:13] = 1
-    #             Fx[20:e] = 1
-    #             Fx[w] = 32 - np.sum(Fx)
-    #             Fx = Fx / Fx.sum()
-    #             Fx = np.cumsum(Fx)
-    #
-    #             # make an agg version: find the jumps and create a dhistogram
-    #             temp = pd.DataFrame(dict(x=xs, F=Fx))
-    #             temp['f'] = np.diff(temp.F, prepend=0)
-    #             temp = temp.query('f > 0')
-    #             pgm = f'agg Tricky 1 claim sev dhistogram xps {temp.x.values} {temp.f.values} fixed'
-    #             a = uw(pgm)
-    #             a.easy_update(10, 0.001)
-    #             # plot
-    #             a.plot(axiter=axs)
-    #             pretty(axs0[0,0].xaxis, tm, tf)
-    #             pretty(axs0[0,2].xaxis, tm, tf)
-    #             pretty(axs0[0,2].yaxis, tm, tf)
-    #
-    #             # lower left plot: distribution function
-    #             ax = next(axs)
-    #             ax.step(xs, Fx, where='post', marker='.')
-    #             ax.plot(a.xs, a.agg_density.cumsum(), linewidth=3, alpha=0.5, label='from agg')
-    #             ax.set(title=f'b={b}, e={e}, w={w}', ylim=-0.05, aspect='equal')
-    #             if x_range  == 1:
-    #                 ax.set(aspect='equal')
-    #             ax.legend(frameon=False, loc='upper left')
-    #             pretty(ax.xaxis, tm, tf)
-    #             pretty(ax.yaxis, tm, tf)
-    #
-    #             # lower middle plot
-    #             ps = np.linspace(0, 1, 301)
-    #             agg_careful = a.careful_q(ps)
-    #             ax = next(axs)
-    #             ax.step(Fx, xs, where='pre', marker='.', label='input')
-    #             ax.plot(Fx, xs, ':', label='input joined')
-    #             ax.plot(ps, agg_careful, linewidth=1, label='agg careful')
-    #             ax.set(title='Inverse', ylim=-0.05)
-    #             if x_range  == 1:
-    #                 ax.set(aspect='equal')
-    #             pretty(ax.xaxis, tm, tf)
-    #             pretty(ax.yaxis, tm, tf)
-    #             ax.legend()
-    #
-    #             # lower right plot
-    #             ax = next(axs)
-    #             dmq = np.zeros_like(ps)
-    #             for i, p in enumerate(ps):
-    #                 try:
-    #                     dmq[i] = a.q(p)
-    #                 except:
-    #                     dmq[i] = 0
-    #             ax.plot(ps, agg_careful, label='careful (agg obj)', linewidth=1, alpha=1)
-    #             ax.plot(ps, dmq, label='agg version')
-    #             ax.legend(frameon=False, loc='upper left')
-    #             pretty(ax.xaxis, tm, tf)
-    #             pretty(ax.yaxis, tm, tf)
-    #             ax.set(title='Check with agg version')
-    #
-    #             plt.tight_layout()
-    #
-    #             return a
-    #
-    #         aw = plot_eg_agg(6, 29, 16)
-    #
-    #     :param p: single or vector of values of ps, 0<1
-    #     :return:  quantiles
-    #     """
-    #     if self._careful_q is None:
-    #         self._careful_q = CarefulInverse.dist_inv1d(self.xs, self.agg_density)
-    #
-    #     return self._careful_q(p)
-
     def tvar(self, p, kind='interp'):
         """
         Compute the tail value at risk at threshold p
 
         Definition 2.6 (Tail mean and Expected Shortfall)
         Assume E[X−] < ∞. Then
         x¯(α) = TM_α(X) = α^{−1}E[X 1{X≤x(α)}] + x(α) (α − P[X ≤ x(α)])
@@ -2671,24 +2711,26 @@
             if type(p) in [int, np.int, float, np.float]:
                 return float(self._inverse_tail_var(p))
             else:
                 return self._inverse_tail_var(p)
         else:
             raise ValueError(f'Inadmissible kind passed to tvar; options are interp (default) or tail')
 
-        # original version
-        # function not vectorized
-        # q = float(self.q(p, 'middle'))
-        # l1 = self.density_df.index.get_loc(q, 'bfill')
-        # q1 = self.density_df.index[l1]
-        #
-        # i1 = np.trapz(self.density_df.loc[q1:, 'S'], dx=self.bs)
-        # i2 = (q1 - q) * (2 - p - self.density_df.at[q1, 'F']) / 2  # trapz adj for first part
-        # return q + (i1 + i2) / (1 - p)
+    def sample(self, n, replace=True, random_state=None):
+        """
+        Draw a sample of n items from the aggregate distribution. Wrapper around
+        pd.DataFrame.sample.
 
+        """
+        bg = PCG64(random_state)
+        if self.density_df is None:
+            raise ValueError('Must update before sampling.')
+        return self.density_df[['loss']].sample(n=n, weights=self.density_df.p_total,
+                                                replace=replace, random_state=bg,
+                                                ignore_index=True)
 
     @property
     def sev(self):
         """
         Make exact sf, cdf and pdfs and store in namedtuple for use as sev.cdf etc.
         """
         if self._sev is None:
@@ -2708,33 +2750,14 @@
                     return np.sum([wts[i] * self.sevs[i].cdf(x) for i in range(len(self.sevs))], axis=0)
                 def _sev_sf(x):
                     return np.sum([wts[i] * self.sevs[i].sf(x) for i in range(len(self.sevs))], axis=0)
                 def _sev_pdf(x):
                     return np.sum([wts[i] * self.sevs[i].pdf(x) for i in range(len(self.sevs))], axis=0)
                 self._sev = SevFunctions(cdf=_sev_cdf, sf=_sev_sf, pdf=_sev_pdf)
         return self._sev
-    #
-    # def sev_cdf(self, x):
-    #     """
-    #     Direct access to the underlying weighted severity, exact computation.
-    #
-    #     """
-    #     if self._sev_cdf is None:
-    #         self._make_exact_cdfs()
-    #     return self._sev_cdf(x)
-    #
-    # def sev_sf(self, x):
-    #     if self._sev_cdf is None:
-    #         self._make_exact_cdfs()
-    #     return self._sev_sf(x)
-    #
-    # def sev_pdf(self, x):
-    #     if self._sev_cdf is None:
-    #         self._make_exact_cdfs()
-    #     return self._sev_pdf(x)
 
     def cdf(self, x, kind='previous'):
         """
         Return cumulative probability distribution at x using kind interpolation.
 
         2022-10 change: kind introduced; default was linear
 
@@ -2821,60 +2844,14 @@
             m, cv, skew = self.report_df.loc[['agg_m', 'agg_cv', 'agg_skew'], 'empirical']
 
         name = f'{approx_type[0:4]}.{self.name[0:5]}'
         agg_str = f'agg {name} 1 claim sev '
         note = f'frozen version of {self.name}'
         return approximate_work(m, cv, skew, name, agg_str, note, approx_type, output)
 
-        # if approx_type == 'norm':
-        #     sd = m*cv
-        #     if output=='scipy':
-        #         return ss.norm(loc=m, scale=sd)
-        #     sev = {'sev_name': 'norm', 'sev_scale': sd, 'sev_loc': m}
-        #     agg_str += f'{sd} @ norm 1 # {m} '
-        #
-        # elif approx_type == 'lognorm':
-        #     mu, sigma = mu_sigma_from_mean_cv(m, cv)
-        #     sev = {'sev_name': 'lognorm', 'sev_shape': sigma, 'sev_scale': np.exp(mu)}
-        #     if output=='scipy':
-        #         return ss.lognorm(sigma, scale=np.exp(mu-sigma**2/2))
-        #     agg_str += f'{np.exp(mu)} * lognorm {sigma} '
-        #
-        # elif approx_type == 'gamma':
-        #     shape = cv ** -2
-        #     scale = m / shape
-        #     if output=='scipy':
-        #         return ss.gamma(shape, scale=scale)
-        #     sev = {'sev_name': 'gamma', 'sev_a': shape, 'sev_scale': scale}
-        #     agg_str += f'{scale} * gamma {shape} '
-        #
-        # elif approx_type == 'slognorm':
-        #     shift, mu, sigma = sln_fit(m, cv, skew)
-        #     if output=='scipy':
-        #         return ss.lognorm(sigma, scale=np.exp(mu-sigma**2/2), loc=shift)
-        #     sev = {'sev_name': 'lognorm', 'sev_shape': sigma, 'sev_scale': np.exp(mu), 'sev_loc': shift}
-        #     agg_str += f'{np.exp(mu)} * lognorm {sigma} + {shift} '
-        #
-        # elif approx_type == 'sgamma':
-        #     shift, alpha, theta = sgamma_fit(m, cv, skew)
-        #     if output=='scipy':
-        #         return ss.gamma(alpha, loc=shift, scale=theta)
-        #     sev = {'sev_name': 'gamma', 'sev_a': alpha, 'sev_scale': theta, 'sev_loc': shift}
-        #     agg_str += f'{theta} * gamma {alpha} + {shift} '
-        #
-        # else:
-        #     raise ValueError(f'Inadmissible approx_type {approx_type} passed to fit')
-        #
-        # if output == 'agg':
-        #     agg_str += ' fixed'
-        #     return agg_str
-        # else:
-        #     return Aggregate(**{'name': name, 'note': f'frozen version of {self.name}',
-        #                         'exp_en': 1, **sev, 'freq_name': 'fixed'})
-
     fit = approximate
 
     def entropy_fit(self, n_moments, tol=1e-10, verbose=False):
         """
         Find the max entropy fit to the aggregate based on n_moments fit.
         The constant is added (sum of probabilities constraint), for two
         moments there are n_const = 3 constrains.
```

### Comparing `aggregate-0.9.6.5/aggregate/parser.py` & `aggregate-0.9.6.8/aggregate/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,16 @@
     literals = {'[', ']', '!', '(', ')'}
 
     # per manual, need to list longer tokens before shorter ones
     # simple but effective notes
     NOTE = r'note\{[^\}]*\}'  # r'[^\}]+'
     BUILTIN_AGG = r'agg\.[a-zA-Z][a-zA-Z0-9._:~]*'
     BUILTIN_SEV = r'sev\.[a-zA-Z][a-zA-Z0-9._:~]*'
-    # PORT_BUILTIN = r'port\.[a-zA-Z][a-zA-Z0-9_:~]*'
-    FREQ = 'binomial|pascal|poisson|bernoulli|geometric|fixed|neyman(a|A)?' # |empirical'
+    FREQ = 'binomial|pascal|poisson|bernoulli|geometric|fixed|neyman(a|A)?'
     DISTORTION = 'dist(ortion)?'
-
     # number regex including unary minus; need before MINUS else that grabs the minus sign in -3 etc.
     NUMBER = r'\-?(\d+\.?\d*|\d*\.\d+)([eE](\+|\-)?\d+)?'
     # NUMBER = r'(\d+\.?\d*|\d*\.\d+)([eE](\+|\-)?\d+)?'
 
     # do not allow _ in line names, use ~ or . or : instead: why: because p_ is used and _ is special
     # on honor system...really need two types of ID, it is OK in a portfolio name
     ID = r'[a-zA-Z][\.:~_a-zA-Z0-9]*'
@@ -128,19 +126,14 @@
     ID['to'] = TO
     ID['po'] = PART_OF
     ID['so'] = SHARE_OF
     ID['zm'] = ZM
     ID['zt'] = ZT
     ID['x'] = XS
 
-    # number regex including unary minus; need before MINUS else that grabs the minus sign in -3 etc.
-    # @_(r'\-?(\d+\.?\d*|\d*\.\d+)([eE](\+|\-)?\d+)?')
-    # def NUMBER(self, t):
-    #     return float(t.value)
-
     @_(r'\n+')
     def newline(self, t):
         self.lineno += t.value.count('\n')
 
     def error(self, t):
         logger.error(f"Illegal character '{t.value[0]:s}'")
         self.index += 1
@@ -889,21 +882,14 @@
         # if it is directly a sev_clause it cannot be adjusted
         self.logger(f'sev <-- BUILTIN_SEV ({p.BUILTIN_SEV})', p)
         built_in_dict = self.safe_lookup(p.BUILTIN_SEV)
         if 'name' in built_in_dict:
             del built_in_dict['name']
         return built_in_dict
 
-    # @_('BUILTIN_PORT')
-    # def builtin_port(self, p):
-    #     # ensure lookup only happens here
-    #     self.logger(f'builtin_agg <-- PORT_BUILTIN', p)
-    #     built_in_dict = self.safe_lookup(p.PORT_BUILTIN)
-    #     return built_in_dict
-
     # ids =========================================================
     @_('ID')
     def name(self, p):
         self.logger(f'name <-- ID = {p.ID}', p)
         return p.ID
 
     # vectors of numbers ==========================================
@@ -926,45 +912,14 @@
         return ans
 
     @_('expr')
     def numbers(self, p):
         self.logger('numbers <-- expr', p)
         return p.expr
 
-    # calculator ===================================================
-    # implement simple calculator with exponents and exp as a convenience,
-    # with % (divide by 100) and unary plus and minus
-    # mimics the Python grammar https://docs.python.org/3/reference/grammar.html
-    # too much bother...keep division, exp and **
-    # @_('sum %prec LOW')
-    # def expr(self, p):
-    #     self.logger('expr <-- sum', p)
-    #     return p.sum
-    #
-    # @_('sum PLUS term')
-    # def sum(self, p):
-    #     self.logger('sum <-- sum + term', p)
-    #     return p.sum + p.term
-    #
-    # @_('sum MINUS term')
-    # def sum(self, p):
-    #     self.logger('sum <-- sum - term', p)
-    #     return p.sum - p.term
-    #
-    # @_('term %prec LOW')
-    # def sum(self, p):
-    #     self.logger('term <-- sum', p)
-    #     return p.term
-    #
-    # @_('term TIMES factor')
-    # def term(self, p):
-    #     self.logger('term <-- term * factor', p)
-    #     return p.term * p.factor
-
-    # cut off here
     @_('term')
     def expr(self, p):
         self.logger('expr <-- term', p)
         return p.term
 
     @_('term DIVIDE factor')
     def term(self, p):
@@ -972,25 +927,14 @@
         return p.term / p.factor
 
     @_('factor')
     def term(self, p):
         self.logger('term <-- factor', p)
         return p.factor
 
-    # this causes an unresolvable difficulty with sev ID expr +expr
-    # can't tell if it is a two param dist or a location shift
-    # folded - into the regex def of a number
-    # @_('PLUS factor', 'MINUS factor')
-    # def factor(self, p):
-    #     self.logger(f'factor <-- {p[0]} factor', p)
-    #     if p[0] == '+':
-    #         return p.factor
-    #     else:
-    #         return -p.factor
-
     @_('power')
     def factor(self, p):
         self.logger('factor <-- power', p)
         return p.power
 
     @_('atom EXPONENT factor')
     def power(self, p):
@@ -1079,15 +1023,15 @@
         for rhs in v[1:]:
             s += f'{" "*20}\t | {rhs:<s}\n'
         s += '\n'
 
     # finally add the language words
     # this is a bit manual, but these shouldnt change much...
     # lang_words = '\n\nlanguage words go here\n\n'
-    lang_words = '''FREQ                    ::= 'binomial|poisson|bernoulli|pascal|geometric|fixed'
+    lang_words = '''FREQ                    ::= 'binomial|poisson|bernoulli|pascal|geometric|neymana?|fixed'
 
 BUILTINID               ::= 'sev|agg|port|meta.ID'
 
 NOTE                    ::= 'note{TEXT}'
 
 EQUAL_WEIGHT            ::= "="
 
@@ -1154,15 +1098,15 @@
 '''
 
     s += lang_words
     # create for docs in one file (that gets included by rst)
     if add_to_doc is True:
         pout.write_text(s, encoding='utf-8')
 
-    # save to user folder gammar
+    # save to user folder grammar
     if save_to_fn == '':
         save_to_fn = Path.home() / 'aggregate/parser/grammar.md'
     Path(save_to_fn).write_text(s, encoding='utf-8')
 
     return s
 
 if __name__ == '__main__':
```

### Comparing `aggregate-0.9.6.5/aggregate/portfolio.py` & `aggregate-0.9.6.8/aggregate/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 import matplotlib as mpl
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 from matplotlib.ticker import (MultipleLocator, StrMethodFormatter, MaxNLocator,
                                FixedLocator, FixedFormatter, AutoMinorLocator)
 import numpy as np
+from numpy.random import PCG64
 import pandas as pd
 from pandas.io.formats.format import EngFormatter
 from pathlib import Path
-import pypandoc
 import re
 import scipy.stats as ss
 from scipy import interpolate
 from scipy.interpolate import interp1d
 from scipy.spatial import ConvexHull
 from textwrap import fill
 from IPython.core.display import HTML, display
 
 from .constants import *
 from .distributions import Aggregate, Severity
 from .spectral import Distortion
 from .utilities import ft, \
     ift, sln_fit, sgamma_fit, \
     axiter_factory, AxisManager, html_title, \
-    suptitle_and_tight, \
+    suptitle_and_tight, pprint_ex, \
     MomentAggregator, Answer, subsets, round_bucket, \
     make_mosaic_figure, iman_conover, approximate_work
 
 # fontsize : int or float or {'xx-small', 'x-small', 'small', 'medium', 'large', 'x-large', 'xx-large'}
 # matplotlib.rcParams['legend.fontsize'] = 'xx-small'
 logger = logging.getLogger(__name__)
 
@@ -86,30 +86,30 @@
         ma = MomentAggregator()
         max_limit = 0
         if (len(spec_list) == 1 and isinstance(spec_list[0], pd.DataFrame)):
             # create from samples...slightly different looping behavior
             logger.info('Creating from sample DataFrame')
             spec_list = spec_list[0]
         if isinstance(spec_list, pd.DataFrame):
-            if 'p_total' in spec_list:
-                probs = spec_list['p_total'].to_numpy()
-            else:
-                probs = np.repeat(1 / len(spec_list), len(spec_list))
+            if 'p_total' not in spec_list:
+                logger.info('Adding p_total column to DataFrame with equal probs')
+                spec_list = spec_list.copy()
+                spec_list['p_total'] = np.repeat(1 / len(spec_list), len(spec_list))
 
         for spec in spec_list:
             if isinstance(spec, Aggregate):
                 # directly passed in an agg object
                 a = spec
                 agg_name = spec.name
             elif isinstance(spec, str) and isinstance(spec_list, pd.DataFrame):
                 if spec not in ['total', 'p_total']:
-                    s = spec_list[spec].sort_values().to_numpy()
+                    s = spec_list[[spec, 'p_total']].groupby(spec).sum()
                     a = Aggregate(name=spec,
                                   exp_en=1,
-                                  sev_name='dhistogram', sev_xs=s, sev_ps=probs,
+                                  sev_name='dhistogram', sev_xs=s.index.values, sev_ps=s.p_total.values,
                                   freq_name='fixed')
                     agg_name = spec
                 else:
                     a = None
             elif isinstance(spec, str):
                 # look up object in uw return actual instance
                 # note here you could do uw.aggregate[spec] and get the dictionary def
@@ -162,15 +162,15 @@
         temp = pd.DataFrame(ma.stats_series('total', max_limit, 0.999, remix=False))
         self.statistics_df = pd.concat([temp_report, temp], axis=1)
         # future storage
         self.density_df = None
         self.augmented_df = None
         self.epd_2_assets = {}
         self.assets_2_epd = {}
-        self.priority_capital_df = None
+        self._priority_capital_df = None
         self.priority_analysis_df = None
         self.audit_df = None
         self.padding = 0
         self.tilt_amount = 0
         self._linear_quantile_function = None
         self._cdf = None
         self._pdf = None
@@ -219,29 +219,29 @@
 
     @property
     def distortion(self):
         return self._distortion
 
     def remove_fuzz(self, df=None, eps=0, force=False, log=''):
         """
-        remove fuzz at threshold eps. if not passed use np.finfo(np.float).eps.
+        remove fuzz at threshold eps. if not passed use np.finfo(float).eps.
 
         Apply to self.density_df unless df is not None
 
         Only apply if self.remove_fuzz or force
         :param eps:
         :param df:  apply to dataframe df, default = self.density_df
         :param force: do regardless of self.remove_fuzz
         :return:
         """
 
         if df is None:
             df = self.density_df
         if eps == 0:
-            eps = np.finfo(np.float).eps
+            eps = np.finfo(float).eps
 
         if self._remove_fuzz or force:
             logger.debug(f'Portfolio.remove_fuzz | Removing fuzz from {self.name} dataframe, caller {log}')
             df[df.select_dtypes(include=['float64']).columns] = \
                 df.select_dtypes(include=['float64']).applymap(lambda x: 0 if abs(x) < eps else x)
 
     def __repr__(self):
@@ -373,17 +373,17 @@
         sev_skew = self.statistics_df.loc[('sev', 'skew'), 'total']
         n_m = self.statistics_df.loc[('freq', 'ex1'), 'total']
         n_cv = self.statistics_df.loc[('freq', 'cv'), 'total']
         n_skew = self.statistics_df.loc[('freq', 'skew'), 'total']
         a_m = self.statistics_df.loc[('agg', 'ex1'), 'total']
         a_cv = self.statistics_df.loc[('agg', 'cv'), 'total']
         a_skew = self.statistics_df.loc[('agg', 'skew'), 'total']
-        df = pd.DataFrame({'E[X]': [sev_m, n_m, a_m], 'CV(X)': [sev_cv, n_cv, a_cv],
-                           'Skew(X)': [sev_skew, n_skew, a_skew]},
-                          index=['Sev', 'Freq', 'Agg'])
+        df = pd.DataFrame({'E[X]': [n_m, sev_m, a_m], 'CV(X)': [n_cv, sev_cv, a_cv],
+                           'Skew(X)': [n_skew, sev_skew, a_skew]},
+                          index=['Freq', 'Sev', 'Agg'])
         df.index.name = 'X'
 
         if self.audit_df is not None:
             df.loc['Sev', 'Est E[X]'] = np.nan
             df.loc['Agg', 'Est E[X]'] = self.est_m
             df['Err E[X]'] = df['Est E[X]'] / df['E[X]'] - 1
             df.loc['Sev', 'Est CV(X)'] = np.nan
@@ -393,14 +393,20 @@
             df.loc['Agg', 'Est Skew(X)'] = self.est_skew
             df = df[['E[X]', 'Est E[X]', 'Err E[X]', 'CV(X)', 'Est CV(X)', 'Err CV(X)', 'Skew(X)',
                      'Est Skew(X)']]
 
         t1 = [a.describe for a in self] + [df]
         t2 = [a.name for a in self] + ['total']
         df = pd.concat(t1, keys=t2, names=['unit', 'X']).fillna('')
+        if self.audit_df is not None:
+            # add estimated severity
+            sev_est_m = (df.xs('Sev', axis=0, level=1)['Est E[X]'].iloc[:-1].astype(float) *
+                df.xs('Freq', axis=0, level=1)['E[X]'].iloc[:-1]).sum() / df.loc[('total', 'Freq'), 'E[X]']
+            df.loc[('total', 'Sev'), 'Err E[X]'] = sev_est_m / df.loc[('total', 'Sev'), 'E[X]'] - 1
+            df.loc[('total', 'Sev'), 'Est E[X]'] = sev_est_m
         return df
 
     @property
     def spec(self):
         """
         Get the dictionary specification.
 
@@ -695,31 +701,14 @@
 
         try:
             return self.density_df.loc[x, 'p_total']
         except KeyError:
             return 0.0
             # raise KeyError(f'Value {x} must be in index for probability mass function.')
 
-    # # make some handy aliases; delete these go strictly with scipy.stats notation
-    # def F(self, x):
-    #     """
-    #     handy alias for distribution, CDF
-    #     :param x:
-    #     :return:
-    #     """
-    #     return self.cdf(x)
-    #
-    # def S(self, x):
-    #     """
-    #     handy alias for survival function, S
-    #     :param x:
-    #     :return:
-    #     """
-    #     return self.sf(x)
-
     def var(self, p):
         """
         value at risk = alias for quantile function
 
         :param p:
         :return:
         """
@@ -1033,15 +1022,15 @@
 
         # bs = sum([a.recommend_bucket(log2, p=recommend_p) for a in self])
         bs = sum([a.recommend_bucket(log2, p=recommend_p) ** 2 for a in self]) ** 0.5
 
         return round_bucket(bs)
 
     def update(self, log2, bs, approx_freq_ge=100, approx_type='slognorm', remove_fuzz=False,
-               sev_calc='discrete', discretization_calc='survival', normalize=True, padding=1, tilt_amount=0, epds=None,
+               sev_calc='discrete', discretization_calc='survival', normalize=True, padding=1, tilt_amount=0,
                trim_df=False, add_exa=True, force_severity=True, recommend_p=0.999, approximation=None, debug=False):
         """
 
         TODO: currently debug doesn't do anything...
 
         Create density_df, performs convolution. optionally adds additional information if ``add_exa=True``
         for allocation and priority analysis
@@ -1196,34 +1185,14 @@
         self.audit_df['MeanErr'] = self.audit_df['EmpMean'] / self.audit_df['Mean'] - 1
         self.audit_df['CVErr'] = self.audit_df['EmpCV'] / self.audit_df['CV'] - 1
         self.audit_df['SkewErr'] = self.audit_df['EmpSkew'] / self.audit_df['Skew'] - 1
 
         # add exa details
         if add_exa:
             self.add_exa(self.density_df, details=True)
-            # default priority analysis
-            logger.debug('Adding EPDs in Portfolio.update')
-            if epds is None:
-                epds = np.hstack(
-                    [np.linspace(0.5, 0.1, 4, endpoint=False)] +
-                    [np.linspace(10 ** -n, 10 ** -(n + 1), 9, endpoint=False) for n in range(1, 7)])
-                epds = np.round(epds, 7)
-            self.priority_capital_df = pd.DataFrame(index=pd.Index(epds))
-            for col in self.line_names:
-                for i in range(3):
-                    self.priority_capital_df['{:}_{:}'.format(col, i)] = self.epd_2_assets[(col, i)](epds)
-                    self.priority_capital_df['{:}_{:}'.format('total', 0)] = self.epd_2_assets[('total', 0)](
-                        epds)
-                col = 'not ' + col
-                for i in range(2):
-                    self.priority_capital_df['{:}_{:}'.format(col, i)] = self.epd_2_assets[(col, i)](epds)
-            self.priority_capital_df['{:}_{:}'.format('total', 0)] = self.epd_2_assets[('total', 0)](epds)
-            self.priority_capital_df.columns = self.priority_capital_df.columns.str.split("_", expand=True)
-            self.priority_capital_df.sort_index(axis=1, level=1, inplace=True)
-            self.priority_capital_df.sort_index(axis=0, inplace=True)
         else:
             # at least want F and S to get quantile functions
             self.density_df['F'] = np.cumsum(self.density_df.p_total)
             self.density_df['S'] = 1 - self.density_df.F
 
         self.ex = self.audit_df.loc['total', 'EmpMean']
         # pull out estimated stats to match Aggergate
@@ -1236,220 +1205,217 @@
         if trim_df:
             self.trim_df()
         # invalidate stored functions
         self._linear_quantile_function = None
         self.q_temp = None
         self._cdf = None
 
-    def update_efficiently(self, log2, bs, approx_freq_ge=100, approx_type='slognorm',
-                           sev_calc='discrete', discretization_calc='survival', normalize=True, padding=1):
-        """
-        Runs stripped down versions of update and add_exa.
-        Code copied from those routines and cleaned for comments etc.
-        NOT UPDATED FOR REINSURANCE.
-
-        TODO: is this enough of a speedup to be useful?
-
-
-        :param log2:
-        :param bs:
-        :param approx_freq_ge:
-        :param approx_type:
-        :param remove_fuzz:
-        :param sev_calc:
-        :param discretization_calc:
-        :param padding:
-        :return:
-        """
-        self.log2 = log2
-        self.bs = bs
-        self.padding = padding
-        self.approx_type = approx_type
-        self.sev_calc = sev_calc
-        self._remove_fuzz = True
-        self.approx_type = approx_type
-        self.approx_freq_ge = approx_freq_ge
-        self.discretization_calc = discretization_calc
-
-        ft_line_density = {}
-        N = 1 << log2
-        MAXL = N * bs
-        xs = np.linspace(0, MAXL, N, endpoint=False)
-        # no tilt for efficient mode
-        tilt_vector = None
-
-        # where the answer will live
-        self.density_df = pd.DataFrame(index=xs)
-        self.density_df['loss'] = xs
-        ft_all = None
-        for agg in self.agg_list:
-            raw_nm = agg.name
-            nm = f'p_{agg.name}'
-            _a = agg.update_efficiently(xs, self.padding, 'exact' if agg.n < approx_freq_ge else approx_type,
-                                        sev_calc, discretization_calc, normalize)
-            ft_line_density[raw_nm] = agg.ftagg_density
-            self.density_df[nm] = agg.agg_density
-            if ft_all is None:
-                ft_all = np.copy(ft_line_density[raw_nm])
-            else:
-                ft_all *= ft_line_density[raw_nm]
-        self.density_df['p_total'] = np.real(ift(ft_all, self.padding, tilt_vector))
-
-        # make the not self.line_density = sum of all but the given line
-        ft_nots = {}
-        for line in self.line_names:
-            ft_not = np.ones_like(ft_all)
-            if np.any(ft_line_density[line] == 0):
-                # have to build up
-                for not_line in self.line_names:
-                    if not_line != line:
-                        ft_not *= ft_line_density[not_line]
-            else:
-                if len(self.line_names) > 1:
-                    ft_not = ft_all / ft_line_density[line]
-            self.density_df[f'ημ_{line}'] = np.real(ift(ft_not, self.padding, tilt_vector))
-            ft_nots[line] = ft_not
-
-        self.remove_fuzz(log='update_efficiently')
-
-        # no audit statistics_df
-
-        # BEGIN add_exa ================================================================================================
-        # add exa details now in-line
-        # def add_exa(self, df, details, ft_nots=None):
-        # Call is self.add_exa(self.density_df, details=True)
-
-        # name in add_exa, keeps code shorter
-        df = self.density_df
-        cut_eps = np.finfo(np.float).eps
-
-        # sum of p_total is so important...we will rescale it...
-        if not np.all(df.p_total >= 0):
-            # have negative densities...get rid of them
-            first_neg = np.argwhere((df.p_total < 0).to_numpy()).min()
-        sum_p_total = df.p_total.sum()
-
-        df['F'] = np.cumsum(df.p_total)
-        df['S'] =  \
-            df.p_total.shift(-1, fill_value=min(df.p_total.iloc[-1], max(0, 1. - (df.p_total.sum()))))[::-1].cumsum()[::-1]
-
-        # E(min(X, a))
-        # df['exa_total'] = self.cumintegral(df['S'])
-        df['exa_total'] = df.S.shift(1, fill_value=0).cumsum() * self.bs
-        df['lev_total'] = df['exa_total']
-
-        df['exlea_total'] = \
-            (df.exa_total - df.loss * df.S) / df.F
-        n_ = df.shape[0]
-        if n_ < 1100:
-            mult = 1
-        elif n_ < 15000:
-            mult = 10
-        else:
-            mult = 100
-        loss_max = df[['loss', 'exlea_total']].query(' exlea_total>loss ').loss.max()
-        if np.isnan(loss_max):
-            loss_max = 0
-        else:
-            loss_max += mult * bs
-        # try nan in place of 0             V
-        df.loc[0:loss_max, 'exlea_total'] = np.nan
-
-        df['e_total'] = np.sum(df.p_total * df.loss)
-        df['exgta_total'] = df.loss + (df.e_total - df.exa_total) / df.S
-        df['exeqa_total'] = df.loss  # E(X | X=a) = a(!) included for symmetry was exa
-
-        # FFT functions for use in exa calculations
-        # computing sums so minimal padding required
-        def loc_ft(x):
-            return ft(x, 1, None)
-
-        def loc_ift(x):
-            return ift(x, 1, None)
-
-        # where is S=0
-        Seq0 = (df.S == 0)
-
-        for col in self.line_names:
-            df['exeqa_' + col] = \
-                np.real(loc_ift(loc_ft(df.loss * df['p_' + col]) *
-                                ft_nots[col])) / df.p_total
-            df.loc[df.p_total < cut_eps, 'exeqa_' + col] = 0
-            df['exeqa_ημ_' + col] = \
-                np.real(loc_ift(loc_ft(df.loss * df['ημ_' + col]) *
-                                loc_ft(df['p_' + col]))) / df.p_total
-            df.loc[df.p_total < cut_eps, 'exeqa_ημ_' + col] = 0
-            stemp = 1 - df['p_' + col].cumsum()
-            # df['lev_' + col] = self.cumintegral(stemp)
-            df['lev_' + col] = stemp.shift(1, fill_value=0).cumsum() * self.bs
-
-            stemp = 1 - df['ημ_' + col].cumsum()
-            df['lev_ημ_' + col] = stemp.shift(1, fill_value=0).cumsum() * self.bs
-
-            # EX_i | X<= a; temp is used in le and gt calcs
-            temp = np.cumsum(df['exeqa_' + col] * df.p_total)
-            df['exlea_' + col] = temp / df.F
-            df.loc[0:loss_max, 'exlea_' + col] = 0  # df.loc[0:loss_max, 'loss']
-            temp_not = np.cumsum(df['exeqa_ημ_' + col] * df.p_total)
-            df['exlea_ημ_' + col] = temp_not / df.F
-            df.loc[0:loss_max, 'exlea_ημ_' + col] = 0  # df.loc[0:loss_max, 'loss']
-
-            # constant value, helpful in calculations
-            # df['e_' + col] = np.sum(df['p_' + col] * df.loss)
-            # df['e_ημ_' + col] = np.sum(df['ημ_' + col] * df.loss)
-            #
-            # df['exgta_' + col] = (df['e_' + col] - temp) / df.S
-
-            # temp = df.loss.iloc[0]  # loss
-            # df.loss.iloc[0] = 1  # avoid divide by zero
-            #
-            # # df['exi_x_' + col] = np.sum(
-            # #     df['exeqa_' + col] * df.p_total / df.loss)
-            # temp_xi_x = np.cumsum(df['exeqa_' + col] * df.p_total / df.loss)
-            # df['exi_xlea_' + col] = temp_xi_x / df.F
-            # df.loc[0, 'exi_xlea_' + col] = 0  # df.F=0 at zero
-            # # more generally F=0 error:                      V
-            # df.loc[df.exlea_total == 0, 'exi_xlea_' + col] = 0
-            # # not version
-            # df['exi_x_ημ_' + col] = np.sum(
-            #     df['exeqa_ημ_' + col] * df.p_total / df.loss)
-            # # as above
-            # temp_xi_x_not = np.cumsum(
-            #     df['exeqa_ημ_' + col] * df.p_total / df.loss)
-            # df['exi_xlea_ημ_' + col] = temp_xi_x_not / df.F
-            # df.loc[0, 'exi_xlea_ημ_' + col] = 0  # df.F=0 at zero
-            # # more generally F=0 error:
-            # df.loc[df.exlea_total == 0, 'exi_xlea_ημ_' + col] = 0
-            # # put value back
-            # df.loss.iloc[0] = temp
-
-            # this is so important we will calculate it directly
-            df['exi_xgta_' + col] = ((df[f'exeqa_{col}'] / df.loss *
-                                      df.p_total).shift(-1)[
-                                     ::-1].cumsum()) / df.S
-            # need this NOT to be nan otherwise exa won't come out correctly
-            df.loc[Seq0, 'exi_xgta_' + col] = 0.
-            df['exi_xgta_ημ_' + col] = ((df[f'exeqa_ημ_{col}'] / df.loss *
-                                         df.p_total).shift(-1)[
-                                        ::-1].cumsum()) / df.S
-            df.loc[Seq0, 'exi_xgta_ημ_' + col] = 0.
-            df['exi_xeqa_' + col] = df['exeqa_' + col] / df['loss']
-            df.loc[0, 'exi_xeqa_' + col] = 0
-            df['exi_xeqa_ημ_' + col] = df['exeqa_ημ_' + col] / df['loss']
-            df.loc[0, 'exi_xeqa_ημ_' + col] = 0
-            df[f'exa_{col}'] = (df.S * df['exi_xgta_' + col]).shift(1, fill_value=0).cumsum() * self.bs
-            df['exa_ημ_' + col] = (df.S * df['exi_xgta_ημ_' + col]).shift(1, fill_value=0).cumsum() * self.bs
-
-        # END add_exa ==================================================================================================
+    @property
+    def priority_capital_df(self):
+        if self._priority_capital_df is None:
+            # default priority analysis
+            # never use these, so movaed out of main update
+            # TODO make a property and create on demand
+            logger.debug('Adding EPDs in Portfolio.update')
+            epds = np.hstack(
+                [np.linspace(0.5, 0.1, 4, endpoint=False)] +
+                [np.linspace(10 ** -n, 10 ** -(n + 1), 9, endpoint=False) for n in range(1, 7)])
+            epds = np.round(epds, 7)
+            self._priority_capital_df = pd.DataFrame(index=pd.Index(epds))
+            for col in self.line_names:
+                for i in range(3):
+                    self._priority_capital_df['{:}_{:}'.format(col, i)] = self.epd_2_assets[(col, i)](epds)
+                    self._priority_capital_df['{:}_{:}'.format('total', 0)] = self.epd_2_assets[('total', 0)](
+                        epds)
+                col = 'not ' + col
+                for i in range(2):
+                    self._priority_capital_df['{:}_{:}'.format(col, i)] = self.epd_2_assets[(col, i)](epds)
+            self._priority_capital_df['{:}_{:}'.format('total', 0)] = self.epd_2_assets[('total', 0)](epds)
+            self._priority_capital_df.columns = self._priority_capital_df.columns.str.split("_", expand=True)
+            self._priority_capital_df.sort_index(axis=1, level=1, inplace=True)
+            self._priority_capital_df.sort_index(axis=0, inplace=True)
+        return self._priority_capital_df
 
-        self.last_update = np.datetime64('now')
-        # invalidate stored functions
-        self._linear_quantile_function = None
-        self.q_temp = None
-        self._cdf = None
+    # def update_efficiently(self, log2, bs, approx_freq_ge=100, approx_type='slognorm',
+    #                        sev_calc='discrete', discretization_calc='survival', normalize=True, padding=1):
+    #     """
+    #     Runs stripped down versions of update and add_exa.
+    #     Code copied from those routines and cleaned for comments etc.
+    #     NOT UPDATED FOR REINSURANCE.
+    #
+    #     TODO: is this enough of a speedup to be useful?
+    #
+    #
+    #     :param log2:
+    #     :param bs:
+    #     :param approx_freq_ge:
+    #     :param approx_type:
+    #     :param remove_fuzz:
+    #     :param sev_calc:
+    #     :param discretization_calc:
+    #     :param padding:
+    #     :return:
+    #     """
+    #     self.log2 = log2
+    #     self.bs = bs
+    #     self.padding = padding
+    #     self.approx_type = approx_type
+    #     self.sev_calc = sev_calc
+    #     self._remove_fuzz = True
+    #     self.approx_type = approx_type
+    #     self.approx_freq_ge = approx_freq_ge
+    #     self.discretization_calc = discretization_calc
+    #
+    #     ft_line_density = {}
+    #     N = 1 << log2
+    #     MAXL = N * bs
+    #     xs = np.linspace(0, MAXL, N, endpoint=False)
+    #     # no tilt for efficient mode
+    #     tilt_vector = None
+    #
+    #     # where the answer will live
+    #     self.density_df = pd.DataFrame(index=xs)
+    #     self.density_df['loss'] = xs
+    #     ft_all = None
+    #     for agg in self.agg_list:
+    #         raw_nm = agg.name
+    #         nm = f'p_{agg.name}'
+    #         _a = agg.update_efficiently(xs, self.padding, 'exact' if agg.n < approx_freq_ge else approx_type,
+    #                                     sev_calc, discretization_calc, normalize)
+    #         ft_line_density[raw_nm] = agg.ftagg_density
+    #         self.density_df[nm] = agg.agg_density
+    #         if ft_all is None:
+    #             ft_all = np.copy(ft_line_density[raw_nm])
+    #         else:
+    #             ft_all *= ft_line_density[raw_nm]
+    #     self.density_df['p_total'] = np.real(ift(ft_all, self.padding, tilt_vector))
+    #
+    #     # make the not self.line_density = sum of all but the given line
+    #     ft_nots = {}
+    #     for line in self.line_names:
+    #         ft_not = np.ones_like(ft_all)
+    #         if np.any(ft_line_density[line] == 0):
+    #             # have to build up
+    #             for not_line in self.line_names:
+    #                 if not_line != line:
+    #                     ft_not *= ft_line_density[not_line]
+    #         else:
+    #             if len(self.line_names) > 1:
+    #                 ft_not = ft_all / ft_line_density[line]
+    #         self.density_df[f'ημ_{line}'] = np.real(ift(ft_not, self.padding, tilt_vector))
+    #         ft_nots[line] = ft_not
+    #
+    #     self.remove_fuzz(log='update_efficiently')
+    #
+    #     # no audit statistics_df
+    #
+    #     # BEGIN add_exa ================================================================================================
+    #     # add exa details now in-line
+    #     # def add_exa(self, df, details, ft_nots=None):
+    #     # Call is self.add_exa(self.density_df, details=True)
+    #
+    #     # name in add_exa, keeps code shorter
+    #     df = self.density_df
+    #     cut_eps = np.finfo(float).eps
+    #
+    #     # sum of p_total is so important...we will rescale it...
+    #     if not np.all(df.p_total >= 0):
+    #         # have negative densities...get rid of them
+    #         first_neg = np.argwhere((df.p_total < 0).to_numpy()).min()
+    #     sum_p_total = df.p_total.sum()
+    #
+    #     df['F'] = np.cumsum(df.p_total)
+    #     df['S'] =  \
+    #         df.p_total.shift(-1, fill_value=min(df.p_total.iloc[-1], max(0, 1. - (df.p_total.sum()))))[::-1].cumsum()[::-1]
+    #
+    #     # E(min(X, a))
+    #     # df['exa_total'] = self.cumintegral(df['S'])
+    #     df['exa_total'] = df.S.shift(1, fill_value=0).cumsum() * self.bs
+    #     df['lev_total'] = df['exa_total']
+    #
+    #     df['exlea_total'] = \
+    #         (df.exa_total - df.loss * df.S) / df.F
+    #     n_ = df.shape[0]
+    #     if n_ < 1100:
+    #         mult = 1
+    #     elif n_ < 15000:
+    #         mult = 10
+    #     else:
+    #         mult = 100
+    #     loss_max = df[['loss', 'exlea_total']].query(' exlea_total>loss ').loss.max()
+    #     if np.isnan(loss_max):
+    #         loss_max = 0
+    #     else:
+    #         loss_max += mult * bs
+    #     # try nan in place of 0             V
+    #     df.loc[0:loss_max, 'exlea_total'] = np.nan
+    #
+    #     df['e_total'] = np.sum(df.p_total * df.loss)
+    #     df['exgta_total'] = df.loss + (df.e_total - df.exa_total) / df.S
+    #     df['exeqa_total'] = df.loss  # E(X | X=a) = a(!) included for symmetry was exa
+    #
+    #     # FFT functions for use in exa calculations
+    #     # computing sums so minimal padding required
+    #     def loc_ft(x):
+    #         return ft(x, 1, None)
+    #
+    #     def loc_ift(x):
+    #         return ift(x, 1, None)
+    #
+    #     # where is S=0
+    #     Seq0 = (df.S == 0)
+    #
+    #     for col in self.line_names:
+    #         df['exeqa_' + col] = \
+    #             np.real(loc_ift(loc_ft(df.loss * df['p_' + col]) *
+    #                             ft_nots[col])) / df.p_total
+    #         df.loc[df.p_total < cut_eps, 'exeqa_' + col] = 0
+    #         df['exeqa_ημ_' + col] = \
+    #             np.real(loc_ift(loc_ft(df.loss * df['ημ_' + col]) *
+    #                             loc_ft(df['p_' + col]))) / df.p_total
+    #         df.loc[df.p_total < cut_eps, 'exeqa_ημ_' + col] = 0
+    #         stemp = 1 - df['p_' + col].cumsum()
+    #         # df['lev_' + col] = self.cumintegral(stemp)
+    #         df['lev_' + col] = stemp.shift(1, fill_value=0).cumsum() * self.bs
+    #
+    #         stemp = 1 - df['ημ_' + col].cumsum()
+    #         df['lev_ημ_' + col] = stemp.shift(1, fill_value=0).cumsum() * self.bs
+    #
+    #         # EX_i | X<= a; temp is used in le and gt calcs
+    #         temp = np.cumsum(df['exeqa_' + col] * df.p_total)
+    #         df['exlea_' + col] = temp / df.F
+    #         df.loc[0:loss_max, 'exlea_' + col] = 0  # df.loc[0:loss_max, 'loss']
+    #         temp_not = np.cumsum(df['exeqa_ημ_' + col] * df.p_total)
+    #         df['exlea_ημ_' + col] = temp_not / df.F
+    #         df.loc[0:loss_max, 'exlea_ημ_' + col] = 0  # df.loc[0:loss_max, 'loss']
+    #
+    #         # this is so important we will calculate it directly
+    #         df['exi_xgta_' + col] = ((df[f'exeqa_{col}'] / df.loss *
+    #                                   df.p_total).shift(-1)[
+    #                                  ::-1].cumsum()) / df.S
+    #         # need this NOT to be nan otherwise exa won't come out correctly
+    #         df.loc[Seq0, 'exi_xgta_' + col] = 0.
+    #         df['exi_xgta_ημ_' + col] = ((df[f'exeqa_ημ_{col}'] / df.loss *
+    #                                      df.p_total).shift(-1)[
+    #                                     ::-1].cumsum()) / df.S
+    #         df.loc[Seq0, 'exi_xgta_ημ_' + col] = 0.
+    #         df['exi_xeqa_' + col] = df['exeqa_' + col] / df['loss']
+    #         df.loc[0, 'exi_xeqa_' + col] = 0
+    #         df['exi_xeqa_ημ_' + col] = df['exeqa_ημ_' + col] / df['loss']
+    #         df.loc[0, 'exi_xeqa_ημ_' + col] = 0
+    #         df[f'exa_{col}'] = (df.S * df['exi_xgta_' + col]).shift(1, fill_value=0).cumsum() * self.bs
+    #         df['exa_ημ_' + col] = (df.S * df['exi_xgta_ημ_' + col]).shift(1, fill_value=0).cumsum() * self.bs
+    #
+    #     # END add_exa ==================================================================================================
+    #
+    #     self.last_update = np.datetime64('now')
+    #     # invalidate stored functions
+    #     self._linear_quantile_function = None
+    #     self.q_temp = None
+    #     self._cdf = None
 
     def trim_df(self):
         """
         Trim out unwanted columns from density_df
 
         epd used in graphics
 
@@ -1665,16 +1631,16 @@
         full_report_list = ['statistics', 'quick', 'audit', 'priority_capital', 'priority_analysis']
         if report_list == 'all':
             report_list = full_report_list
         for r in full_report_list:
             if r in report_list:
                 html_title(f'{r} Report for {self.name}', 1)
                 if r == 'priority_capital':
-                    if self.priority_capital_df is not None:
-                        display(self.priority_capital_df.loc[1e-3:1e-2, :].style)
+                    if self._priority_capital_df is not None:
+                        display(self._priority_capital_df.loc[1e-3:1e-2, :].style)
                     else:
                         html_title(f'Report {r} not generated', 2)
                 elif r == 'quick':
                     if self.audit_df is not None:
                         df = self.audit_df[['Mean', 'EmpMean', 'MeanErr', 'CV', 'EmpCV', 'CVErr', 'P99.0']]
                         display(df.style)
                     else:
@@ -1713,14 +1679,21 @@
                          'P99.0_emp','P99.6_emp']]
             df.columns.name = 'unit'
             df.index.name = 'statistic'
         else:
             df = None
         return df
 
+    @property
+    def pprogram(self):
+        """
+        pretty print the program to html
+        """
+        pprint_ex(self.program, 20)
+
     def limits(self, stat='range', kind='linear', zero_mass='include'):
         """
         Suggest sensible plotting limits for kind=range, density, .. (same as Aggregate).
 
         Should optionally return a locator for plots?
 
         Called by ploting routines. Single point of failure!
@@ -2114,32 +2087,32 @@
                 return x
 
             return new_fun
 
         # eps is used NOT to do silly things when x is so small F(x)< eps
         # below this percentile you do not try to condition on the event!
         # np.finfo(np.float).eps = 2.2204460492503131e-16
-        cut_eps = np.finfo(np.float).eps
+        cut_eps = np.finfo(float).eps
 
         # get this done
         # defuzz(self.density_df, cut_eps)
 
         # bucket size
         bs = self.bs  # self.density_df['loss'].iloc[1] - self.density_df['loss'].iloc[0]
         # index has already been reset
 
         # sum of p_total is so important...we will rescale it...
         if not np.all(df.p_total >= 0):
             # have negative densities...get rid of them
-            first_neg = df.query('p_total < 0')
-            logger.warning(
-                f'Portfolio.add_exa | p_total has a negative value starting at {first_neg.head()}; NOT setting to zero...')
+            first_neg = df.query(f'p_total < {-cut_eps}')
+            logger.log(WL,
+                # f'Portfolio.add_exa | p_total has a negative value starting at {first_neg.head()}; NOT setting to zero...')
+                f'p_total has {len(first_neg)} negative values; NOT setting to zero...')
         sum_p_total = df.p_total.sum()
-        logger.info(f'Portfolio.add_exa | {self.name}: sum of p_total is 1 - '
-                    f'{1 - sum_p_total:12.8e} NOT RESCALING')
+        logger.info(f'{self.name}: sum of p_total is 1 - {1 - sum_p_total:12.8e} NOT rescaling.')
         # df.p_total /= sum_p_total
         df['F'] = np.cumsum(df.p_total)
         # this method is terrible because you lose precision for very small values of S
         # df['S'] = 1 - df.F
         # old method
         # df['S'] = np.hstack((df.p_total.to_numpy()[:0:-1].cumsum()[::-1],
         #                      min(df.p_total.iloc[-1],
@@ -2726,15 +2699,15 @@
         ROE returned as COC in modern parlance.
         """
         if self.dist_ans is None:
             return None
 
         df = self.dist_ans.iloc[:, [0,4,5,6,7,8,9,10]].copy()
         df.index.names = ['a', 'LR', 'method']
-        df.columns = ['S', 'EL', 'P', 'PQ', 'Q', 'COC', 'param', 'error']
+        df.columns = ['S', 'L', 'P', 'PQ', 'Q', 'COC', 'param', 'error']
         return df
 
     def apply_distortions(self, dist_dict, As=None, Ps=None, kind='lower', axiter=None, num_plots=1, efficient=False):
         """
         Apply a list of distortions, summarize pricing and produce graphical output
         show loss values where  :math:`s_ub > S(loss) > s_lb` by jump
 
@@ -2887,16 +2860,18 @@
         # the original density_df
         # df.loc[df.p_total < 0, :] = 0
         # df['p_total'] = df['p_total'] / df['p_total'].sum()
         # df['F'] = df.p_total.cumsum()
         # df['S'] = 1 - df.F
 
         # floating point issues: THIS HAPPENS, so needs to be corrected...
+        cut_eps = np.finfo(float).eps
         if len(df.loc[df.S < 0, 'S'] > 0):
-            logger.warning(f"{len(df.loc[df.S < 0, 'S'] > 0)} negative S values being set to zero...")
+            logger.log(WL, f"{len(df.loc[df.S < -cut_eps, 'S'] > 0)} negative S < -eps values being set to zero...")
+            # logger.log(WL, f"{len(df.loc[df.S < 0, 'S'] > 0)} negative S values being set to zero...")
         df.loc[df.S < 0, 'S'] = 0
 
         # add the exag and distorted probs
         df['gS'] = g(df.S)
         df['gF'] = 1 - df.gS
         # updated for ability to prepend 0 in newer numpy
         # df['gp_total'] = np.diff(np.hstack((0, df.gF)))
@@ -2966,29 +2941,29 @@
 
         if dist.mass and mass_hints is None:
             idx_ess_sup = df.S.to_numpy().nonzero()[0][-1] + 1
             logger.info(f'Index of ess_sup is {idx_ess_sup}')
             # only add masses upto ess_sup
             # mass_S = pd.Series(0.0 index=df.index)
             # mass_S.iloc[:idx_ess_sup] =
-            # logger.warning('No mass_hints given...estimating...')
+            # logger.log(WL, 'No mass_hints given...estimating...')
             mass_hints = pd.Series(index=self.line_names)
             for line in self.line_names:
-                # logger.warning(f'Individual line={line}')
+                # logger.log(WL, f'Individual line={line}')
                 # print(f'Individual line={line}')
                 mass_hints[line] = df[f'exi_xeqa_{line}'].iloc[-1]
                 for ii in range(1, min(4, max(self.log2 - 8, 0))):
                     avg_xix = df[f'exi_xeqa_{line}'].iloc[idx_ess_sup - (1 << ii):].mean()
                     logger.debug(f'Avg weight last {1 << ii} observations is  = {avg_xix:.5g} vs. last trusted '
                                    f'is {mass_hints[line]:.5g}')
                                    # f'is {self.density_df[f"exi_xeqa_{line}"].iloc[idx_ess_sup]:.5g}')
                     # print(f'Avg weight last {1 << ii} observations is  = {avg_xix:.5g} vs. last '
                     #                f'is {mass_hints[line]:.5g}')
                 logger.debug('Generally, you want these values to be consistent, except for discrete distributions.')
-            logger.warning(f'No mass_hints given, using estimated mass_hints = {mass_hints.to_numpy()} for {dist.name}'
+            logger.log(WL, f'No mass_hints given, using estimated mass_hints = {mass_hints.to_numpy()} for {dist.name}'
                            f' mass {dist.mass} {dist}')
             # print(f'Using estimated mass_hints = {mass_hints.to_numpy()}')
 
 
         for line in self.line_names:
             # avoid double count: going up sum needs to be stepped one back, hence use cumintegral is perfect
             # for <=a cumintegral,  for > a reverse and use cumsum (no step back)
@@ -3022,20 +2997,20 @@
             # mass = 0
             # if dist.mass:
             #     logger.error("You cannot use a distortion with a mass at this time...")
             #     # this is John's problem: the last scenario is getting all the weight...
             #     # not clear how accurately this is computed numerically
             #     # this amount is a
             #     mass = total_mass * self.density_df[f'exi_xeqa_{line}'].iloc[idx_ess_sup]
-            #     logger.warning(f'Individual line={line} weight from portfolio mass = {mass}')
+            #     logger.log(WL, f'Individual line={line} weight from portfolio mass = {mass}')
             #     for ii in range(1, max(self.log2 - 4, 0)):
             #         avg_xix = self.density_df[f'exi_xeqa_{line}'].iloc[idx_ess_sup - (1 << ii):].mean()
-            #         logger.warning(f'Avg weight last {1 << ii} observations is  = {avg_xix:.5g} vs. last '
+            #         logger.log(WL, f'Avg weight last {1 << ii} observations is  = {avg_xix:.5g} vs. last '
             #                        f'is {self.density_df[f"exi_xeqa_{line}"].iloc[idx_ess_sup]}:.5g')
-            #     logger.warning('You want these values all to be consistent!')
+            #     logger.log(WL, 'You want these values all to be consistent!')
             # old
             # mass = dist.mass * self.density_df.loss * self.density_df[f'exi_xeqa_{line}'] * \
             #        np.where(self.density_df.S > 0, 1, 0)
 
             # when computed using np.cumsum exixgtaUC is a pd.Series has an index so when it is mult by .loss
             # (which also has an index) it gets re-sorted into ascending order
             # when computed using cumintegral it is a numpy array with no index and so need reversing
@@ -3450,15 +3425,15 @@
         if a is None:
             assert p is not None
             a = self.q(p, kind)
         else:
             p = self.cdf(a)
             ql = self.q(p, 'lower')
             qu = self.q(p, 'upper')
-            logger.warning(
+            logger.log(WL,
                 f'Input a={a} to gamma; computed p={p:.8g}, lower and upper quantiles are {ql:.8g} and {qu:.8g}')
 
         # alter in place or return a copy? For now return a copy...
         temp = self.density_df.filter(regex='^(p_|e1xi_1gta_|exi_xgta_|exi_xeqa_|'
                                     'exeqa_)[a-zA-Z]|^S$|^loss$').copy()
 
         # var dictionaries
@@ -3506,76 +3481,14 @@
             gam_name = f'gamma_{self.name}_{ln}'
             # unconditional version avoid divide and multiply by a small number
             # exeqa is closest to the raw output...
             temp[f'exi_x1gta_{ln}'] = (temp[f'exeqa_{ln}'] * temp.p_total / temp.loss).shift(-1)[::-1].cumsum() * self.bs
             temp[gam_name] = (min_xa * temp[f'exi_xeqa_{ln}'] * temp.p_total).shift(-1)[::-1].cumsum() / \
                              (temp[f'exi_x1gta_{ln}']) * self.bs
 
-        # other stuff helpful for plotting
-        # temp['BEST'] = 1
-        # temp.loc[a:, 'BEST'] = a / temp.loc[a:, 'loss']
-        # temp['WORST'] = np.maximum(0, 1 - temp.loc[a, 'S'] / temp.S)
-
-        # single plot
-        # if axs is not None:
-        #     axs = axs.flat
-        #     ax0 = axs[0]
-        #     renamer = self.renamer
-        #     temp.filter(regex='gamma|BEST|WORST').rename(columns=renamer).sort_index(1). \
-        #             plot(ylim=[-.05, 1.05], linewidth=1, ax=ax0)
-        #     for ln in ax0.lines[:2]:
-        #         lbl = ln.get_label()
-        #         if lbl == lbl.upper():
-        #             ln.set(linewidth=0.5, c='C7', linestyle='--' if lbl=='BEST' else ':', label=lbl.title())
-        #     nl = len(self.line_names)
-        #     for i, ln in enumerate(ax0.lines[2:-1:2]):
-        #         ln.set(c=f'C{i}')
-        #         ax0.lines[2*i+3].set(c=f'C{i}', lw=.5)
-        #         if ln.get_label().find('part of'):
-        #             ln.set(ls='-', lw=1)
-        #     ax0.lines[-1].set(lw=1, c='C7')
-        #     ax0.grid('b')
-        #     # update to reflect changes to line styles
-        #     ax0.legend()
-        #     ax0.set(title=f'Layer Effectiveness, a={a:,.0f} at p={p:.3f}', xlim=[0, extreme_var_dict['total']])
-        #
-        # # fancy comparison plots
-        # temp_ex = None
-        # if axs is not None:
-        #     # ax1 = return period scale, ax2 = linear scale, ax3 = survival functions
-        #     ax1, ax2 = axs[1:]
-        #
-            # temp_ex = temp.query(f'loss < {extreme_var_dict["total"]}').filter(regex='^gamma_|^p_')
-            # temp_ex[[f'S_{l[2:]}' for l in temp_ex.filter(regex='p_').columns]] = \
-            #     temp_ex.filter(regex='p_').shift(-1, fill_value=0).iloc[::-1].cumsum()
-        #     btemp = temp_ex.filter(regex='gamma_').rename(columns=renamer).sort_index(axis=1)
-        #     # first two plots are same except for scales
-        #     (1 / (1 - btemp.iloc[1:])).plot(logy=True, ylim=[0,1000], ax=ax1)
-        #     btemp.plot(ax=ax2, ylim=[0, 1.005])
-        #     ax1.set(title='Gamma Functions (Return Period Scale)')
-        #     ax2.set(title='Gamma Functions')
-        #     # third plot: like first but log S scale on x and y
-        #
-        #     # sort out colors
-        #     for ax in axs:
-        #         for i, line in enumerate(ax.lines[:-1:2]):
-        #             line.set(c=f'C{i}', lw=1)
-        #             ax.lines[2*i+1].set(c=f'C{i}', lw=.5)
-        #         ax.grid(which='major', axis='y')
-        #         ax.lines[2*nl].set(c='C7', lw=1)
-        #     # put in asset levels
-        #     for ax in axs:
-        #         for i, l in enumerate(self.line_names + [self.name]):
-        #             ln = ax.plot([var_dict[l], var_dict[l]], [1 if ax is ax1 else 0, ylim_zoom[1]],
-        #                          label=f'{l} s/a assets {var_dict[l]/1e6:,.1f}M')
-        #             ln[0].set(linewidth=.5, linestyle='--', c=f'C{i}')
-        #             # update legend to reflect line style changes
-        #         ax.lines[-1].set(c='C7')
-        #         ax.legend(loc='upper right')
-
         if axs is not None:
             axi = iter(axs.flat)
             nr, nc = axs.shape
             v = self.var_dict(.996, 'lower', 'total')
             ef = EngFormatter(3, True)
 
             if plot_mode == 'return':
@@ -4396,80 +4309,14 @@
         ax.legend(loc='upper left')
         # slightly evil
         ans.update(fig_distortion=f_distortion, fig_six_up_down=f_6_part,
             fig_trinity=f_trinity, fig_eight=f_8_part, fig_close=f_close)
 
         return ans
 
-    def top_down(self, distortions, A_or_p):
-        """
-        DataFrame summary and nice plots showing marginal and average ROE, lr etc. as you write a layer from x to A
-        If A=0 A=q(log) is used
-
-        Not integrated into graphics format (plot)
-
-        :param distortions: list or dictionary of CDistortion objects, or a single CDist object
-        :param A_or_p: if <1 interpreted as a quantile, otherwise assets
-        :return:
-        """
-
-        logger.warning('Portfolio.top_down is deprecated. It has been replaced by Portfolio.example_factory.')
-
-        # assert A_or_p > 0
-        #
-        # if A_or_p < 1:
-        #     # call with one arg and interpret as log
-        #     A = self.q(A_or_p)
-        # else:
-        #     A = A_or_p
-        #
-        # if isinstance(distortions, dict):
-        #     list_specs = distortions.values()
-        # elif isinstance(distortions, list):
-        #     list_specs = distortions
-        # else:
-        #     list_specs = [distortions]
-        #
-        # dfs = []
-        # for dist in list_specs:
-        #     g, g_inv = dist.g, dist.g_inv
-        #
-        #     S = self.density_df.S
-        #     loss = self.density_df.loss
-        #
-        #     a = A - self.bs  # A-bs for pandas series (includes endpoint), a for numpy indexing; int(A / self.bs)
-        #     lossa = loss[0:a]
-        #
-        #     Sa = S[0:a]
-        #     Fa = 1 - Sa
-        #     gSa = g(Sa)
-        #     premium = np.cumsum(gSa[::-1])[::-1] * self.bs
-        #     el = np.cumsum(Sa[::-1])[::-1] * self.bs
-        #     capital = A - lossa - premium
-        #     risk_margin = premium - el
-        #     assets = capital + premium
-        #     marg_roe = (gSa - Sa) / (1 - gSa)
-        #     lr = el / premium
-        #     roe = (premium - el) / capital
-        #     leverage = premium / capital
-        #     # rp = -np.log(Sa) # return period
-        #     marg_lr = Sa / gSa
-        #
-        #     # sns.set_palette(sns.color_palette("Paired", 4))
-        #     df = pd.DataFrame({'$F(x)$': Fa, '$x$': lossa, 'Premium': premium, r'$EL=E(X\wedge x)$': el,
-        #                        'Capital': capital, 'Risk Margin': risk_margin, 'Assets': assets, '$S(x)$': Sa,
-        #                        '$g(S(x))$': gSa, 'Loss Ratio': lr, 'Marginal LR': marg_lr, 'ROE': roe,
-        #                        'Marginal ROE': marg_roe, 'P:S levg': leverage})
-        #     df = df.set_index('$F(x)$', drop=True)
-        #     df.plot(subplots=True, rot=0, figsize=(14, 4), layout=(-1, 7))
-        #     suptitle_and_tight(f'{str(dist)}: Statistics for Layer $x$ to $a$ vs. $F(x)$')
-        #     df['distortion'] = dist.name
-        #     dfs.append(df)
-        # return pd.concat(dfs)
-
     def analysis_priority(self, asset_spec, output='df'):
         """
         Create priority analysis report_ser.
         Can be called multiple times with different ``asset_specs``
         asset_spec either a float used as an epd percentage or a dictionary. Entering an epd percentage
         generates the dictionary
 
@@ -4549,32 +4396,34 @@
             af2 = float(ea[(line, 1)](e))
             a3 = float(ea[(line, 2)](e))
             a4 = float(ea[(f'not {line}', 1)](e))
 
             story = f"""
 Consider adding **{line}** to the existing portfolio. The existing portfolio has capital {a:,.1f} and and epd of {e:.4g}.
 
-* If {line} is added as second priority to the existing lines with no increase in capital it has an epd of {e2:.4g}.
-* If the regulator requires the overall epd be a constant then the firm must increase capital to {a0:,.1f} or by {(a0 / a - 1) * 100:.2f} percent.
+<ul>
+<li> If {line} is added as second priority to the existing lines with no increase in capital it has an epd of {e2:.4g}.
+<li> If the regulator requires the overall epd be a constant then the firm must increase capital to {a0:,.1f} or by {(a0 / a - 1) * 100:.2f} percent.
     - At the higher capital {line} has an epd of {e2a0:.4g} as second priority and the existing lines have an epd of {eb0a0:.4g} as first priority.
     - The existing and {line} epds under equal priority are {eba0:.4g} and {e1a0:.4g}.
-* If {line} *thought* it was added at equal priority it would have expected an epd of {e1:.4g}.
+<li> If {line} *thought* it was added at equal priority it would have expected an epd of {e1:.4g}.
   In order to achieve this epd as second priority would require capital of {a2:,.1f}, an increase of {(a2 / a - 1) * 100:.2f} percent.
-* In order for {line} to have an epd equal to the existing lines as second priority would require capital
+<li> In order for {line} to have an epd equal to the existing lines as second priority would require capital
   of {a3:,.1f}, and increase of {(a3 / a - 1) * 100:.2f} percent.
-* In order for {line} to be added at equal priority and for the existing lines to have an unchanged epd requires capital of {af:,.1f}, an
+<li> In order for {line} to be added at equal priority and for the existing lines to have an unchanged epd requires capital of {af:,.1f}, an
   increase of {(af / a - 1) * 100:.2f} percent.
-* In order for {line} to be added at equal priority and to have an epd equal to the existing line epd requires capital of {af2:,.1f}, an
+<li> In order for {line} to be added at equal priority and to have an epd equal to the existing line epd requires capital of {af2:,.1f}, an
   increase of {(af2 / a - 1) * 100:.2f} percent.
-* In order for the existing lines to have an unchanged epd at equal priority requires capital of {a4:,.1f}, an increase of {(a4 / a - 1) * 100:.2f} percent.
+<li> In order for the existing lines to have an unchanged epd at equal priority requires capital of {a4:,.1f}, an increase of {(a4 / a - 1) * 100:.2f} percent.
+<ul>
 """
             ans.append(story)
         ans = '\n'.join(ans)
         if output == 'html':
-            display(HTML(pypandoc.convert_text(ans, to='html', format='markdown')))
+            display(HTML(ans))
         else:
             return ans
 
     def analysis_collateral(self, line, c, a, debug=False):
         """
         E(C(a,c)) expected value of line against not line with collateral c and assets a, c <= a
 
@@ -4967,158 +4816,14 @@
             a = self.q(p)
         elif p:
             a = self.q(p)
             # click to exact
             p = self.cdf(a)
         return a, float(p)
 
-    # def example_factory_sublines(self, data_in, xlim=0):
-    #     """
-    #     plausible plots for the specified example and a summary table
-    #
-    #     data_in is augmented_df or Answer object coming out of example_factory
-    #
-    #     example_factor is total; these exhibits look at subplots...
-    #
-    #     The line names must be of the form [A-Z]anything and identified by the capital letter
-    #
-    #     was agg extensions.plot_example
-    #
-    #     :param data_in: result of running self.apply_distortion()
-    #     :param xlim:         for plots
-    #     :return:
-    #     """
-    #
-    #     if isinstance(data_in, Answer):
-    #         augmented_df = data_in.augmented_df
-    #     else:
-    #         augmented_df = data_in
-    #
-    #     temp = augmented_df.filter(regex='exi_xgtag?_(?!sum)|^S|^gS|^(M|T)\.').copy()
-    #     # add extra stats
-    #     # you have:
-    #     # ['M.M_Atame', 'M.M_Dthick', 'M.M_total',
-    #     #  'M.Q_Atame', 'M.Q_Dthick', 'M.Q_total',
-    #     #  'M.ROE', 'S',
-    #     #  'T.LR_Atame', 'T.LR_Dthick', 'T.LR_total',
-    #     #  'T.M_Atame', 'T.M_Dthick', 'T.M_total',
-    #     #  'T.Q_Atame', 'T.Q_Dthick', 'T.Q_total',
-    #     #  'T.ROE_Atame', 'T.ROE_Dthick', 'T.ROE_total',
-    #     #  'exi_xgta_Atame', 'exi_xgta_Dthick',
-    #     #  'exi_xgtag_Atame', 'exi_xgtag_Dthick',
-    #     #  'gS']
-    #
-    #     # temp['M.LR'] = temp['M.L'] / temp['M.P']
-    #     # temp['M.ROE'] = (temp['M.P'] - temp['M.L']) / (1 - temp['M.P'])
-    #     # temp['M.M'] = temp['M.P'] - temp['M.L']
-    #     for l in self.line_names_ex:
-    #         if l != 'total':
-    #             temp[f'M.L_{l}'] = temp[f'exi_xgta_{l}'] * temp.S
-    #             temp[f'M.P_{l}'] = temp[f'exi_xgtag_{l}'] * temp.gS
-    #             # temp[f'M.M.{l}'] = temp[f'exi_xgtag_{l}'] * temp['M.P'] - temp[f'exi_xgta_{l}'] * temp['M.L']
-    #             temp[f'beta/alpha.{l}'] = temp[f'exi_xgtag_{l}'] / temp[f'exi_xgta_{l}']
-    #         else:
-    #             temp[f'M.L_{l}'] = temp.S
-    #             temp[f'M.P_{l}'] = temp.gS
-    #             # temp[f'M.M.{l}'] = temp['M.P'] - temp['M.L']
-    #         temp[f'M.LR_{l}'] = temp[f'M.L_{l}'] / temp[f'M.P_{l}']
-    #         # should be zero:
-    #         temp[f'Chk L+M=p_{l}'] = temp[f'M.P_{l}'] - temp[f'M.L_{l}'] - temp[f'M.M_{l}']
-    #
-    #     renamer = self.renamer.copy()
-    #     # want to recast these now too...(special)
-    #     renamer.update({'S': 'M.L total', 'gS': 'M.P total'})
-    #     augmented_df.index.name = 'Assets a'
-    #     temp.index.name = 'Assets a'
-    #     if xlim == 0:
-    #         xlim = self.q(1 - 1e-5)
-    #
-    #     f, axs = plt.subplots(4, 2, figsize=(8, 10), constrained_layout=True, squeeze=False)
-    #     ax = iter(axs.flatten())
-    #
-    #     # ONE
-    #     a = (1 - augmented_df.filter(regex='p_').cumsum()).rename(columns=renamer).sort_index(1). \
-    #         plot(ylim=[0, 1], xlim=[0, xlim], title='Survival functions', ax=next(ax))
-    #     a.grid('b')
-    #
-    #     # TWO
-    #     a = augmented_df.filter(regex='exi_xgtag?').rename(columns=renamer).sort_index(1). \
-    #         plot(ylim=[0, 1], xlim=[0, xlim], title=r'$\alpha=E[X_i/X | X>a],\beta=E_Q$ by Line', ax=next(ax))
-    #     a.grid('b')
-    #
-    #     # THREE total margins
-    #     a = augmented_df.filter(regex=r'^T\.M').rename(columns=renamer).sort_index(1). \
-    #         plot(xlim=[0, xlim], title='Total Margins by Line', ax=next(ax))
-    #     a.grid('b')
-    #
-    #     # FOUR marginal margins was dividing by bs end of first line
-    #     # for some reason the last entry in M.M_total can be problematic.
-    #     a = (augmented_df.filter(regex=r'^M\.M').rename(columns=renamer).sort_index(1).iloc[:-1, :].
-    #          plot(xlim=[0, xlim], title='Marginal Margins by Line', ax=next(ax)))
-    #     a.grid('b')
-    #
-    #     # FIVE
-    #     a = augmented_df.filter(regex=r'^M\.Q|gF').rename(columns=renamer).sort_index(1). \
-    #         plot(xlim=[0, xlim], title='Capital = 1-gS = F!', ax=next(ax))
-    #     a.grid('b')
-    #     for _ in a.lines:
-    #         if _.get_label() == 'gF':
-    #             _.set(linewidth=5, alpha=0.3)
-    #     # recreate legend because changed lines
-    #     a.legend()
-    #
-    #     # SIX see apply distortion, line 1890 ROE is in augmented_df
-    #     a = augmented_df.filter(regex='^ROE$|exi_xeqa').rename(columns=renamer).sort_index(1). \
-    #         plot(xlim=[0, xlim], title='M.ROE Total and $E[X_i/X | X=a]$ by line', ax=next(ax))
-    #     a.grid('b')
-    #
-    #     # SEVEN improve scale selection
-    #     a = temp.filter(regex='beta/alpha\.|M\.LR').rename(columns=renamer).sort_index(1). \
-    #         plot(ylim=[-.05, 1.5], xlim=[0, xlim], title='Alpha, Beta and Marginal LR',
-    #              ax=next(ax))
-    #     a.grid('b')
-    #
-    #     # EIGHT
-    #     a = augmented_df.filter(regex='LR').rename(columns=renamer).sort_index(1). \
-    #         plot(ylim=[-.05, 1.25], xlim=[0, xlim], title='Total ↑LR by Line',
-    #              ax=next(ax))
-    #     a.grid('b')
-    #
-    #     # return
-    #     if isinstance(data_in, Answer):
-    #         data_in['subline_summary'] = temp
-    #         data_in['fig_eight_plots'] = f
-    #     else:
-    #         data_in = Answer(summary=temp, fig_eight_by_line=f)
-    #     return data_in
-
-    # def cumintegral(self, v, bs_override=0):
-    #     """
-    #     cumulative integral of v with buckets size bs
-    #
-    #     :param bs_override:
-    #     :param v:
-    #     :return:
-    #     """
-    #
-    #     if bs_override != 0:
-    #         bs = bs_override
-    #     else:
-    #         bs = self.bs
-    #
-    #     if type(v) == np.ndarray:
-    #         logger.warning('CALLING cumintegral on a numpy array!!\n' * 5)
-    #         return np.hstack((0, v[:-1])).cumsum() * bs
-    #     else:
-    #         # was consistently (and obviously) the same
-    #         # t1 = np.hstack((0, v.values[:-1])).cumsum() * bs
-    #         # t2 = v.shift(1, fill_value=0).cumsum() * bs
-    #         # logger.warning(f'Alternative cumintegral allclose={np.allclose(t1, t2)}')
-    #         return v.shift(1, fill_value=0).cumsum() * bs
-
     @staticmethod
     def from_DataFrame(name, df):
         """
         create portfolio from pandas dataframe
         uses columns with appropriate names
 
         Can be fed the agg output of uw.write_test( agg_program )
@@ -5973,48 +5678,58 @@
             if min(pi, pj) <= premium <= max(pi, pj):
                 il = df.iat[i, 0]
                 ir = df.iat[i, 1]
                 jl = df.iat[j, 0]
                 jr = df.iat[j, 1]
                 w = (premium - pj) / (pi - pj)
                 wts[(il, ir, jl, jr)] = w
-                # spoon feed into a dummy distortion
+                # feed into a dummy distortion
                 temp = Distortion('ph', .599099)
                 temp.name = 'blend'
                 # temp.display_name  = f'Extension ({il}, {ir}), ({jl}, {jr})'
                 temp.g = lambda x: (
                         w * dists[(il, ir)](x) + (1 - w) * dists[(jl, jr)](x))
                 temp.g_inv = None
                 wdists[(il, ir, jl, jr)] = temp
-
+        if len(wdists) == 0:
+            # failed to extrapolate, but still want a reasonable blend
+            logger.warning('Failed to fit blend')
+            # TODO placeholder - FIX!
+            wdists[0] = Distortion('ph', .599099)
+            wdists[0].name = 'blend'
         if debug is True:
             return wdists, df, pricer, dists, wts
         else:
             return wdists
 
-    def resample(self, n, desired_correlation=None):
+    def sample(self, n, replace=True, random_state=None, desired_correlation=None, keep_total=True):
         """
-        Resample from port object lines
-        Apply Iman Conover if required
+        Pull multivariate sample. Apply Iman Conover to induce correlation if required.
 
         """
+        # bit generator
+        bg = PCG64(random_state)
         df = pd.DataFrame(index=range(n))
         for c in self.line_names:
             pc = f'p_{c}'
-            df[c] = self.density_df[['loss', pc]].query(f'`{pc}` > 0').\
-                sample(n, replace=True, weights=pc).\
-                drop(columns=pc).reset_index(drop=True)
+            df[c] = self.density_df[['loss', pc]].\
+                    query(f'`{pc}` > 0').\
+                    sample(n, replace=replace, weights=pc, ignore_index=True, random_state=bg).\
+                    drop(columns=pc)
 
         if desired_correlation is not None:
             df = iman_conover(df, desired_correlation)
         else:
             df['total'] = df.sum(axis=1)
-            df = df.set_index('total')
+            df = df.set_index('total', drop=not keep_total)
+        df = df.reset_index(drop=True)
         return df
 
+    resample = sample
+
     @property
     def unit_names(self):
         # what these should have been called!
         return self.line_names
 
     @property
     def unit_names_ex(self):
```

### Comparing `aggregate-0.9.6.5/aggregate/spectral.py` & `aggregate-0.9.6.8/aggregate/spectral.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,18 +290,19 @@
             raise ValueError(
                 "Incorrect spec passed to Distortion; implemented g types are ph, wang, tvar, "
                 "ly (linear yield), lep (layer equivalent pricing) and clin (clipped linear)")
 
         self.g = g
         self.g_inv = g_inv
 
-        def g_dual(x):
-            return 1 - self.g(x)
-
-        self.g_dual = g_dual
+    def g_dual(self, x):
+        """
+        The dual of the distortion function g.
+        """
+        return 1 - self.g(1 - x)
 
     def __str__(self):
         if self.display_name != '':
             s = self.display_name
             return s
         elif isinstance(self.shape, str):
             s = f'{self._distortion_names_.get(self._name, self._name)}, {self.shape}'
@@ -614,7 +615,68 @@
         :return:
         """
         s = np.array(s)
         gs = np.array(gs)
         return Distortion('convex', None, df=pd.DataFrame({'s': s.flat, 'gs': gs.flat}),
                           col_x='s', col_y='gs', display_name=display_name)
 
+    def price(self, ser, a=np.inf, kind='ask', S_calculation='forwards'):
+        r"""
+        Compute the bid and ask prices for the distribution determined by ``ser`` with
+        an asset limit ``a``. Uses ``np.trapz`` to compute :math:`\int_0^a S` or
+        :math:`\int_0^a g(S)`. Index of ``ser`` need not be equally spaced, so it can
+        be applied to :math:`\kappa`. To do this for unit A in portfolio port::
+
+            ser = port.density_df[['exeqa_A', 'p_total']].\
+                set_index('exeqa_A').groupby('exeqa_A').\
+                sum()['p_total']
+            dist.price(ser, port.q(0.99), 'both')
+
+
+        :param ser: pd.Series of is probabilities, indexed by outcomes. Outcomes must
+          be spaced evenly. ``ser`` is usually a probability column from ``density_df``.
+        :param kind: is "ask", "bid",  or "both", giving the pricing view.
+        :param a: asset level. ``ser`` is truncated at ``a``.
+        """
+
+        if not isinstance(ser, pd.Series):
+            raise ValueError(f'ser must be a pandas Series, not {type(ser)}')
+
+        if kind in ['bid', 'ask']:
+            pass
+        elif kind == 'both':
+            return [*self.price(ser, a, 'bid', S_calculation),
+                    self.price(ser, a, 'ask', S_calculation)[0]]
+        else:
+            raise ValueError(f'kind must be bid, ask, or both, not {kind}')
+
+        # apply limit
+        if a < np.inf:
+            ser = ser.copy()
+            tail = ser[a:].sum()
+            ser = ser[:a]
+            ser[a] = tail
+        else:
+            ser = ser.sort_index(ascending=True)
+
+        if S_calculation == 'forwards':
+            S = 1 - ser.cumsum()
+        else:
+            fill_value = max(0, 1 - ser.sum())
+            S = np.minimum(1, fill_value +
+                           ser.shift(-1, fill_value=0)[::-1].cumsum())
+
+        # not all distortions return numpy; force conversion
+        if kind == 'ask':
+            gS = np.array(self.g(S))
+        else:
+            gS = np.array(self.g_dual(S))
+
+        # trapz is not correct with our interpretation elsewhere; we use a step function
+        # loss = np.trapz(S, S.index)
+        # prem = np.trapz(gS, S.index)
+        dx = np.diff(S.index)
+        loss = (S.iloc[:-1].values * dx).sum()
+        prem = (gS[:-1] * dx).sum()
+
+        return prem, loss
+
```

### Comparing `aggregate-0.9.6.5/aggregate/underwriter.py` & `aggregate-0.9.6.8/aggregate/underwriter.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import pandas as pd
 from pathlib import Path
 import re
 from IPython.display import HTML, display
 # from inspect import signature
 
+from .constants import *
 from .portfolio import Portfolio
 from .distributions import Aggregate, Severity
 from .spectral import Distortion
 from .parser import UnderwritingLexer, UnderwritingParser
 from .utilities import logger_level, round_bucket, Answer, LoggerManager, pprint, show_fig
 
 logger = logging.getLogger(__name__)
@@ -78,14 +79,19 @@
         self.default_dir = Path(__file__).parent / 'agg'
 
         # site dir is in Users's home directory and stores their files
         self.site_dir = Path.home() / 'aggregate/databases'
         # check site dir exists
         self.site_dir.mkdir(parents=True, exist_ok=True)
 
+        # case dir
+        self.case_dir = Path.home() / 'aggregate/cases'
+        # check case dir exists
+        self.case_dir.mkdir(parents=True, exist_ok=True)
+
         self.template_dir = self.default_dir.parent / 'templates'
         self.template_dir.mkdir(parents=True, exist_ok=True)
 
         # make sure all database entries are stored:
         if databases is None:
             # nothing to do
             databases = []
@@ -186,16 +192,16 @@
                 kind, name, spec, program = rows.reset_index().iloc[0]
                 return Answer(kind=kind, name=name, spec=spec, program=program, object=None)
             else:
                 raise KeyError(f'Error: no unique object found matching {item}. Found {len(rows)} objects.')
 
     def __repr__(self):
         s = []
-        s.append(f'Underwriter   {self.name}')
-        s.append(f'Knowledge     {len(self._knowledge)} programs')
+        s.append(f'underwriter   {self.name}')
+        s.append(f'knowledge     {len(self._knowledge)} programs')
         for k in ['log2', 'update', 'debug', 'site_dir', 'default_dir']:
             s.append(f'{k:<14s}{getattr(self, k)}')
         # s.append(super().__repr__())
         return '\n'.join(s)
 
     def _repr_html_(self):
         s = [f'<p><h3>Underwriter {self.name}</h3>',
@@ -235,15 +241,15 @@
             # need to drop the 'agg', name before the spec that gets returned
             # by the parser. Hence:
             agg_list = [k for i, j, k in spec['spec']]
             obj = Portfolio(name, agg_list, uw=self)
             obj.program = program
         elif kind == 'sev':
             if 'sev_wt' in spec and spec['sev_wt'] != 1:
-                logger.warning(
+                logger.log(WL,
                     f'Mixed severity cannot be created, returning spec. You had {spec["sev_wt"]}, expected 1')
                 obj = None
             else:
                 obj = Severity(**spec)
                 # ? set outside...
                 obj.program = program
         elif kind == 'distortion':
@@ -335,15 +341,15 @@
                     update_method = getattr(answer.object, 'update', None)
                     if update_method is not None:
                         update_method(log2, bs, **kwargs)
             rv.append(answer)
 
         # report on what has been done
         if rv is None:
-            logger.warning(f'Program did not contain any output')
+            logger.log(WL, f'Program did not contain any output')
         else:
             if len(rv):
                 logger.info(f'Program created {len(rv)} objects.')
 
         # return created objects
         return rv
 
@@ -503,15 +509,15 @@
             lm = LoggerManager(log_level)
 
         # make stuff
         # write will return a dict with keys (kind, name) and value a WriteAnswer namedtuple
         rv = self.write(program, update=False, force_severity=True)
 
         if rv is None or len(rv) == 0:
-            logger.warning('build produced no output')
+            logger.log(WL, 'build produced no output')
             return None
 
         # in this loop bs_ and log2_ are the values actually used for each update;
         # they do not overwrite the input default values
         for answer in rv:
             if answer.object is None:
                 # object not created
@@ -837,114 +843,13 @@
                     rs = r.split(' ')
                     if rs[0] in ['agg', 'port', 'dist', 'distortion', 'sev']:
                         entries.append([dn, fn.name] + rs[:2])
 
         ans = pd.DataFrame(entries, columns=['Directory', 'Database', 'kind', 'name'])
         return ans
 
-    # def list(self, regex='', kind=''):
-    #     """
-    #     Not sure what the best name is!
-    #     """
-    #
-    #     # catch called with kind = these seem to work...
-    #     if regex in ('agg', 'port', 'sev'):
-    #         kind = regex
-    #         regex = ''
-    #
-    #     if regex == '' and kind == '':
-    #         return self.knowledge
-    #     elif kind == '':
-    #         return self.knowledge.filter(regex=regex, axis=0)
-    #     elif regex == '':
-    #         return self.knowledge.loc[kind]
-    #     else:
-    #         return self.knowledge.loc[kind].filter(regex=regex, axis=0)
-
-    # def describe(self, kind='agg'):
-    #     """
-    #     TODO this is not rationlized...and as a prop it needs to return something
-    #     More informative version of knowledge showing the agg programs. Only Aggregates that have a program.
-    #
-    #     TODO Add severities
-    #
-    #     :return:
-    #     """
-    #     from IPython.display import HTML
-    #
-    #     if kind == 'all':
-    #         kinds = ['agg', 'port']
-    #     else:
-    #         kinds = [kind]
-    #
-    #     if 'port' in kinds:
-    #         cols = ['Name', 'Type', 'Agg1', 'Agg2', 'Agg3', 'Notes']
-    #         df_port = pd.DataFrame(columns=cols)
-    #         df_port = df_port.set_index('Name')
-    #         for (kind, name), (spec, program) in self._knowledge.xs('port', axis=0, level=0,
-    #                                                                 drop_level=False).iterrows():
-    #             aggs = spec['spec'][:3]  # the list of agg items
-    #             if len(aggs) == 1:
-    #                 aggs.extend(['', ''])
-    #             elif len(aggs) == 2:
-    #                 aggs.extend([''])
-    #             note = spec['note']
-    #             df_port.loc[name, :] = [kind] + aggs + [note]
-    #         df_port = df_port.sort_index()
-    #         return df_port
-    #         # display(HTML('<h3>Known Portfolios</h3>'))
-    #         # display(df_port)
-    #
-    #     if 'agg' in kinds:
-    #         cols = ['Name', 'Type', 'ELoss', 'Severity', 'ESev', 'SevCV', 'Sev_a', 'Sev_b', 'Freq', 'EN', 'Freq_a',
-    #                 'Notes']
-    #         # what they are actually called
-    #         cols_agg = ['exp_el', 'sev_name', 'sev_mean', 'sev_cv', 'sev_a', 'sev_b', 'freq_name', 'exp_en', 'freq_a',
-    #                     'note']
-    #         df_agg = pd.DataFrame(columns=cols)
-    #         df_agg = df_agg.set_index('Name')
-    #         for (kind, name), (spec, program) in self._knowledge.xs('agg', axis=0, level=0,
-    #                                                                 drop_level=False).iterrows():
-    #             df_agg.loc[name, :] = [kind] + [str(spec.get(f, '')) for f in cols_agg]
-    #         df_agg = df_agg.sort_index()
-    #         # compute E loss... but careful about arrays
-    #         # TODO must be a better way
-    #         for i in df_agg.query('ELoss == ""').index:
-    #             es, en = df_agg.loc[i, ['ESev', 'EN']]
-    #             try:
-    #                 es = float(es)
-    #                 en = float(en)
-    #             except (ValueError, TypeError):
-    #                 df_agg.loc[i, 'ELoss'] = '...'
-    #             else:
-    #                 df_agg.loc[i, 'ELoss'] = es * en
-    #
-    #         df_agg = df_agg.drop(columns='Sev_b')
-    #         return df_agg
-    #         # display(HTML('<h3>Known Aggregates</h3>'))
-    #         # display(df_agg)
-    #
-    #     if 'distortion' in kinds:
-    #         return self._knowledge.loc['distortion']
-
-    # @property
-    # def programs(self):
-    #     """
-    #     Return the knowledge as a nice dataframe
-    #
-    #     :return:
-    #     """
-    #     bit = self._knowledge[['program']]
-    #     bit['note'] = [s['note'] for s in self._knowledge.spec]
-    #     bit['clean program'] = bit.program.str.replace(r'note\{[^}]*\}|[ ]{2,}|\t+', ' ')
-    #     bit = bit.sort_index(ascending=[False, True])
-    #     bit = bit.reset_index(0, drop=False)
-    #     bit = bit[['kind', 'note', 'clean program']].query('`clean program` != ""')
-    #     bit = bit[['kind', 'clean program', 'note']]
-    #     return bit
-
 
 # exported instance
 # self = dbuild = None
 logger_level(30)
 build = Underwriter(databases='test_suite', update=True, debug=False, log2=16)
 debug_build = Underwriter(name='Debug', update=True, debug=True, log2=13)
```

### Comparing `aggregate-0.9.6.5/aggregate/utilities.py` & `aggregate-0.9.6.8/aggregate/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,21 @@
     ans = []
     # programs come in as multiline
     txt = txt.replace('\n\tagg', ' agg')
     for t in txt.split('\n'):
         clean = re.sub(r'[ \t]+', ' ', t.strip())
         clean = re.sub(r' note\{[^}]*\}', '', clean)
         if split > 0 and len(clean) > split:
-            clean = re.sub(r' (d?sev|occurrence|agg|aggregate|mixed|poisson|fixed)', r'\n    \1', clean)
-            s = clean.split(' ')
-            clean = ' '.join(s[:2]) + '\n\t' + ' '.join(s[2:])
+            clean = re.sub(
+                r' ((dfreq )([0-9]+ )|([0-9]+ )(claims?|premium|loss|exposure)|d?sev|occurrence|agg|aggregate|wts?|mixed|poisson|fixed)',
+                           r'\n  \1', clean)
+        if clean[:4] == 'port':
+            # put in extra tabs at agg for portfolios
+            sc = clean.split('\n')
+            clean = sc[0] + '\n' + '\n'.join([i if i[:5] == '  agg' else '  ' + i for i in sc[1:]])
         ans.append(clean)
     ans = '\n'.join(ans)
     if html is True:
         ans = f'<p><code>{ans}\n</code></p>'
         notes = re.findall('note\{([^}]*)\}', txt)
         for i, n in enumerate(notes):
             ans += f'<p><small>Note {i+1}. {n}</small><p>'
@@ -194,15 +198,15 @@
         return -np.inf, np.inf, 0
     else:
         eta = (((np.sqrt(skew ** 2 + 4)) / 2) + (skew / 2)) ** (1 / 3) - (
                 1 / (((np.sqrt(skew ** 2 + 4)) / 2) + (skew / 2)) ** (1 / 3))
         sigma = np.sqrt(np.log(1 + eta ** 2))
         shift = m - cv * m / eta
         if shift > m:
-            logger.warning(f'utils sln_fit | shift > m, {shift} > {m}, too extreme skew {skew}')
+            logger.log(WL, f'utils sln_fit | shift > m, {shift} > {m}, too extreme skew {skew}')
             shift = m - 1e-6
         mu = np.log(m - shift) - sigma ** 2 / 2
         return shift, mu, sigma
 
 
 def sgamma_fit(m, cv, skew):
     """
@@ -1164,21 +1168,31 @@
 
 def xsden_to_meancv(xs, den):
     """
     Compute mean and cv from xs and density.
 
     Consider adding: np.nan_to_num(den)
 
+    Note: cannot rely on pd.Series[-1] to work... it depends on the index.
+    xs could be an index
     :param xs:
     :param den:
     :return:
     """
+    pg = 1 - den.sum()
     xd = xs * den
-    ex1 = np.sum(xd)
-    ex2 = np.sum(xd * xs)
+    if isinstance(xs, np.ndarray):
+        xsm = xs[-1]
+    elif isinstance(xs, pd.Series):
+        xsm = xs.iloc[-1]
+    else:
+        xsm = np.array(xs)[-1]
+    ex1 = np.sum(xd) + pg * xsm
+    # logger.log(WL, f'tail mass mean adjustment {pg * xsm}')
+    ex2 = np.sum(xd * xs) + pg * xsm ** 2
     sd = np.sqrt(ex2 - ex1 ** 2)
     if ex1 != 0:
         cv = sd / ex1
     else:
         cv = np.nan
     return ex1, cv
 
@@ -1189,19 +1203,27 @@
 
         Consider adding: np.nan_to_num(den)
 
         :param xs:
         :param den:
         :return:
         """
+    pg = 1 - den.sum()
     xd = xs * den
-    ex1 = np.sum(xd)
+    if isinstance(xs, np.ndarray):
+        xsm = xs[-1]
+    elif isinstance(xs, pd.Series):
+        xsm = xs.iloc[-1]
+    else:
+        xsm = np.array(xs)[-1]
+    ex1 = np.sum(xd) + pg * xsm
+    # logger.log(WL, f'tail mass mean adjustment {pg * xsm}')
     xd *= xs
-    ex2 = np.sum(xd)
-    ex3 = np.sum(xd * xs)
+    ex2 = np.sum(xd) + pg * xsm ** 2
+    ex3 = np.sum(xd * xs) + pg * xsm ** 3
     mw = MomentWrangler()
     mw.noncentral = ex1, ex2, ex3
     return mw.mcvsk
 
 
 def tweedie_convert(*, p=None, μ=None, σ2=None, λ=None, α=None, β=None, m=None, cv=None):
     """
@@ -1993,62 +2015,14 @@
         'selector': 'td',
         'props': f'text-align: right;'
     }
     all_styles = [cell_hover, index_names, headers, center_heading,  left_index, td]
     return df.style.set_table_styles(all_styles)
 
 
-# styling blue to match graphs...not great
-# def style_df(df):
-#     """
-#     Style a df similar to pricinginsurancerisk.com styles.
-#
-#     graph background color is B4C3DC and figure (paler) background is F1F8F#
-#
-#     Dropped row lines; bold level0, caption
-#
-#     :param df:
-#     :return: styled dataframe
-#
-#     """
-#
-#     cell_hover = {
-#         'selector': 'td:hover',
-#         'props': [('background-color', '#ffffb3')]
-#     }
-#     index_names = {
-#         'selector': '.index_name',
-#         'props': 'font-style: italic; color: black; background-color: white; '
-#                  'font-weight:bold; border: 0px solid #a4b3dc; text-transform: capitalize; '
-#                  'text-align:left;'
-#     }
-#     headers = {
-#         'selector': 'th:not(.index_name)',
-#         'props': 'background-color: #b4c3dc; color: black;  border: 1px solid #ffffff;'
-#     }
-#     center_heading = {
-#         'selector': 'th.col_heading',
-#         'props': 'text-align: center;'
-#     }
-#     left_index = {
-#         'selector': '.row_heading',
-#         'props': 'text-align: left;'
-#     }
-#     td = {
-#         'selector': 'td',
-#         'props': f'text-align: right; '
-#     }
-#     nrow = {
-#         'selector': 'tr:nth-child(even)',
-#         'props': 'background-color: #f1f8fe;'
-#     }
-#     all_styles = [cell_hover, index_names, headers, center_heading, nrow, left_index, td]
-#     return df.style.set_table_styles(all_styles)
-
-
 def friendly(df):
     """
     Attempt to format df "nicely", in a user-friendly manner. Not designed for big dataframes!
 
     :param df:
     :return:
     """
@@ -2367,16 +2341,16 @@
         rank_samples[:, j] = s[ranks[:,j]]
     return rank_samples
 
 def iman_conover(marginals, desired_correlation, dof=0, add_total=True):
     """
     Perform Iman Conover shuffling on input marginals to achieve desired_correlation
     Desired_correlation must be positive definite and of the correct size.
-    The result has the same rand correlation as a reference sample with the
-    desired linear correlation. Thus the process relies on linear and rank
+    The result has the same rank correlation as a reference sample with the
+    desired linear correlation. Thus, the process relies on linear and rank
     correlation (for the reference and the input sample) being close.
 
     if dof==0 use normal scores; else you mv t
 
     Sample code:
     ::
 
@@ -2420,15 +2394,15 @@
     n, d = marginals.shape
 
     # "square root" of "variance"
     # step 7
     C = np.linalg.cholesky(desired_correlation)
 
     # make a perfectly uncorrelated reference: noise function = steps 1-6; product is step 8 (transposed)
-    if dof==0:
+    if dof == 0:
         N = ic_noise(n, d) @ C.T
     else:
         N = ic_t_noise(n, d, dof) @ C.T
 
     # required ordering of marginals determined by reference sample, step 9
     R = ic_rank(N)
 
@@ -2437,15 +2411,15 @@
         shuffled_marginals = ic_reorder(R, marginals)
         df = pd.DataFrame(shuffled_marginals)
     else:
         shuffled_marginals = ic_reorder(R, marginals.to_numpy())
         df = pd.DataFrame(shuffled_marginals, columns=marginals.columns)
 
     # add total if requested
-    if add_total is True:
+    if add_total:
         df['total'] = df.sum(axis=1)
         df = df.set_index('total')
         df = df.sort_index(ascending=False)
 
     return df
 
 
@@ -2512,15 +2486,15 @@
 
     :param df: Input DataFrame containing samples from each marginal. RA will only combine the
         top 1-p proportion of values from each marginal.
     :param p: If ``p==0`` assume df has already truncated to the top p values (for each marginal).
         Otherwise truncate each at the ``int(1-p * len(df))``
     :param tau: simulation tolerance
     :param max_iter: maximum number of iterations to attempt
-    :return:
+    :return: the top 1-p values of the rearranged DataFrame
     """
 
     sorted_marginals = {}
 
     # worst N shuffled
     if p:
         N = int(np.round((1 - p) * len(df), 0))
@@ -2550,21 +2524,21 @@
         # achieved VaR is minimum value
         v = df_out.sum(axis=1).sort_values(ascending=False).iloc[-1]
         chg_var = last_var - v
         last_var = v
         # reporting and loop control
         n_iter += 1
         if n_iter >= 2:
-            print(f'Iteration {n_iter:d}\t{v:5.3e}\tChg\t{chg_var:5.3e}')
+            logger.info(f'Iteration {n_iter:d}\t{v:5.3e}\tChg\t{chg_var:5.3e}')
         if n_iter > max_n_iter:
-            print("ERROR: not converging...breaking")
+            logger.error("ERROR: not converging...breaking")
             break
 
     df_out['total'] = df_out.sum(axis=1)
-    print(f'Ending VaR\t{v:7.5e}\ns lower {df_out.total.min():7.5e}')
+    logger.info(f'Ending VaR\t{v:7.5e}\ns lower {df_out.total.min():7.5e}')
     return df_out.sort_values('total')
 
 
 def make_corr_matrix(vine_spec):
     r"""
     Make a correlation matrix from a vine specification, https://en.wikipedia.org/wiki/Vine_copula.
 
@@ -2719,15 +2693,15 @@
         α = fz.args[0]
         λ = fz.kwds['scale']
         loc = fz.kwds.get('loc', 0.0)
         # regular Pareto is scale=lambda, loc=-lambda, so this has no effect
         # single parameter Pareto is scale=lambda, loc=0
         # these formulae for regular pareto, hence
         if λ + loc != 0:
-            logger.warning('Pareto not shifted to x>0 range...using numeric moments.')
+            logger.log(WL, 'Pareto not shifted to x>0 range...using numeric moments.')
             return partial_e_numeric(fz, a, n)
         ans = []
         # will return inf if the Pareto does not have the relevant moments
         # TODO: formula for shape=1,2,3
         for k in range(n + 1):
             b = [α * (-1) ** (k - i) * binom(k, i) * λ ** (k + α - i) *
                  ((λ + a) ** (i - α) - λ ** (i - α)) / (i - α)
@@ -2839,14 +2813,21 @@
                     # 'max_colwidth': 10,
                     'sparsify': True,
                     'justify': None
                     }
             args.update(kwargs)
             print(x.to_string(**args))
             # print(x.to_string(formatters={c: f for c in x.columns}))
+        elif isinstance(x, pd.Series):
+            args = {'max_rows': 25,
+                    'float_format': ff,
+                    'name': True
+                    }
+            args.update(kwargs)
+            print(x.to_string(**args))
         elif isinstance(x, int):
             print(x)
         elif isinstance(x, Number):
             print(ff(x))
         else:
             print(x)
 
@@ -3149,15 +3130,15 @@
     density.loc[attachments[-1]:, 'S_adj'] = density.loc[attachments[-1]:, 'S']
     # adj probs as difference of S
     density['p_adj'] = density['S_adj'].shift(1, fill_value=1) - density['S_adj']
     achieved = density.groupby(density.layer.shift(-1)).apply(lambda g: g['S_adj'].sum() * bs)
     # display(achieved)
     if abs(achieved.iloc[0] - target[0]) > 1e-3:
         # issues with hitting 1
-        logger.warning(f'achieved[0] = {achieved.iloc[0]} != target[0] = {target[0]}')
+        logger.log(WL, f'achieved[0] = {achieved.iloc[0]} != target[0] = {target[0]}')
         # take top right corner off
         if target[0] > attachments[0]:
             raise ValueError(f'target[0] = {target[0]} > first attachment[0] = {attachments[0]} which is impossible.')
         s0 = 2 * (attachments[0] - target[0]) / (1 - layers.loc[1, 'ω'])
         # snap to index
         s0 = bs * np.round(s0 / bs, 0)
         # convert to probability
@@ -3165,25 +3146,25 @@
         density.loc[0:s, 'S_adj'] = 1.0
         temp = np.array(density.loc[s+bs:attachments[0]].index)
         wts = (temp - s) / s0
         density.loc[s+bs:attachments[0], 'S_adj'] = 1 - wts + layers.loc[1, 'ω'] * wts
         # update
         density['p_adj'] = density['S_adj'].shift(1, fill_value=1) - density['S_adj']
         achieved = density.groupby(density.layer.shift(-1)).apply(lambda g: g['S_adj'].sum() * bs)
-        logger.warning(f'Revised layer 1 achieved = {achieved.iloc[0]}')
+        logger.log(WL, f'Revised layer 1 achieved = {achieved.iloc[0]}')
 
     density['diff S'] = density['S'] - density['Sa']
 
     if debug is False:
         return density['p_adj'].values
 
     # data frame of layer statistics from input density
     exact = None
     if sf is not None:
-        logger.warning('sf passed in; computing exact layer statistics')
+        logger.log(WL, 'sf passed in; computing exact layer statistics')
         exact = pd.DataFrame(columns=['a', 'lev', 'aS', 'S'],
                              index=range(1, 1+len(attachments)), dtype=float)
         for i, x in enumerate(attachments):
             ix = quad(sf, 0, x)
             # check error is small
             assert ix[1] < 1e-6
             sf_ = sf(x)
@@ -3200,7 +3181,40 @@
                    density.groupby(density.layer.shift(-1)).apply(lambda g: g['S'].sum() * bs),
                    achieved,
                    ), keys=[ln, 'computed', 'adj'], axis=1)
     t.loc['sum'] = t.sum()
     Picks = namedtuple('picks', ['layers', 'exact', 'density', 'audit'])
     return Picks(layers=layers, exact=exact, density=density, audit=t)
 
+
+def integral_by_doubling(func, x0, err=1e-8):
+    r"""
+    Compute :math:`\int_{x_0}^\infty f` as the sum
+
+    .. math::
+
+        \int_{x_0}^\infty f = \sum_{n \ge 0} \int_{2^nx_0}^{2^{n+1}x_0} f
+
+    Caller should check the integral actually converges.
+
+    :param func: function to be integrated.
+    :param x0: starting x value
+    :param err: desired accuracy: stop when incremental integral is <= err.
+    """
+    ans = 0.
+    counter = 0
+    # from to
+    f, t = x0, 2 * x0
+    last_int = 10
+    while last_int > err:
+        s = quad(func, f, t)
+        if s[1] > err:
+            raise ValueError(
+                f'Questionable integral numeric convergence, err {s[1]:.4g}\n'
+                f'f={f}, t={t}, x0={x0}, counter={counter}')
+        last_int = s[0]
+        ans += s[0]
+        f, t = t, 2 * t
+        counter += 1
+        if counter > 96:
+            raise ValueError(f'counter = {counter} and error = {err}')
+    return -ans
```

### Comparing `aggregate-0.9.6.5/aggregate.egg-info/PKG-INFO` & `aggregate-0.9.6.8/aggregate.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aggregate
-Version: 0.9.6.5
+Version: 0.9.6.8
 Summary: aggregate - working with compound probability distributions
 Author: Stephen J. Mildenhall
 Author-email: steve@convexrisk.com
 Maintainer: Stephen J. Mildenhall
 Maintainer-email: steve@convexrisk.com
 License: BSD
 Project-URL: Documentation, https://aggregate.readthedocs.io/en/latest/
@@ -13,28 +13,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Education
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Education
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 aggregate: a powerful aggregate distribution modeling library in Python
 ========================================================================
 
 What is it?
 -----------
 
-**aggregate** is a Python package providing an expressive language and fast,
-accurate computations to make working with aggregate (compound) probability
-distributions easy and intuitive. It allows students and practitioners to
-use realistic real-world distributions that reflect the underlying
-frequency and severity generating processes. It has applications in
-insurance, risk management, actuarial science, and related areas.
+``aggregate`` solves insurance, risk management, and actuarial problems using realistic models that reflect underlying frequency and severity.
+It delivers the speed and accuracy of parametric distributions to situations that usually require simulation, making it as easy to work with an aggregate (compound) probability distribution as the lognormal.
+``aggregate`` includes an expressive language called DecL to describe aggregate distributions and is implemented in Python under an open source BSD-license.
+
 
 Documentation
 -------------
 
 https://aggregate.readthedocs.io/
```

### Comparing `aggregate-0.9.6.5/setup.py` & `aggregate-0.9.6.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     'cycler',
     'ipykernel',
     'jinja2',
     'matplotlib',
     'numpy',
     'pandas',
     'psutil',
-    'pypandoc',
     'scipy',
     'sly',
     'titlecase',
     # docs
     # 'docutils',
     # 'jupyter-sphinx',
     # 'nbsphinx',
@@ -42,20 +41,18 @@
 
 long_description = """aggregate: a powerful aggregate distribution modeling library in Python
 ========================================================================
 
 What is it?
 -----------
 
-**aggregate** is a Python package providing an expressive language and fast,
-accurate computations to make working with aggregate (compound) probability
-distributions easy and intuitive. It allows students and practitioners to
-use realistic real-world distributions that reflect the underlying
-frequency and severity generating processes. It has applications in
-insurance, risk management, actuarial science, and related areas.
+``aggregate`` solves insurance, risk management, and actuarial problems using realistic models that reflect underlying frequency and severity.
+It delivers the speed and accuracy of parametric distributions to situations that usually require simulation, making it as easy to work with an aggregate (compound) probability distribution as the lognormal.
+``aggregate`` includes an expressive language called DecL to describe aggregate distributions and is implemented in Python under an open source BSD-license.
+
 
 Documentation
 -------------
 
 https://aggregate.readthedocs.io/
 
 
@@ -92,23 +89,23 @@
 """
 
 version = aggregate.__version__
 
 setup(name="aggregate",
       description="aggregate - working with compound probability distributions",
       long_description=long_description,
-      license="""BSD""",
+      long_description_content_type='text/x-rst',
+      license="BSD",
       version=version,
       author="Stephen J. Mildenhall",
       author_email="steve@convexrisk.com",
       maintainer="Stephen J. Mildenhall",
       maintainer_email="steve@convexrisk.com",
       packages=['aggregate'],
-      package_data={'': ['*.txt', '*.rst', '*.md', 'agg/*.agg', 'examples/*.py', 'examples/*.ipynb',
-                         'test/*.py']},
+      package_data={'': ['*.txt', '*.rst', '*.md', 'agg/*.agg']},
       tests_require=tests_require,
       install_requires=install_requires,
       classifiers=[
           'Development Status :: 4 - Beta',
           'Programming Language :: Python :: 3',
           'License :: OSI Approved :: BSD License',
           'Topic :: Education',
```

