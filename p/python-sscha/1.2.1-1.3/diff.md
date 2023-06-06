# Comparing `tmp/python-sscha-1.2.1.tar.gz` & `tmp/python-sscha-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sscha-1.2.1.tar", last modified: Thu Sep 15 10:06:02 2022, max compression
+gzip compressed data, was "python-sscha-1.3.tar", last modified: Tue Jun  6 10:23:25 2023, max compression
```

## Comparing `python-sscha-1.2.1.tar` & `python-sscha-1.3.tar`

### file list

```diff
@@ -1,41 +1,49 @@
-drwxrwxr-x   0 lmonacelli  (1001) lmonacelli  (1002)        0 2022-09-15 10:06:02.669170 python-sscha-1.2.1/
-drwxrwxr-x   0 lmonacelli  (1001) lmonacelli  (1002)        0 2022-09-15 10:06:02.669170 python-sscha-1.2.1/Modules/
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)    10879 2022-06-09 15:44:45.304328 python-sscha-1.2.1/Modules/AdvancedCalculations.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     4823 2022-01-04 14:31:02.941229 python-sscha-1.2.1/Modules/Calculator.py
--rw-r--r--   0 lmonacelli  (1001) lmonacelli  (1002)    65504 2022-09-12 07:38:34.358215 python-sscha-1.2.1/Modules/Cluster.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)    10288 2022-01-04 14:31:02.941229 python-sscha-1.2.1/Modules/Dynamical.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)   132416 2022-09-12 07:39:16.845775 python-sscha-1.2.1/Modules/Ensemble.py
--rw-r--r--   0 lmonacelli  (1001) lmonacelli  (1002)    15683 2022-05-23 09:04:27.741150 python-sscha-1.2.1/Modules/Minimizer.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)    15751 2022-05-20 15:52:58.659346 python-sscha-1.2.1/Modules/Optimizer.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     1173 2022-01-04 14:31:02.945229 python-sscha-1.2.1/Modules/Parallel.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)    32819 2022-09-12 07:39:16.845775 python-sscha-1.2.1/Modules/Relax.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)    76692 2022-09-12 07:39:16.845775 python-sscha-1.2.1/Modules/SchaMinimizer.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)    18362 2022-05-20 15:52:58.659346 python-sscha-1.2.1/Modules/Tools.py
--rw-r--r--   0 lmonacelli  (1001) lmonacelli  (1002)    24140 2022-05-23 09:04:27.741150 python-sscha-1.2.1/Modules/Utilities.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)       80 2022-01-04 14:31:02.945229 python-sscha-1.2.1/Modules/__init__.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)      264 2022-09-15 10:06:02.669170 python-sscha-1.2.1/PKG-INFO
-drwxrwxr-x   0 lmonacelli  (1001) lmonacelli  (1002)        0 2022-09-15 10:06:02.669170 python-sscha-1.2.1/SCHAModules/
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)      870 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/cell_force.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     3354 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/get_cmat.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     1442 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/get_emat.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     1333 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/get_g.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)    17132 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/get_gradient_supercell.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)    14175 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/get_gradient_supercell_fast.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     5029 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/get_odd_straight.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     4215 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/get_odd_straight_with_v4.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)    10186 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/get_stress_tensor.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     1997 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/get_upsilon_matrix.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     4044 2022-09-12 07:39:16.845775 python-sscha-1.2.1/SCHAModules/get_v3.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     3540 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/get_v4.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     9696 2022-09-12 07:39:16.845775 python-sscha-1.2.1/SCHAModules/module_anharmonic.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     3172 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/module_new_thermodynamic.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     8213 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/module_stochastic.f90
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     4547 2022-01-04 14:31:02.945229 python-sscha-1.2.1/SCHAModules/multiply_lambda_tensor.f90
-drwxrwxr-x   0 lmonacelli  (1001) lmonacelli  (1002)        0 2022-09-15 10:06:02.669170 python-sscha-1.2.1/scripts/
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     3585 2022-01-04 14:31:03.061228 python-sscha-1.2.1/scripts/cluster_check.x
--rwxrwxr-x   0 lmonacelli  (1001) lmonacelli  (1002)      842 2022-05-20 15:52:58.663346 python-sscha-1.2.1/scripts/plot_frequencies.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     3565 2022-01-04 14:31:03.061228 python-sscha-1.2.1/scripts/read_incomplete_ensemble.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     4960 2022-05-20 15:52:58.663346 python-sscha-1.2.1/scripts/sscha
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     4715 2022-05-24 07:55:47.377235 python-sscha-1.2.1/scripts/sscha-plot-data.py
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     8052 2022-01-04 14:31:03.061228 python-sscha-1.2.1/scripts/static-vc-relax.pyx
--rw-rw-r--   0 lmonacelli  (1001) lmonacelli  (1002)     6937 2022-09-15 10:05:49.501297 python-sscha-1.2.1/setup.py
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:23:25.297097 python-sscha-1.3/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    35149 2023-02-13 14:58:18.000000 python-sscha-1.3/LICENSE.txt
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:23:25.281097 python-sscha-1.3/Modules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10879 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/AdvancedCalculations.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4823 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Calculator.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    66394 2023-05-16 12:51:43.000000 python-sscha-1.3/Modules/Cluster.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10288 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Dynamical.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   132589 2023-02-23 10:36:25.000000 python-sscha-1.3/Modules/Ensemble.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    15683 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Minimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    15751 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Optimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1173 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Parallel.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    32819 2023-02-23 10:36:25.000000 python-sscha-1.3/Modules/Relax.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    76682 2023-02-23 10:37:43.000000 python-sscha-1.3/Modules/SchaMinimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    18362 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Tools.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    24140 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Utilities.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       80 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/__init__.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      227 2023-06-06 10:23:25.297097 python-sscha-1.3/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8066 2023-05-16 12:51:43.000000 python-sscha-1.3/README.md
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:23:25.285097 python-sscha-1.3/SCHAModules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      870 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/cell_force.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3354 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_cmat.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1442 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_emat.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1333 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_g.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    17132 2023-02-23 10:36:26.000000 python-sscha-1.3/SCHAModules/get_gradient_supercell.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    14175 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_gradient_supercell_fast.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5029 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_odd_straight.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4215 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_odd_straight_with_v4.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10186 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_stress_tensor.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1997 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_upsilon_matrix.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4044 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_v3.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3540 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_v4.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     9696 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/module_anharmonic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3172 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/module_new_thermodynamic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8213 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/module_stochastic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4547 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/multiply_lambda_tensor.f90
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:23:25.285097 python-sscha-1.3/python_sscha.egg-info/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      227 2023-06-06 10:23:25.000000 python-sscha-1.3/python_sscha.egg-info/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1126 2023-06-06 10:23:25.000000 python-sscha-1.3/python_sscha.egg-info/SOURCES.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-06 10:23:25.000000 python-sscha-1.3/python_sscha.egg-info/dependency_links.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       18 2023-06-06 10:23:25.000000 python-sscha-1.3/python_sscha.egg-info/top_level.txt
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:23:25.297097 python-sscha-1.3/scripts/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3585 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/cluster_check.x
+-rwxrwxr-x   0 monacell  (1001) monacell  (1001)      842 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/plot_frequencies.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3565 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/read_incomplete_ensemble.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4960 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/sscha
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4715 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/sscha-plot-data.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8052 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/static-vc-relax.pyx
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-06 10:23:25.297097 python-sscha-1.3/setup.cfg
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     6935 2023-06-06 10:23:07.000000 python-sscha-1.3/setup.py
```

### Comparing `python-sscha-1.2.1/Modules/AdvancedCalculations.py` & `python-sscha-1.3/Modules/AdvancedCalculations.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/Modules/Calculator.py` & `python-sscha-1.3/Modules/Calculator.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/Modules/Cluster.py` & `python-sscha-1.3/Modules/Cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 __CLUSTER_UTIME__ = "use_time"
 __CLUSTER_VMEM__ = "v_memory"
 __CLUSTER_NMEM__ = "max_ram"
 __CLUSTER_UMEM__ = "use_memory"
 __CLUSTER_VPART__ = "v_partition"
 __CLUSTER_NPART__ = "partition_name"
 __CLUSTER_UPART__ = "use_partition"
+__CLUSTER_VQOS__ = "v_qos"
+__CLUSTER_NQOS__ = "qos_name"
+__CLUSTER_UQOS__ = "use_qos"
 __CLUSTER_INITSCRIPT__ = "init_script"
 __CLUSTER_MAXRECALC__ = "max_recalc"
 __CLUSTER_BATCHSIZE__ = "batch_size"
 __CLUSTER_LOCALWD__ = "local_workdir"
 __CLUSTER_VACCOUNT__ = "v_account"
 __CLUSTER_UACCOUNT__ = "use_account"
 __CLUSTER_SSHCMD__ = "sshcmd"
@@ -87,15 +90,16 @@
 # List all the possible keys
 __CLUSTER_KEYS__ = [__CLUSTER_NAMELIST__, __CLUSTER_TEMPLATE__, __CLUSTER_HOST__, __CLUSTER_PWD__,
                     __CLUSTER_ACCOUNT__, __CLUSTER_BINARY__, __CLUSTER_MPICMD__, __CLUSTER_TERMINAL__,
                     __CLUSTER_SUBCMD__, __CLUSTER_SUBNAME__, __CLUSTER_VNODES__, __CLUSTER_NNODES__,
                     __CLUSTER_UNODES__, __CLUSTER_VCPU__, __CLUSTER_NCPU__, __CLUSTER_UCPU__,
                     __CLUSTER_VTIME__, __CLUSTER_NTIME__, __CLUSTER_UTIME__, __CLUSTER_VMEM__,
                     __CLUSTER_NMEM__, __CLUSTER_UMEM__, __CLUSTER_VPART__, __CLUSTER_NPART__,
-                    __CLUSTER_UPART__, __CLUSTER_INITSCRIPT__, __CLUSTER_MAXRECALC__, __CLUSTER_BATCHSIZE__,
+                    __CLUSTER_UPART__, __CLUSTER_VQOS__, __CLUSTER_NQOS__, __CLUSTER_UQOS__,
+                    __CLUSTER_INITSCRIPT__, __CLUSTER_MAXRECALC__, __CLUSTER_BATCHSIZE__,
                     __CLUSTER_LOCALWD__, __CLUSTER_VACCOUNT__, __CLUSTER_UACCOUNT__, __CLUSTER_SSHCMD__,
                     __CLUSTER_SCPCMD__, __CLUSTER_WORKDIR__, __CLUSTER_TIMEOUT__, 
                     __CLUSTER_JOBNUMBER__, __CLUSTER_NPARALLEL__, __CLUSTER_NPOOLS__,
                     __CLUSTER_ATTEMPTS__, __CLUSTER_PORT__]
 
 
 SPECIAL_SYMBOLS = ["$", ";", "|"]
@@ -128,15 +132,15 @@
 
 
 
 
 class Cluster(object):
     
     def __init__(self, hostname=None, pwd=None, extra_options="", workdir = "",
-                 account_name = "", partition_name = "", binary="pw.x -npool NPOOL -i PREFIX.pwi > PREFIX.pwo",
+                 account_name = "", partition_name = "", qos_name = "", binary="pw.x -npool NPOOL -i PREFIX.pwi > PREFIX.pwo",
                  mpi_cmd=r"srun --mpi=pmi2 -n NPROC"):
         """
         SETUP THE CLUSTER
         =================
         It is strongly suggested to use public/private keys.
         However, sometimes for some reasons it is not possible to do so.
         Then you must install sshpass, and provide the password 
@@ -159,14 +163,16 @@
             workdir:
                 The workinig directory in the cluster. This is the directory
                 in which the job will be runned.
             account_name:
                 The name of the account for the job submission
             partition_name:
                 The partition name for the job submission
+            qos_name:
+                The QOS name for the job submission
         """
         
         self.hostname = hostname
         self.pwd = pwd
 
         self.sshcmd = "ssh"
         self.sshcmd = "ssh " + extra_options
@@ -185,14 +191,17 @@
             self.scpcmd = "scp " + extra_options.replace("-p", "-P")
 
     
         self.account_name = account_name
         self.partition_name = partition_name
         if partition_name:
             self.use_partition = True
+        self.qos_name = qos_name
+        if qos_name:
+            self.use_qos = True
             
         self.binary = binary
         self.mpi_cmd = mpi_cmd
 
         self.workdir=r""
         self.submit_command="sbatch"
         self.submit_name="SBATCH"
@@ -205,14 +214,16 @@
         self.use_account = True
         self.v_time="--time="
         self.use_time = True
         self.v_memory="--mem="
         self.use_memory = False
         self.v_partition="--partition="
         self.use_partition= False
+        self.v_qos = "--qos="
+        self.use_qos = False
         self.timeout = 1000
         self.use_timeout = False
 
         # Check the status of the job every TOT seconds
         self.check_timeout = 300
         self.nonblocking_command = True # True if you use a different version of slurm that does not accept blocking commands
 
@@ -255,14 +266,17 @@
         
         # The ram required for the calculation
         self.ram="10000Mb" # 10Gb
         
         # The default partition in which to submit calculations
         self.partition_name = ""
         
+        # The default qos in which to submit calculations
+        self.qos_name = ""
+
         # Still unused
         self.prefix_name = "prefix" # Variable in the calculator for differentiating the calculations
         
         # This directory is used to work with clusters.
         self.local_workdir = "cluster_work/"
         
         # The batch size is the maximum number of job to be submitted together.
@@ -477,14 +491,16 @@
             submission += "#%s %s%s\n" % (self.submit_name, self.v_time, self.time)
         if self.use_account:
             submission += "#%s %s%s\n" % (self.submit_name, self.v_account, self.account_name)
         if self.use_memory:
             submission += "#%s %s%s\n" % (self.submit_name, self.v_memory, self.ram)
         if self.use_partition:
             submission += "#%s %s%s\n" % (self.submit_name, self.v_partition, self.partition_name)
+        if self.use_qos:
+            submission += "#%s %s%s\n" % (self.submit_name, self.v_qos, self.qos_name)
 
         # Append the additional parameters
         for add_parameter in self.custom_params:
 
             adder_string = "--{}".format(add_parameter)
             if add_parameter.startswith("-"):
                 adder_string = add_parameter
@@ -1299,14 +1315,21 @@
         if __CLUSTER_VPART__ in keys:
             self.v_partition = c_info[__CLUSTER_VPART__]
         if __CLUSTER_NPART__ in keys:
             self.partition_name = c_info[__CLUSTER_NPART__]
             self.use_partition = True
         #if __CLUSTER_UPART__ in keys:
         #    self.use_partition = c_info[__CLUSTER_UPART__]
+        if __CLUSTER_VQOS__ in keys:
+            self.v_qos = c_info[__CLUSTER_VQOS__]
+        if __CLUSTER_NQOS__ in keys:
+            self.qos_name = c_info[__CLUSTER_NQOS__]
+            self.use_qos = True
+        if __CLUSTER_UQOS__ in keys:
+            self.use_qos = c_info[__CLUSTER_UQOS__]
         if __CLUSTER_UACCOUNT__ in keys:
             self.use_account = c_info[__CLUSTER_UACCOUNT__]
         if __CLUSTER_VACCOUNT__ in keys:
             self.v_account = c_info[__CLUSTER_VACCOUNT__]
         if __CLUSTER_NPOOLS__ in keys:
             self.n_pool = int(c_info[__CLUSTER_NPOOLS__])
```

### Comparing `python-sscha-1.2.1/Modules/Dynamical.py` & `python-sscha-1.3/Modules/Dynamical.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/Modules/Ensemble.py` & `python-sscha-1.3/Modules/Ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -1775,17 +1775,21 @@
         # Interpolate the dynamical matrix
         if support_dyn_fine is not None:
             new_dyn = self.current_dyn.Interpolate( self.current_dyn.GetSupercell(),
                                                     target_supercell,
                                                     support_dyn_coarse,
                                                     support_dyn_fine)
         else:
-            new_dyn = self.current_dyn.InterpolateMesh(target_supercell, lo_to_splitting = True)
+            new_dyn = self.current_dyn.Interpolate( self.current_dyn.GetSupercell(),
+                                                    target_supercell)
+
+        #else:
+        #    new_dyn = self.current_dyn.InterpolateMesh(target_supercell, lo_to_splitting = True)
 
-        print("dyn after interpolation:", new_dyn.GetSupercell())
+        #print("dyn after interpolation:", new_dyn.GetSupercell())
 
 
         # Get the new harmonic free energy
         harm_fe = new_dyn.GetHarmonicFreeEnergy(self.current_T,
                                                 not error_on_imaginary_frequency)
         harm_fe /= np.prod(target_supercell)
```

### Comparing `python-sscha-1.2.1/Modules/Minimizer.py` & `python-sscha-1.3/Modules/Minimizer.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/Modules/Optimizer.py` & `python-sscha-1.3/Modules/Optimizer.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/Modules/Parallel.py` & `python-sscha-1.3/Modules/Parallel.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/Modules/Relax.py` & `python-sscha-1.3/Modules/Relax.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/Modules/SchaMinimizer.py` & `python-sscha-1.3/Modules/SchaMinimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
                         print('    [symmetrization]  Time to prepare the suprecell dyn   : {:.6f} s'.format(t_6 - t_5))
                         print('    [symmetrization]  Time to symmetrize in the supercell : {:.6f} s'.format(t_7 - t_6))
                         print('    [symmetrization]  Time to return in fourier space     : {:.6f} s'.format(t_8 - t_7))
                     
                     # Apply the sum rule at gamma
                     CC.symmetries.CustomASR(dyn_grad[0,:,:])
                 else:
-                    qe_sym.SymmetrizeFCQ(dyn_grad, np.array(self.dyn.q_stars), asr = "custom")
+                    qe_sym.SymmetrizeFCQ(dyn_grad, self.dyn.q_stars, asr = "custom")
                     #qe_sym.SymmetrizeFCQ(err, np.array(self.dyn.q_stars), asr = "custom")
 
                 # Just divide the error by the square root the number of symmetries
                 err /= np.sqrt(qe_sym.QE_nsym * np.prod(self.ensemble.supercell))
             else:
                 CC.symmetries.CustomASR(dyn_grad[0, :,:])
         t2 = time.time()
```

### Comparing `python-sscha-1.2.1/Modules/Tools.py` & `python-sscha-1.3/Modules/Tools.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/Modules/Utilities.py` & `python-sscha-1.3/Modules/Utilities.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/cell_force.f90` & `python-sscha-1.3/SCHAModules/cell_force.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_cmat.f90` & `python-sscha-1.3/SCHAModules/get_cmat.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_emat.f90` & `python-sscha-1.3/SCHAModules/get_emat.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_g.f90` & `python-sscha-1.3/SCHAModules/get_g.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_gradient_supercell.f90` & `python-sscha-1.3/SCHAModules/get_gradient_supercell.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_gradient_supercell_fast.f90` & `python-sscha-1.3/SCHAModules/get_gradient_supercell_fast.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_odd_straight.f90` & `python-sscha-1.3/SCHAModules/get_odd_straight.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_odd_straight_with_v4.f90` & `python-sscha-1.3/SCHAModules/get_odd_straight_with_v4.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_stress_tensor.f90` & `python-sscha-1.3/SCHAModules/get_stress_tensor.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_upsilon_matrix.f90` & `python-sscha-1.3/SCHAModules/get_upsilon_matrix.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_v3.f90` & `python-sscha-1.3/SCHAModules/get_v3.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/get_v4.f90` & `python-sscha-1.3/SCHAModules/get_v4.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/module_anharmonic.f90` & `python-sscha-1.3/SCHAModules/module_anharmonic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/module_new_thermodynamic.f90` & `python-sscha-1.3/SCHAModules/module_new_thermodynamic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/module_stochastic.f90` & `python-sscha-1.3/SCHAModules/module_stochastic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/SCHAModules/multiply_lambda_tensor.f90` & `python-sscha-1.3/SCHAModules/multiply_lambda_tensor.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/scripts/cluster_check.x` & `python-sscha-1.3/scripts/cluster_check.x`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/scripts/plot_frequencies.py` & `python-sscha-1.3/scripts/plot_frequencies.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/scripts/read_incomplete_ensemble.py` & `python-sscha-1.3/scripts/read_incomplete_ensemble.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/scripts/sscha` & `python-sscha-1.3/scripts/sscha`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/scripts/sscha-plot-data.py` & `python-sscha-1.3/scripts/sscha-plot-data.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/scripts/static-vc-relax.pyx` & `python-sscha-1.3/scripts/static-vc-relax.pyx`

 * *Files identical despite different names*

### Comparing `python-sscha-1.2.1/setup.py` & `python-sscha-1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 #                   extra_link_args = mpi_link_args + extra_link_args_c
 #                   )
 
 
 
 # Prepare the compilation of the Python Conde
 setup( name = "python-sscha",
-       version = "1.2.1",
+       version = "1.3",
        description = "Python implementation of the sscha code",
        author = "Lorenzo Monacelli",
        url = "https://github.com/mesonepigreco/python-sscha",
        packages = ["sscha"],
        package_dir = {"sscha": "Modules"},
        setup_requires = ["numpy", "ase", "scipy", "cellconstructor", "spglib", "matplotlib"],
        ext_modules = [SCHAModules], # odd_HP
```

