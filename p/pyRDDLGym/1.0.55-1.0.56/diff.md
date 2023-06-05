# Comparing `tmp/pyRDDLGym-1.0.55.tar.gz` & `tmp/pyRDDLGym-1.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRDDLGym-1.0.55.tar", last modified: Mon Jun  5 13:15:41 2023, max compression
+gzip compressed data, was "pyRDDLGym-1.0.56.tar", last modified: Mon Jun  5 22:34:40 2023, max compression
```

## Comparing `pyRDDLGym-1.0.55.tar` & `pyRDDLGym-1.0.56.tar`

### file list

```diff
@@ -1,271 +1,271 @@
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.992559 pyRDDLGym-1.0.55/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1264 2022-12-08 22:55:23.000000 pyRDDLGym-1.0.55/LICENSE.MD
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/MANIFEST.in
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      912 2023-06-05 13:15:41.992269 pyRDDLGym-1.0.55/PKG-INFO
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8094 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/README.md
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.934797 pyRDDLGym-1.0.55/pyRDDLGym/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.935867 pyRDDLGym-1.0.55/pyRDDLGym/Core/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.938687 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8347 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLDecompiler.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11135 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    17227 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    18950 2023-04-06 22:49:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLModel.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    47583 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5216 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.939254 pyRDDLGym-1.0.55/pyRDDLGym/Core/Debug/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2168 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Debug/Logger.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-01-27 22:40:35.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Debug/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.940372 pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5797 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/RDDLConstraints.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    12772 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/RDDLEnv.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      413 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/RDDLEnvSeeder.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.941210 pyRDDLGym-1.0.55/pyRDDLGym/Core/ErrorHandling/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1378 2023-04-20 23:10:37.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/ErrorHandling/RDDLException.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/ErrorHandling/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.941636 pyRDDLGym-1.0.55/pyRDDLGym/Core/Grounder/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    27395 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Grounder/RDDLGrounder.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Grounder/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.944749 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    29366 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxParameterTuning.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    53812 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11956 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    69234 2023-04-07 15:03:00.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    18972 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLLogic.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    12925 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLModelError.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7027 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.948474 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1620 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/RDDLReader.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1146 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/cpf.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    10193 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/domain.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7819 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/expr.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1293 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/instance.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1221 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/nonfluents.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    38755 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/parser.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)   123443 2023-02-22 22:24:57.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/parsetab.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3242 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/pvariable.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    10773 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/rddl.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      801 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/utils.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.949199 pyRDDLGym-1.0.55/pyRDDLGym/Core/Simulator/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    49156 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Simulator/RDDLSimulator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Simulator/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.950142 pyRDDLGym-1.0.55/pyRDDLGym/Examples/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.929194 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.950858 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      238 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3419 2023-03-21 16:55:28.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      945 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.951675 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      256 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3510 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      928 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.952721 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      218 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    10524 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1408 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1628 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5211 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/ExampleManager.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.954631 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      161 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5768 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      364 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      389 2023-04-07 02:46:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      579 2023-05-25 19:49:15.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance1c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      455 2023-04-07 02:46:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance2.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      963 2023-05-25 19:56:55.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance3c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3744 2023-05-31 00:03:12.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance5c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3825 2023-05-29 22:41:23.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerator.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.956437 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2687 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3058 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3264 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3594 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4075 2023-05-29 22:41:23.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2285 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1819 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.957695 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      210 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4495 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1411 2023-03-30 14:37:35.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      751 2023-05-25 20:01:15.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance1c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2211 2023-05-25 20:04:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance3c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4363 2023-05-31 00:14:18.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance5c.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.959830 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      219 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4408 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2551 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/domain_old.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    14883 2023-04-16 21:02:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      960 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance0_old.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    15237 2023-05-25 20:08:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance1c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    15117 2023-06-05 01:35:32.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance3c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    15085 2023-05-31 00:17:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance5c.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.929876 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.960562 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      101 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2890 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      655 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.963374 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      105 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1401 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      193 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.930128 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.964691 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      239 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4403 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1610 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      791 2023-05-25 20:06:43.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance1c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1380 2023-05-25 20:07:33.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance3c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2583 2023-05-31 00:14:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance5c.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.965391 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      164 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3383 2023-02-27 22:52:10.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.966051 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PropDBN/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PropDBN/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2283 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PropDBN/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      268 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PropDBN/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.967761 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      176 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4995 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     9478 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      995 2023-04-07 02:51:57.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1245 2023-05-25 19:57:11.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance1c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2309 2023-05-25 19:59:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance3c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3347 2023-05-31 00:07:05.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance5c.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.969745 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      189 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4153 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1327 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    15525 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2051 2023-06-01 18:46:28.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance1c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    85747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance2.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    16852 2023-06-01 18:49:08.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance3c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)   194658 2023-06-01 18:50:40.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance5c.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.930595 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.971450 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      237 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4435 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      391 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      710 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      721 2023-05-25 20:17:38.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance1c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2622 2023-05-25 20:19:22.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance3c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8968 2023-05-31 00:28:29.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance5c.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.972236 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      162 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4544 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      390 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      709 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.972794 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      118 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3550 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      635 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.973325 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      129 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4622 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.974392 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.931002 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.975403 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20730 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7653 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     9656 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    24387 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.975594 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Experiments/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6386 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       91 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    16438 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4951 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    25150 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    23064 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/netgen.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.931405 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.977105 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      241 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5492 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1053 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1063 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      600 2023-05-25 20:00:05.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance1c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1094 2023-05-25 20:00:46.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance3c.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    10413 2023-05-31 00:10:12.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance5c.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.979144 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      185 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5440 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.979944 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      179 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5491 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.980680 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      121 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4280 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1398 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2655 2023-06-05 01:41:10.000000 pyRDDLGym-1.0.55/pyRDDLGym/GymExample.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8336 2023-06-05 01:25:16.000000 pyRDDLGym-1.0.55/pyRDDLGym/InstGenExample.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5596 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/JaxExample.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4442 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/JaxLossPlotExample.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2533 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/JaxTuningExample.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.981210 pyRDDLGym-1.0.55/pyRDDLGym/Planner/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4346 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Planner/JaxConfigManager.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Planner/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.981951 pyRDDLGym-1.0.55/pyRDDLGym/Policies/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1381 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Policies/Agents.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     9818 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Policies/RDDLSimAgent.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Policies/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      396 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/RDDLSimClientExample.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.986752 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2924 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/CartPoleViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7420 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ChartViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5528 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ColorViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8708 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ElevatorViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    12057 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/HVACViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6278 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MarsRoverViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4797 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MountainCarViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3950 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MovieGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8522 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/PowerGenViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2880 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/RacecarViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7196 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/RecSimViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11706 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ReservoirViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      516 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/StateViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2767 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/TextViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20753 2023-03-02 18:32:16.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/TrafficViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4754 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/UAVsViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5987 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/WildfireViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20186 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/visualize_dbn.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.988333 pyRDDLGym-1.0.55/pyRDDLGym/XADD/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2383 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    17224 2023-03-22 17:18:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLModelXADD.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6162 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLSimulatorXADD.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       41 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/XADD/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      111 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.991472 pyRDDLGym-1.0.55/pyRDDLGym/tests/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7362 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/RDDLGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    13792 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/_deprecated.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.991931 pyRDDLGym-1.0.55/pyRDDLGym/tests/seeding/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1735 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/seeding/Seedtest.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/seeding/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      701 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/testDiscrete.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1265 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/testGymDrone.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1672 2022-10-24 03:39:07.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/testViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1267 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/test_basic.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      658 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/test_dbn_vis.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1055 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/test_termination.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2534 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/test_xadd.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5114 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/unit_test_mars_rover.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2782 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/unit_test_power_gen.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.935713 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      912 2023-06-05 13:15:41.000000 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/PKG-INFO
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     9173 2023-06-05 13:15:41.000000 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/SOURCES.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2023-06-05 13:15:41.000000 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/dependency_links.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       67 2023-06-05 13:15:41.000000 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/requires.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       10 2023-06-05 13:15:41.000000 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/top_level.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       38 2023-06-05 13:15:41.992604 pyRDDLGym-1.0.55/setup.cfg
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2811 2023-06-05 13:06:40.000000 pyRDDLGym-1.0.55/setup.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.500477 pyRDDLGym-1.0.56/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1264 2022-12-08 22:55:23.000000 pyRDDLGym-1.0.56/LICENSE.MD
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/MANIFEST.in
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      912 2023-06-05 22:34:40.500266 pyRDDLGym-1.0.56/PKG-INFO
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8094 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/README.md
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.447781 pyRDDLGym-1.0.56/pyRDDLGym/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.448925 pyRDDLGym-1.0.56/pyRDDLGym/Core/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.451449 pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8347 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLDecompiler.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    11135 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    17227 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    18950 2023-04-06 22:49:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLModel.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    47583 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5216 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.451873 pyRDDLGym-1.0.56/pyRDDLGym/Core/Debug/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2168 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Debug/Logger.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-01-27 22:40:35.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Debug/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.452703 pyRDDLGym-1.0.56/pyRDDLGym/Core/Env/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5797 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Env/RDDLConstraints.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    12772 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Env/RDDLEnv.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      413 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Env/RDDLEnvSeeder.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Env/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.453098 pyRDDLGym-1.0.56/pyRDDLGym/Core/ErrorHandling/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1378 2023-04-20 23:10:37.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/ErrorHandling/RDDLException.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/ErrorHandling/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.453469 pyRDDLGym-1.0.56/pyRDDLGym/Core/Grounder/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    27395 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Grounder/RDDLGrounder.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Grounder/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.455963 pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    29366 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxParameterTuning.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    53812 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    11956 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    69234 2023-04-07 15:03:00.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    18972 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLLogic.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    12925 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLModelError.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7027 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.459346 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1620 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/RDDLReader.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1146 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/cpf.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10193 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/domain.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7819 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/expr.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1293 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/instance.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1221 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/nonfluents.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    38755 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/parser.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)   123443 2023-02-22 22:24:57.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/parsetab.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3242 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/pvariable.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10773 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/rddl.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      801 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/utils.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.460333 pyRDDLGym-1.0.56/pyRDDLGym/Core/Simulator/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    49156 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Simulator/RDDLSimulator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/Simulator/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/Core/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.461071 pyRDDLGym-1.0.56/pyRDDLGym/Examples/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.441494 pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.461694 pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      238 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3419 2023-03-21 16:55:28.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      945 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.462574 pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      256 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3510 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      928 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.463545 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Elevators/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      218 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Elevators/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10524 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Elevators/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1408 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Elevators/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1628 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Elevators/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5211 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/ExampleManager.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.465583 pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      161 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5768 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      364 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      389 2023-04-07 02:46:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      579 2023-05-25 19:49:15.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      455 2023-04-07 02:46:06.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/instance2.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      963 2023-05-25 19:56:55.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3744 2023-05-31 00:03:12.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/instance5c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3825 2023-05-29 22:41:23.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerator.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.467748 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2687 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3101 2023-06-05 22:22:42.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3264 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3594 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4075 2023-05-29 22:41:23.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2285 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1819 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.469307 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      210 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4495 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1411 2023-03-30 14:37:35.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      751 2023-05-25 20:01:15.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2211 2023-05-25 20:04:24.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4363 2023-05-31 00:14:18.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.471139 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      219 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4408 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2551 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/domain_old.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    14883 2023-04-16 21:02:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      960 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/instance0_old.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    15264 2023-06-05 22:25:44.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    15144 2023-06-05 22:25:44.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    15112 2023-06-05 22:25:44.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.442171 pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.471936 pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      101 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2890 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      655 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.472553 pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      105 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1401 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      193 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.442409 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.473849 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      239 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4403 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1610 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      791 2023-05-25 20:06:43.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1380 2023-05-25 20:07:33.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2583 2023-05-31 00:14:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.474633 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      164 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3383 2023-02-27 22:52:10.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.475213 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PropDBN/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PropDBN/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2283 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PropDBN/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      268 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/PropDBN/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.476922 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      176 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4995 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9478 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      995 2023-04-07 02:51:57.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1245 2023-05-25 19:57:11.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2309 2023-05-25 19:59:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3347 2023-05-31 00:07:05.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.478909 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      189 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4153 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1327 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    15525 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2051 2023-06-01 18:46:28.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    85747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance2.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    16852 2023-06-01 18:49:08.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)   194658 2023-06-01 18:50:40.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.442907 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.481421 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      237 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4435 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      391 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      710 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      721 2023-05-25 20:17:38.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2622 2023-05-25 20:19:22.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8968 2023-05-31 00:28:29.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.482303 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      162 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4544 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      390 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Discrete/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      709 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.482878 pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChain/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      118 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChain/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3550 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChain/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      635 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChain/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.483395 pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChainNet/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      129 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChainNet/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4622 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChainNet/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.484379 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.443302 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Deprecated/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.485459 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    20730 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7653 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9656 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    24387 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.485721 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Experiments/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     6386 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       91 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    16438 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4951 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    25150 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    23064 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/netgen.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.443716 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.487301 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      241 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5492 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1053 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1063 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      600 2023-05-25 20:00:05.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1094 2023-05-25 20:00:46.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10413 2023-05-31 00:10:12.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.487950 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      185 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5440 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.488706 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Mixed/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      179 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Mixed/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5491 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Mixed/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.489351 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Wildfire/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      121 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Wildfire/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4280 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Wildfire/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1398 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/Wildfire/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Examples/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2655 2023-06-05 01:41:10.000000 pyRDDLGym-1.0.56/pyRDDLGym/GymExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8336 2023-06-05 22:23:55.000000 pyRDDLGym-1.0.56/pyRDDLGym/InstGenExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5596 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/JaxExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4442 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/JaxLossPlotExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2533 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/JaxTuningExample.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.489817 pyRDDLGym-1.0.56/pyRDDLGym/Planner/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4346 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Planner/JaxConfigManager.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Planner/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.490511 pyRDDLGym-1.0.56/pyRDDLGym/Policies/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1381 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Policies/Agents.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9818 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Policies/RDDLSimAgent.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/Policies/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      396 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/RDDLSimClientExample.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.494921 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2924 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/CartPoleViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7420 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/ChartViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5528 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/ColorViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8708 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/ElevatorViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    12057 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/HVACViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     6278 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/MarsRoverViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4797 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/MountainCarViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3950 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/MovieGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8522 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/PowerGenViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2880 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/RacecarViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7196 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/RecSimViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    11706 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/ReservoirViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      516 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/StateViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2767 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/TextViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    20753 2023-03-02 18:32:16.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/TrafficViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4754 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/UAVsViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5987 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/WildfireViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    20186 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/visualize_dbn.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.496662 pyRDDLGym-1.0.56/pyRDDLGym/XADD/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2383 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.56/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    17224 2023-03-22 17:18:24.000000 pyRDDLGym-1.0.56/pyRDDLGym/XADD/RDDLModelXADD.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     6162 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.56/pyRDDLGym/XADD/RDDLSimulatorXADD.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       41 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.56/pyRDDLGym/XADD/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      111 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.56/pyRDDLGym/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.499586 pyRDDLGym-1.0.56/pyRDDLGym/tests/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7362 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/RDDLGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    13792 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/_deprecated.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.500038 pyRDDLGym-1.0.56/pyRDDLGym/tests/seeding/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1735 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/seeding/Seedtest.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/seeding/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      701 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/testDiscrete.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1265 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/testGymDrone.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1672 2022-10-24 03:39:07.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/testViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1267 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/test_basic.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      658 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/test_dbn_vis.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1055 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/test_termination.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2534 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/test_xadd.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5114 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/unit_test_mars_rover.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2782 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.56/pyRDDLGym/tests/unit_test_power_gen.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 22:34:40.448768 pyRDDLGym-1.0.56/pyRDDLGym.egg-info/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      912 2023-06-05 22:34:40.000000 pyRDDLGym-1.0.56/pyRDDLGym.egg-info/PKG-INFO
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9173 2023-06-05 22:34:40.000000 pyRDDLGym-1.0.56/pyRDDLGym.egg-info/SOURCES.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2023-06-05 22:34:40.000000 pyRDDLGym-1.0.56/pyRDDLGym.egg-info/dependency_links.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       67 2023-06-05 22:34:40.000000 pyRDDLGym-1.0.56/pyRDDLGym.egg-info/requires.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       10 2023-06-05 22:34:40.000000 pyRDDLGym-1.0.56/pyRDDLGym.egg-info/top_level.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       38 2023-06-05 22:34:40.500526 pyRDDLGym-1.0.56/setup.cfg
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2811 2023-06-05 22:34:17.000000 pyRDDLGym-1.0.56/setup.py
```

### Comparing `pyRDDLGym-1.0.55/LICENSE.MD` & `pyRDDLGym-1.0.56/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/PKG-INFO` & `pyRDDLGym-1.0.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRDDLGym
-Version: 1.0.55
+Version: 1.0.56
 Summary: pyRDDLGym: RDDL automatic generation tool for OpenAI Gym
 Home-page: https://github.com/ataitler/pyRDDLGym
 Author: Ayal Taitler, Michael Gimelfarb, Scott Sanner, Jihwan Jeong, Sriram Gopalakrishnan, Martin Mladenov, jack liu
 Author-email: ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, sriram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyRDDLGym-1.0.55/README.md` & `pyRDDLGym-1.0.56/README.md`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLDecompiler.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLDecompiler.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLModel.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLModel.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Debug/Logger.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Debug/Logger.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/RDDLConstraints.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Env/RDDLConstraints.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/RDDLEnv.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Env/RDDLEnv.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/ErrorHandling/RDDLException.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/ErrorHandling/RDDLException.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Grounder/RDDLGrounder.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Grounder/RDDLGrounder.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxParameterTuning.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxParameterTuning.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLLogic.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLLogic.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLModelError.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLModelError.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/RDDLReader.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/RDDLReader.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/cpf.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/cpf.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/domain.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/domain.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/expr.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/expr.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/instance.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/instance.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/nonfluents.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/nonfluents.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/parser.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/parsetab.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/pvariable.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/pvariable.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/rddl.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/rddl.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/utils.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Core/Simulator/RDDLSimulator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Core/Simulator/RDDLSimulator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Elevators/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Elevators/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/instance1.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Elevators/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/ExampleManager.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/ExampleManager.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance1c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/instance1c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance3c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/instance3c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance5c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/HVAC/instance5c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
                                          params['terrain_widths'],
                                          params['terrain_heights'])
         
         points = self.generate_terrain_points(fx, params['num_points'], *xrange)
         segments = [f's{i + 1}' for i in range(len(points))]
         
         nonfluents = {}
+        nonfluents['ACTION-PENALTY'] = 0.0
         nonfluents['MIN-POS'] = xrange[0]
         nonfluents['MAX-POS'] = xrange[1]
         nonfluents['GOAL-MIN'] = params['goal-min']
         for (i, (x1, y1, x2, y2)) in enumerate(points):
             nonfluents[f'X-START({segments[i]})'] = x1
             nonfluents[f'Y-START({segments[i]})'] = y1
             nonfluents[f'X-END({segments[i]})'] = x2
```

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance1c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/instance1c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance3c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/instance3c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance5c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MarsRover/instance5c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/domain_old.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/domain_old.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance0_old.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/instance0_old.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance1c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/instance1c.rddl`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 non-fluents nf_mountain_car_1c {
 	domain = mountain_car;
 	objects {
 		segment : {s1, s2, s3, s4, s5, s6, s7, s8, s9, s10, s11, s12, s13, s14, s15, s16, s17, s18, s19, s20, s21, s22, s23, s24, s25, s26, s27, s28, s29, s30, s31, s32, s33, s34, s35, s36, s37, s38, s39, s40, s41, s42, s43, s44, s45, s46, s47, s48, s49, s50, s51, s52, s53, s54, s55, s56, s57, s58, s59, s60, s61, s62, s63, s64, s65, s66, s67, s68, s69, s70, s71, s72, s73, s74, s75, s76, s77, s78, s79, s80, s81, s82, s83, s84, s85, s86, s87, s88, s89, s90, s91, s92, s93, s94, s95, s96, s97, s98, s99};
 	};
 	non-fluents {
+	    ACTION-PENALTY = 0.0;
 		MIN-POS = -1.2;
 		MAX-POS = 0.6000000000000001;
 		GOAL-MIN = 0.5;
 		X-START(s1) = -1.2;
 		Y-START(s1) = 0.5203955092681039;
 		X-END(s1) = -1.1818181818181819;
 		Y-END(s1) = 0.5003840142464886;
```

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance3c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/instance3c.rddl`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 non-fluents nf_mountain_car_3c {
 	domain = mountain_car;
 	objects {
 		segment : {s1, s2, s3, s4, s5, s6, s7, s8, s9, s10, s11, s12, s13, s14, s15, s16, s17, s18, s19, s20, s21, s22, s23, s24, s25, s26, s27, s28, s29, s30, s31, s32, s33, s34, s35, s36, s37, s38, s39, s40, s41, s42, s43, s44, s45, s46, s47, s48, s49, s50, s51, s52, s53, s54, s55, s56, s57, s58, s59, s60, s61, s62, s63, s64, s65, s66, s67, s68, s69, s70, s71, s72, s73, s74, s75, s76, s77, s78, s79, s80, s81, s82, s83, s84, s85, s86, s87, s88, s89, s90, s91, s92, s93, s94, s95, s96, s97, s98, s99};
 	};
 	non-fluents {
+	    ACTION-PENALTY = 0.0;
 		MIN-POS = -1.2;
 		MAX-POS = 5.0;
 		GOAL-MIN = 4.9;
 		X-START(s1) = -1.2;
 		Y-START(s1) = 0.5203955092681039;
 		X-END(s1) = -1.1373737373737374;
 		Y-END(s1) = 0.45112199621376564;
```

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance5c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/MountainCar/instance5c.rddl`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 non-fluents nf_mountain_car_5c {
 	domain = mountain_car;
 	objects {
 		segment : {s1, s2, s3, s4, s5, s6, s7, s8, s9, s10, s11, s12, s13, s14, s15, s16, s17, s18, s19, s20, s21, s22, s23, s24, s25, s26, s27, s28, s29, s30, s31, s32, s33, s34, s35, s36, s37, s38, s39, s40, s41, s42, s43, s44, s45, s46, s47, s48, s49, s50, s51, s52, s53, s54, s55, s56, s57, s58, s59, s60, s61, s62, s63, s64, s65, s66, s67, s68, s69, s70, s71, s72, s73, s74, s75, s76, s77, s78, s79, s80, s81, s82, s83, s84, s85, s86, s87, s88, s89, s90, s91, s92, s93, s94, s95, s96, s97, s98, s99};
 	};
 	non-fluents {
+	    ACTION-PENALTY = 0.0;
 		MIN-POS = -1.2;
 		MAX-POS = 7.199999999999999;
 		GOAL-MIN = 7.1;
 		X-START(s1) = -1.2;
 		Y-START(s1) = 0.2891086162600577;
 		X-END(s1) = -1.1151515151515152;
 		Y-END(s1) = 0.23691601093926404;
```

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance1c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/instance1c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance3c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/instance3c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance5c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Continuous/instance5c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PropDBN/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/PropDBN/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance1.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance1c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/instance1c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance3c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/instance3c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance5c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RaceCar/instance5c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance1.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance1c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance1c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance2.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance2.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance3c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance3c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance5c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/RecSim/instance5c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance1c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/instance1c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance3c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/instance3c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance5c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Continuous/instance5c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChain/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChain/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChainNet/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/instance1.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/netgen.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Traffic/netgen.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance1c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/instance1c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance3c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/instance3c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance5c.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Continuous/instance5c.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Mixed/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/domain.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Wildfire/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/instance0.rddl` & `pyRDDLGym-1.0.56/pyRDDLGym/Examples/Wildfire/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/GymExample.py` & `pyRDDLGym-1.0.56/pyRDDLGym/GymExample.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/InstGenExample.py` & `pyRDDLGym-1.0.56/pyRDDLGym/InstGenExample.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pyRDDLGym.Policies.Agents import RandomAgent
 
 ENVS = ['HVAC', 'RaceCar', 'UAV_continuous', 'MarsRover', 'PowerGen_continuous', 'MountainCar', 'RecSim', 'Reservoir_continuous']
 
 ###################
 # Competition run instances
 ###################
-INST_NAMES = ['1c', '3c', '5c']
+INST_NAMES = ['0c', '3c', '5c']
 HVAC_PARAMS = [
     # difficulty is controlled by the number of zones + heaters (e.g. scale)
     # and the switching of occupancy affects more zones (this should make it
     # difficult for determinization methods)
     {'num_heaters': 3, 'num_zones': 2, 'density': 0.2,
      'temp-zone-range-init': (0., 15.), 'temp-heater-range-init': (0., 10.),
      'TEMP-ZONE-MIN': 22.0, 'TEMP-ZONE-MAX': 25.0,
@@ -175,12 +175,12 @@
 
 
 
 
 
 if __name__ == "__main__":
     inst_index = 0
-    env = ENVS[7]
+    env = ENVS[5]
     inst_name = INST_NAMES[inst_index]
     inst_params = INST_PARAMS[env][inst_index]
 
     main(env, inst_params, inst_name)
```

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/JaxExample.py` & `pyRDDLGym-1.0.56/pyRDDLGym/JaxExample.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/JaxLossPlotExample.py` & `pyRDDLGym-1.0.56/pyRDDLGym/JaxLossPlotExample.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/JaxTuningExample.py` & `pyRDDLGym-1.0.56/pyRDDLGym/JaxTuningExample.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Planner/JaxConfigManager.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Planner/JaxConfigManager.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Policies/Agents.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Policies/Agents.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Policies/RDDLSimAgent.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Policies/RDDLSimAgent.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/CartPoleViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/CartPoleViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ChartViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/ChartViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ColorViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/ColorViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ElevatorViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/ElevatorViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/HVACViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/HVACViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MarsRoverViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/MarsRoverViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MountainCarViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/MountainCarViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MovieGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/MovieGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/PowerGenViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/PowerGenViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/RacecarViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/RacecarViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/RecSimViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/RecSimViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ReservoirViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/ReservoirViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/StateViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/StateViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/TextViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/TextViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/TrafficViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/TrafficViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/UAVsViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/UAVsViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/WildfireViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/WildfireViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/visualize_dbn.py` & `pyRDDLGym-1.0.56/pyRDDLGym/Visualizer/visualize_dbn.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py` & `pyRDDLGym-1.0.56/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLModelXADD.py` & `pyRDDLGym-1.0.56/pyRDDLGym/XADD/RDDLModelXADD.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLSimulatorXADD.py` & `pyRDDLGym-1.0.56/pyRDDLGym/XADD/RDDLSimulatorXADD.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/RDDLGenerator.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/RDDLGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/_deprecated.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/seeding/Seedtest.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/seeding/Seedtest.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/testDiscrete.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/testDiscrete.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/testGymDrone.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/testGymDrone.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/testViz.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/testViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/test_basic.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/test_dbn_vis.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/test_dbn_vis.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/test_termination.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/test_termination.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/test_xadd.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/test_xadd.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/unit_test_mars_rover.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/unit_test_mars_rover.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym/tests/unit_test_power_gen.py` & `pyRDDLGym-1.0.56/pyRDDLGym/tests/unit_test_power_gen.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym.egg-info/PKG-INFO` & `pyRDDLGym-1.0.56/pyRDDLGym.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRDDLGym
-Version: 1.0.55
+Version: 1.0.56
 Summary: pyRDDLGym: RDDL automatic generation tool for OpenAI Gym
 Home-page: https://github.com/ataitler/pyRDDLGym
 Author: Ayal Taitler, Michael Gimelfarb, Scott Sanner, Jihwan Jeong, Sriram Gopalakrishnan, Martin Mladenov, jack liu
 Author-email: ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, sriram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyRDDLGym-1.0.55/pyRDDLGym.egg-info/SOURCES.txt` & `pyRDDLGym-1.0.56/pyRDDLGym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.55/setup.py` & `pyRDDLGym-1.0.56/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup, find_packages
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setup(
       name='pyRDDLGym',
-      version='1.0.55',
+      version='1.0.56',
       author="Ayal Taitler, Michael Gimelfarb, Scott Sanner, Jihwan Jeong, Sriram Gopalakrishnan, Martin Mladenov, jack liu",
       author_email="ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, sriram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca",
       description="pyRDDLGym: RDDL automatic generation tool for OpenAI Gym",
       # long_description=long_description,
       license="MIT License",
       url="https://github.com/ataitler/pyRDDLGym",
       packages=find_packages(),
```

