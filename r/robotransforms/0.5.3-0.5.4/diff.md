# Comparing `tmp/robotransforms-0.5.3.tar.gz` & `tmp/robotransforms-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotransforms-0.5.3.tar", last modified: Thu Jun  1 22:33:19 2023, max compression
+gzip compressed data, was "robotransforms-0.5.4.tar", last modified: Tue Jun  6 21:31:17 2023, max compression
```

## Comparing `robotransforms-0.5.3.tar` & `robotransforms-0.5.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.342161 robotransforms-0.5.3/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1076 2022-12-01 23:55:43.000000 robotransforms-0.5.3/LICENSE
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       37 2022-12-02 15:43:21.000000 robotransforms-0.5.3/MANIFEST.in
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-06-01 22:33:19.342161 robotransforms-0.5.3/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      347 2023-05-03 23:31:19.000000 robotransforms-0.5.3/README.md
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       60 2023-05-03 23:34:03.000000 robotransforms-0.5.3/pyproject.toml
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.330161 robotransforms-0.5.3/robotransforms/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      148 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       22 2023-06-01 22:30:33.000000 robotransforms-0.5.3/robotransforms/_version.py
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.338161 robotransforms-0.5.3/robotransforms/dead_reckon/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/dead_reckon/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    10020 2023-06-01 22:30:33.000000 robotransforms-0.5.3/robotransforms/dead_reckon/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      732 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/dead_reckon/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2811 2023-03-07 00:07:47.000000 robotransforms-0.5.3/robotransforms/dead_reckon/dead_reckon.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     7588 2023-06-01 22:30:47.000000 robotransforms-0.5.3/robotransforms/dead_reckon/dead_reckon_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15825 2023-03-07 00:44:08.000000 robotransforms-0.5.3/robotransforms/dead_reckon/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.342161 robotransforms-0.5.3/robotransforms/euclidean/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      120 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/euclidean/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8310 2023-05-03 23:28:26.000000 robotransforms-0.5.3/robotransforms/euclidean/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1566 2023-05-03 23:28:26.000000 robotransforms-0.5.3/robotransforms/euclidean/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11585 2023-05-03 23:28:26.000000 robotransforms-0.5.3/robotransforms/euclidean/euclidean.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14307 2023-05-04 15:04:49.000000 robotransforms-0.5.3/robotransforms/euclidean/euclidean_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6960 2023-05-03 23:28:26.000000 robotransforms-0.5.3/robotransforms/euclidean/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.342161 robotransforms-0.5.3/robotransforms/utils/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/utils/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3680 2022-12-02 19:58:46.000000 robotransforms-0.5.3/robotransforms/utils/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      351 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/utils/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      545 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/utils/utils.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1055 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/utils/utils_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6290 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/utils/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.338161 robotransforms-0.5.3/robotransforms.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-06-01 22:33:19.000000 robotransforms-0.5.3/robotransforms.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      943 2023-06-01 22:33:19.000000 robotransforms-0.5.3/robotransforms.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-06-01 22:33:19.000000 robotransforms-0.5.3/robotransforms.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       12 2023-06-01 22:33:19.000000 robotransforms-0.5.3/robotransforms.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2023-06-01 22:33:19.000000 robotransforms-0.5.3/robotransforms.egg-info/top_level.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-06-01 22:33:19.342161 robotransforms-0.5.3/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1907 2022-12-02 17:09:02.000000 robotransforms-0.5.3/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.228878 robotransforms-0.5.4/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1076 2022-12-01 23:55:43.000000 robotransforms-0.5.4/LICENSE
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       37 2022-12-02 15:43:21.000000 robotransforms-0.5.4/MANIFEST.in
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-06-06 21:31:17.224878 robotransforms-0.5.4/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      347 2023-05-03 23:31:19.000000 robotransforms-0.5.4/README.md
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       60 2023-05-03 23:34:03.000000 robotransforms-0.5.4/pyproject.toml
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.220878 robotransforms-0.5.4/robotransforms/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      148 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       22 2023-06-06 21:29:02.000000 robotransforms-0.5.4/robotransforms/_version.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.224878 robotransforms-0.5.4/robotransforms/dead_reckon/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/dead_reckon/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11493 2023-06-06 21:25:33.000000 robotransforms-0.5.4/robotransforms/dead_reckon/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      732 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/dead_reckon/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2811 2023-03-07 00:07:47.000000 robotransforms-0.5.4/robotransforms/dead_reckon/dead_reckon.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8728 2023-06-06 21:27:21.000000 robotransforms-0.5.4/robotransforms/dead_reckon/dead_reckon_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15825 2023-03-07 00:44:08.000000 robotransforms-0.5.4/robotransforms/dead_reckon/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.224878 robotransforms-0.5.4/robotransforms/euclidean/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      120 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/euclidean/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8310 2023-05-03 23:28:26.000000 robotransforms-0.5.4/robotransforms/euclidean/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1566 2023-05-03 23:28:26.000000 robotransforms-0.5.4/robotransforms/euclidean/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11585 2023-05-03 23:28:26.000000 robotransforms-0.5.4/robotransforms/euclidean/euclidean.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14307 2023-05-04 15:04:49.000000 robotransforms-0.5.4/robotransforms/euclidean/euclidean_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6960 2023-05-03 23:28:26.000000 robotransforms-0.5.4/robotransforms/euclidean/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.224878 robotransforms-0.5.4/robotransforms/utils/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/utils/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3680 2022-12-02 19:58:46.000000 robotransforms-0.5.4/robotransforms/utils/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      351 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/utils/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      545 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/utils/utils.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1055 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/utils/utils_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6290 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/utils/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.220878 robotransforms-0.5.4/robotransforms.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-06-06 21:31:17.000000 robotransforms-0.5.4/robotransforms.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      943 2023-06-06 21:31:17.000000 robotransforms-0.5.4/robotransforms.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-06-06 21:31:17.000000 robotransforms-0.5.4/robotransforms.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       12 2023-06-06 21:31:17.000000 robotransforms-0.5.4/robotransforms.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2023-06-06 21:31:17.000000 robotransforms-0.5.4/robotransforms.egg-info/top_level.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-06-06 21:31:17.228878 robotransforms-0.5.4/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1907 2022-12-02 17:09:02.000000 robotransforms-0.5.4/setup.py
```

### Comparing `robotransforms-0.5.3/LICENSE` & `robotransforms-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/PKG-INFO` & `robotransforms-0.5.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotransforms
-Version: 0.5.3
+Version: 0.5.4
 Summary: A transformation library for robot motion
 Home-page: https://github.com/Nova-Dynamics/transforms-python
 Author: Jonathan D. B. Van Schenck
 Author-email: jvschenck@novadynamics.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `robotransforms-0.5.3/robotransforms/dead_reckon/base.cpp` & `robotransforms-0.5.4/robotransforms/dead_reckon/base.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 constexpr double DR_D_EFF_PARAMS[3] = {0.505225138, 4.55440687, 0.00237199585};
 
 // Is this a bad idea?
 constexpr double L_PLUS_LAMBDA = 3;
 
 // State vector size
 constexpr int SS = 4+3;
-constexpr int ESS = 4+3+2;
+constexpr int ESS = 4+3+2+4;
 constexpr int SM = 3+3;
-constexpr int ESM = 3+3+2;
+constexpr int ESM = 3+3+2+3;
 
 double sinc(double x) {
     // Use power series for small x
     if (std::abs(x) < 1e-4) return 1 - (x*x/6) + (x*x*x*x/120);
     return std::sin(x)/x;
 }
 
@@ -62,17 +62,24 @@
         double ddl = (dl_scale * std::abs(dl));
         double ddr = (dl_scale * std::abs(dr));
         double rho = 1 - 1e-8;
         if ( std::abs(vdiff) >= 1e-3 ) {
             rho = std::abs(std::tanh( vave / vdiff ));
         }
 
+        // TODO : make this configurable in the future
+        // TODO : do we actually need the penalty?
+        // the dq has a rotvec representation [ e1, e2, e3 ], these are the errors therein
+        double var_de = 1e-5; // var_de ~ 4*var_dq = (2 * delta_dq)^2 ~ var_ypr
         out[0] = ddl*ddl + 1e-8;
         out[1] = rho*ddl*ddr;
         out[2] = ddr*ddr + 1e-8;
+        out[3] = var_de;
+        out[4] = var_de;
+        out[5] = var_de;
     }
 
     int dead_reckon_apply(double* step, double *x, double *cov) {
         if ( step[1] == 0 && step[2] == 0 ) {
             // If the tracks didn't move, then just update the quaternion-part. There are two reasons dl=dr=0:
             //   1) The tracks didn't quite accrue a tick. In this case, the quaternion part might still have a
             //      bit of rotation, that we don't want to loose. However, the error accrual is SUPER small, and
@@ -95,33 +102,41 @@
             x[2],    // z
             x[3],    // a
             x[4],    // b
             x[5],    // c
             x[6],    // d
             step[1], // dl
             step[2], // dr
+            step[3], // dq_a
+            step[4], // dq_b
+            step[5], // dq_c
+            step[6], // dq_d
+
         };
 
-        double dr_cov[3];
+        double dr_cov[3+3];
         dead_reckon_step_errors(
                 step[1], step[2], // dl, dr
                 step[7], step[8], // vave, vdiff
                 0.005,
                 dr_cov);          // output
 
         // Create extended covariance matrix
         double P_z[ESM*ESM] = {
-            cov[0*SM + 0],cov[0*SM + 1],cov[0*SM + 2],cov[0*SM + 3],cov[0*SM + 4],cov[0*SM + 5],0,0,
-            cov[1*SM + 0],cov[1*SM + 1],cov[1*SM + 2],cov[1*SM + 3],cov[1*SM + 4],cov[1*SM + 5],0,0,
-            cov[2*SM + 0],cov[2*SM + 1],cov[2*SM + 2],cov[2*SM + 3],cov[2*SM + 4],cov[2*SM + 5],0,0,
-            cov[3*SM + 0],cov[3*SM + 1],cov[3*SM + 2],cov[3*SM + 3],cov[3*SM + 4],cov[3*SM + 5],0,0,
-            cov[4*SM + 0],cov[4*SM + 1],cov[4*SM + 2],cov[4*SM + 3],cov[4*SM + 4],cov[4*SM + 5],0,0,
-            cov[5*SM + 0],cov[5*SM + 1],cov[5*SM + 2],cov[5*SM + 3],cov[5*SM + 4],cov[5*SM + 5],0,0,
-            0,0,0,0,0,0,dr_cov[0],dr_cov[1],
-            0,0,0,0,0,0,dr_cov[1],dr_cov[2],
+            cov[0*SM + 0],cov[0*SM + 1],cov[0*SM + 2],cov[0*SM + 3],cov[0*SM + 4],cov[0*SM + 5],0,0,0,0,0,
+            cov[1*SM + 0],cov[1*SM + 1],cov[1*SM + 2],cov[1*SM + 3],cov[1*SM + 4],cov[1*SM + 5],0,0,0,0,0,
+            cov[2*SM + 0],cov[2*SM + 1],cov[2*SM + 2],cov[2*SM + 3],cov[2*SM + 4],cov[2*SM + 5],0,0,0,0,0,
+            cov[3*SM + 0],cov[3*SM + 1],cov[3*SM + 2],cov[3*SM + 3],cov[3*SM + 4],cov[3*SM + 5],0,0,0,0,0,
+            cov[4*SM + 0],cov[4*SM + 1],cov[4*SM + 2],cov[4*SM + 3],cov[4*SM + 4],cov[4*SM + 5],0,0,0,0,0,
+            cov[5*SM + 0],cov[5*SM + 1],cov[5*SM + 2],cov[5*SM + 3],cov[5*SM + 4],cov[5*SM + 5],0,0,0,0,0,
+            0,0,0,0,0,0,dr_cov[0],dr_cov[1],0,0,0,
+            0,0,0,0,0,0,dr_cov[1],dr_cov[2],0,0,0,
+            0,0,0,0,0,0,0,0,dr_cov[3],0,0,
+            0,0,0,0,0,0,0,0,0,dr_cov[4],0,
+            0,0,0,0,0,0,0,0,0,0,dr_cov[5]
         };
 
         // Get the sigma points
         // n = length of single sigma point: ESS
         // L = length size of covariance: ESM
         int n = ESS;
         int L = ESM;
@@ -138,41 +153,56 @@
             double dlrQ1[SS], dlrQ2[SS], R_neg_row[SM];
             for ( int j = 0; j < SM; j++ ) {
                 R_neg_row[j] = -R[i*L + j];
             }
             euclidean::convert_lrrv_to_lrQ(&R[i*L], dlrQ1);
             euclidean::convert_lrrv_to_lrQ(R_neg_row, dlrQ2);
 
-            // Write into the the sigma point the difference
+            // Extract the ddquat from the last rotvec
+            double ddquat1[4], ddquat2[4], R_neg_row2[3];
+            for ( int j = 0; j < 3; j++ ) {
+                R_neg_row2[j] = -R[i*L + j + (ESM-3)];
+            }
+            euclidean::convert_rotvec_to_quat(&R[i*L+(ESM-3)], ddquat1);
+            euclidean::convert_rotvec_to_quat(R_neg_row2, ddquat2);
+
+            // Write into the the sigma point the lrQ
             euclidean::compose_lrQ(z, dlrQ1,  &Z[(i+1)*n]);
             euclidean::compose_lrQ(z, dlrQ2, &Z[(i+L+1)*n]);
 
-            // Also add in the last two elements
+            // Also add the dl/drs
             Z[(i+1)*n + SS + 0] = z[SS + 0] + R[i*L + SM + 0];
             Z[(i+1)*n + SS + 1] = z[SS + 1] + R[i*L + SM + 1];
             Z[(i+L+1)*n + SS + 0] = z[SS + 0] - R[i*L + SM + 0];
             Z[(i+L+1)*n + SS + 1] = z[SS + 1] - R[i*L + SM + 1];
+
+            // Write into the the sigma point the difference: dquat*ddquat
+            euclidean::compose_quat(&z[ESS-4], ddquat1, &Z[(i+1)*n + (ESS-4)]);
+            euclidean::compose_quat(&z[ESS-4], ddquat2, &Z[(i+L+1)*n + (ESS-4)]);
+
         }
 
         // Transform the sigma points
         double Y[(2*L+1)*SS];
         for ( int i = 0; i < 2*L+1; i ++ ) {
             dead_reckon_step(
                 &Z[i*n + 3], //quat
                 z[SS + 0],   // dl
                 z[SS + 1],   // dr
                 step[7],     // vave
                 step[8],     // vave
                 &Y[i*SS]     // delta change
             );
+            // Note, this is basically a compose_lrQ(...) call. dx = quat^-1 @ [dx_body, dy_body, 0]
+            //  so Y = compose_lrQ(z, [ dx_body, dy_body, 0, dquat ]) = [ z_t + quat^-1@[dx_body, dy_body, 0], quat * dquat ]
             for ( int j = 0; j < 3; j ++ ) {
                 Y[i*SS + j] += Z[i*n + j]; // add initial value
             }
             // Write over the quaternion part with the new quaterion estimate
-            euclidean::compose_quat(&Z[i*n + 3], &step[3], &Y[i*SS + 3]);
+            euclidean::compose_quat(&Z[i*n + 3], &Z[i*n + (ESS-4)], &Y[i*SS + 3]);
         }
 
         // Iteratively calculate the lrQ mean
         // Copy Y[0] as my initial guess for y_bar
         double y_bar[SS];
         for ( int i = 0; i < SS; i++ ) {
             y_bar[i] = Y[i];
```

### Comparing `robotransforms-0.5.3/robotransforms/dead_reckon/base.h` & `robotransforms-0.5.4/robotransforms/dead_reckon/base.h`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/dead_reckon/dead_reckon.py` & `robotransforms-0.5.4/robotransforms/dead_reckon/dead_reckon.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/dead_reckon/dead_reckon_pure.py` & `robotransforms-0.5.4/robotransforms/dead_reckon/dead_reckon_pure.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,51 +47,64 @@
 def dead_reckon_step_errors( dl, dr, vave, vdiff, dl_scale=0.005):
     ddl = (dl_scale * np.abs(dl))
     ddr = (dl_scale * np.abs(dr))
     rho = 1-1e-8
     if ( np.abs(vdiff) >= 1e-3 ) :
         rho = np.abs(np.tanh( vave / vdiff ))
 
-    #  [ var_dl, cov_dldr, var_dr, var_b, var_c, var_d ]
-    return [ ddl*ddl + 1e-8, rho*ddl*ddr, ddr*ddr + 1e-8 ] # TODO : these are estimates, based on gps's 1Hz
+    # TODO : make this configurable in the future
+    # TODO : do we actually need the penalty?
+    # the dq has a rotvec representation [ e1, e2, e3 ], these are the errors therein
+    var_de = 1e-5 # var_de ~ 4*var_dq = (2 * delta_dq)^2 ~ var_ypr
+    #  [ var_dl, cov_dldr, var_dr, var_dqb, var_dqc, var_dqd ]
+    return [ ddl*ddl + 1e-8, rho*ddl*ddr, ddr*ddr + 1e-8, var_de, var_de, var_de ] # TODO : these are estimates, based on gps's 1Hz
 
 def dead_reckon_apply(x_hat, P_hat, step):
     SS = 7 # Full state size
+    ESS = 7 + 2 + 4 # dl/dr and then dq
     SM = 6 # Manifold state size
+    ESM = 6 + 2 + 3 # dl/dr and then de (rotvec of dq)
 
     if (step[1] == 0 and step[2] == 0):
         # If the tracks didn't move, then just update the quaternion-part. There are two reasons dl=dr=0:
         #   1) The tracks didn't quite accrue a tick. In this case, the quaternion part might still have a
         #      bit of rotation, that we don't want to loose. However, the error accrual is SUPER small, and
         #      this should only happen 'infrequently' so the loss of error is probably negilible. Fun fact,
         #      since the tick is gross, it turns out droping the quaternion correction builds up, so you loose
         #      something like 20degs over a 180deg turn. Wild, dude.
         #   2) The tracks really haven't been moving. In this case, the IMU is probably not moving either --
         #      except for drift (which we are handling elsewhere in the KF), so we are fine to just accrue
         #      the IMU corrections.
         return np.hstack([x_hat[:3], t.compose_quat(x_hat[3:SS], step[3:SS])]), P_hat.copy()
 
     # Build up extended state vector
-    z = np.zeros((SS+2))
+    z = np.zeros((ESS))
     z[:SS] = x_hat[:]
-    z[SS+0] = step[1]
-    z[SS+1] = step[2]
+    z[SS+0] = step[1] # dl
+    z[SS+1] = step[2] # dr
+    z[SS+2] = step[3] # dq_a
+    z[SS+3] = step[4] # dq_b
+    z[SS+4] = step[5] # dq_c
+    z[SS+5] = step[6] # dq_d
 
     # Build up extended covariance on manifold
-    P_z = np.zeros((SM+2,SM+2))
+    P_z = np.zeros((ESM,ESM))
     P_z[:SM,:SM] = P_hat[:SM,:SM]
     e = dead_reckon_step_errors( step[1], step[2], step[7], step[8] )
     P_z[0+SM][0+SM] = e[0] # var_dl
     P_z[0+SM][1+SM] = e[1] # cov_dldr
     P_z[1+SM][0+SM] = e[1] # cov_dldr
     P_z[1+SM][1+SM] = e[2] # var_dr
+    P_z[2+SM][2+SM] = e[3] # var_de1 (rotvec for dq)
+    P_z[3+SM][3+SM] = e[4] # var_de2 (rotvec for dq)
+    P_z[4+SM][4+SM] = e[5] # var_de3 (rotvec for dq)
 
     # Generate sigma points along manifold from enclosing deviation vectors with the state
-    L = SM+2
-    Z = np.zeros((2*L+1,SS+2))
+    L = ESM
+    Z = np.zeros((2*L+1,ESS))
     Z[0] = z.copy()
 
     scaled_cov = P_z * L_PLUS_LAMBDA
     # Rows of the R matrix in A=R^TR function like a square root
     try:
         # Generate the deviation vectors along manifold
         dz = np.linalg.cholesky( scaled_cov ).T # NOTE, np returns L, not R, so we transpose it
@@ -109,26 +122,34 @@
         # print(v)
         # print(w.T)
         raise e
 
 
     # extract the mean lrQ part
     lrQ = z[:SS]
+    dquat = z[-4:]
     for i in range(L):
         Z[1 + i][:SS] = t.compose_lrQ(lrQ, t.lrrv2lrQ(dz[i,:SM]))
-        Z[1 + i][-2:] = Z[0,-2:] + dz[i,-2:]
+        Z[1 + i][SS:SS+2] = Z[0,SS:SS+2] + dz[i,SS:SS+2]
+        Z[1 + i][-4:] = t.compose_quat(dquat, t.rotvec2quat(dz[i,-3:]))
 
         Z[1 + i + L][:SS] = t.compose_lrQ(lrQ, t.lrrv2lrQ(-dz[i,:SM]))
-        Z[1 + i + L][-2:] = Z[0,-2:] - dz[i,-2:]
+        Z[1 + i + L][SS:SS+2] = Z[0,SS:SS+2] - dz[i,SS:SS+2]
+        Z[1 + i + L][-4:] = t.compose_quat(dquat, t.rotvec2quat(-dz[i,-3:]))
 
     # Transform to new vectors
     def T(_z):
+        # initial quaternion part
         quat = _z[3:SS]
         dx = dead_reckon_step( quat=quat, dl=z[SS+0], dr=z[SS+1], vave=step[7], vdiff=step[8] )
-        nquat = t.compose_quat(quat,step[3:7])
+        # Post rotation quaternion part
+        nquat = t.compose_quat(quat,_z[-4:])
+
+        # Note, this is basically a compose_lrQ(...) call. dx = quat^-1 @ [dx_body, dy_body, 0]
+        #  so z_new = compose_lrQ(z, [ dx_body, dy_body, 0, dquat ]) = [ z_t + quat^-1@[dx_body, dy_body, 0], quat * dquat ]
         return np.hstack([_z[:3] + dx, nquat]);
 
     Y = np.array([ T(_z) for _z in Z ])
 
     LAMBDA = L_PLUS_LAMBDA - L
     W0 = LAMBDA / L_PLUS_LAMBDA
     W = 1 / ( 2 * L_PLUS_LAMBDA )
```

### Comparing `robotransforms-0.5.3/robotransforms/dead_reckon/wrapper.cpp` & `robotransforms-0.5.4/robotransforms/dead_reckon/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/euclidean/base.cpp` & `robotransforms-0.5.4/robotransforms/euclidean/base.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/euclidean/base.h` & `robotransforms-0.5.4/robotransforms/euclidean/base.h`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/euclidean/euclidean.py` & `robotransforms-0.5.4/robotransforms/euclidean/euclidean.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/euclidean/euclidean_pure.py` & `robotransforms-0.5.4/robotransforms/euclidean/euclidean_pure.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/euclidean/wrapper.cpp` & `robotransforms-0.5.4/robotransforms/euclidean/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/utils/base.cpp` & `robotransforms-0.5.4/robotransforms/utils/base.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/utils/utils.py` & `robotransforms-0.5.4/robotransforms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/utils/utils_pure.py` & `robotransforms-0.5.4/robotransforms/utils/utils_pure.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms/utils/wrapper.cpp` & `robotransforms-0.5.4/robotransforms/utils/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/robotransforms.egg-info/PKG-INFO` & `robotransforms-0.5.4/robotransforms.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotransforms
-Version: 0.5.3
+Version: 0.5.4
 Summary: A transformation library for robot motion
 Home-page: https://github.com/Nova-Dynamics/transforms-python
 Author: Jonathan D. B. Van Schenck
 Author-email: jvschenck@novadynamics.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `robotransforms-0.5.3/robotransforms.egg-info/SOURCES.txt` & `robotransforms-0.5.4/robotransforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.3/setup.py` & `robotransforms-0.5.4/setup.py`

 * *Files identical despite different names*

