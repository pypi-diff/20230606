# Comparing `tmp/tcflow-0.0.9.tar.gz` & `tmp/tcflow-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcflow-0.0.9.tar", last modified: Tue Apr 11 18:54:50 2023, max compression
+gzip compressed data, was "tcflow-0.1.0.tar", last modified: Tue Jun  6 08:05:48 2023, max compression
```

## Comparing `tcflow-0.0.9.tar` & `tcflow-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 18:54:50.708644 tcflow-0.0.9/
--rw-rw-rw-   0        0        0    11558 2023-04-04 09:02:41.000000 tcflow-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     7499 2023-04-11 18:54:50.707642 tcflow-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     6959 2023-04-04 09:02:41.000000 tcflow-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 18:54:50.708644 tcflow-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      950 2023-04-11 09:21:24.000000 tcflow-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:54:50.702644 tcflow-0.0.9/tcflow/
--rw-rw-rw-   0        0        0     2743 2023-04-11 09:17:35.000000 tcflow-0.0.9/tcflow/EMD_MD_OPs.py
--rw-rw-rw-   0        0        0     3891 2023-04-11 10:12:49.000000 tcflow-0.0.9/tcflow/EMD_reprocess_OPs.py
--rw-rw-rw-   0        0        0     5142 2023-04-11 10:01:59.000000 tcflow-0.0.9/tcflow/EMD_run.py
--rw-rw-rw-   0        0        0     1984 2023-04-11 10:08:36.000000 tcflow-0.0.9/tcflow/NEMD_MD_OPs.py
--rw-rw-rw-   0        0        0     6180 2023-04-11 18:34:20.000000 tcflow-0.0.9/tcflow/NEMD_reprocess_OPs.py
--rw-rw-rw-   0        0        0     3736 2023-04-11 17:48:41.000000 tcflow-0.0.9/tcflow/NEMD_run.py
--rw-rw-rw-   0        0        0        0 2023-04-04 09:02:41.000000 tcflow-0.0.9/tcflow/__init__.py
--rw-rw-rw-   0        0        0     9180 2023-04-04 09:02:41.000000 tcflow-0.0.9/tcflow/input_gen.py
--rw-rw-rw-   0        0        0     8812 2023-04-04 09:02:41.000000 tcflow-0.0.9/tcflow/run_emd.py
--rw-rw-rw-   0        0        0     9501 2023-04-04 09:02:41.000000 tcflow-0.0.9/tcflow/run_nemd.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:54:50.707642 tcflow-0.0.9/tcflow.egg-info/
--rw-rw-rw-   0        0        0     7499 2023-04-11 18:54:50.000000 tcflow-0.0.9/tcflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-04-11 18:54:50.000000 tcflow-0.0.9/tcflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 18:54:50.000000 tcflow-0.0.9/tcflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-04-11 18:54:50.000000 tcflow-0.0.9/tcflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 18:54:50.000000 tcflow-0.0.9/tcflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 08:05:48.509075 tcflow-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-05-28 09:19:52.000000 tcflow-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0    16106 2023-06-06 08:05:48.509075 tcflow-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    15282 2023-05-29 20:07:24.000000 tcflow-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 08:05:48.509075 tcflow-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2023-06-06 08:04:43.000000 tcflow-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:05:48.509075 tcflow-0.1.0/tcflow/
+-rw-rw-rw-   0        0        0     2784 2023-05-28 20:00:29.000000 tcflow-0.1.0/tcflow/EMD_MD_OPs.py
+-rw-rw-rw-   0        0        0     3891 2023-05-28 09:19:52.000000 tcflow-0.1.0/tcflow/EMD_reprocess_OPs.py
+-rw-rw-rw-   0        0        0     7074 2023-05-29 20:29:24.000000 tcflow-0.1.0/tcflow/EMD_run.py
+-rw-rw-rw-   0        0        0     1973 2023-05-28 20:00:32.000000 tcflow-0.1.0/tcflow/NEMD_MD_OPs.py
+-rw-rw-rw-   0        0        0     6240 2023-05-28 09:19:52.000000 tcflow-0.1.0/tcflow/NEMD_reprocess_OPs.py
+-rw-rw-rw-   0        0        0     6638 2023-05-28 19:48:42.000000 tcflow-0.1.0/tcflow/NEMD_run.py
+-rw-rw-rw-   0        0        0        0 2023-05-28 09:19:52.000000 tcflow-0.1.0/tcflow/__init__.py
+-rw-rw-rw-   0        0        0     9272 2023-05-29 13:04:41.000000 tcflow-0.1.0/tcflow/input_gen.py
+-rw-rw-rw-   0        0        0     1395 2023-05-28 09:19:52.000000 tcflow-0.1.0/tcflow/submit.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:05:48.509075 tcflow-0.1.0/tcflow.egg-info/
+-rw-rw-rw-   0        0        0    16106 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/top_level.txt
```

### Comparing `tcflow-0.0.9/LICENSE` & `tcflow-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcflow-0.0.9/setup.py` & `tcflow-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tcflow",
-    version="0.0.9",
+    version="0.1.0",
     author="Wenjie Zhang",
     author_email="gdbhcxhmjk@163.com",
     description="A framework for thermal conductivity calculation based on EMD&NEMD methods",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gdbhcxhmjk-z/ThermalConductivity-Workflow.git",
     packages=setuptools.find_packages(),
@@ -23,9 +23,13 @@
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
-    provides=["tcflow"]
+    provides=["tcflow"],
+    script=[],
+    entry_points={'console_scripts': [
+         'tcflow = tcflow.submit:tc_main',
+     ]}
 )
```

### Comparing `tcflow-0.0.9/tcflow/EMD_MD_OPs.py` & `tcflow-0.1.0/tcflow/EMD_MD_OPs.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     def __init__(self):
         pass
 
     @classmethod
     def get_input_sign(cls):
         return OPIOSign({
             "data":Artifact(Path),
+            "param":dict,
             "input": Artifact(Path),
             #"input_gen":Artifact(Path),
             "force_field":Artifact(List[Path]),
         })
 
     @classmethod
     def get_output_sign(cls):
@@ -37,15 +38,16 @@
         print(input)
         print(data)
         print(force_field)
         Path('in.lammps').symlink_to(input)
         Path('data.lammps').symlink_to(data)
         for field in force_field:
             Path(field.parts[-1]).symlink_to(field)
-        os.system(f"mpirun -n 1 lmp < in.lammps")
+        input_gen.NVT_input(param)
+        os.system(param["md_command"])
         logfile=Path("log.lammps")
         dumpfile=Path("NVT.lammpstrj")
         op_out = OPIO({
             "dump":dumpfile,
             "log":logfile,
         })
         return op_out
@@ -87,14 +89,14 @@
         name.mkdir()
         cwd = os.getcwd()
         os.chdir(name)
         for field in force_field:
             Path(field.parts[-1]).symlink_to(field)
         Path('data.lammps').symlink_to(data)
         input_gen.NVE_input(param)
-        os.system(f"mpirun -n 1 lmp < in.lammps")
+        os.system(param["md_command"])
         os.chdir(cwd)
         logfile=name/"log.lammps"
         op_out = OPIO({
             "dat":logfile,
         })
         return op_out
```

### Comparing `tcflow-0.0.9/tcflow/EMD_reprocess_OPs.py` & `tcflow-0.1.0/tcflow/EMD_reprocess_OPs.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.0.9/tcflow/NEMD_MD_OPs.py` & `tcflow-0.1.0/tcflow/NEMD_MD_OPs.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         name.mkdir()
         cwd = os.getcwd()
         os.chdir(name)
         for field in force_field:
             Path(field.parts[-1]).symlink_to(field)
         Path('data.lammps').symlink_to(data)
         input_gen.NEMD_input(param)
-        os.system(f"mpirun -n 1 lmp < in.lammps")
+        os.system(param["md_command"])
         # os.system(f"mv log.lammps {name}.log")
         # logfile=Path(f"{name}.log")
         os.chdir(cwd)
         allfile= name
         # logfile=name/"log.lammps"
         # datafile=name/"data.lammps"
         # tempfile=name/"temp_profile.txt"
```

### Comparing `tcflow-0.0.9/tcflow/NEMD_reprocess_OPs.py` & `tcflow-0.1.0/tcflow/NEMD_reprocess_OPs.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         kappa = np.array(kappa)
         extrapolation = stats.linregress(1/L, 1/kappa)
         plt.plot(1/L,1/kappa,'o')
         x=np.arange(0,1.2*max(1/L),max(1/L)/100)
         plt.plot(x, extrapolation.intercept + extrapolation.slope*x, 'r')
         extra = plt.Rectangle((0, 0), 0, 0, fc="w", fill=False, edgecolor='none', linewidth=0)
         plt.legend([extra],[f"EXTRAP. 1/K = {extrapolation.intercept:02f}+{extrapolation.slope:02f}*1/L" ],loc="upper left",fontsize="small")
+        plt.ylim(extrapolation.intercept,1.2*max(1/kappa))
         plt.xlabel('1/L($\AA$^-1)')
         plt.ylabel('1/kappa(mK/W)')
         plt.title("Thermal Conductivity:NEMD Extrapolation")
         plt.savefig("thermal_conductivity.png")
         plt.close()
         with open("result.txt",'w') as f:
             for i in range(len(kappa)):
```

### Comparing `tcflow-0.0.9/tcflow/input_gen.py` & `tcflow-0.1.0/tcflow/input_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 def make_structure(file,force_field,mass):
     file+="""
 #####################################################################
 #                       Read Structure
 #####################################################################
 read_data data.lammps
 """
-    file+=force_field+'\n'
+    for l in force_field:
+        file+=l+'\n'
     for i in range(len(mass)):
         file+=f"mass {i+1} {mass[i]} \n"
     return file
 
 def energy_minimization(file):
     file+="""
 #####################################################################
@@ -204,15 +205,16 @@
 
 def NVT_input(param):
     NVT ="#NVT simulation for different configurations\n"
     NVT = variable_initialization(NVT,param['temperature'],param['time_step'],param['thermo_print_interval'],param['traj_print_interval'])
     NVT = make_structure(NVT,param['load_force_field'],param['mass_map'])
     NVT = energy_minimization(NVT)
     NVT = velocity_initialization(NVT)
-    steps = np.max((param['num_configurations']*param['traj_print_interval']*10,200000))
+    num = param.get("num_configurations",None) if param.get("num_configurations",None) else 0
+    steps = np.max((num*param['traj_print_interval']*10,200000))
     NVT = NVT_equilibrium(NVT,steps)
     with open("NVT.lammps",'w') as fp:
         fp.write(NVT)
 
 def NVE_input(param):
     NVE ="#NVE simulation for heat flux\n"
     NVE = variable_initialization(NVE,param['temperature'],param['time_step'],param['thermo_print_interval'],param['traj_print_interval'])
```

