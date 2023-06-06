# Comparing `tmp/orr_sommerfeld_convmix_cgb-0.1.8.tar.gz` & `tmp/orr_sommerfeld_convmix_cgb-0.1.9.tar.gz`

## Comparing `orr_sommerfeld_convmix_cgb-0.1.8.tar` & `orr_sommerfeld_convmix_cgb-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.8/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.8/src/Orr_Sommerfeld_convmix_CGB/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.8/LICENSE
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.8/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/src/Orr_Sommerfeld_convmix_CGB/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/LICENSE
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/PKG-INFO
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.8/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py` & `orr_sommerfeld_convmix_cgb-0.1.9/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,34 +279,38 @@
     #b=-v[i]**2/(vr[i]*sqrt(norm[i]))
     c= a + (1j*b)   
     #Luego normalizo todas las autofunciones con el c hallado
     v=c*v
     u=c*u
     w=c*w
     tita=c*tita
+    v= (hstack(( [0.],v , [0.])))
+    u= (hstack(( [0.],u , [0.])))
+    w= (hstack(( [0.],w , [0.])))
+    tita= (hstack(( [0.],tita , [0.])))
     return v,u,w,tita  
 def grafica_autofunciones(N,Ra,Pr,Re,alpha,beta):
     #plt.style.use('ggplot')
     #Vector y
     D,y = cheb(N)
     #Vectores de perturbaciones para un autovalor dado. En este caso tomo el mayor de todos dado que Orr_Sommerfeld() las ordena y voy a elegir n=0
     n=0
     lam,V,max_real,max_imag=Orr_Sommerfeld(N,Ra,Pr,Re,alpha,beta)
 
     v,u,w,tita=vector_perturbaciones(N,lam,V,n,alpha,beta)
     v,u,w,tita=normalizacion(v,u,w,tita)
 
-    realv = (hstack(( [0.],v.real , [0.])))
-    imv = (hstack(( [0.],v.imag , [0.])))
-    realtita = (hstack(( [0.],tita.real , [0.])))
-    imtita = (hstack(( [0.],tita.imag , [0.])))
-    realu = (hstack(( [0.],u.real , [0.])))
-    imu = (hstack(( [0.],u.imag , [0.])))
-    realw = (hstack(( [0.],w.real , [0.])))
-    imw = (hstack(( [0.],w.imag , [0.])))
+    realv = v.real
+    imv = v.imag
+    realtita = tita.real
+    imtita = tita.imag
+    realu = u.real
+    imu = u.imag 
+    realw = w.real 
+    imw = w.imag
 
     plt.plot(y,realv,c='red',label= "$v_r(y)$")
     plt.plot(y,imv,"--",c='red',label= "$v_i(y)$")
     plt.plot(y,realtita,"-",c='blue',label= r'$\theta_{r}(y)$')
     plt.plot(y,imtita,"--",c='blue',label= r'$\theta_{i}(y)$')
     plt.plot(y,realu,c='lightgreen',label= r'$u_{r}(y)$')
     plt.plot(y,imu,"--",c='lightgreen',label= r'$u_{i}(y)$')
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.8/LICENSE` & `orr_sommerfeld_convmix_cgb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.1.8/pyproject.toml` & `orr_sommerfeld_convmix_cgb-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Orr_Sommerfeld_convmix_CGB"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Pablo Szuban", email="pablo.szuban@ib.edu.ar" },
 ]
 description = "Paquete para cálculo de autovalores y autofunciones."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.8/PKG-INFO` & `orr_sommerfeld_convmix_cgb-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orr_Sommerfeld_convmix_CGB
-Version: 0.1.8
+Version: 0.1.9
 Summary: Paquete para cálculo de autovalores y autofunciones.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Pablo Szuban <pablo.szuban@ib.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

