# Comparing `tmp/dolfin_mech-2023.3.22.tar.gz` & `tmp/dolfin_mech-2023.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolfin_mech-2023.3.22.tar", last modified: Wed Mar 22 10:49:06 2023, max compression
+gzip compressed data, was "dolfin_mech-2023.6.6.tar", last modified: Tue Jun  6 16:52:58 2023, max compression
```

## Comparing `dolfin_mech-2023.3.22.tar` & `dolfin_mech-2023.6.6.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:49:06.840488 dolfin_mech-2023.3.22/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/LICENSE
--rw-r--r--   0 root         (0) root         (0)      725 2023-03-22 10:49:06.838488 dolfin_mech-2023.3.22/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:49:06.836488 dolfin_mech-2023.3.22/dolfin_mech/
--rw-rw-rw-   0 root         (0) root         (0)     4546 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Ball_Hyperelasticity.py
--rw-rw-rw-   0 root         (0) root         (0)     2382 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Ball_Mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     2627 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     5685 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Disc_Hyperelasticity.py
--rw-rw-rw-   0 root         (0) root         (0)     3966 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Disc_Mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Expression_MeshFunction_cpp.py
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/FOI.py
--rw-rw-rw-   0 root         (0) root         (0)     7190 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/HeartSlice_Hyperelasticity.py
--rw-rw-rw-   0 root         (0) root         (0)     4762 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/HeartSlice_Mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     3657 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Kinematics.py
--rw-rw-rw-   0 root         (0) root         (0)     2229 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Kinematics_Inverse.py
--rw-rw-rw-   0 root         (0) root         (0)     1528 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Kinematics_Linearized.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Loading.py
--rw-rw-rw-   0 root         (0) root         (0)    12102 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic.py
--rw-rw-rw-   0 root         (0) root         (0)     2612 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_CiarletGeymonat.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_CiarletGeymonatNeoHookean.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_CiarletGeymonatNeoHookeanMooneyRivlin.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_ExponentialCiarletGeymonat.py
--rw-rw-rw-   0 root         (0) root         (0)     4738 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Hooke.py
--rw-rw-rw-   0 root         (0) root         (0)     4868 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Kirchhoff.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Lung_Wbulk.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Lung_Wpore.py
--rw-rw-rw-   0 root         (0) root         (0)     1294 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Lung_Wskel.py
--rw-rw-rw-   0 root         (0) root         (0)     3867 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_MooneyRivlin.py
--rw-rw-rw-   0 root         (0) root         (0)     3139 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_NeoHookean.py
--rw-rw-rw-   0 root         (0) root         (0)     1813 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_NeoHookeanMooneyRivlin.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Porous.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Material_Inelastic.py
--rw-rw-rw-   0 root         (0) root         (0)    23381 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/NonlinearSolver.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_HyperElasticity.py
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_HyperHydrostaticPressure.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_HyperIncompressibility.py
--rw-rw-rw-   0 root         (0) root         (0)     1598 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Inertia.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_LinearizedElasticity.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_LinearizedHydrostaticPressure.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_LinearizedIncompressibility.py
--rw-rw-rw-   0 root         (0) root         (0)     1967 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Loading_SurfaceForce.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Loading_SurfacePressure.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Loading_SurfacePressureGradient.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Loading_SurfaceTension.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Loading_VolumeForce.py
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_MacroscopicStress.py
--rw-rw-rw-   0 root         (0) root         (0)     1678 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Penalty_DirectionalDisplacement.py
--rw-rw-rw-   0 root         (0) root         (0)     2679 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Penalty_MacroscopicStressComponent.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Penalty_MacroscopicStretchComponent.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Penalty_MacroscopicStretchSymmetry.py
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Penalty_NormalDisplacement.py
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Poro_Pf.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Poro_Wbulk.py
--rw-rw-rw-   0 root         (0) root         (0)     2312 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Poro_Wpore.py
--rw-rw-rw-   0 root         (0) root         (0)     2333 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_Poro_Wskel.py
--rw-rw-rw-   0 root         (0) root         (0)     1393 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Operator_TensorSymmetry.py
--rw-rw-rw-   0 root         (0) root         (0)    21335 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Problem.py
--rw-rw-rw-   0 root         (0) root         (0)    10790 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Problem_Elasticity.py
--rw-rw-rw-   0 root         (0) root         (0)    12726 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Problem_Hyperelasticity.py
--rw-rw-rw-   0 root         (0) root         (0)     2209 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Problem_Hyperelasticity_Inverse.py
--rw-rw-rw-   0 root         (0) root         (0)    17566 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Problem_Hyperelasticity_MicroPoro.py
--rw-rw-rw-   0 root         (0) root         (0)    14571 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Problem_Hyperelasticity_Poro.py
--rw-rw-rw-   0 root         (0) root         (0)     5017 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Problem_Hyperelasticity_Poro_Inverse.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/QOI.py
--rw-rw-rw-   0 root         (0) root         (0)     6950 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/RivlinCube_Elasticity.py
--rw-rw-rw-   0 root         (0) root         (0)    10047 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/RivlinCube_Hyperelasticity.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/RivlinCube_Mesh.py
--rw-rw-rw-   0 root         (0) root         (0)    10555 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/RivlinCube_PoroHyperelasticity.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/Step.py
--rw-rw-rw-   0 root         (0) root         (0)     7782 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/SubDomain_Periodic.py
--rw-rw-rw-   0 root         (0) root         (0)     2085 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/SubDomain_Pinpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2106 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/SubSol.py
--rw-rw-rw-   0 root         (0) root         (0)     9738 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/TimeIntegrator.py
--rw-rw-rw-   0 root         (0) root         (0)     3752 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/TimeVaryingConstant.py
--rw-rw-rw-   0 root         (0) root         (0)     1243 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/XDMFFile.py
--rw-rw-rw-   0 root         (0) root         (0)     3027 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      933 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/compute_error.py
--rw-rw-rw-   0 root         (0) root         (0)     5630 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/mesh2ugrid.py
--rw-rw-rw-   0 root         (0) root         (0)     1604 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/dolfin_mech/write_VTU_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:49:06.838488 dolfin_mech-2023.3.22/dolfin_mech.egg-info/
--rw-r--r--   0 root         (0) root         (0)      725 2023-03-22 10:49:06.000000 dolfin_mech-2023.3.22/dolfin_mech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3207 2023-03-22 10:49:06.000000 dolfin_mech-2023.3.22/dolfin_mech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 10:49:06.000000 dolfin_mech-2023.3.22/dolfin_mech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-03-22 10:49:06.000000 dolfin_mech-2023.3.22/dolfin_mech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-22 10:49:06.000000 dolfin_mech-2023.3.22/dolfin_mech.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-22 10:49:06.840488 dolfin_mech-2023.3.22/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-03-22 10:48:55.000000 dolfin_mech-2023.3.22/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:52:58.680792 dolfin_mech-2023.6.6/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-06 16:52:58.679792 dolfin_mech-2023.6.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:52:58.676792 dolfin_mech-2023.6.6/dolfin_mech/
+-rw-rw-rw-   0 root         (0) root         (0)     4546 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Ball_Hyperelasticity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2382 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Ball_Mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     2627 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     5685 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Disc_Hyperelasticity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3966 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Disc_Mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Expression_MeshFunction_cpp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/FOI.py
+-rw-rw-rw-   0 root         (0) root         (0)     7190 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/HeartSlice_Hyperelasticity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4762 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/HeartSlice_Mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     3669 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Kinematics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2241 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Kinematics_Inverse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Kinematics_Linearized.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Loading.py
+-rw-rw-rw-   0 root         (0) root         (0)    13685 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_ExponentialOgdenCiarletGeymonat.py
+-rw-rw-rw-   0 root         (0) root         (0)     5248 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Hooke.py
+-rw-rw-rw-   0 root         (0) root         (0)     5360 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Kirchhoff.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Lung_Wbulk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Lung_Wpore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Lung_Wskel.py
+-rw-rw-rw-   0 root         (0) root         (0)     4525 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_MooneyRivlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_NeoHookean.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_NeoHookeanMooneyRivlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_OgdenCiarletGeymonat.py
+-rw-rw-rw-   0 root         (0) root         (0)     2232 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_OgdenCiarletGeymonatNeoHookean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_OgdenCiarletGeymonatNeoHookeanMooneyRivlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Porous.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Material_Inelastic.py
+-rw-rw-rw-   0 root         (0) root         (0)    23381 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/NonlinearSolver.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_HyperElasticity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_HyperHydrostaticPressure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_HyperIncompressibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Inertia.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_LinearizedElasticity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_LinearizedHydrostaticPressure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_LinearizedIncompressibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Loading_SurfaceForce.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Loading_SurfacePressure.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Loading_SurfacePressureGradient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Loading_SurfaceTension.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Loading_VolumeForce.py
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_MacroscopicStress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Penalty_DirectionalDisplacement.py
+-rw-rw-rw-   0 root         (0) root         (0)     2679 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Penalty_MacroscopicStressComponent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Penalty_MacroscopicStretchComponent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Penalty_MacroscopicStretchSymmetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Penalty_NormalDisplacement.py
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Poro_Pf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Poro_Wbulk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Poro_Wpore.py
+-rw-rw-rw-   0 root         (0) root         (0)     2333 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_Poro_Wskel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Operator_TensorSymmetry.py
+-rw-rw-rw-   0 root         (0) root         (0)    21335 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Problem.py
+-rw-rw-rw-   0 root         (0) root         (0)    10790 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Problem_Elasticity.py
+-rw-rw-rw-   0 root         (0) root         (0)    13389 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Problem_Hyperelasticity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2209 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Problem_Hyperelasticity_Inverse.py
+-rw-rw-rw-   0 root         (0) root         (0)    17566 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Problem_Hyperelasticity_MicroPoro.py
+-rw-rw-rw-   0 root         (0) root         (0)    14571 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Problem_Hyperelasticity_Poro.py
+-rw-rw-rw-   0 root         (0) root         (0)     5017 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Problem_Hyperelasticity_Poro_Inverse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/QOI.py
+-rw-rw-rw-   0 root         (0) root         (0)     6950 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/RivlinCube_Elasticity.py
+-rw-rw-rw-   0 root         (0) root         (0)    10127 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/RivlinCube_Hyperelasticity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/RivlinCube_Mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)    10555 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/RivlinCube_PoroHyperelasticity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/Step.py
+-rw-rw-rw-   0 root         (0) root         (0)     7782 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/SubDomain_Periodic.py
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/SubDomain_Pinpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2106 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/SubSol.py
+-rw-rw-rw-   0 root         (0) root         (0)     9738 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/TimeIntegrator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3752 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/TimeVaryingConstant.py
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/XDMFFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      933 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/compute_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/mesh2ugrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1604 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/dolfin_mech/write_VTU_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:52:58.679792 dolfin_mech-2023.6.6/dolfin_mech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-06 16:52:58.000000 dolfin_mech-2023.6.6/dolfin_mech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-06-06 16:52:58.000000 dolfin_mech-2023.6.6/dolfin_mech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 16:52:58.000000 dolfin_mech-2023.6.6/dolfin_mech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-06 16:52:58.000000 dolfin_mech-2023.6.6/dolfin_mech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-06 16:52:58.000000 dolfin_mech-2023.6.6/dolfin_mech.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 16:52:58.680792 dolfin_mech-2023.6.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-06-06 16:52:46.000000 dolfin_mech-2023.6.6/setup.py
```

### Comparing `dolfin_mech-2023.3.22/LICENSE` & `dolfin_mech-2023.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/PKG-INFO` & `dolfin_mech-2023.6.6/dolfin_mech.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dolfin_mech
-Version: 2023.3.22
+Name: dolfin-mech
+Version: 2023.6.6
 Summary: A set of FEniCS-based python tools for Computational Mechanics.
 Home-page: https://gitlab.inria.fr/mgenet/dolfin_mech
 Author: Martin Genet
 Author-email: martin.genet@polytechnique.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Ball_Hyperelasticity.py` & `dolfin_mech-2023.6.6/dolfin_mech/Ball_Hyperelasticity.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Ball_Mesh.py` & `dolfin_mech-2023.6.6/dolfin_mech/Ball_Mesh.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Constraint.py` & `dolfin_mech-2023.6.6/dolfin_mech/Constraint.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Disc_Hyperelasticity.py` & `dolfin_mech-2023.6.6/dolfin_mech/Disc_Hyperelasticity.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Disc_Mesh.py` & `dolfin_mech-2023.6.6/dolfin_mech/Disc_Mesh.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Expression_MeshFunction_cpp.py` & `dolfin_mech-2023.6.6/dolfin_mech/Expression_MeshFunction_cpp.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/FOI.py` & `dolfin_mech-2023.6.6/dolfin_mech/FOI.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/HeartSlice_Hyperelasticity.py` & `dolfin_mech-2023.6.6/dolfin_mech/HeartSlice_Hyperelasticity.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/HeartSlice_Mesh.py` & `dolfin_mech-2023.6.6/dolfin_mech/HeartSlice_Mesh.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Kinematics.py` & `dolfin_mech-2023.6.6/dolfin_mech/Kinematics.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,30 +39,30 @@
         self.IIC   = (dolfin.tr(self.C)*dolfin.tr(self.C) - dolfin.tr(self.C*self.C))/2
         self.E     = (self.C - self.I)/2
         self.E     = dolfin.variable(self.E)
 
         self.E_sph = dolfin.tr(self.E)/self.dim * self.I
         self.E_dev = self.E - self.E_sph
 
-        self.F_bar     = self.J**(-1./3) * self.F
+        self.F_bar     = self.J**(-1/self.dim) * self.F
         self.C_bar     = self.F_bar.T * self.F_bar
         self.C_bar_inv = dolfin.inv(self.C_bar)
         self.IC_bar    = dolfin.tr(self.C_bar)
         self.IIC_bar   = (dolfin.tr(self.C_bar)*dolfin.tr(self.C_bar) - dolfin.tr(self.C_bar*self.C_bar))/2
         self.E_bar     = (self.C_bar - self.I)/2
 
         if (U_old is not None):
             self.U_old = U_old
 
             self.F_old = self.I + dolfin.grad(U_old)
             self.J_old = dolfin.det(self.F_old)
             self.C_old = self.F_old.T * self.F_old
             self.E_old = (self.C_old - self.I)/2
 
-            self.F_bar_old = self.J_old**(-1./3) * self.F_old
+            self.F_bar_old = self.J_old**(-1/self.dim) * self.F_old
             self.C_bar_old = self.F_bar_old.T * self.F_bar_old
             self.E_bar_old = (self.C_bar_old - self.I)/2
 
             self.F_mid = (self.F_old + self.F)/2
             self.J_mid = (self.J_old + self.J)/2
             self.C_mid = (self.C_old + self.C)/2
             self.E_mid = (self.E_old + self.E)/2
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Kinematics_Inverse.py` & `dolfin_mech-2023.6.6/dolfin_mech/Kinematics_Inverse.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,25 +36,25 @@
         self.C     = dolfin.variable(self.C)
         self.C_inv = dolfin.inv(self.C)
         self.IC    = dolfin.tr(self.C)
         self.IIC   = (dolfin.tr(self.C)*dolfin.tr(self.C) - dolfin.tr(self.C*self.C))/2
         self.E     = (self.C - self.I)/2
         self.E     = dolfin.variable(self.E)
 
-        self.F_bar   = self.J**(-1./3) * self.F
+        self.F_bar   = self.J**(-1/self.dim) * self.F
         self.C_bar   = self.F_bar.T * self.F_bar
         self.IC_bar  = dolfin.tr(self.C_bar)
         self.IIC_bar = (dolfin.tr(self.C_bar)*dolfin.tr(self.C_bar) - dolfin.tr(self.C_bar*self.C_bar))/2
         self.E_bar   = (self.C_bar - self.I)/2
 
         if (u_old is not None):
             self.u_old = u_old
 
             self.f_old = self.I + dolfin.grad(self.u_old)
             self.F_old = dolfin.inv(self.f_old)
             self.J_old = dolfin.det(self.F_old)
             self.C_old = self.F_old.T * self.F_old
             self.E_old = (self.C_old - self.I)/2
 
-            self.F_bar_old = self.J_old**(-1./3) * self.F_old
+            self.F_bar_old = self.J_old**(-1/self.dim) * self.F_old
             self.C_bar_old = self.F_bar_old.T * self.F_bar_old
             self.E_bar_old = (self.C_bar_old - self.I)/2
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Kinematics_Linearized.py` & `dolfin_mech-2023.6.6/dolfin_mech/Kinematics_Linearized.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Loading.py` & `dolfin_mech-2023.6.6/dolfin_mech/Loading.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,18 +66,15 @@
     def get_K_from_parameters(self,
             parameters):
 
         if ("K" in parameters):
             K = parameters["K"]
         else:
             lmbda, mu = self.get_lambda_and_mu_from_parameters(parameters)
-            if (parameters.get("dim", 3) == 2):
-                K = (2*lmbda+2*mu)/2
-            else:
-                K = (3*lmbda+2*mu)/3
+            K = (3*lmbda+2*mu)/3
         return dolfin.Constant(K)
 
 
 
     def get_G_from_parameters(self,
             parameters):
 
@@ -86,14 +83,33 @@
         else:
             mu = self.get_mu_from_parameters(parameters)
             G = mu
         return dolfin.Constant(G)
 
 
     
+    def get_C0_from_parameters(self,
+            parameters,
+            decoup=False):
+
+        if ("C0" in parameters):
+            C0 = parameters["C0"]
+        elif ("c0" in parameters):
+            C0 = parameters["c0"]
+        else:
+            if (decoup):
+                K = self.get_K_from_parameters(parameters)
+                C0 = K/4
+            else:
+                lmbda = self.get_lambda_from_parameters(parameters)
+                C0 = lmbda/4
+        return dolfin.Constant(C0)
+
+
+    
     def get_C1_from_parameters(self,
             parameters):
 
         if ("C1" in parameters):
             C1 = parameters["C1"]
         elif ("c1" in parameters):
             C1 = parameters["c1"]
@@ -298,44 +314,46 @@
 
 
 def material_factory(
         kinematics,
         model,
         parameters):
 
-    if   (model in ("hooke", "H")):
+    if   (model in ("hooke", "Hooke", "H")):
         material = dmech.HookeElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("hooke_dev", "H_dev")):
+    elif (model in ("hooke_dev", "Hooke_dev", "H_dev")):
         material = dmech.HookeDevElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("hooke_bulk", "H_bulk")):
+    elif (model in ("hooke_bulk", "Hooke_bulk", "H_bulk")):
         material = dmech.HookeBulkElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("saintvenantkirchhoff", "kirchhoff", "SVK")):
+    elif (model in ("saintvenantkirchhoff", "SaintVenantKirchhoff", "kirchhoff", "Kirchhoff", "SVK")):
         material = dmech.KirchhoffElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("saintvenantkirchhoff_dev", "kirchhoff_dev", "SVK_dev")):
+    elif (model in ("saintvenantkirchhoff_dev", "SaintVenantKirchhoff_dev", "kirchhoff_dev", "Kirchhoff_dev", "SVK_dev")):
         material = dmech.KirchhoffDevElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("saintvenantkirchhoff_bulk", "kirchhoff_bulk", "SVK_bulk")):
+    elif (model in ("saintvenantkirchhoff_bulk", "SaintVenantKirchhoff_bulk", "kirchhoff_bulk", "Kirchhoff_bulk", "SVK_bulk")):
         material = dmech.KirchhoffBulkElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("neohookean", "NH")):
+    elif (model in ("neohookean", "NeoHookean", "NH")):
         material = dmech.NeoHookeanElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("neohookean_bar", "NH_bar")):
+    elif (model in ("neohookean_bar", "NeoHookean_bar", "NH_bar")):
         material = dmech.NeoHookeanElasticMaterial(kinematics=kinematics, parameters=parameters, decoup=True)
-    elif (model in ("mooneyrivlin", "MR")):
+    elif (model in ("mooneyrivlin", "MooneyRivlin", "MR")):
         material = dmech.MooneyRivlinElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("mooneyrivlin_bar", "MR_bar")):
+    elif (model in ("mooneyrivlin_bar", "MooneyRivlin_bar", "MR_bar")):
         material = dmech.MooneyRivlinElasticMaterial(kinematics=kinematics, parameters=parameters, decoup=True)
-    elif (model in ("neohookeanmooneyrivlin", "NHMR")):
+    elif (model in ("neohookeanmooneyrivlin", "NeoHookeanMooneyRivlin", "NHMR")):
         material = dmech.NeoHookeanMooneyRivlinElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("neohookeanmooneyrivlin_bar", "NHMR_bar")):
+    elif (model in ("neohookeanmooneyrivlin_bar", "NeoHookeanMooneyRivlin_bar", "NHMR_bar")):
         material = dmech.NeoHookeanMooneyRivlinElasticMaterial(kinematics=kinematics, parameters=parameters, decoup=True)
-    elif (model in ("ciarletgeymonat", "CG")):
-        material = dmech.CiarletGeymonatElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("ciarletgeymonatneohookean", "CGNH")):
-        material = dmech.CiarletGeymonatNeoHookeanElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("ciarletgeymonatneohookean_bar", "CGNH_bar")):
-        material = dmech.CiarletGeymonatNeoHookeanElasticMaterial(kinematics=kinematics, parameters=parameters, decoup=True)
-    elif (model in ("ciarletgeymonatneohookeanmooneyrivlin", "CGNHMR")):
-        material = dmech.CiarletGeymonatNeoHookeanMooneyRivlinElasticMaterial(kinematics=kinematics, parameters=parameters)
-    elif (model in ("ciarletgeymonatneohookeanmooneyrivlin_bar", "CGNHMR_bar")):
-        material = dmech.CiarletGeymonatNeoHookeanMooneyRivlinElasticMaterial(kinematics=kinematics, parameters=parameters, decoup=True)
+    elif (model in ("ogdenciarletgeymonat", "OgdenCiarletGeymonat", "OCG", "ciarletgeymonat", "CiarletGeymonat", "CG")):
+        material = dmech.OgdenCiarletGeymonatElasticMaterial(kinematics=kinematics, parameters=parameters)
+    elif (model in ("ogdenciarletgeymonat_bar", "OgdenCiarletGeymonat_bar", "OCG_bar", "ciarletgeymonat_bar", "CiarletGeymonat_bar", "CG_bar")):
+        material = dmech.OgdenCiarletGeymonatElasticMaterial(kinematics=kinematics, parameters=parameters, decoup=True)
+    elif (model in ("ogdenciarletgeymonatneohookean", "OgdenCiarletGeymonatNeoHookean", "OCGNH", "ciarletgeymonatneohookean", "CiarletGeymonatNeoHookean", "CGNH")):
+        material = dmech.OgdenCiarletGeymonatNeoHookeanElasticMaterial(kinematics=kinematics, parameters=parameters)
+    elif (model in ("ogdenciarletgeymonatneohookean_bar", "OgdenCiarletGeymonatNeoHookean_bar", "OCGNH_bar", "ciarletgeymonatneohookean_bar", "CiarletGeymonatNeoHookean_bar", "CGNH_bar")):
+        material = dmech.OgdenCiarletGeymonatNeoHookeanElasticMaterial(kinematics=kinematics, parameters=parameters, decoup=True)
+    elif (model in ("ogdenciarletgeymonatneohookeanmooneyrivlin", "OgdenCiarletGeymonatNeoHookeanMooneyRivlin", "OCGNHMR", "ciarletgeymonatneohookeanmooneyrivlin", "CiarletGeymonatNeoHookeanMooneyRivlin", "CGNHMR")):
+        material = dmech.OgdenCiarletGeymonatNeoHookeanMooneyRivlinElasticMaterial(kinematics=kinematics, parameters=parameters)
+    elif (model in ("ogdenciarletgeymonatneohookeanmooneyrivlin_bar", "OgdenCiarletGeymonatNeoHookeanMooneyRivlin_bar", "OCGNHMR_bar", "ciarletgeymonatneohookeanmooneyrivlin_bar", "CiarletGeymonatNeoHookeanMooneyRivlin_bar", "CGNHMR_bar")):
+        material = dmech.OgdenCiarletGeymonatNeoHookeanMooneyRivlinElasticMaterial(kinematics=kinematics, parameters=parameters, decoup=True)
     else:
         assert(0), "Material model (\""+model+"\") not recognized. Aborting."
     return material
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_CiarletGeymonat.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_OgdenCiarletGeymonat.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,51 +11,56 @@
 import dolfin
 
 import dolfin_mech as dmech
 from .Material_Elastic import ElasticMaterial
 
 ################################################################################
 
-class CiarletGeymonatElasticMaterial(ElasticMaterial):
+class OgdenCiarletGeymonatElasticMaterial(ElasticMaterial):
 
 
 
     def __init__(self,
             kinematics,
-            parameters):
+            parameters,
+            decoup=False):
 
         self.kinematics = kinematics
 
-        self.lmbda = self.get_lambda_from_parameters(parameters)
+        self.C0 = self.get_C0_from_parameters(parameters, decoup)
 
-        self.Psi = (self.lmbda/4) * (self.kinematics.J**2 - 1 - 2*dolfin.ln(self.kinematics.J)) # MG20180516: In 2d, plane strain
+        self.Psi = self.C0 * (self.kinematics.J**2 - 1 - 2*dolfin.ln(self.kinematics.J)) # MG20180516: In 2d, plane strain
 
         self.checkJ = parameters.get("checkJ", False)
         if (self.checkJ):
             self.Sigma = dolfin.conditional( # MG20230320: Otherwise Sigma is well defined for J < 0…
                 dolfin.gt(self.kinematics.J, 0.),
-                (self.lmbda/2) * (self.kinematics.J**2 - 1) * self.kinematics.C_inv, # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
+                2*self.C0 * (self.kinematics.J**2 - 1) * self.kinematics.C_inv, # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
                 self.kinematics.C_inv/dolfin.Constant(0.))
         else:
-            self.Sigma = (self.lmbda/2) * (self.kinematics.J**2 - 1) * self.kinematics.C_inv # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
+            self.Sigma = 2*self.C0 * (self.kinematics.J**2 - 1) * self.kinematics.C_inv # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
+
+        if (self.kinematics.dim == 2):
+            self.Sigma_ZZ = 2*self.C0 * (self.kinematics.J**2 - 1)
 
         # self.P = dolfin.diff(self.Psi, self.kinematics.F) # MG20220426: Cannot do that for micromechanics problems
-        # self.P = (self.lmbda/2) * (self.kinematics.J**2 - 1) * self.kinematics.F_inv.T
+        # self.P = 2*self.C0 * (self.kinematics.J**2 - 1) * self.kinematics.F_inv.T
         self.P = self.kinematics.F * self.Sigma
 
         self.sigma = self.P * self.kinematics.F.T / self.kinematics.J
 
 
+
     # def get_free_energy(self,
     #         U=None,
     #         C=None):
 
     #     C  = self.get_C_from_U_or_C(U, C)
     #     JF = dolfin.sqrt(dolfin.det(C)) # MG20200207: Watch out! This is well defined for inverted elements!
 
-    #     Psi   = (self.lmbda/4) * (JF**2 - 1 - 2*dolfin.ln(JF)) # MG20180516: in 2d, plane strain
+    #     Psi   = self.C0 * (JF**2 - 1 - 2*dolfin.ln(JF)) # MG20180516: in 2d, plane strain
     #     Sigma = 2*dolfin.diff(Psi, C)
 
     #     # C_inv = dolfin.inv(C)
-    #     # Sigma = (self.lmbda/2) * (JF**2 - 1) * C_inv
+    #     # Sigma = 2*self.C0 * (JF**2 - 1) * C_inv
 
     #     return Psi, Sigma
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_CiarletGeymonatNeoHookean.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_OgdenCiarletGeymonatNeoHookean.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 ###                                                                          ###
 ### Created by Martin Genet, 2018-2023                                       ###
 ###                                                                          ###
 ### École Polytechnique, Palaiseau, France                                   ###
 ###                                                                          ###
 ################################################################################
 
-import dolfin
-
 import dolfin_mech as dmech
 from .Material_Elastic import ElasticMaterial
 
 ################################################################################
 
-class CiarletGeymonatNeoHookeanElasticMaterial(ElasticMaterial):
+class OgdenCiarletGeymonatNeoHookeanElasticMaterial(ElasticMaterial):
 
 
 
     def __init__(self,
             kinematics,
             parameters,
             decoup=False):
 
         self.kinematics = kinematics
 
-        self.bulk = dmech.CiarletGeymonatElasticMaterial(kinematics, parameters)
+        self.bulk = dmech.OgdenCiarletGeymonatElasticMaterial(kinematics, parameters, decoup)
         self.dev  = dmech.NeoHookeanElasticMaterial(kinematics, parameters, decoup)
 
         self.Psi   = self.bulk.Psi   + self.dev.Psi
         self.Sigma = self.bulk.Sigma + self.dev.Sigma
+        if (self.kinematics.dim == 2):
+            self.Sigma_ZZ = self.bulk.Sigma_ZZ + self.dev.Sigma_ZZ
         self.P     = self.bulk.P     + self.dev.P
         self.sigma = self.bulk.sigma + self.dev.sigma
 
 
 
     # def get_free_energy(self, *args, **kwargs):
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_CiarletGeymonatNeoHookeanMooneyRivlin.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_OgdenCiarletGeymonatNeoHookeanMooneyRivlin.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 ###                                                                          ###
 ### Created by Martin Genet, 2018-2023                                       ###
 ###                                                                          ###
 ### École Polytechnique, Palaiseau, France                                   ###
 ###                                                                          ###
 ################################################################################
 
-import dolfin
-
 import dolfin_mech as dmech
 from .Material_Elastic import ElasticMaterial
 
 ################################################################################
 
-class CiarletGeymonatNeoHookeanMooneyRivlinElasticMaterial(ElasticMaterial):
+class OgdenCiarletGeymonatNeoHookeanMooneyRivlinElasticMaterial(ElasticMaterial):
 
 
 
     def __init__(self,
             kinematics,
             parameters,
             decoup=False):
 
         self.kinematics = kinematics
 
-        self.bulk = dmech.CiarletGeymonatElasticMaterial(kinematics, parameters)
+        self.bulk = dmech.OgdenCiarletGeymonatElasticMaterial(kinematics, parameters, decoup)
         self.dev  = dmech.NeoHookeanMooneyRivlinElasticMaterial(kinematics, parameters, decoup)
 
         self.Psi   = self.bulk.Psi   + self.dev.Psi
         self.Sigma = self.bulk.Sigma + self.dev.Sigma
+        if (self.kinematics.dim == 2):
+            self.Sigma_ZZ = self.bulk.Sigma_ZZ + self.dev.Sigma_ZZ
         self.P     = self.bulk.P     + self.dev.P
         self.sigma = self.bulk.sigma + self.dev.sigma
 
 
 
     # def get_free_energy(self, *args, **kwargs):
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_ExponentialCiarletGeymonat.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_ExponentialOgdenCiarletGeymonat.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import dolfin
 
 import dolfin_mech as dmech
 from .Material_Elastic import ElasticMaterial
 
 ################################################################################
 
-class ExponentialCiarletGeymonat(ElasticMaterial):
+class ExponentialOgdenCiarletGeymonat(ElasticMaterial):
 
 
 
     def __init__(self,
             kinematics,
             parameters):
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Hooke.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Hooke.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
         self.sigma = dolfin.diff(self.psi, self.kinematics.epsilon)
         # self.sigma = self.lmbda * dolfin.tr(self.kinematics.epsilon) * self.kinematics.I + 2 * self.mu * self.kinematics.epsilon
 
         self.Sigma = self.sigma
         self.P     = self.sigma
 
+        if (self.kinematics.dim == 2):
+            self.sigma_ZZ = self.lmbda * dolfin.tr(self.kinematics.epsilon)
+
 
 
     # def get_free_energy(self,
     #         U=None,
     #         epsilon=None):
 
     #     epsilon = self.get_epsilon_from_U_or_epsilon(
@@ -63,22 +66,27 @@
 
     def __init__(self,
             kinematics,
             parameters):
 
         self.kinematics = kinematics
 
-        self.K = self.get_K_from_parameters(parameters)
+        # self.K = self.get_K_from_parameters(parameters)
+        self.lmbda, self.mu = self.get_lambda_and_mu_from_parameters(parameters)
+        self.K = (self.kinematics.dim*self.lmbda + 2*self.mu)/self.kinematics.dim
 
         self.psi   = (self.kinematics.dim*self.K/2) * dolfin.tr(self.kinematics.epsilon_sph)**2
         self.sigma =  self.kinematics.dim*self.K    *           self.kinematics.epsilon_sph
 
         self.Sigma = self.sigma
         self.P     = self.sigma
 
+        if (self.kinematics.dim == 2):
+            self.sigma_ZZ = self.K * dolfin.tr(self.kinematics.epsilon)
+
 
 
     # def get_free_energy(self,
     #         U=None,
     #         epsilon=None,
     #         epsilon_sph=None):
 
@@ -124,14 +132,17 @@
 
         self.psi   =   self.G * dolfin.inner(self.kinematics.epsilon_dev, self.kinematics.epsilon_dev)
         self.sigma = 2*self.G *              self.kinematics.epsilon_dev
 
         self.Sigma = self.sigma
         self.P     = self.sigma
 
+        if (self.kinematics.dim == 2):
+            self.sigma_ZZ = -2*self.G/3 * dolfin.tr(self.kinematics.epsilon)
+
 
 
     # def get_free_energy(self,
     #         U=None,
     #         epsilon=None,
     #         epsilon_dev=None):
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Kirchhoff.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Kirchhoff.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         self.kinematics.E = dolfin.variable(self.kinematics.E)
 
         self.Psi = (self.lmbda/2) * dolfin.tr(self.kinematics.E)**2 + self.mu * dolfin.inner(self.kinematics.E, self.kinematics.E)
 
         self.Sigma = dolfin.diff(self.Psi, self.kinematics.E)
         # self.Sigma = self.lmbda * dolfin.tr(self.kinematics.E) * self.kinematics.I + 2 * self.mu * self.kinematics.E
 
+        if (self.kinematics.dim == 2):
+            self.Sigma_ZZ = self.lmbda * dolfin.tr(self.kinematics.E)
+
         self.P = self.kinematics.F * self.Sigma
         
         self.sigma = self.P * self.kinematics.F.T / self.kinematics.J
 
 
 
     # def get_free_energy(self,
@@ -66,19 +69,24 @@
 
     def __init__(self,
             kinematics,
             parameters):
 
         self.kinematics = kinematics
 
-        self.K = self.get_K_from_parameters(parameters)
+        # self.K = self.get_K_from_parameters(parameters)
+        self.lmbda, self.mu = self.get_lambda_and_mu_from_parameters(parameters)
+        self.K = (self.kinematics.dim*self.lmbda + 2*self.mu)/self.kinematics.dim
 
         self.Psi   = (self.kinematics.dim*self.K/2) * dolfin.tr(self.kinematics.E_sph)**2
         self.Sigma =  self.kinematics.dim*self.K    *           self.kinematics.E_sph
 
+        if (self.kinematics.dim == 2):
+            self.Sigma_ZZ = self.K * dolfin.tr(self.kinematics.E)
+
         # self.P = dolfin.diff(self.Psi, self.kinematics.F) # MG20220426: Cannot do that for micromechanics problems
         self.P     = self.kinematics.F * self.Sigma
 
         self.sigma = self.P * self.kinematics.F.T / self.kinematics.J
 
 
 
@@ -128,14 +136,17 @@
         self.kinematics = kinematics
 
         self.G = self.get_G_from_parameters(parameters)
 
         self.Psi   =   self.G * dolfin.inner(self.kinematics.E_dev, self.kinematics.E_dev)
         self.Sigma = 2*self.G *              self.kinematics.E_dev
 
+        if (self.kinematics.dim == 2):
+            self.Sigma_ZZ = -2*self.G/3 * dolfin.tr(self.kinematics.E)
+
         # self.P     = dolfin.diff(self.Psi, self.kinematics.F)
         self.P     = self.kinematics.F * self.Sigma
 
         self.sigma = self.P * self.kinematics.F.T / self.kinematics.J
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Lung_Wbulk.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Lung_Wbulk.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Lung_Wpore.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Lung_Wpore.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Lung_Wskel.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Lung_Wskel.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 
     def __init__(self,
             kinematics,
             parameters):
 
         self.kinematics = kinematics
 
-        self.bulk = dmech.ExponentialCiarletGeymonat(kinematics, parameters)
+        self.bulk = dmech.ExponentialOgdenCiarletGeymonat(kinematics, parameters)
         self.dev  = dmech.NeoHookeanMooneyRivlinElasticMaterial(kinematics, parameters)
 
         self.Psi   = self.bulk.Psi   + self.dev.Psi
         self.Sigma = self.bulk.Sigma + self.dev.Sigma
         self.P     = self.bulk.P     + self.dev.P
         self.sigma = self.bulk.sigma + self.dev.sigma
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_MooneyRivlin.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_MooneyRivlin.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,23 +26,25 @@
 
         self.kinematics = kinematics
 
         self.C2 = self.get_C2_from_parameters(parameters)
 
         if (decoup):
             if   (self.kinematics.dim == 2):
-                self.Psi   =   self.C2 * (self.kinematics.IIC_bar + self.kinematics.J**(-2/3) * self.kinematics.IC_bar - 3) # MG20200206: Plane strain
-                assert (0), "ToDo. Aborting."
+                self.Psi      =   self.C2 * (self.kinematics.IIC_bar + self.kinematics.J**(-2/3) * self.kinematics.IC_bar - 3) # MG20200206: Plane strain
+                self.Sigma    = 2*self.C2 * self.kinematics.J**(-4/3) * ((self.kinematics.IC+1) * self.kinematics.I - self.kinematics.C - 2*(self.kinematics.IIC+self.kinematics.IC)/3 * self.kinematics.C_inv) # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
+                self.Sigma_ZZ = 2*self.C2 * self.kinematics.J**(-4/3) * (self.kinematics.IC - 2*(self.kinematics.IIC+self.kinematics.IC)/3)
             elif (self.kinematics.dim == 3):
                 self.Psi   =   self.C2 * (self.kinematics.IIC_bar - 3)
-                self.Sigma = dolfin.diff(self.Psi, self.kinematics.C)
+                self.Sigma = 2*self.C2 * self.kinematics.J**(-4/3) * (self.kinematics.IC * self.kinematics.I - self.kinematics.C - 2*self.kinematics.IIC/3 * self.kinematics.C_inv) # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
         else:
             if   (self.kinematics.dim == 2):
-                self.Psi   =   self.C2 * (self.kinematics.IIC + self.kinematics.IC - 3 - 4*dolfin.ln(self.kinematics.J)) # MG20200206: Plane strain
-                self.Sigma = 2*self.C2 * (self.kinematics.IC * self.kinematics.I - self.kinematics.C + self.kinematics.I - 2*self.kinematics.C_inv) # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
+                self.Psi      =   self.C2 * (self.kinematics.IIC + self.kinematics.IC - 3 - 4*dolfin.ln(self.kinematics.J)) # MG20200206: Plane strain
+                self.Sigma    = 2*self.C2 * ((self.kinematics.IC+1) * self.kinematics.I - self.kinematics.C - 2*self.kinematics.C_inv) # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
+                self.Sigma_ZZ = 2*self.C2 * (self.kinematics.IC - 2)
             elif (self.kinematics.dim == 3):
                 self.Psi   =   self.C2 * (self.kinematics.IIC - 3 - 4*dolfin.ln(self.kinematics.J))
                 self.Sigma = 2*self.C2 * (self.kinematics.IC * self.kinematics.I - self.kinematics.C - 2*self.kinematics.C_inv) # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
         
         # self.P = dolfin.diff(self.Psi, self.kinematics.F) # MG20220426: Cannot do that for micromechanics problems
         self.P = self.kinematics.F * self.Sigma
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_NeoHookean.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_NeoHookean.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,23 +26,26 @@
 
         self.kinematics = kinematics
 
         self.C1 = self.get_C1_from_parameters(parameters)
 
         if (decoup):
             if   (self.kinematics.dim == 2):
-                self.Psi   = self.C1 * (self.kinematics.IC_bar + self.kinematics.J**(-2/3) - 3)  # MG20200206: Plane strain
-                assert (0), "ToDo. Aborting."
+                # self.Psi      =   self.C1 * (self.kinematics.J**(-2/3) * (self.kinematics.J * self.kinematics.IC_bar + 1) - 3) # MG20200206: Plane strain, written with IC_bar_2D (I prefer the expression with IC_2D)
+                self.Psi      =   self.C1 * (self.kinematics.J**(-2/3) * (self.kinematics.IC + 1) - 3) # MG20200206: Plane strain, written with IC_2D
+                self.Sigma    = 2*self.C1 * self.kinematics.J**(-2/3) * (self.kinematics.I - (self.kinematics.IC + 1)/3 * self.kinematics.C_inv) # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
+                self.Sigma_ZZ = 2*self.C1 * self.kinematics.J**(-2/3) * (1 - (self.kinematics.IC + 1)/3)
             elif (self.kinematics.dim == 3):
-                self.Psi   = self.C1 * (self.kinematics.IC_bar - 3)
-                self.Sigma = dolfin.diff(self.Psi, self.kinematics.C)
+                self.Psi   =   self.C1 * (self.kinematics.IC_bar - 3)
+                self.Sigma = 2*self.C1 * self.kinematics.J**(-2/3) * (self.kinematics.I - self.kinematics.IC/3 * self.kinematics.C_inv) # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
         else:
             if   (self.kinematics.dim == 2):
-                self.Psi   =   self.C1 * (self.kinematics.IC - 2 - 2*dolfin.ln(self.kinematics.J)) # MG20200206: Plane strain
-                self.Sigma = 2*self.C1 * (self.kinematics.I - self.kinematics.C_inv) # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
+                self.Psi      =   self.C1 * (self.kinematics.IC - 2 - 2*dolfin.ln(self.kinematics.J)) # MG20200206: Plane strain
+                self.Sigma    = 2*self.C1 * (self.kinematics.I - self.kinematics.C_inv) # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
+                self.Sigma_ZZ = dolfin.Constant(0.)
             elif (self.kinematics.dim == 3):
                 self.Psi   =   self.C1 * (self.kinematics.IC - 3 - 2*dolfin.ln(self.kinematics.J))
                 self.Sigma = 2*self.C1 * (self.kinematics.I - self.kinematics.C_inv) # MG20200206: Cannot differentiate Psi wrt to C because J is not defined as a function of C
 
         # self.P = dolfin.diff(self.Psi, self.kinematics.F) # MG20220426: Cannot do that for micromechanics problems
         self.P = self.kinematics.F * self.Sigma
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_NeoHookeanMooneyRivlin.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_NeoHookeanMooneyRivlin.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         parameters["C2"] = C2
 
         self.nh = dmech.NeoHookeanElasticMaterial(kinematics, parameters, decoup)
         self.mr = dmech.MooneyRivlinElasticMaterial(kinematics, parameters, decoup)
 
         self.Psi   = self.nh.Psi   + self.mr.Psi
         self.Sigma = self.nh.Sigma + self.mr.Sigma
+        if (self.kinematics.dim == 2):
+            self.Sigma_ZZ = self.nh.Sigma_ZZ + self.mr.Sigma_ZZ
         self.P     = self.nh.P     + self.mr.P
         self.sigma = self.nh.sigma + self.mr.sigma
 
 
 
     # def get_free_energy(self, *args, **kwargs):
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Elastic_Porous.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Elastic_Porous.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Material_Inelastic.py` & `dolfin_mech-2023.6.6/dolfin_mech/Material_Inelastic.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/NonlinearSolver.py` & `dolfin_mech-2023.6.6/dolfin_mech/NonlinearSolver.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_HyperElasticity.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_HyperElasticity.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_HyperHydrostaticPressure.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_HyperHydrostaticPressure.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_HyperIncompressibility.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_HyperIncompressibility.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Inertia.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Inertia.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_LinearizedElasticity.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_LinearizedElasticity.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_LinearizedHydrostaticPressure.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_LinearizedHydrostaticPressure.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_LinearizedIncompressibility.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_LinearizedIncompressibility.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Loading_SurfaceForce.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Loading_SurfaceForce.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Loading_SurfacePressure.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Loading_SurfacePressure.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Loading_SurfacePressureGradient.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Loading_SurfacePressureGradient.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Loading_SurfaceTension.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Loading_SurfaceTension.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Loading_VolumeForce.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Loading_VolumeForce.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_MacroscopicStress.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_MacroscopicStress.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Penalty_DirectionalDisplacement.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Penalty_DirectionalDisplacement.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Penalty_MacroscopicStressComponent.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Penalty_MacroscopicStressComponent.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Penalty_MacroscopicStretchComponent.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Penalty_MacroscopicStretchComponent.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Penalty_MacroscopicStretchSymmetry.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Penalty_MacroscopicStretchSymmetry.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Penalty_NormalDisplacement.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Penalty_NormalDisplacement.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Poro_Pf.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Poro_Pf.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Poro_Wbulk.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Poro_Wbulk.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Poro_Wpore.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Poro_Wpore.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_Poro_Wskel.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_Poro_Wskel.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Operator_TensorSymmetry.py` & `dolfin_mech-2023.6.6/dolfin_mech/Operator_TensorSymmetry.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Problem.py` & `dolfin_mech-2023.6.6/dolfin_mech/Problem.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Problem_Elasticity.py` & `dolfin_mech-2023.6.6/dolfin_mech/Problem_Elasticity.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Problem_Hyperelasticity.py` & `dolfin_mech-2023.6.6/dolfin_mech/Problem_Hyperelasticity.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,13 +362,30 @@
                     expr=sum([getattr(operator.material, stress)[1,2]*operator.measure for operator in self.operators if (hasattr(operator, "material") and hasattr(operator.material, stress))]))
                 self.add_qoi(
                     name=basename+"ZX",
                     expr=sum([getattr(operator.material, stress)[2,0]*operator.measure for operator in self.operators if (hasattr(operator, "material") and hasattr(operator.material, stress))]))
 
 
 
+    def add_global_out_of_plane_stress_qois(self,
+            stress_type="PK2"):
+
+        if (stress_type in ("Cauchy", "cauchy", "sigma")):
+            assert (0), "To do. Aborting."
+        elif (stress_type in ("Piola", "piola", "PK2", "Sigma")):
+            basename = "S_ZZ"
+            stress = "Sigma_ZZ"
+        elif (stress_type in ("Boussinesq", "boussinesq", "PK1", "P")):
+            assert (0), "To do. Aborting."
+
+        self.add_qoi(
+            name=basename,
+            expr=sum([getattr(operator.material, stress)*operator.measure for operator in self.operators if (hasattr(operator, "material") and hasattr(operator.material, stress))]))
+
+
+
     def add_global_pressure_qoi(self):
 
         self.add_qoi(
             name="P",
             expr=sum([operator.P*operator.measure for operator in self.operators if hasattr(operator, "P")]))
             # expr=sum([-dolfin.tr(operator.material.sigma)/3*operator.measure for operator in self.operators if (hasattr(operator, "material") and hasattr(operator.material, "sigma"))])+sum([operator.P*operator.measure for operator in self.operators if hasattr(operator, "P")]))
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Problem_Hyperelasticity_Inverse.py` & `dolfin_mech-2023.6.6/dolfin_mech/Problem_Hyperelasticity_Inverse.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Problem_Hyperelasticity_MicroPoro.py` & `dolfin_mech-2023.6.6/dolfin_mech/Problem_Hyperelasticity_MicroPoro.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Problem_Hyperelasticity_Poro.py` & `dolfin_mech-2023.6.6/dolfin_mech/Problem_Hyperelasticity_Poro.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Problem_Hyperelasticity_Poro_Inverse.py` & `dolfin_mech-2023.6.6/dolfin_mech/Problem_Hyperelasticity_Poro_Inverse.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/QOI.py` & `dolfin_mech-2023.6.6/dolfin_mech/QOI.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/RivlinCube_Elasticity.py` & `dolfin_mech-2023.6.6/dolfin_mech/RivlinCube_Elasticity.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/RivlinCube_Hyperelasticity.py` & `dolfin_mech-2023.6.6/dolfin_mech/RivlinCube_Hyperelasticity.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,15 @@
             k_step=k_step)
 
     ################################################# Quantities of Interest ###
 
     problem.add_global_strain_qois()
     problem.add_global_stress_qois()
     if (incomp): problem.add_global_pressure_qoi()
+    if (inverse==0) and (dim==2): problem.add_global_out_of_plane_stress_qois()
 
     ################################################################# Solver ###
 
     solver = dmech.NonlinearSolver(
         problem=problem,
         parameters={
             "sol_tol":[1e-6]*len(problem.subsols),
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/RivlinCube_Mesh.py` & `dolfin_mech-2023.6.6/dolfin_mech/RivlinCube_Mesh.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/RivlinCube_PoroHyperelasticity.py` & `dolfin_mech-2023.6.6/dolfin_mech/RivlinCube_PoroHyperelasticity.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/Step.py` & `dolfin_mech-2023.6.6/dolfin_mech/Step.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/SubDomain_Periodic.py` & `dolfin_mech-2023.6.6/dolfin_mech/SubDomain_Periodic.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/SubDomain_Pinpoint.py` & `dolfin_mech-2023.6.6/dolfin_mech/SubDomain_Pinpoint.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/SubSol.py` & `dolfin_mech-2023.6.6/dolfin_mech/SubSol.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/TimeIntegrator.py` & `dolfin_mech-2023.6.6/dolfin_mech/TimeIntegrator.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/TimeVaryingConstant.py` & `dolfin_mech-2023.6.6/dolfin_mech/TimeVaryingConstant.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/XDMFFile.py` & `dolfin_mech-2023.6.6/dolfin_mech/XDMFFile.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/__init__.py` & `dolfin_mech-2023.6.6/dolfin_mech/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from .HeartSlice_Mesh import *
 from .Kinematics import *
 from .Kinematics_Inverse import *
 from .Kinematics_Linearized import *
 from .Loading import *
 from .Material import *
 from .Material_Elastic import *
-from .Material_Elastic_CiarletGeymonat import *
-from .Material_Elastic_CiarletGeymonatNeoHookean import *
-from .Material_Elastic_CiarletGeymonatNeoHookeanMooneyRivlin import *
-from .Material_Elastic_ExponentialCiarletGeymonat import *
+from .Material_Elastic_OgdenCiarletGeymonat import *
+from .Material_Elastic_OgdenCiarletGeymonatNeoHookean import *
+from .Material_Elastic_OgdenCiarletGeymonatNeoHookeanMooneyRivlin import *
+from .Material_Elastic_ExponentialOgdenCiarletGeymonat import *
 from .Material_Elastic_Hooke import *
 from .Material_Elastic_Kirchhoff import *
 from .Material_Elastic_Lung_Wbulk import *
 from .Material_Elastic_Lung_Wpore import *
 from .Material_Elastic_Lung_Wskel import *
 from .Material_Elastic_MooneyRivlin import *
 from .Material_Elastic_NeoHookean import *
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/compute_error.py` & `dolfin_mech-2023.6.6/dolfin_mech/compute_error.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/mesh2ugrid.py` & `dolfin_mech-2023.6.6/dolfin_mech/mesh2ugrid.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech/write_VTU_file.py` & `dolfin_mech-2023.6.6/dolfin_mech/write_VTU_file.py`

 * *Files identical despite different names*

### Comparing `dolfin_mech-2023.3.22/dolfin_mech.egg-info/PKG-INFO` & `dolfin_mech-2023.6.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dolfin-mech
-Version: 2023.3.22
+Name: dolfin_mech
+Version: 2023.6.6
 Summary: A set of FEniCS-based python tools for Computational Mechanics.
 Home-page: https://gitlab.inria.fr/mgenet/dolfin_mech
 Author: Martin Genet
 Author-email: martin.genet@polytechnique.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dolfin_mech-2023.3.22/dolfin_mech.egg-info/SOURCES.txt` & `dolfin_mech-2023.6.6/dolfin_mech.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 dolfin_mech/HeartSlice_Mesh.py
 dolfin_mech/Kinematics.py
 dolfin_mech/Kinematics_Inverse.py
 dolfin_mech/Kinematics_Linearized.py
 dolfin_mech/Loading.py
 dolfin_mech/Material.py
 dolfin_mech/Material_Elastic.py
-dolfin_mech/Material_Elastic_CiarletGeymonat.py
-dolfin_mech/Material_Elastic_CiarletGeymonatNeoHookean.py
-dolfin_mech/Material_Elastic_CiarletGeymonatNeoHookeanMooneyRivlin.py
-dolfin_mech/Material_Elastic_ExponentialCiarletGeymonat.py
+dolfin_mech/Material_Elastic_ExponentialOgdenCiarletGeymonat.py
 dolfin_mech/Material_Elastic_Hooke.py
 dolfin_mech/Material_Elastic_Kirchhoff.py
 dolfin_mech/Material_Elastic_Lung_Wbulk.py
 dolfin_mech/Material_Elastic_Lung_Wpore.py
 dolfin_mech/Material_Elastic_Lung_Wskel.py
 dolfin_mech/Material_Elastic_MooneyRivlin.py
 dolfin_mech/Material_Elastic_NeoHookean.py
 dolfin_mech/Material_Elastic_NeoHookeanMooneyRivlin.py
+dolfin_mech/Material_Elastic_OgdenCiarletGeymonat.py
+dolfin_mech/Material_Elastic_OgdenCiarletGeymonatNeoHookean.py
+dolfin_mech/Material_Elastic_OgdenCiarletGeymonatNeoHookeanMooneyRivlin.py
 dolfin_mech/Material_Elastic_Porous.py
 dolfin_mech/Material_Inelastic.py
 dolfin_mech/NonlinearSolver.py
 dolfin_mech/Operator.py
 dolfin_mech/Operator_HyperElasticity.py
 dolfin_mech/Operator_HyperHydrostaticPressure.py
 dolfin_mech/Operator_HyperIncompressibility.py
```

### Comparing `dolfin_mech-2023.3.22/setup.py` & `dolfin_mech-2023.6.6/setup.py`

 * *Files identical despite different names*

