# Comparing `tmp/cashocs-2.0.2.tar.gz` & `tmp/cashocs-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashocs-2.0.2.tar", last modified: Tue Jun  6 07:55:17 2023, max compression
+gzip compressed data, was "cashocs-2.0.3.tar", last modified: Tue Jun  6 11:57:03 2023, max compression
```

## Comparing `cashocs-2.0.2.tar` & `cashocs-2.0.3.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.138937 cashocs-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-06-06 07:55:01.000000 cashocs-2.0.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-06 07:55:17.138937 cashocs-2.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    11025 2023-06-06 07:55:01.000000 cashocs-2.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.106937 cashocs-2.0.2/cashocs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4546 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.106937 cashocs-2.0.2/cashocs/_cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11080 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_cli/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.110936 cashocs-2.0.2/cashocs/_constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_constraints/constrained_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_constraints/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_constraints/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.110936 cashocs-2.0.2/cashocs/_database/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_database/form_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_database/function_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_database/geometry_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_database/parameter_database.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.110936 cashocs-2.0.2/cashocs/_forms/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_forms/control_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_forms/form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_forms/general_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_forms/shape_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_forms/shape_regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.110936 cashocs-2.0.2/cashocs/_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/cost_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.114937 cashocs-2.0.2/cashocs/_optimization/line_search/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/line_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/line_search/armijo_line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/line_search/line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/line_search/polynomial_line_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.114937 cashocs-2.0.2/cashocs/_optimization/optimal_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimal_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimal_control/box_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimal_control/control_variable_abstractions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21515 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimal_control/optimal_control_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.114937 cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/gradient_descent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13523 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/l_bfgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/ncg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/newton.py
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29701 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/optimization_variable_abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.114937 cashocs-2.0.2/cashocs/_optimization/shape_optimization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/shape_optimization/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24150 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/shape_optimization/shape_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.118937 cashocs-2.0.2/cashocs/_optimization/topology_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/topology_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/topology_optimization/topology_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_optimization/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.118937 cashocs-2.0.2/cashocs/_pde_problems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_pde_problems/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5602 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_pde_problems/adjoint_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4272 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_pde_problems/control_gradient_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17636 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_pde_problems/hessian_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_pde_problems/pde_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9445 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_pde_problems/shape_gradient_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7315 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_pde_problems/state_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.118937 cashocs-2.0.2/cashocs/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_utils/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_utils/interpolations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/_utils/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.122937 cashocs-2.0.2/cashocs/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/geometry/boundary_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/geometry/deformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/geometry/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/geometry/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    26963 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/geometry/mesh_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/geometry/mesh_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/geometry/quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.122937 cashocs-2.0.2/cashocs/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31284 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/io/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/io/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/io/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/io/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/io/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.122937 cashocs-2.0.2/cashocs/nonlinear_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/nonlinear_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/nonlinear_solvers/linear_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/nonlinear_solvers/newton_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/nonlinear_solvers/picard_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.122937 cashocs-2.0.2/cashocs/space_mapping/
--rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/space_mapping/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36090 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/space_mapping/optimal_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37353 2023-06-06 07:55:01.000000 cashocs-2.0.2/cashocs/space_mapping/shape_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.106937 cashocs-2.0.2/cashocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-06 07:55:17.000000 cashocs-2.0.2/cashocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-06-06 07:55:17.000000 cashocs-2.0.2/cashocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:55:17.000000 cashocs-2.0.2/cashocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 07:55:17.000000 cashocs-2.0.2/cashocs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-06 07:55:17.000000 cashocs-2.0.2/cashocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 07:55:17.000000 cashocs-2.0.2/cashocs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.122937 cashocs-2.0.2/demos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.098937 cashocs-2.0.2/demos/documented/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.090937 cashocs-2.0.2/demos/documented/cashocs_as_solver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/cashocs_as_solver/control_solver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7337 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/cashocs_as_solver/shape_solver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7422 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.094936 cashocs-2.0.2/demos/documented/misc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/misc/xdmf_io/
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/misc/xdmf_io/demo_xdmf_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.098937 cashocs-2.0.2/demos/documented/optimal_control/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/box_constraints/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5441 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/box_constraints/demo_box_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/constraints/demo_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/control_boundary_conditions/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4275 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/dirichlet_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8197 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/heat_equation/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8961 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/heat_equation/demo_heat_equation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/iterative_solvers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7527 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/monolithic_problems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6405 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/multiple_variables/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8034 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/neumann_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5100 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/neumann_control/demo_neumann_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/nonlinear_pdes/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/picard_iteration/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/poisson/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11379 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/poisson/demo_poisson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/pre_post_callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/scalar_control_tracking/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.126937 cashocs-2.0.2/demos/documented/optimal_control/sparse_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3535 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/sparse_control/demo_sparse_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/optimal_control/state_constraints/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6600 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/state_constraints/demo_state_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/optimal_control/stokes/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7851 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/optimal_control/stokes/demo_stokes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.102937 cashocs-2.0.2/demos/documented/shape_optimization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/custom_scalar_product/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4273 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/eikonal_stiffness/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5712 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/inverse_tomography/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13339 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/p_laplacian/
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/regularization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5398 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/regularization/demo_regularization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/remeshing/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9439 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/remeshing/demo_remeshing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/scaling/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/scaling/demo_scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/shape_poisson/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/shape_stokes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10178 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/space_mapping_semilinear_transmission/
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/test_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.102937 cashocs-2.0.2/demos/undocumented/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.102937 cashocs-2.0.2/demos/undocumented/optimal_control/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/undocumented/optimal_control/different_state_adjoint_spaces/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2535 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.106937 cashocs-2.0.2/demos/undocumented/shape_optimization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/undocumented/shape_optimization/custom_functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/undocumented/shape_optimization/custom_functional/custom_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.130937 cashocs-2.0.2/demos/undocumented/shape_optimization/pipe_optimization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-06-06 07:55:01.000000 cashocs-2.0.2/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.106937 cashocs-2.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.134937 cashocs-2.0.2/docs/source/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4747 2023-06-06 07:55:01.000000 cashocs-2.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-06 07:55:01.000000 cashocs-2.0.2/docs/source/jupytext_process.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3175 2023-06-06 07:55:01.000000 cashocs-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 07:55:17.138937 cashocs-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:55:17.138937 cashocs-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7691 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_control_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19518 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2945 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_log_level.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_nonlinear_solvers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25328 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_optimal_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6571 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_optimal_control_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_optimal_control_space_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_p_laplacian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_pde_problems.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_picard_iterations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7247 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_remeshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_shape_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40742 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_shape_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_shape_optimization_space_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_topology_optimization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8955 2023-06-06 07:55:01.000000 cashocs-2.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.947599 cashocs-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-06-06 11:56:50.000000 cashocs-2.0.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-06 11:57:03.947599 cashocs-2.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11025 2023-06-06 11:56:50.000000 cashocs-2.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.923599 cashocs-2.0.3/cashocs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4546 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.923599 cashocs-2.0.3/cashocs/_cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11080 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_cli/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.923599 cashocs-2.0.3/cashocs/_constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_constraints/constrained_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_constraints/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_constraints/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.927599 cashocs-2.0.3/cashocs/_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/form_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/function_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/geometry_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/parameter_database.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.927599 cashocs-2.0.3/cashocs/_forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/control_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/general_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/shape_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/shape_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.927599 cashocs-2.0.3/cashocs/_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/cost_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.927599 cashocs-2.0.3/cashocs/_optimization/line_search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/line_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/line_search/armijo_line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/line_search/line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/line_search/polynomial_line_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.931599 cashocs-2.0.3/cashocs/_optimization/optimal_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimal_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimal_control/box_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimal_control/control_variable_abstractions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21515 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimal_control/optimal_control_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.931599 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/gradient_descent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13523 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/l_bfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/ncg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29701 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_variable_abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.931599 cashocs-2.0.3/cashocs/_optimization/shape_optimization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/shape_optimization/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24150 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/shape_optimization/shape_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.931599 cashocs-2.0.3/cashocs/_optimization/topology_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/topology_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.931599 cashocs-2.0.3/cashocs/_pde_problems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5602 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/adjoint_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4272 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/control_gradient_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17636 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/hessian_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/pde_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9445 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/shape_gradient_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7315 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/state_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/cashocs/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_utils/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_utils/interpolations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_utils/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/cashocs/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/boundary_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/deformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27202 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/mesh_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/mesh_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/cashocs/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31284 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/cashocs/nonlinear_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/nonlinear_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/nonlinear_solvers/linear_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/nonlinear_solvers/newton_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/nonlinear_solvers/picard_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/cashocs/space_mapping/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/space_mapping/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36090 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/space_mapping/optimal_control.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37353 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/space_mapping/shape_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.923599 cashocs-2.0.3/cashocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/demos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.915598 cashocs-2.0.3/demos/documented/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.911599 cashocs-2.0.3/demos/documented/cashocs_as_solver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/cashocs_as_solver/control_solver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7337 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/cashocs_as_solver/shape_solver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7422 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.911599 cashocs-2.0.3/demos/documented/misc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/misc/xdmf_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/misc/xdmf_io/demo_xdmf_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.915598 cashocs-2.0.3/demos/documented/optimal_control/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/box_constraints/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5441 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/box_constraints/demo_box_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/constraints/demo_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/control_boundary_conditions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4275 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/dirichlet_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8197 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/heat_equation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8961 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/heat_equation/demo_heat_equation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/iterative_solvers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7527 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/monolithic_problems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6405 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/multiple_variables/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8034 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/neumann_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5100 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/neumann_control/demo_neumann_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/nonlinear_pdes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/picard_iteration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/poisson/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11379 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/poisson/demo_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/pre_post_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/scalar_control_tracking/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/sparse_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3535 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/sparse_control/demo_sparse_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/state_constraints/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6600 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/state_constraints/demo_state_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/stokes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7851 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/stokes/demo_stokes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.919599 cashocs-2.0.3/demos/documented/shape_optimization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/shape_optimization/custom_scalar_product/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4273 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/shape_optimization/eikonal_stiffness/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5712 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/shape_optimization/inverse_tomography/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13339 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/shape_optimization/p_laplacian/
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/shape_optimization/regularization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5398 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/regularization/demo_regularization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/remeshing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9439 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/remeshing/demo_remeshing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/scaling/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/scaling/demo_scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/shape_poisson/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/shape_stokes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10178 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_semilinear_transmission/
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/test_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.919599 cashocs-2.0.3/demos/undocumented/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.919599 cashocs-2.0.3/demos/undocumented/optimal_control/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/undocumented/optimal_control/different_state_adjoint_spaces/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2535 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.919599 cashocs-2.0.3/demos/undocumented/shape_optimization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/undocumented/shape_optimization/custom_functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/undocumented/shape_optimization/custom_functional/custom_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/undocumented/shape_optimization/pipe_optimization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.919599 cashocs-2.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/docs/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4747 2023-06-06 11:56:50.000000 cashocs-2.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-06 11:56:50.000000 cashocs-2.0.3/docs/source/jupytext_process.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3175 2023-06-06 11:56:50.000000 cashocs-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:57:03.947599 cashocs-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.947599 cashocs-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7691 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_control_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19518 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2945 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_log_level.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_nonlinear_solvers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25328 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_optimal_control.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6571 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_optimal_control_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_optimal_control_space_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_p_laplacian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_pde_problems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_picard_iterations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7247 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_remeshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_shape_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40742 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_shape_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_shape_optimization_space_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_topology_optimization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8955 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_utils.py
```

### Comparing `cashocs-2.0.2/COPYING` & `cashocs-2.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/PKG-INFO` & `cashocs-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashocs
-Version: 2.0.2
+Version: 2.0.3
 Summary: Computational Adjoint-Based Shape Optimization and Optimal Control Software
 Author: Sebastian Blauth
 Author-email: sebastian.blauth@itwm.fraunhofer.de
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://cashocs.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/sblauth/cashocs
 Project-URL: Tutorial, https://cashocs.readthedocs.io/en/latest/user
```

### Comparing `cashocs-2.0.2/README.rst` & `cashocs-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/__init__.py` & `cashocs-2.0.3/cashocs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 from cashocs.io import convert
 from cashocs.io import import_mesh
 from cashocs.io import load_config
 from cashocs.nonlinear_solvers import linear_solve
 from cashocs.nonlinear_solvers import newton_solve
 from cashocs.nonlinear_solvers import picard_iteration
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 __citation__ = """
 @Article{Blauth2021cashocs,
     author   = {Sebastian Blauth},
     journal  = {SoftwareX},
     title    = {{cashocs: A Computational, Adjoint-Based Shape Optimization and
         Optimal Control Software}},
```

### Comparing `cashocs-2.0.2/cashocs/_cli/__init__.py` & `cashocs-2.0.3/cashocs/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_cli/_convert.py` & `cashocs-2.0.3/cashocs/_cli/_convert.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_constraints/__init__.py` & `cashocs-2.0.3/cashocs/_constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_constraints/constrained_problems.py` & `cashocs-2.0.3/cashocs/_constraints/constrained_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_constraints/constraints.py` & `cashocs-2.0.3/cashocs/_constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_constraints/solvers.py` & `cashocs-2.0.3/cashocs/_constraints/solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_database/__init__.py` & `cashocs-2.0.3/cashocs/_database/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_database/database.py` & `cashocs-2.0.3/cashocs/_database/database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_database/form_database.py` & `cashocs-2.0.3/cashocs/_database/form_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_database/function_database.py` & `cashocs-2.0.3/cashocs/_database/function_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_database/geometry_database.py` & `cashocs-2.0.3/cashocs/_database/geometry_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_database/parameter_database.py` & `cashocs-2.0.3/cashocs/_database/parameter_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_exceptions.py` & `cashocs-2.0.3/cashocs/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_forms/__init__.py` & `cashocs-2.0.3/cashocs/_forms/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_forms/control_form_handler.py` & `cashocs-2.0.3/cashocs/_forms/control_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_forms/form_handler.py` & `cashocs-2.0.3/cashocs/_forms/form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_forms/general_form_handler.py` & `cashocs-2.0.3/cashocs/_forms/general_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_forms/shape_form_handler.py` & `cashocs-2.0.3/cashocs/_forms/shape_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_forms/shape_regularization.py` & `cashocs-2.0.3/cashocs/_forms/shape_regularization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_loggers.py` & `cashocs-2.0.3/cashocs/_loggers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/__init__.py` & `cashocs-2.0.3/cashocs/_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/cost_functional.py` & `cashocs-2.0.3/cashocs/_optimization/cost_functional.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/line_search/__init__.py` & `cashocs-2.0.3/cashocs/_optimization/line_search/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/line_search/armijo_line_search.py` & `cashocs-2.0.3/cashocs/_optimization/line_search/armijo_line_search.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/line_search/line_search.py` & `cashocs-2.0.3/cashocs/_optimization/line_search/line_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,22 @@
         self.state_problem = optimization_problem.state_problem
         self.optimization_variable_abstractions = (
             optimization_problem.optimization_variable_abstractions
         )
         self.cost_functional = optimization_problem.reduced_cost_functional
 
         if self.db.parameter_db.problem_type == "shape":
-            self.deformation_function = fenics.Function(
-                self.db.function_db.control_spaces[0]
-            )
+            if "deformation_function" in self.db.parameter_db.temp_dict.keys():
+                self.deformation_function = self.db.parameter_db.temp_dict[
+                    "deformation_function"
+                ]
+            else:
+                self.deformation_function = fenics.Function(
+                    self.db.function_db.control_spaces[0]
+                )
             self.global_deformation_vector = self.deformation_function.vector().vec()
 
         self.stepsize = self.config.getfloat("LineSearch", "initial_stepsize")
         self.safeguard_stepsize = self.config.getboolean(
             "LineSearch", "safeguard_stepsize"
         )
```

### Comparing `cashocs-2.0.2/cashocs/_optimization/line_search/polynomial_line_search.py` & `cashocs-2.0.3/cashocs/_optimization/line_search/polynomial_line_search.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimal_control/__init__.py` & `cashocs-2.0.3/cashocs/_optimization/optimal_control/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimal_control/box_constraints.py` & `cashocs-2.0.3/cashocs/_optimization/optimal_control/box_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimal_control/control_variable_abstractions.py` & `cashocs-2.0.3/cashocs/_optimization/optimal_control/control_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimal_control/optimal_control_problem.py` & `cashocs-2.0.3/cashocs/_optimization/optimal_control/optimal_control_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/__init__.py` & `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/callback.py` & `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/callback.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/gradient_descent.py` & `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/l_bfgs.py` & `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/l_bfgs.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/ncg.py` & `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/ncg.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/newton.py` & `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/newton.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py` & `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimization_problem.py` & `cashocs-2.0.3/cashocs/_optimization/optimization_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/optimization_variable_abstractions.py` & `cashocs-2.0.3/cashocs/_optimization/optimization_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/shape_optimization/__init__.py` & `cashocs-2.0.3/cashocs/_optimization/shape_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/shape_optimization/shape_optimization_problem.py` & `cashocs-2.0.3/cashocs/_optimization/shape_optimization/shape_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py` & `cashocs-2.0.3/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/topology_optimization/__init__.py` & `cashocs-2.0.3/cashocs/_optimization/topology_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py` & `cashocs-2.0.3/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py` & `cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/topology_optimization/topology_optimization_problem.py` & `cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py` & `cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_optimization/verification.py` & `cashocs-2.0.3/cashocs/_optimization/verification.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_pde_problems/__init__.py` & `cashocs-2.0.3/cashocs/_pde_problems/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_pde_problems/adjoint_problem.py` & `cashocs-2.0.3/cashocs/_pde_problems/adjoint_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_pde_problems/control_gradient_problem.py` & `cashocs-2.0.3/cashocs/_pde_problems/control_gradient_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_pde_problems/hessian_problems.py` & `cashocs-2.0.3/cashocs/_pde_problems/hessian_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_pde_problems/pde_problem.py` & `cashocs-2.0.3/cashocs/_pde_problems/pde_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_pde_problems/shape_gradient_problem.py` & `cashocs-2.0.3/cashocs/_pde_problems/shape_gradient_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_pde_problems/state_problem.py` & `cashocs-2.0.3/cashocs/_pde_problems/state_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_typing.py` & `cashocs-2.0.3/cashocs/_typing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_utils/__init__.py` & `cashocs-2.0.3/cashocs/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_utils/forms.py` & `cashocs-2.0.3/cashocs/_utils/forms.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_utils/helpers.py` & `cashocs-2.0.3/cashocs/_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_utils/interpolations.py` & `cashocs-2.0.3/cashocs/_utils/interpolations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/_utils/linalg.py` & `cashocs-2.0.3/cashocs/_utils/linalg.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/geometry/__init__.py` & `cashocs-2.0.3/cashocs/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/geometry/boundary_distance.py` & `cashocs-2.0.3/cashocs/geometry/boundary_distance.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/geometry/deformations.py` & `cashocs-2.0.3/cashocs/geometry/deformations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/geometry/measure.py` & `cashocs-2.0.3/cashocs/geometry/measure.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/geometry/mesh.py` & `cashocs-2.0.3/cashocs/geometry/mesh.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/geometry/mesh_handler.py` & `cashocs-2.0.3/cashocs/geometry/mesh_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -633,15 +633,15 @@
             self.db.parameter_db.temp_dict["OptimizationRoutine"][
                 "iteration_counter"
             ] = solver.iteration
             self.db.parameter_db.temp_dict["OptimizationRoutine"][
                 "gradient_norm_initial"
             ] = solver.gradient_norm_initial
 
-            self._update_mesh_transfer_matrix(new_xdmf_file)
+            self._update_mesh_transfer_matrix(new_xdmf_file, solver)
 
             self._reinitialize(solver)
             self._check_imported_mesh_quality(solver)
 
     def _check_imported_mesh_quality(self, solver: OptimizationAlgorithm) -> None:
         """Checks the quality of an imported mesh.
 
@@ -671,19 +671,22 @@
             mesh,
             mesh_quality_type,
             mesh_quality_measure,
         )
 
         check_mesh_quality_tolerance(current_mesh_quality, mesh_quality_tol_upper)
 
-    def _update_mesh_transfer_matrix(self, xdmf_filename: str) -> None:
+    def _update_mesh_transfer_matrix(
+        self, xdmf_filename: str, solver: OptimizationAlgorithm
+    ) -> None:
         """Updates the transfer matrix for the global deformation after remeshing.
 
         Args:
             xdmf_filename: The filename for the new mesh (in XDMF format).
+            solver: The optimization algorithm.
 
         """
         pre_log_level = (
             _loggers._cashocs_logger.level  # pylint: disable=protected-access
         )
         _loggers.set_log_level(_loggers.LogLevel.WARNING)
         mesh, _, _, _, _, _ = import_mesh(xdmf_filename)
@@ -696,7 +699,10 @@
         new_transfer_matrix = self.db.geometry_db.transfer_matrix.matMult(
             interpolator.transfer_matrix
         )
         self.db.parameter_db.temp_dict["transfer_matrix"] = new_transfer_matrix.copy()
         self.db.parameter_db.temp_dict[
             "old_transfer_matrix"
         ] = self.db.geometry_db.transfer_matrix.copy()
+        self.db.parameter_db.temp_dict[
+            "deformation_function"
+        ] = solver.line_search.deformation_function.copy(True)
```

### Comparing `cashocs-2.0.2/cashocs/geometry/mesh_testing.py` & `cashocs-2.0.3/cashocs/geometry/mesh_testing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/geometry/quality.py` & `cashocs-2.0.3/cashocs/geometry/quality.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/io/__init__.py` & `cashocs-2.0.3/cashocs/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/io/config.py` & `cashocs-2.0.3/cashocs/io/config.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/io/function.py` & `cashocs-2.0.3/cashocs/io/function.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/io/managers.py` & `cashocs-2.0.3/cashocs/io/managers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/io/mesh.py` & `cashocs-2.0.3/cashocs/io/mesh.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/io/output.py` & `cashocs-2.0.3/cashocs/io/output.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/nonlinear_solvers/__init__.py` & `cashocs-2.0.3/cashocs/nonlinear_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/nonlinear_solvers/linear_solver.py` & `cashocs-2.0.3/cashocs/nonlinear_solvers/linear_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/nonlinear_solvers/newton_solver.py` & `cashocs-2.0.3/cashocs/nonlinear_solvers/newton_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/nonlinear_solvers/picard_solver.py` & `cashocs-2.0.3/cashocs/nonlinear_solvers/picard_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/space_mapping/__init__.py` & `cashocs-2.0.3/cashocs/space_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/space_mapping/optimal_control.py` & `cashocs-2.0.3/cashocs/space_mapping/optimal_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs/space_mapping/shape_optimization.py` & `cashocs-2.0.3/cashocs/space_mapping/shape_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/cashocs.egg-info/PKG-INFO` & `cashocs-2.0.3/cashocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashocs
-Version: 2.0.2
+Version: 2.0.3
 Summary: Computational Adjoint-Based Shape Optimization and Optimal Control Software
 Author: Sebastian Blauth
 Author-email: sebastian.blauth@itwm.fraunhofer.de
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://cashocs.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/sblauth/cashocs
 Project-URL: Tutorial, https://cashocs.readthedocs.io/en/latest/user
```

### Comparing `cashocs-2.0.2/cashocs.egg-info/SOURCES.txt` & `cashocs-2.0.3/cashocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py` & `cashocs-2.0.3/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py` & `cashocs-2.0.3/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/misc/xdmf_io/demo_xdmf_io.py` & `cashocs-2.0.3/demos/documented/misc/xdmf_io/demo_xdmf_io.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/box_constraints/demo_box_constraints.py` & `cashocs-2.0.3/demos/documented/optimal_control/box_constraints/demo_box_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/constraints/demo_constraints.py` & `cashocs-2.0.3/demos/documented/optimal_control/constraints/demo_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py` & `cashocs-2.0.3/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py` & `cashocs-2.0.3/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/heat_equation/demo_heat_equation.py` & `cashocs-2.0.3/demos/documented/optimal_control/heat_equation/demo_heat_equation.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py` & `cashocs-2.0.3/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py` & `cashocs-2.0.3/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py` & `cashocs-2.0.3/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/neumann_control/demo_neumann_control.py` & `cashocs-2.0.3/demos/documented/optimal_control/neumann_control/demo_neumann_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py` & `cashocs-2.0.3/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py` & `cashocs-2.0.3/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/poisson/demo_poisson.py` & `cashocs-2.0.3/demos/documented/optimal_control/poisson/demo_poisson.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py` & `cashocs-2.0.3/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py` & `cashocs-2.0.3/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/sparse_control/demo_sparse_control.py` & `cashocs-2.0.3/demos/documented/optimal_control/sparse_control/demo_sparse_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/state_constraints/demo_state_constraints.py` & `cashocs-2.0.3/demos/documented/optimal_control/state_constraints/demo_state_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/optimal_control/stokes/demo_stokes.py` & `cashocs-2.0.3/demos/documented/optimal_control/stokes/demo_stokes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py` & `cashocs-2.0.3/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py` & `cashocs-2.0.3/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py` & `cashocs-2.0.3/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py` & `cashocs-2.0.3/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/regularization/demo_regularization.py` & `cashocs-2.0.3/demos/documented/shape_optimization/regularization/demo_regularization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/remeshing/demo_remeshing.py` & `cashocs-2.0.3/demos/documented/shape_optimization/remeshing/demo_remeshing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/scaling/demo_scaling.py` & `cashocs-2.0.3/demos/documented/shape_optimization/scaling/demo_scaling.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py` & `cashocs-2.0.3/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py` & `cashocs-2.0.3/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py` & `cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py` & `cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/test.py` & `cashocs-2.0.3/demos/test.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/test_mpi.py` & `cashocs-2.0.3/demos/test_mpi.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py` & `cashocs-2.0.3/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py` & `cashocs-2.0.3/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/undocumented/shape_optimization/custom_functional/custom_functional.py` & `cashocs-2.0.3/demos/undocumented/shape_optimization/custom_functional/custom_functional.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py` & `cashocs-2.0.3/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/docs/source/conf.py` & `cashocs-2.0.3/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "cashocs"
 copyright = "2020-2023, Sebastian Blauth"
 author = "Sebastian Blauth"
 
 # The full version, including alpha/beta/rc tags
-release = "2.0.2"
+release = "2.0.3"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `cashocs-2.0.2/docs/source/jupytext_process.py` & `cashocs-2.0.3/docs/source/jupytext_process.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/pyproject.toml` & `cashocs-2.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cashocs"
-version = "2.0.2"
+version = "2.0.3"
 description = "Computational Adjoint-Based Shape Optimization and Optimal Control Software"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
 authors = [
 	{name = "Sebastian Blauth"},
 	{email = "sebastian.blauth@itwm.fraunhofer.de"}
```

### Comparing `cashocs-2.0.2/tests/conftest.py` & `cashocs-2.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_cli.py` & `cashocs-2.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_config.py` & `cashocs-2.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_control_constraints.py` & `cashocs-2.0.3/tests/test_control_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_exceptions.py` & `cashocs-2.0.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_geometry.py` & `cashocs-2.0.3/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_log_level.py` & `cashocs-2.0.3/tests/test_log_level.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_nonlinear_solvers.py` & `cashocs-2.0.3/tests/test_nonlinear_solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_optimal_control.py` & `cashocs-2.0.3/tests/test_optimal_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_optimal_control_multiple.py` & `cashocs-2.0.3/tests/test_optimal_control_multiple.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_optimal_control_space_mapping.py` & `cashocs-2.0.3/tests/test_optimal_control_space_mapping.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_output.py` & `cashocs-2.0.3/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_p_laplacian.py` & `cashocs-2.0.3/tests/test_p_laplacian.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_pde_problems.py` & `cashocs-2.0.3/tests/test_pde_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_picard_iterations.py` & `cashocs-2.0.3/tests/test_picard_iterations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_remeshing.py` & `cashocs-2.0.3/tests/test_remeshing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_shape_constraints.py` & `cashocs-2.0.3/tests/test_shape_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_shape_optimization.py` & `cashocs-2.0.3/tests/test_shape_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_shape_optimization_space_mapping.py` & `cashocs-2.0.3/tests/test_shape_optimization_space_mapping.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_topology_optimization.py` & `cashocs-2.0.3/tests/test_topology_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.2/tests/test_utils.py` & `cashocs-2.0.3/tests/test_utils.py`

 * *Files identical despite different names*

