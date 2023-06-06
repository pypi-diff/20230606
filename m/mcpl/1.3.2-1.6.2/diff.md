# Comparing `tmp/mcpl-1.3.2-py2.py3-none-any.whl.zip` & `tmp/mcpl-1.6.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,10 @@
-Zip file size: 21498 bytes, number of entries: 9
--rw-r-----  2.0 unx    68931 b- defN 20-Mar-18 13:06 mcpl.py
--rw-r-----  2.0 unx       10 b- defN 20-Mar-18 13:06 mcpl-1.3.2.dist-info/DESCRIPTION.rst
--rw-r-----  2.0 unx       42 b- defN 20-Mar-18 13:06 mcpl-1.3.2.dist-info/entry_points.txt
--rw-r-----  2.0 unx      623 b- defN 20-Mar-18 13:06 mcpl-1.3.2.dist-info/metadata.json
--rw-r-----  2.0 unx        5 b- defN 20-Mar-18 13:06 mcpl-1.3.2.dist-info/top_level.txt
--rw-r-----  2.0 unx        1 b- defN 20-Mar-18 13:06 mcpl-1.3.2.dist-info/zip-safe
--rw-r-----  2.0 unx      110 b- defN 20-Mar-18 13:06 mcpl-1.3.2.dist-info/WHEEL
--rw-r-----  2.0 unx      277 b- defN 20-Mar-18 13:06 mcpl-1.3.2.dist-info/METADATA
--rw-r-----  2.0 unx      715 b- defN 20-Mar-18 13:06 mcpl-1.3.2.dist-info/RECORD
-9 files, 70714 bytes uncompressed, 20274 bytes compressed:  71.3%
+Zip file size: 23718 bytes, number of entries: 8
+-rw-r-----  2.0 unx    68917 b- defN 23-Jun-06 10:08 mcpl.py
+-rw-r-----  2.0 unx     7048 b- defN 23-Jun-06 10:08 mcpl-1.6.2.dist-info/LICENSE.txt
+-rw-r-----  2.0 unx      276 b- defN 23-Jun-06 10:08 mcpl-1.6.2.dist-info/METADATA
+-rw-r-----  2.0 unx      110 b- defN 23-Jun-06 10:08 mcpl-1.6.2.dist-info/WHEEL
+-rw-r-----  2.0 unx       42 b- defN 23-Jun-06 10:08 mcpl-1.6.2.dist-info/entry_points.txt
+-rw-r-----  2.0 unx        5 b- defN 23-Jun-06 10:08 mcpl-1.6.2.dist-info/top_level.txt
+-rw-r-----  2.0 unx        1 b- defN 23-Jun-06 10:08 mcpl-1.6.2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      614 b- defN 23-Jun-06 10:08 mcpl-1.6.2.dist-info/RECORD
+8 files, 77013 bytes uncompressed, 22646 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,28 +1,25 @@
 Filename: mcpl.py
 Comment: 
 
-Filename: mcpl-1.3.2.dist-info/DESCRIPTION.rst
+Filename: mcpl-1.6.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: mcpl-1.3.2.dist-info/entry_points.txt
+Filename: mcpl-1.6.2.dist-info/METADATA
 Comment: 
 
-Filename: mcpl-1.3.2.dist-info/metadata.json
+Filename: mcpl-1.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: mcpl-1.3.2.dist-info/top_level.txt
+Filename: mcpl-1.6.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: mcpl-1.3.2.dist-info/zip-safe
+Filename: mcpl-1.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mcpl-1.3.2.dist-info/WHEEL
+Filename: mcpl-1.6.2.dist-info/zip-safe
 Comment: 
 
-Filename: mcpl-1.3.2.dist-info/METADATA
-Comment: 
-
-Filename: mcpl-1.3.2.dist-info/RECORD
+Filename: mcpl-1.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mcpl.py

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 """Python module for accessing MCPL files.
 
 The MCPL (Monte Carlo Particle Lists) format is thoroughly documented on the
 project homepage, from where it is also possible to download the entire MCPL
 distribution:
 
      https://mctools.github.io/mcpl/
@@ -17,34 +17,34 @@
 
 A substantial effort went into developing MCPL. If you use it for your work, we
 would appreciate it if you would use the following reference in your work:
 
    T. Kittelmann, et al., Monte Carlo Particle Lists: MCPL, Computer Physics
    Communications 218, 17-42 (2017), https://doi.org/10.1016/j.cpc.2017.04.012
 
-mcpl.py written by Thomas Kittelmann, 2017-2019. The work was supported by the
+mcpl.py written by Thomas Kittelmann, 2017-2022. The work was supported by the
 European Union's Horizon 2020 research and innovation programme under grant
 agreement No 676548 (the BrightnESS project)
 """
 
 from __future__ import division, print_function, absolute_import,unicode_literals#enable py3 behaviour in py2.6+
 
 try:
     _str = lambda s : s.encode('ascii') if (hasattr(s,'encode') and bytes==str) else s
 except SyntaxError:
     print('MCPL ERROR: Unsupported obsolete Python detected')
     raise SystemExit(1)
 
 __license__ = _str('CC0 1.0 Universal')
-__copyright__ = _str('Copyright 2017-2019')
-__version__ = _str('1.3.2')
+__copyright__ = _str('Copyright 2017-2022')
+__version__ = _str('1.6.2')
 __status__ = _str('Production')
 __author__ = _str('Thomas Kittelmann')
 __maintainer__ = _str('Thomas Kittelmann')
-__email__ = _str('thomas.kittelmann@esss.se')
+__email__ = _str('thomas.kittelmann@ess.eu')
 __all__ = [_str('MCPLFile'),
            _str('MCPLParticle'),
            _str('MCPLParticleBlock'),
            _str('MCPLError'),
            _str('dump_file'),
            _str('convert2ascii'),
            _str('app_pymcpltool'),
@@ -844,15 +844,15 @@
         dt= np_dtype("u8,5u4,i4,2u4").newbyteorder(endianness)
         y = self._fileread(dtype=dt,count=1)
         if len(y)!=1:
             raise MCPLError('Invalid header')
         (nparticles,(ncomments,nblobs,opt_userflags,opt_polarisation,opt_singleprec),
          opt_universalpdgcode,(particlesize,_tmp)) = y[0]
         #convert all int types to python 'int' (which is 64bit), to avoid
-        #conversions like int+np.uint64->np.float64, and flags to bool:
+        #conversions like int+np.uint64->float, and flags to bool:
         nparticles = int(nparticles)
         self._np = nparticles#needs frequent access
         particlesize = int(particlesize)
         opt_universalpdgcode = int(opt_universalpdgcode)
         opt_userflags = bool(opt_userflags)
         opt_polarisation = bool(opt_polarisation)
         opt_singleprec = bool(opt_singleprec)
@@ -1264,15 +1264,15 @@
             s += ')'
             return s
     return None
 
 def _unique_count(a,weights=None):
     """returns (unique,count) where unique is an array of sorted unique values in a, and count is the corresponding frequency counts"""
     unique, inverse = np_unique(a, return_inverse=True)
-    count = np.zeros(len(unique), np.int if weights is None else np_dtype(type(weights[0])))
+    count = np.zeros(len(unique), int if weights is None else np_dtype(type(weights[0])))
     _np_add_at(count, inverse, 1 if weights is None else weights)
     return (unique, count)
 
 def _merge_unique_count(uc1,uc2):
     """merges the results of calling _unique_count on two separate data sets"""
     u = np.append(uc1[0],uc2[0])
     c = np.append(uc1[1],uc2[1])
@@ -1407,15 +1407,15 @@
             weight_sum = sc['integral']
         ranges[s] = [max(sc['min'],sc['mean']-2*sc['rms']),
                      min(sc['max'],sc['mean']+2*sc['rms'])]
         if not ranges[s][0]<ranges[s][1]:
             ranges[s] = (ranges[s][0]-1.0,ranges[s][1]+1.0)
 
     hists={}
-    freq_uc=dict((s,(np.asarray([],dtype=np.int),np.asarray([],dtype=np.float))) for s in freq_stats)
+    freq_uc=dict((s,(np.asarray([],dtype=int),np.asarray([],dtype=float))) for s in freq_stats)
     if (std_stats and bin_data) or freq_stats:
         #pass through and collect data:
         if weight_sum is None:
             sumw = 0.0
         for pb in mcplfile.particle_blocks:
             vals_weight = pb.weight
             disable=[]
```

