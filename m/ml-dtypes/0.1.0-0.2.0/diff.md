# Comparing `tmp/ml_dtypes-0.1.0.tar.gz` & `tmp/ml_dtypes-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_dtypes-0.1.0.tar", last modified: Tue Apr 11 20:49:30 2023, max compression
+gzip compressed data, was "ml_dtypes-0.2.0.tar", last modified: Tue Jun  6 14:42:34 2023, max compression
```

## Comparing `ml_dtypes-0.1.0.tar` & `ml_dtypes-0.2.0.tar`

### file list

```diff
@@ -1,238 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.150654 ml_dtypes-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/LICENSE.eigen
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15618 2023-04-11 20:49:30.150654 ml_dtypes-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.118654 ml_dtypes-0.1.0/ml_dtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_finfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.118654 ml_dtypes-0.1.0/ml_dtypes/_src/
--rw-r--r--   0 runner    (1001) docker     (123)    57117 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_src/custom_float.h
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_src/dtypes.cc
--rw-r--r--   0 runner    (1001) docker     (123)    52762 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_src/float8.h
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_src/numpy.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_src/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.118654 ml_dtypes-0.1.0/ml_dtypes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    29497 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/tests/custom_float_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/tests/finfo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/tests/metadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.118654 ml_dtypes-0.1.0/ml_dtypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15618 2023-04-11 20:49:30.000000 ml_dtypes-0.1.0/ml_dtypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-04-11 20:49:30.000000 ml_dtypes-0.1.0/ml_dtypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:49:30.000000 ml_dtypes-0.1.0/ml_dtypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-11 20:49:30.000000 ml_dtypes-0.1.0/ml_dtypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 20:49:30.000000 ml_dtypes-0.1.0/ml_dtypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:49:30.150654 ml_dtypes-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.114654 ml_dtypes-0.1.0/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.114654 ml_dtypes-0.1.0/third_party/eigen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.118654 ml_dtypes-0.1.0/third_party/eigen/Eigen/
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/Core
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.114654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.130654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (123)    41912 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/AssignEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    19246 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (123)    63843 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    37759 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (123)    32035 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    28937 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    49384 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/InternalHeaderCheck.h
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    61532 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    24419 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    23983 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    48620 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (123)    55121 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    16006 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (123)    38143 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)    35183 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.114654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.130654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    83727 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.134654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    47758 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)   110036 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h
--rw-r--r--   0 runner    (1001) docker     (123)    56830 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.134654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (123)    20546 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)   129018 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 runner    (1001) docker     (123)    28128 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h
--rw-r--r--   0 runner    (1001) docker     (123)    91478 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)   119359 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.134654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (123)    34597 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)    94749 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    58287 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.114654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    33649 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)   194432 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    51898 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    72921 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.142654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    21994 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.142654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    36916 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.142654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    31940 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    45622 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.146654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (123)   140899 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (123)    20980 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.150654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Assert.h
--rw-r--r--   0 runner    (1001) docker     (123)    26278 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (123)    48039 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    49577 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Memory.h
--rw-r--r--   0 runner    (1001) docker     (123)    20264 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Serializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)    35298 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.150654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    58948 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/InternalHeaderCheck.h
--rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.568742 ml_dtypes-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/LICENSE.eigen
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19727 2023-06-06 14:42:34.568742 ml_dtypes-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.540742 ml_dtypes-0.2.0/ml_dtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/_finfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/_iinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.544742 ml_dtypes-0.2.0/ml_dtypes/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/_src/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36054 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/_src/custom_float.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14016 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/_src/dtypes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    27008 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/_src/int4.h
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/_src/numpy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/_src/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/_src/ufuncs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.544742 ml_dtypes-0.2.0/ml_dtypes/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    51367 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/include/float8.h
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.544742 ml_dtypes-0.2.0/ml_dtypes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    29615 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/tests/custom_float_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/tests/finfo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/tests/iinfo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/tests/int4_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/ml_dtypes/tests/metadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.540742 ml_dtypes-0.2.0/ml_dtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19727 2023-06-06 14:42:34.000000 ml_dtypes-0.2.0/ml_dtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-06-06 14:42:34.000000 ml_dtypes-0.2.0/ml_dtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:42:34.000000 ml_dtypes-0.2.0/ml_dtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-06 14:42:34.000000 ml_dtypes-0.2.0/ml_dtypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-06 14:42:34.000000 ml_dtypes-0.2.0/ml_dtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:42:34.568742 ml_dtypes-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-06 14:42:20.000000 ml_dtypes-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.536742 ml_dtypes-0.2.0/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.536742 ml_dtypes-0.2.0/third_party/eigen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.544742 ml_dtypes-0.2.0/third_party/eigen/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/Core
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.540742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.552742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41912 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/AssignEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19246 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    63843 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37759 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32035 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28937 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49384 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/InternalHeaderCheck.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61532 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24419 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23983 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48620 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55121 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16006 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38143 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35183 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.540742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.552742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    83727 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.556742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47758 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)   110036 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56830 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.556742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (123)    20546 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)   129018 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28128 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    91478 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)   119359 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.556742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (123)    34597 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94749 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.556742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58287 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.540742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.556742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.560742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33649 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.560742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)   194432 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51898 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.560742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    72921 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.560742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.560742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21994 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.560742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36916 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.560742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31940 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45622 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.564742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (123)   140899 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20980 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.568742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Assert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26278 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48039 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49577 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20264 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Serializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35298 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:42:34.568742 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58948 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/InternalHeaderCheck.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-06 14:42:23.000000 ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h
```

### Comparing `ml_dtypes-0.1.0/LICENSE` & `ml_dtypes-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/LICENSE.eigen` & `ml_dtypes-0.2.0/LICENSE.eigen`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/PKG-INFO` & `ml_dtypes-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_dtypes
-Version: 0.1.0
+Version: 0.2.0
 Author-email: ml_dtypes authors <ml_dtypes@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,27 +220,28 @@
 
 # ml_dtypes
 
 [![Unittests](https://github.com/jax-ml/ml_dtypes/actions/workflows/test.yml/badge.svg)](https://github.com/jax-ml/ml_dtypes/actions/workflows/test.yml)
 [![Wheel Build](https://github.com/jax-ml/ml_dtypes/actions/workflows/wheels.yml/badge.svg)](https://github.com/jax-ml/ml_dtypes/actions/workflows/wheels.yml)
 [![PyPI version](https://badge.fury.io/py/ml_dtypes.svg)](https://badge.fury.io/py/ml_dtypes)
 
-*This is not an officially supported Google product.*
-
 `ml_dtypes` is a stand-alone implementation of several NumPy dtype extensions used in machine learning libraries, including:
 
 - [`bfloat16`](https://en.wikipedia.org/wiki/Bfloat16_floating-point_format):
   an alternative to the standard [`float16`](https://en.wikipedia.org/wiki/Half-precision_floating-point_format) format
 - `float8_*`: several experimental 8-bit floating point representations
   including:
-  * `float8_e4m3b11`
+  * `float8_e4m3b11fnuz`
   * `float8_e4m3fn`
   * `float8_e4m3fnuz`
   * `float8_e5m2`
   * `float8_e5m2fnuz`
+- `int4` and `uint4`: low precision integer types.
+
+See below for specifications of these number formats.
 
 ## Installation
 
 The `ml_dtypes` package is tested with Python versions 3.8-3.11, and can be installed
 with the following command:
 ```
 pip install ml_dtypes
@@ -270,13 +271,121 @@
 ```python
 >>> np.dtype('bfloat16')
 dtype(bfloat16)
 >>> np.dtype('float8_e5m2')
 dtype(float8_e5m2)
 ```
 
+## Specifications of implemented floating point formats
+
+### `bfloat16`
+
+A `bfloat16` number is a single-precision float truncated at 16 bits.
+
+Exponent: 8, Mantissa: 7, exponent bias: 127. IEEE 754, with NaN and inf.
+
+### `float8_e4m3b11fnuz`
+
+Exponent: 4, Mantissa: 3, bias: 11.
+
+Extended range: no inf, NaN represented by 0b1000'0000.
+
+### `float8_e4m3fn`
+
+Exponent: 4, Mantissa: 3, bias: 7.
+
+Extended range: no inf, NaN represented by 0bS111'1111.
+
+The `fn` suffix is for consistency with the corresponding LLVM/MLIR type, signaling this type is not consistent with IEEE-754.  The `f` indicates it is finite values only. The `n` indicates it includes NaNs, but only at the outer range.
+
+### `float8_e4m3fnuz`
+
+8-bit floating point with 3 bit mantissa.
+
+An 8-bit floating point type with 1 sign bit, 4 bits exponent and 3 bits mantissa. The suffix `fnuz` is consistent with LLVM/MLIR naming and is derived from the differences to IEEE floating point conventions. `F` is for "finite" (no infinities), `N` for with special NaN encoding, `UZ` for unsigned zero.
+
+This type has the following characteristics:
+ * bit encoding: S1E4M3 - `0bSEEEEMMM`
+ * exponent bias: 8
+ * infinities: Not supported
+ * NaNs: Supported with sign bit set to 1, exponent bits and mantissa bits set to all 0s - `0b10000000`
+ * denormals when exponent is 0
+
+### `float8_e5m2`
+
+Exponent: 5, Mantissa: 2, bias: 15. IEEE 754, with NaN and inf.
+
+### `float8_e5m2fnuz`
+
+8-bit floating point with 2 bit mantissa.
+
+An 8-bit floating point type with 1 sign bit, 5 bits exponent and 2 bits mantissa. The suffix `fnuz` is consistent with LLVM/MLIR naming and is derived from the differences to IEEE floating point conventions. `F` is for "finite" (no infinities), `N` for with special NaN encoding, `UZ` for unsigned zero.
+
+This type has the following characteristics:
+ * bit encoding: S1E5M2 - `0bSEEEEEMM`
+ * exponent bias: 16
+ * infinities: Not supported
+ * NaNs: Supported with sign bit set to 1, exponent bits and mantissa bits set to all 0s - `0b10000000`
+ * denormals when exponent is 0
+
+## `int4` and `uint4`
+
+4-bit integer types, where each element is represented unpacked (i.e., padded up
+to a byte in memory).
+
+NumPy does not support types smaller than a single byte. For example, the
+distance between adjacent elements in an array (`.strides`) is expressed in
+bytes. Relaxing this restriction would be a considerable engineering project.
+The `int4` and `uint4` types therefore use an unpacked representation, where
+each element of the array is padded up to a byte in memory. The lower four bits
+of each byte contain the representation of the number, whereas the upper four
+bits are ignored.
+
+## Quirks of low-precision Arithmetic
+
+If you're exploring the use of low-precision dtypes in your code, you should be
+careful to anticipate when the precision loss might lead to surprising results.
+One example is the behavior of aggregations like `sum`; consider this `bfloat16`
+summation in NumPy (run with version 1.24.2):
+```python
+>>> from ml_dtypes import bfloat16
+>>> import numpy as np
+>>> rng = np.random.default_rng(seed=0)
+>>> vals = rng.uniform(size=10000).astype(bfloat16)
+>>> vals.sum()
+256
+```
+The true sum should be close to 5000, but numpy returns exactly 256: this is
+because `bfloat16` does not have the precision to increment `256` by values less than
+`1`:
+```python
+>>> bfloat16(256) + bfloat16(1)
+256
+```
+After 256, the next representable value in bfloat16 is 258:
+```python
+>>> np.nextafter(bfloat16(256), bfloat16(np.inf))
+258
+```
+For better results you can specify that the accumulation should happen in a
+higher-precision type like `float32`:
+```python
+>>> vals.sum(dtype='float32').astype(bfloat16)
+4992
+```
+In contrast to NumPy, projects like [JAX](http://jax.readthedocs.io/) which support
+low-precision arithmetic more natively will often do these kinds of higher-precision
+accumulations automatically:
+```python
+>>> import jax.numpy as jnp
+>>> jnp.array(vals).sum()
+Array(4992, dtype=bfloat16)
+```
+
 ## License
 
+*This is not an officially supported Google product.*
+
 The `ml_dtypes` source code is licensed under the Apache 2.0 license
 (see [LICENSE](LICENSE)). Pre-compiled wheels are built with the
 [EIGEN](https://eigen.tuxfamily.org/) project, which is released under the
 MPL 2.0 license (see [LICENSE.eigen](LICENSE.eigen)).
```

### Comparing `ml_dtypes-0.1.0/ml_dtypes/_finfo.py` & `ml_dtypes-0.2.0/ml_dtypes/_finfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # limitations under the License.
 
 """Overload of numpy.finfo to handle dtypes defined in ml_dtypes."""
 
 from typing import Dict
 
 from ml_dtypes._custom_floats import bfloat16
-from ml_dtypes._custom_floats import float8_e4m3b11
+from ml_dtypes._custom_floats import float8_e4m3b11fnuz
 from ml_dtypes._custom_floats import float8_e4m3fn
 from ml_dtypes._custom_floats import float8_e4m3fnuz
 from ml_dtypes._custom_floats import float8_e5m2
 from ml_dtypes._custom_floats import float8_e5m2fnuz
 
 import numpy as np
 
 _bfloat16_dtype = np.dtype(bfloat16)
-_float8_e4m3b11_dtype = np.dtype(float8_e4m3b11)
+_float8_e4m3b11fnuz_dtype = np.dtype(float8_e4m3b11fnuz)
 _float8_e4m3fn_dtype = np.dtype(float8_e4m3fn)
 _float8_e4m3fnuz_dtype = np.dtype(float8_e4m3fnuz)
 _float8_e5m2_dtype = np.dtype(float8_e5m2)
 _float8_e5m2fnuz_dtype = np.dtype(float8_e5m2fnuz)
 
 
 class _Bfloat16MachArLike:
@@ -38,33 +38,33 @@
   def __init__(self):
     smallest_normal = float.fromhex("0x1p-126")
     self.smallest_normal = bfloat16(smallest_normal)
     smallest_subnormal = float.fromhex("0x1p-133")
     self.smallest_subnormal = bfloat16(smallest_subnormal)
 
 
-class _Float8E4m3B11MachArLike:
+class _Float8E4m3b11fnuzMachArLike:
 
   def __init__(self):
     smallest_normal = float.fromhex("0x1p-10")
-    self.smallest_normal = float8_e4m3b11(smallest_normal)
+    self.smallest_normal = float8_e4m3b11fnuz(smallest_normal)
     smallest_subnormal = float.fromhex("0x1p-13")
-    self.smallest_subnormal = float8_e4m3b11(smallest_subnormal)
+    self.smallest_subnormal = float8_e4m3b11fnuz(smallest_subnormal)
 
 
-class _Float8E4m3FnMachArLike:
+class _Float8E4m3fnMachArLike:
 
   def __init__(self):
     smallest_normal = float.fromhex("0x1p-6")
     self.smallest_normal = float8_e4m3fn(smallest_normal)
     smallest_subnormal = float.fromhex("0x1p-9")
     self.smallest_subnormal = float8_e4m3fn(smallest_subnormal)
 
 
-class _Float8E4m3FnuzMachArLike:
+class _Float8E4m3fnuzMachArLike:
 
   def __init__(self):
     smallest_normal = float.fromhex("0x1p-7")
     self.smallest_normal = float8_e4m3fnuz(smallest_normal)
     smallest_subnormal = float.fromhex("0x1p-10")
     self.smallest_subnormal = float8_e4m3fnuz(smallest_subnormal)
 
@@ -74,15 +74,15 @@
   def __init__(self):
     smallest_normal = float.fromhex("0x1p-14")
     self.smallest_normal = float8_e5m2(smallest_normal)
     smallest_subnormal = float.fromhex("0x1p-16")
     self.smallest_subnormal = float8_e5m2(smallest_subnormal)
 
 
-class _Float8E5m2FnuzMachArLike:
+class _Float8E5m2fnuzMachArLike:
 
   def __init__(self):
     smallest_normal = float.fromhex("0x1p-15")
     self.smallest_normal = float8_e5m2fnuz(smallest_normal)
     smallest_subnormal = float.fromhex("0x1p-17")
     self.smallest_subnormal = float8_e5m2fnuz(smallest_subnormal)
 
@@ -133,44 +133,44 @@
     obj._str_epsneg = float_to_str(epsneg)
     obj._str_eps = float_to_str(eps)
     obj._str_resolution = float_to_str(resolution)
     # pylint: enable=protected-access
     return obj
 
   @staticmethod
-  def _float8_e4m3b11_finfo():
+  def _float8_e4m3b11fnuz_finfo():
     def float_to_str(f):
       return "%6.2e" % float(f)
 
     tiny = float.fromhex("0x1p-10")
     resolution = 0.1
     eps = float.fromhex("0x1p-3")
     epsneg = float.fromhex("0x1p-4")
     max_ = float.fromhex("0x1.Ep4")
 
     obj = object.__new__(np.finfo)
-    obj.dtype = _float8_e4m3b11_dtype
+    obj.dtype = _float8_e4m3b11fnuz_dtype
     obj.bits = 8
-    obj.eps = float8_e4m3b11(eps)
-    obj.epsneg = float8_e4m3b11(epsneg)
+    obj.eps = float8_e4m3b11fnuz(eps)
+    obj.epsneg = float8_e4m3b11fnuz(epsneg)
     obj.machep = -3
     obj.negep = -4
-    obj.max = float8_e4m3b11(max_)
-    obj.min = float8_e4m3b11(-max_)
+    obj.max = float8_e4m3b11fnuz(max_)
+    obj.min = float8_e4m3b11fnuz(-max_)
     obj.nexp = 4
     obj.nmant = 3
     obj.iexp = obj.nexp
     obj.maxexp = 5
     obj.minexp = -10
     obj.precision = 1
-    obj.resolution = float8_e4m3b11(resolution)
+    obj.resolution = float8_e4m3b11fnuz(resolution)
     # pylint: disable=protected-access
-    obj._machar = _Float8E4m3B11MachArLike()
+    obj._machar = _Float8E4m3b11fnuzMachArLike()
     if not hasattr(obj, "tiny"):
-      obj.tiny = float8_e4m3b11(tiny)
+      obj.tiny = float8_e4m3b11fnuz(tiny)
     if not hasattr(obj, "smallest_normal"):
       obj.smallest_normal = obj._machar.smallest_normal
     obj.smallest_subnormal = obj._machar.smallest_subnormal
 
     obj._str_tiny = float_to_str(tiny)
     obj._str_smallest_normal = float_to_str(tiny)
     obj._str_smallest_subnormal = float_to_str(obj.smallest_subnormal)
@@ -205,15 +205,15 @@
     obj.nmant = 3
     obj.iexp = obj.nexp
     obj.maxexp = 9
     obj.minexp = -6
     obj.precision = 1
     obj.resolution = float8_e4m3fn(resolution)
     # pylint: disable=protected-access
-    obj._machar = _Float8E4m3FnMachArLike()
+    obj._machar = _Float8E4m3fnMachArLike()
     if not hasattr(obj, "tiny"):
       obj.tiny = float8_e4m3fn(tiny)
     if not hasattr(obj, "smallest_normal"):
       obj.smallest_normal = obj._machar.smallest_normal
     obj.smallest_subnormal = obj._machar.smallest_subnormal
 
     obj._str_tiny = float_to_str(tiny)
@@ -250,15 +250,15 @@
     obj.nmant = 3
     obj.iexp = obj.nexp
     obj.maxexp = 8
     obj.minexp = -7
     obj.precision = 1
     obj.resolution = float8_e4m3fnuz(resolution)
     # pylint: disable=protected-access
-    obj._machar = _Float8E4m3FnuzMachArLike()
+    obj._machar = _Float8E4m3fnuzMachArLike()
     if not hasattr(obj, "tiny"):
       obj.tiny = float8_e4m3fnuz(tiny)
     if not hasattr(obj, "smallest_normal"):
       obj.smallest_normal = obj._machar.smallest_normal
     obj.smallest_subnormal = obj._machar.smallest_subnormal
 
     obj._str_tiny = float_to_str(tiny)
@@ -340,15 +340,15 @@
     obj.nmant = 2
     obj.iexp = obj.nexp
     obj.maxexp = 16
     obj.minexp = -15
     obj.precision = 1
     obj.resolution = float8_e5m2fnuz(resolution)
     # pylint: disable=protected-access
-    obj._machar = _Float8E5m2FnuzMachArLike()
+    obj._machar = _Float8E5m2fnuzMachArLike()
     if not hasattr(obj, "tiny"):
       obj.tiny = float8_e5m2fnuz(tiny)
     if not hasattr(obj, "smallest_normal"):
       obj.smallest_normal = obj._machar.smallest_normal
     obj.smallest_subnormal = obj._machar.smallest_subnormal
 
     obj._str_tiny = float_to_str(tiny)
@@ -368,20 +368,22 @@
         or dtype == _bfloat16_dtype
     ):
       if _bfloat16_dtype not in cls._finfo_cache:
         cls._finfo_cache[_bfloat16_dtype] = cls._bfloat16_finfo()
       return cls._finfo_cache[_bfloat16_dtype]
     if (
         isinstance(dtype, str)
-        and dtype == "float8_e4m3b11"
-        or dtype == _float8_e4m3b11_dtype
+        and dtype == "float8_e4m3b11fnuz"
+        or dtype == _float8_e4m3b11fnuz_dtype
     ):
-      if _float8_e4m3b11_dtype not in cls._finfo_cache:
-        cls._finfo_cache[_float8_e4m3b11_dtype] = cls._float8_e4m3b11_finfo()
-      return cls._finfo_cache[_float8_e4m3b11_dtype]
+      if _float8_e4m3b11fnuz_dtype not in cls._finfo_cache:
+        cls._finfo_cache[_float8_e4m3b11fnuz_dtype] = (
+            cls._float8_e4m3b11fnuz_finfo()
+        )
+      return cls._finfo_cache[_float8_e4m3b11fnuz_dtype]
     if (
         isinstance(dtype, str)
         and dtype == "float8_e4m3fn"
         or dtype == _float8_e4m3fn_dtype
     ):
       if _float8_e4m3fn_dtype not in cls._finfo_cache:
         cls._finfo_cache[_float8_e4m3fn_dtype] = cls._float8_e4m3fn_finfo()
```

### Comparing `ml_dtypes-0.1.0/ml_dtypes/_src/dtypes.cc` & `ml_dtypes-0.2.0/ml_dtypes/_src/dtypes.cc`

 * *Files 14% similar despite different names*

```diff
@@ -25,25 +25,28 @@
 #include <cmath>   // NOLINT
 #include <limits>  // NOLINT
 #include <locale>  // NOLINT
 
 // Place `<locale>` before <Python.h> to avoid a build failure in macOS.
 #include <Python.h>
 
+#include "Eigen/Core"
 #include "_src/custom_float.h"
-#include "_src/float8.h"
-#include "eigen/Eigen/Core"
+#include "_src/int4.h"
+#include "include/float8.h"
 
 namespace ml_dtypes {
 
 using bfloat16 = Eigen::bfloat16;
 
 template <>
-struct TypeDescriptor<bfloat16> : CustomFloatTypeDescriptor<bfloat16> {
+struct TypeDescriptor<bfloat16> : CustomFloatType<bfloat16> {
   typedef bfloat16 T;
+  static constexpr bool is_floating = true;
+  static constexpr bool is_integral = false;
   static constexpr const char* kTypeName = "bfloat16";
   static constexpr const char* kQualifiedTypeName = "ml_dtypes.bfloat16";
   static constexpr const char* kTpDoc = "bfloat16 floating-point values";
   // We must register bfloat16 with a kind other than "f", because numpy
   // considers two types with the same kind and size to be equal, but
   // float16 != bfloat16.
   // The downside of this is that NumPy scalar promotion does not work with
@@ -52,36 +55,41 @@
   // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
   // character is unique.
   static constexpr char kNpyDescrType = 'E';
   static constexpr char kNpyDescrByteorder = '=';
 };
 
 template <>
-struct TypeDescriptor<float8_e4m3b11>
-    : CustomFloatTypeDescriptor<float8_e4m3b11> {
-  typedef float8_e4m3b11 T;
-  static constexpr const char* kTypeName = "float8_e4m3b11";
-  static constexpr const char* kQualifiedTypeName = "ml_dtypes.float8_e4m3b11";
-  static constexpr const char* kTpDoc = "float8_e4m3b11 floating-point values";
-  // We must register float8_e4m3b11 with a kind other than "f", because numpy
-  // considers two types with the same kind and size to be equal, and we
+struct TypeDescriptor<float8_e4m3b11fnuz>
+    : CustomFloatType<float8_e4m3b11fnuz> {
+  typedef float8_e4m3b11fnuz T;
+  static constexpr bool is_floating = true;
+  static constexpr bool is_integral = false;
+  static constexpr const char* kTypeName = "float8_e4m3b11fnuz";
+  static constexpr const char* kQualifiedTypeName =
+      "ml_dtypes.float8_e4m3b11fnuz";
+  static constexpr const char* kTpDoc =
+      "float8_e4m3b11fnuz floating-point values";
+  // We must register float8_e4m3b11fnuz with a kind other than "f", because
+  // numpy considers two types with the same kind and size to be equal, and we
   // expect multiple 1 byte floating point types.
   // The downside of this is that NumPy scalar promotion does not work with
-  // float8_e4m3b11 values.
+  // float8_e4m3b11fnuz values.
   static constexpr char kNpyDescrKind = 'V';
   // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
   // character is unique.
   static constexpr char kNpyDescrType = 'L';
   static constexpr char kNpyDescrByteorder = '=';
 };
 
 template <>
-struct TypeDescriptor<float8_e4m3fn>
-    : CustomFloatTypeDescriptor<float8_e4m3fn> {
+struct TypeDescriptor<float8_e4m3fn> : CustomFloatType<float8_e4m3fn> {
   typedef float8_e4m3fn T;
+  static constexpr bool is_floating = true;
+  static constexpr bool is_integral = false;
   static constexpr const char* kTypeName = "float8_e4m3fn";
   static constexpr const char* kQualifiedTypeName = "ml_dtypes.float8_e4m3fn";
   static constexpr const char* kTpDoc = "float8_e4m3fn floating-point values";
   // We must register float8_e4m3fn with a unique kind, because numpy
   // considers two types with the same kind and size to be equal.
   // The downside of this is that NumPy scalar promotion does not work with
   // float8 values.  Using 'V' to mirror bfloat16 vs float16.
@@ -89,55 +97,89 @@
   // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
   // character is unique.
   static constexpr char kNpyDescrType = '4';
   static constexpr char kNpyDescrByteorder = '=';
 };
 
 template <>
-struct TypeDescriptor<float8_e4m3fnuz>
-    : CustomFloatTypeDescriptor<float8_e4m3fnuz> {
+struct TypeDescriptor<float8_e4m3fnuz> : CustomFloatType<float8_e4m3fnuz> {
   typedef float8_e4m3fnuz T;
+  static constexpr bool is_floating = true;
+  static constexpr bool is_integral = false;
   static constexpr const char* kTypeName = "float8_e4m3fnuz";
   static constexpr const char* kQualifiedTypeName = "ml_dtypes.float8_e4m3fnuz";
   static constexpr const char* kTpDoc = "float8_e4m3fnuz floating-point values";
   static constexpr char kNpyDescrKind = 'V';
   // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
   // character is unique.
   static constexpr char kNpyDescrType = 'G';
   static constexpr char kNpyDescrByteorder = '=';
 };
 
 template <>
-struct TypeDescriptor<float8_e5m2> : CustomFloatTypeDescriptor<float8_e5m2> {
+struct TypeDescriptor<float8_e5m2> : CustomFloatType<float8_e5m2> {
   typedef float8_e5m2 T;
+  static constexpr bool is_floating = true;
+  static constexpr bool is_integral = false;
   static constexpr const char* kTypeName = "float8_e5m2";
   static constexpr const char* kQualifiedTypeName = "ml_dtypes.float8_e5m2";
   static constexpr const char* kTpDoc = "float8_e5m2 floating-point values";
   // Treating e5m2 as the natural "float" type since it is IEEE-754 compliant.
   static constexpr char kNpyDescrKind = 'f';
   // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
   // character is unique.
   static constexpr char kNpyDescrType = '5';
   static constexpr char kNpyDescrByteorder = '=';
 };
 
 template <>
-struct TypeDescriptor<float8_e5m2fnuz>
-    : CustomFloatTypeDescriptor<float8_e5m2fnuz> {
+struct TypeDescriptor<float8_e5m2fnuz> : CustomFloatType<float8_e5m2fnuz> {
   typedef float8_e5m2fnuz T;
+  static constexpr bool is_floating = true;
+  static constexpr bool is_integral = false;
   static constexpr const char* kTypeName = "float8_e5m2fnuz";
   static constexpr const char* kQualifiedTypeName = "ml_dtypes.float8_e5m2fnuz";
   static constexpr const char* kTpDoc = "float8_e5m2fnuz floating-point values";
   static constexpr char kNpyDescrKind = 'V';
   // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
   // character is unique.
   static constexpr char kNpyDescrType = 'C';
   static constexpr char kNpyDescrByteorder = '=';
 };
 
+template <>
+struct TypeDescriptor<int4> : Int4TypeDescriptor<int4> {
+  typedef int4 T;
+  static constexpr bool is_floating = false;
+  static constexpr bool is_integral = true;
+  static constexpr const char* kTypeName = "int4";
+  static constexpr const char* kQualifiedTypeName = "ml_dtypes.int4";
+  static constexpr const char* kTpDoc = "int4 integer values";
+  static constexpr char kNpyDescrKind = 'V';
+  // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
+  // character is unique.
+  static constexpr char kNpyDescrType = 'a';
+  static constexpr char kNpyDescrByteorder = '=';
+};
+
+template <>
+struct TypeDescriptor<uint4> : Int4TypeDescriptor<uint4> {
+  typedef uint4 T;
+  static constexpr bool is_floating = false;
+  static constexpr bool is_integral = true;
+  static constexpr const char* kTypeName = "uint4";
+  static constexpr const char* kQualifiedTypeName = "ml_dtypes.uint4";
+  static constexpr const char* kTpDoc = "uint4 integer values";
+  static constexpr char kNpyDescrKind = 'V';
+  // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
+  // character is unique.
+  static constexpr char kNpyDescrType = 'A';
+  static constexpr char kNpyDescrByteorder = '=';
+};
+
 namespace {
 
 // Performs a NumPy array cast from type 'From' to 'To' via float.
 template <typename From, typename To>
 void FloatPyCast(void* from_void, void* to_void, npy_intp n, void* fromarr,
                  void* toarr) {
   const auto* from = static_cast<From*>(from_void);
@@ -176,72 +218,80 @@
     return false;
   }
   Safe_PyObjectPtr numpy = make_safe(PyImport_Import(numpy_str.get()));
   if (!numpy) {
     return false;
   }
 
-  if (!RegisterNumpyDtype<bfloat16>(numpy.get())) {
+  if (!RegisterFloatDtype<bfloat16>(numpy.get())) {
     return false;
   }
-  bool float8_e4m3b11_already_registered;
-  if (!RegisterNumpyDtype<float8_e4m3b11>(numpy.get(),
-                                          &float8_e4m3b11_already_registered)) {
+  bool float8_e4m3b11fnuz_already_registered;
+  if (!RegisterFloatDtype<float8_e4m3b11fnuz>(
+          numpy.get(), &float8_e4m3b11fnuz_already_registered)) {
     return false;
   }
   bool float8_e4m3fn_already_registered;
-  if (!ml_dtypes::RegisterNumpyDtype<float8_e4m3fn>(
+  if (!ml_dtypes::RegisterFloatDtype<float8_e4m3fn>(
           numpy.get(), &float8_e4m3fn_already_registered)) {
     return false;
   }
   bool float8_e4m3fnuz_already_registered;
-  if (!ml_dtypes::RegisterNumpyDtype<float8_e4m3fnuz>(
+  if (!ml_dtypes::RegisterFloatDtype<float8_e4m3fnuz>(
           numpy.get(), &float8_e4m3fnuz_already_registered)) {
     return false;
   }
   bool float8_e5m2_already_registered;
-  if (!ml_dtypes::RegisterNumpyDtype<float8_e5m2>(
+  if (!ml_dtypes::RegisterFloatDtype<float8_e5m2>(
           numpy.get(), &float8_e5m2_already_registered)) {
     return false;
   }
   bool float8_e5m2fnuz_already_registered;
-  if (!ml_dtypes::RegisterNumpyDtype<float8_e5m2fnuz>(
+  if (!ml_dtypes::RegisterFloatDtype<float8_e5m2fnuz>(
           numpy.get(), &float8_e5m2fnuz_already_registered)) {
     return false;
   }
 
-  // Casts between bfloat16 and float8_e4m3b11. Only perform the cast if
-  // float8_e4m3b11 hasn't been previously registered, presumably by a different
-  // library. In this case, we assume the cast has also already been registered,
-  // and registering it again can cause segfaults due to accessing an
-  // uninitialized type descriptor in this library.
-  if (!float8_e4m3b11_already_registered &&
-      !RegisterCustomFloatCast<float8_e4m3b11, bfloat16>()) {
+  if (!ml_dtypes::RegisterInt4Dtype<int4>(numpy.get())) {
+    return false;
+  }
+
+  if (!ml_dtypes::RegisterInt4Dtype<uint4>(numpy.get())) {
+    return false;
+  }
+
+  // Casts between bfloat16 and float8_e4m3b11nuz. Only perform the cast if
+  // float8_e4m3b11nuz hasn't been previously registered, presumably by a
+  // different library. In this case, we assume the cast has also already been
+  // registered, and registering it again can cause segfaults due to accessing
+  // an uninitialized type descriptor in this library.
+  if (!float8_e4m3b11fnuz_already_registered &&
+      !RegisterCustomFloatCast<float8_e4m3b11fnuz, bfloat16>()) {
     return false;
   }
   if (!float8_e4m3fnuz_already_registered &&
       !float8_e5m2fnuz_already_registered &&
       !RegisterTwoWayCustomCast<float8_e4m3fnuz, float8_e5m2fnuz>()) {
     return false;
   }
   if (!float8_e4m3fn_already_registered && !float8_e5m2_already_registered &&
       !RegisterCustomFloatCast<float8_e4m3fn, float8_e5m2>()) {
     return false;
   }
   bool success = true;
   // Continue trying to register casts, just in case some types are not
-  // registered (i.e. float8_e4m3b11)
-  success &= RegisterTwoWayCustomCast<float8_e4m3b11, float8_e4m3fn>();
-  success &= RegisterTwoWayCustomCast<float8_e4m3b11, float8_e5m2>();
+  // registered (i.e. float8_e4m3b11fnuz)
+  success &= RegisterTwoWayCustomCast<float8_e4m3b11fnuz, float8_e4m3fn>();
+  success &= RegisterTwoWayCustomCast<float8_e4m3b11fnuz, float8_e5m2>();
   success &= RegisterTwoWayCustomCast<bfloat16, float8_e4m3fn>();
   success &= RegisterTwoWayCustomCast<bfloat16, float8_e5m2>();
   success &= RegisterTwoWayCustomCast<float8_e4m3fnuz, bfloat16>();
   success &= RegisterTwoWayCustomCast<float8_e5m2fnuz, bfloat16>();
-  success &= RegisterTwoWayCustomCast<float8_e4m3fnuz, float8_e4m3b11>();
-  success &= RegisterTwoWayCustomCast<float8_e5m2fnuz, float8_e4m3b11>();
+  success &= RegisterTwoWayCustomCast<float8_e4m3fnuz, float8_e4m3b11fnuz>();
+  success &= RegisterTwoWayCustomCast<float8_e5m2fnuz, float8_e4m3b11fnuz>();
   success &= RegisterTwoWayCustomCast<float8_e4m3fnuz, float8_e4m3fn>();
   success &= RegisterTwoWayCustomCast<float8_e5m2fnuz, float8_e4m3fn>();
   success &= RegisterTwoWayCustomCast<float8_e4m3fnuz, float8_e5m2>();
   success &= RegisterTwoWayCustomCast<float8_e5m2fnuz, float8_e5m2>();
   return success;
 }
 
@@ -266,18 +316,18 @@
   if (!Initialize()) {
     if (!PyErr_Occurred()) {
       PyErr_SetString(PyExc_RuntimeError, "cannot load _custom_floats module.");
     }
     return nullptr;
   }
 
-  if (PyObject_SetAttrString(m.get(), "float8_e4m3b11",
-                             reinterpret_cast<PyObject*>(
-                                 TypeDescriptor<float8_e4m3b11>::type_ptr)) <
-      0) {
+  if (PyObject_SetAttrString(
+          m.get(), "float8_e4m3b11fnuz",
+          reinterpret_cast<PyObject*>(
+              TypeDescriptor<float8_e4m3b11fnuz>::type_ptr)) < 0) {
     return nullptr;
   }
   if (PyObject_SetAttrString(m.get(), "float8_e4m3fn",
                              reinterpret_cast<PyObject*>(
                                  TypeDescriptor<float8_e4m3fn>::type_ptr)) <
       0) {
     return nullptr;
@@ -300,10 +350,20 @@
     return nullptr;
   }
   if (PyObject_SetAttrString(m.get(), "bfloat16",
                              reinterpret_cast<PyObject*>(
                                  TypeDescriptor<bfloat16>::type_ptr)) < 0) {
     return nullptr;
   }
+  if (PyObject_SetAttrString(
+          m.get(), "int4",
+          reinterpret_cast<PyObject*>(TypeDescriptor<int4>::type_ptr)) < 0) {
+    return nullptr;
+  }
+  if (PyObject_SetAttrString(
+          m.get(), "uint4",
+          reinterpret_cast<PyObject*>(TypeDescriptor<uint4>::type_ptr)) < 0) {
+    return nullptr;
+  }
   return m.release();
 }
 }  // namespace ml_dtypes
```

### Comparing `ml_dtypes-0.1.0/ml_dtypes/_src/float8.h` & `ml_dtypes-0.2.0/ml_dtypes/include/float8.h`

 * *Files 16% similar despite different names*

```diff
@@ -15,60 +15,93 @@
 
 #ifndef ML_DTYPES_FLOAT8_H_
 #define ML_DTYPES_FLOAT8_H_
 
 // 8-bit Floating Point Interchange Format, as described by
 //   https://arxiv.org/abs/2209.05433
 
+#include <algorithm>
 #include <cmath>
 #include <cstdint>
 #include <limits>
 #include <ostream>
-#include <version>
+#include <type_traits>
+#include <utility>
 
-#include "eigen/Eigen/Core"
+#ifdef __has_include
+# if __has_include(<version>)
+#   include <version>
+# endif
+#endif
 
-namespace ml_dtypes {
+#if (defined(__cpp_lib_bitops) && __cpp_lib_bitops >= 201907L)
+#include <bit>
+#endif
 
+#include "Eigen/Core"
+
+namespace ml_dtypes {
 namespace float8_internal {
 
 // Forward-declarations of classes.
 class float8_e4m3fn;
 class float8_e4m3fnuz;
-class float8_e4m3b11;
+class float8_e4m3b11fnuz;
 class float8_e5m2;
 class float8_e5m2fnuz;
 
 template <typename Derived>
 class float8_base {
  protected:
   // Constructor tag to allow constexpr construction from bit representation.
   struct ConstructFromRepTag {};
-
-  constexpr float8_base() : rep_(0) {}
   constexpr float8_base(uint8_t rep, ConstructFromRepTag) : rep_{rep} {}
 
  public:
+  constexpr float8_base() : rep_(0) {}
+
+  template <typename T,
+            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
+  explicit EIGEN_DEVICE_FUNC float8_base(T f)
+      : float8_base(ConvertFrom(static_cast<float>(f)).rep(),
+                    ConstructFromRepTag{}) {}
+  explicit EIGEN_DEVICE_FUNC float8_base(double f64)
+      : float8_base(ConvertFrom(f64).rep(), ConstructFromRepTag{}) {}
+  explicit EIGEN_DEVICE_FUNC float8_base(float f32)
+      : float8_base(ConvertFrom(f32).rep(), ConstructFromRepTag{}) {}
+  explicit EIGEN_DEVICE_FUNC float8_base(Eigen::bfloat16 bf16)
+      : float8_base(ConvertFrom(bf16).rep(), ConstructFromRepTag{}) {}
+  explicit EIGEN_DEVICE_FUNC float8_base(Eigen::half f16)
+      : float8_base(ConvertFrom(f16).rep(), ConstructFromRepTag{}) {}
+
   constexpr uint8_t rep() const { return rep_; }
 
-  constexpr Derived operator-() const {
-    return Derived(static_cast<uint8_t>(rep() ^ 0x80), ConstructFromRepTag{});
+  template <typename T,
+            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
+  explicit EIGEN_DEVICE_FUNC operator T() const {
+    return static_cast<T>(static_cast<float>(derived()));
   }
-
-  constexpr bool operator==(const Derived& other) const {
-    if (Eigen::numext::isnan(derived()) || Eigen::numext::isnan(other)) {
-      return false;
-    } else if ((rep() & 0x7F) == 0) {
-      return (other.rep() & 0x7F) == 0;
-    }
-    return rep() == other.rep();
+  explicit EIGEN_DEVICE_FUNC operator double() const {
+    return ConvertTo<double>(derived());
+  }
+  explicit EIGEN_DEVICE_FUNC operator float() const {
+    return ConvertTo<float>(derived());
+  }
+  explicit EIGEN_DEVICE_FUNC operator Eigen::bfloat16() const {
+    return ConvertTo<Eigen::bfloat16>(derived());
+  }
+  explicit EIGEN_DEVICE_FUNC operator Eigen::half() const {
+    return ConvertTo<Eigen::half>(derived());
+  }
+  explicit EIGEN_DEVICE_FUNC operator bool() const {
+    return (rep() & 0x7F) != 0;
   }
 
-  constexpr bool operator!=(const Derived& other) const {
-    return !(derived() == other);
+  constexpr Derived operator-() const {
+    return Derived(static_cast<uint8_t>(rep() ^ 0x80), ConstructFromRepTag{});
   }
 
   constexpr const Derived& derived() const {
     return *static_cast<const Derived*>(this);
   }
 
   constexpr Derived& derived() { return *static_cast<Derived*>(this); }
@@ -101,32 +134,41 @@
   }
 
   EIGEN_STRONG_INLINE EIGEN_DEVICE_FUNC Derived
   operator/(const Derived& other) const {
     return Derived{float{derived()} / float{other}};
   }
 
+  constexpr bool operator==(const Derived& other) const {
+    return Compare(derived(), other) == Ordering::kEquivalent;
+  }
+
+  constexpr bool operator!=(const Derived& other) const {
+    return Compare(derived(), other) != Ordering::kEquivalent;
+  }
+
   EIGEN_STRONG_INLINE EIGEN_DEVICE_FUNC bool operator<(
       const Derived& other) const {
-    return float{derived()} < float{other};
+    return Compare(derived(), other) == Ordering::kLess;
   }
 
   EIGEN_STRONG_INLINE EIGEN_DEVICE_FUNC bool operator<=(
       const Derived& other) const {
-    return float{derived()} <= float{other};
+    return Compare(derived(), other) <= Ordering::kEquivalent;
   }
 
   EIGEN_STRONG_INLINE EIGEN_DEVICE_FUNC bool operator>(
       const Derived& other) const {
-    return float{derived()} > float{other};
+    return Compare(derived(), other) == Ordering::kGreater;
   }
 
   EIGEN_STRONG_INLINE EIGEN_DEVICE_FUNC bool operator>=(
       const Derived& other) const {
-    return float{derived()} >= float{other};
+    Ordering ordering = Compare(derived(), other);
+    return ordering == Ordering::kGreater || ordering == Ordering::kEquivalent;
   }
 
   // Compound assignment.
   EIGEN_STRONG_INLINE EIGEN_DEVICE_FUNC Derived& operator+=(
       const Derived& other) {
     derived() = derived() + other;
     return derived();
@@ -147,142 +189,114 @@
   EIGEN_STRONG_INLINE EIGEN_DEVICE_FUNC Derived& operator/=(
       const Derived& other) {
     derived() = derived() / other;
     return derived();
   }
 
  private:
+  static EIGEN_STRONG_INLINE EIGEN_DEVICE_FUNC std::pair<uint8_t, uint8_t>
+  SignAndMagnitude(Derived x) {
+    const uint8_t x_abs_bits =
+        Eigen::numext::bit_cast<uint8_t>(Eigen::numext::abs(x));
+    const uint8_t x_bits = Eigen::numext::bit_cast<uint8_t>(x);
+    const uint8_t x_sign = x_bits ^ x_abs_bits;
+    return {x_sign, x_abs_bits};
+  }
+  static EIGEN_STRONG_INLINE EIGEN_DEVICE_FUNC int8_t
+  SignAndMagnitudeToTwosComplement(uint8_t sign, uint8_t magnitude) {
+    return magnitude ^ (static_cast<int8_t>(sign) < 0 ? -1 : 0);
+  }
+
+  enum Ordering : int8_t {
+    kLess = -1,
+    kEquivalent = 0,
+    kGreater = 1,
+    kUnordered = 2,
+  };
+
+  EIGEN_STRONG_INLINE EIGEN_DEVICE_FUNC friend Ordering Compare(
+      const Derived& lhs, const Derived& rhs) {
+    if (Eigen::numext::isnan(lhs) || Eigen::numext::isnan(rhs)) {
+      return Ordering::kUnordered;
+    }
+    auto [lhs_sign, lhs_mag] = SignAndMagnitude(lhs);
+    auto [rhs_sign, rhs_mag] = SignAndMagnitude(rhs);
+    if (lhs_mag == 0 && rhs_mag == 0) {
+      return Ordering::kEquivalent;
+    }
+    int8_t lhs_twos_complement =
+        SignAndMagnitudeToTwosComplement(lhs_sign, lhs_mag);
+    int8_t rhs_twos_complement =
+        SignAndMagnitudeToTwosComplement(rhs_sign, rhs_mag);
+    if (lhs_twos_complement < rhs_twos_complement) {
+      return Ordering::kLess;
+    }
+    if (lhs_twos_complement > rhs_twos_complement) {
+      return Ordering::kGreater;
+    }
+    return Ordering::kEquivalent;
+  }
+
   uint8_t rep_;
 };
 
 class float8_e4m3fn : public float8_base<float8_e4m3fn> {
   // Exponent: 4, Mantissa: 3, bias: 7.
   // Extended range: no inf, NaN represented by 0bS111'1111.
   // The "fn" suffix is for consistency with the corresponding LLVM/MLIR type,
   // signaling this type is not consistent with IEEE-754.  The "f" indicates
   // it is finite values only. The "n" indicates it includes NaNs, but only
   // at the outer range.
  private:
   using Base = float8_base<float8_e4m3fn>;
   friend class float8_base<float8_e4m3fn>;
-
-  constexpr float8_e4m3fn(uint8_t rep, ConstructFromRepTag)
-      : Base(rep, ConstructFromRepTag{}) {}
+  using Base::Base;
 
  public:
-  constexpr float8_e4m3fn() = default;
-
-  template <typename T,
-            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(T f)
-      : float8_e4m3fn(ConvertFrom(static_cast<float>(f))) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(double f64)
-      : float8_e4m3fn(ConvertFrom(f64)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(float f32)
-      : float8_e4m3fn(ConvertFrom(f32)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(Eigen::bfloat16 bf16)
-      : float8_e4m3fn(ConvertFrom(bf16)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(Eigen::half f16)
-      : float8_e4m3fn(ConvertFrom(f16)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3fn(const float8_e5m2& f8)
       : float8_e4m3fn(ConvertFrom(f8)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(const float8_e5m2fnuz& f8)
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(const float8_e4m3b11fnuz& f8)
       : float8_e4m3fn(ConvertFrom(f8)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(const float8_e4m3b11& f8)
-      : float8_e4m3fn(ConvertFrom(f8)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(const float8_e4m3fnuz& f8)
-      : float8_e4m3fn(ConvertFrom(f8)) {}
-
-  template <typename T,
-            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
-  explicit EIGEN_DEVICE_FUNC operator T() const {
-    return static_cast<T>(static_cast<float>(*this));
-  }
-  explicit EIGEN_DEVICE_FUNC operator double() const {
-    return ConvertTo<double>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator float() const {
-    return ConvertTo<float>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator Eigen::bfloat16() const {
-    return ConvertTo<Eigen::bfloat16>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator Eigen::half() const {
-    return ConvertTo<Eigen::half>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator bool() const {
-    return (rep() & 0x7F) != 0;
-  }
 };
 
-class float8_e4m3b11 : public float8_base<float8_e4m3b11> {
+class float8_e4m3b11fnuz : public float8_base<float8_e4m3b11fnuz> {
   // Exponent: 4, Mantissa: 3, bias: 11.
   // Extended range: no inf, NaN represented by 0b1000'0000.
  private:
-  using Base = float8_base<float8_e4m3b11>;
-  friend class float8_base<float8_e4m3b11>;
-
-  constexpr float8_e4m3b11(uint8_t rep, ConstructFromRepTag)
-      : Base(rep, ConstructFromRepTag{}) {}
+  using Base = float8_base<float8_e4m3b11fnuz>;
+  friend class float8_base<float8_e4m3b11fnuz>;
+  using Base::Base;
 
  public:
-  constexpr float8_e4m3b11() = default;
-
-  template <typename T,
-            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
-  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(T f)
-      : float8_e4m3b11(ConvertFrom(static_cast<float>(f))) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(double f64)
-      : float8_e4m3b11(ConvertFrom(f64)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(float f32)
-      : float8_e4m3b11(ConvertFrom(f32)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(Eigen::bfloat16 bf16)
-      : float8_e4m3b11(ConvertFrom(bf16)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(Eigen::half f16)
-      : float8_e4m3b11(ConvertFrom(f16)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(const float8_e5m2& f8)
-      : float8_e4m3b11(ConvertFrom(f8)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(const float8_e5m2fnuz& f8)
-      : float8_e4m3b11(ConvertFrom(f8)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(const float8_e4m3fn& f8)
-      : float8_e4m3b11(ConvertFrom(f8)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(const float8_e4m3fnuz& f8)
-      : float8_e4m3b11(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3b11fnuz(const float8_e5m2& f8)
+      : float8_e4m3b11fnuz(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3b11fnuz(const float8_e5m2fnuz& f8)
+      : float8_e4m3b11fnuz(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3b11fnuz(const float8_e4m3fn& f8)
+      : float8_e4m3b11fnuz(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3b11fnuz(const float8_e4m3fnuz& f8)
+      : float8_e4m3b11fnuz(ConvertFrom(f8)) {}
 
-  constexpr float8_e4m3b11 operator-() const {
+  constexpr float8_e4m3b11fnuz operator-() const {
     if ((rep() & 0x7f) == 0x00) {
-      return float8_e4m3b11(rep(), ConstructFromRepTag{});
+      return *this;
     }
     return Base::operator-();
   }
 
-  float8_e4m3b11 operator-(const float8_e4m3b11& other) const {
+  float8_e4m3b11fnuz operator-(const float8_e4m3b11fnuz& other) const {
     return Base::operator-(other);
   }
 
-  template <typename T,
-            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
-  explicit EIGEN_DEVICE_FUNC operator T() const {
-    return static_cast<T>(static_cast<float>(*this));
-  }
-  explicit EIGEN_DEVICE_FUNC operator double() const {
-    return ConvertTo<double>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator float() const {
-    return ConvertTo<float>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator Eigen::bfloat16() const {
-    return ConvertTo<Eigen::bfloat16>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator Eigen::half() const {
-    return ConvertTo<Eigen::half>(*this);
-  }
   explicit EIGEN_DEVICE_FUNC operator bool() const { return rep() != 0; }
 };
 
+// Legacy name used in XLA (TODO(jewillco): remove).
+using float8_e4m3b11 = float8_e4m3b11fnuz;
+
 class float8_e4m3fnuz : public float8_base<float8_e4m3fnuz> {
   // 8-bit floating point with 3 bit mantissa.
   //
   // An 8-bit floating point type with 1 sign bit, 4 bits exponent and 3 bits
   // mantissa. The suffix "fnuz" is consistent with LLVM/MLIR naming and is
   // derived from the differences to IEEE floating point conventions. `F` is
   // for "finite" (no infinities), `N` for with special NaN encoding, `UZ` for
@@ -294,127 +308,57 @@
   // * infinities: Not supported
   // * NaNs: Supported with sign bit set to 1, exponent bits and mantissa bits
   // set to all 0s - `0b10000000`
   // * denormals when exponent is 0
  private:
   using Base = float8_base<float8_e4m3fnuz>;
   friend class float8_base<float8_e4m3fnuz>;
-
-  constexpr float8_e4m3fnuz(uint8_t rep, ConstructFromRepTag)
-      : Base(rep, ConstructFromRepTag{}) {}
+  using Base::Base;
 
  public:
-  constexpr float8_e4m3fnuz() = default;
-
-  template <typename T,
-            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(T f)
-      : float8_e4m3fnuz(ConvertFrom(static_cast<float>(f))) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(double f64)
-      : float8_e4m3fnuz(ConvertFrom(f64)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(float f32)
-      : float8_e4m3fnuz(ConvertFrom(f32)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(Eigen::bfloat16 bf16)
-      : float8_e4m3fnuz(ConvertFrom(bf16)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(Eigen::half f16)
-      : float8_e4m3fnuz(ConvertFrom(f16)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(const float8_e5m2& f8)
       : float8_e4m3fnuz(ConvertFrom(f8)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(const float8_e5m2fnuz& f8)
       : float8_e4m3fnuz(ConvertFrom(f8)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(const float8_e4m3b11& f8)
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(const float8_e4m3b11fnuz& f8)
       : float8_e4m3fnuz(ConvertFrom(f8)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(const float8_e4m3fn& f8)
       : float8_e4m3fnuz(ConvertFrom(f8)) {}
 
   constexpr float8_e4m3fnuz operator-() const {
     if ((rep() & 0x7f) == 0x00) {
-      return float8_e4m3fnuz(rep(), ConstructFromRepTag{});
+      return *this;
     }
     return Base::operator-();
   }
 
   float8_e4m3fnuz operator-(const float8_e4m3fnuz& other) const {
     return Base::operator-(other);
   }
 
-  template <typename T,
-            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
-  explicit EIGEN_DEVICE_FUNC operator T() const {
-    return static_cast<T>(static_cast<float>(*this));
-  }
-  explicit EIGEN_DEVICE_FUNC operator double() const {
-    return ConvertTo<double>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator float() const {
-    return ConvertTo<float>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator Eigen::bfloat16() const {
-    return ConvertTo<Eigen::bfloat16>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator Eigen::half() const {
-    return ConvertTo<Eigen::half>(*this);
-  }
   explicit EIGEN_DEVICE_FUNC operator bool() const { return rep() != 0; }
 };
 
 class float8_e5m2 : public float8_base<float8_e5m2> {
   // Exponent: 5, Mantissa: 2, bias: 15.
   // IEEE 754.
  private:
   using Base = float8_base<float8_e5m2>;
   friend class float8_base<float8_e5m2>;
-
-  constexpr float8_e5m2(uint8_t rep, ConstructFromRepTag)
-      : Base(rep, ConstructFromRepTag{}) {}
+  using Base::Base;
 
  public:
-  constexpr float8_e5m2() = default;
-
-  template <typename T,
-            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
-  explicit EIGEN_DEVICE_FUNC float8_e5m2(T f)
-      : float8_e5m2(ConvertFrom(static_cast<float>(f))) {}
-  explicit EIGEN_DEVICE_FUNC float8_e5m2(double f64)
-      : float8_e5m2(ConvertFrom(f64)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e5m2(float f32)
-      : float8_e5m2(ConvertFrom(f32)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e5m2(Eigen::bfloat16 bf16)
-      : float8_e5m2(ConvertFrom(bf16)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e5m2(Eigen::half f16)
-      : float8_e5m2(ConvertFrom(f16)) {}
   explicit EIGEN_DEVICE_FUNC float8_e5m2(float8_e4m3fn f8)
       : float8_e5m2(ConvertFrom(f8)) {}
   explicit EIGEN_DEVICE_FUNC float8_e5m2(float8_e4m3fnuz f8)
       : float8_e5m2(ConvertFrom(f8)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e5m2(float8_e4m3b11 f8)
+  explicit EIGEN_DEVICE_FUNC float8_e5m2(float8_e4m3b11fnuz f8)
       : float8_e5m2(ConvertFrom(f8)) {}
   explicit EIGEN_DEVICE_FUNC float8_e5m2(float8_e5m2fnuz& f8)
       : float8_e5m2(ConvertFrom(f8)) {}
-
-  template <typename T,
-            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
-  explicit EIGEN_DEVICE_FUNC operator T() const {
-    return static_cast<T>(static_cast<float>(*this));
-  }
-  explicit EIGEN_DEVICE_FUNC operator double() const {
-    return ConvertTo<double>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator float() const {
-    return ConvertTo<float>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator Eigen::bfloat16() const {
-    return ConvertTo<Eigen::bfloat16>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator Eigen::half() const {
-    return ConvertTo<Eigen::half>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator bool() const {
-    return (rep() & 0x7F) != 0;
-  }
 };
 
 class float8_e5m2fnuz : public float8_base<float8_e5m2fnuz> {
   // 8-bit floating point with 2 bit mantissa.
   //
   // An 8-bit floating point type with 1 sign bit, 5 bits exponent and 2 bits
   // mantissa. The suffix "fnuz" is consistent with LLVM/MLIR naming and is
@@ -428,73 +372,101 @@
   // * infinities: Not supported
   // * NaNs: Supported with sign bit set to 1, exponent bits and mantissa bits
   // set to all 0s - `0b10000000`
   // * denormals when exponent is 0
  private:
   using Base = float8_base<float8_e5m2fnuz>;
   friend class float8_base<float8_e5m2fnuz>;
-
-  constexpr float8_e5m2fnuz(uint8_t rep, ConstructFromRepTag)
-      : Base(rep, ConstructFromRepTag{}) {}
+  using Base::Base;
 
  public:
-  constexpr float8_e5m2fnuz() = default;
-
-  template <typename T,
-            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
-  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(T f)
-      : float8_e5m2fnuz(ConvertFrom(static_cast<float>(f))) {}
-  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(double f64)
-      : float8_e5m2fnuz(ConvertFrom(f64)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(float f32)
-      : float8_e5m2fnuz(ConvertFrom(f32)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(Eigen::bfloat16 bf16)
-      : float8_e5m2fnuz(ConvertFrom(bf16)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(Eigen::half f16)
-      : float8_e5m2fnuz(ConvertFrom(f16)) {}
   explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(const float8_e5m2& f8)
       : float8_e5m2fnuz(ConvertFrom(f8)) {}
-  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(const float8_e4m3b11& f8)
+  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(const float8_e4m3b11fnuz& f8)
       : float8_e5m2fnuz(ConvertFrom(f8)) {}
   explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(const float8_e4m3fn& f8)
       : float8_e5m2fnuz(ConvertFrom(f8)) {}
   explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(const float8_e4m3fnuz& f8)
       : float8_e5m2fnuz(ConvertFrom(f8)) {}
 
   constexpr float8_e5m2fnuz operator-() const {
     if ((rep() & 0x7f) == 0x00) {
-      return float8_e5m2fnuz(rep(), ConstructFromRepTag{});
+      return *this;
     }
     return Base::operator-();
   }
 
   float8_e5m2fnuz operator-(const float8_e5m2fnuz& other) const {
     return Base::operator-(other);
   }
 
-  template <typename T,
-            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
-  explicit EIGEN_DEVICE_FUNC operator T() const {
-    return static_cast<T>(static_cast<float>(*this));
-  }
-  explicit EIGEN_DEVICE_FUNC operator double() const {
-    return ConvertTo<double>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator float() const {
-    return ConvertTo<float>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator Eigen::bfloat16() const {
-    return ConvertTo<Eigen::bfloat16>(*this);
-  }
-  explicit EIGEN_DEVICE_FUNC operator Eigen::half() const {
-    return ConvertTo<Eigen::half>(*this);
-  }
   explicit EIGEN_DEVICE_FUNC operator bool() const { return rep() != 0; }
 };
 
+constexpr double ConstexprAbs(double x) { return x < 0.0 ? -x : x; }
+
+constexpr double ConstexprCeil(double x) {
+  constexpr double kIntegerThreshold =
+      uint64_t{1} << (std::numeric_limits<double>::digits - 1);
+  // Too big or NaN inputs get returned unchanged.
+  if (!(ConstexprAbs(x) < kIntegerThreshold)) {
+    return x;
+  }
+  const double x_trunc = static_cast<double>(static_cast<int64_t>(x));
+  return x_trunc < x ? x_trunc + 1.0 : x_trunc;
+}
+
+constexpr double ConstexprFloor(double x) { return -ConstexprCeil(-x); }
+
+constexpr double kLog10Of2 = 0.3010299956639812;
+// C17 5.2.4.2.2p11:
+// "number of decimal digits, q, such that any floating-point number with q
+// decimal digits can be rounded into a floating-point number with p radix b
+// digits and back again without change to the q decimal digits"
+// floor((p - 1) * log10(2));
+constexpr int Digits10FromDigits(int digits) {
+  return static_cast<int>(ConstexprFloor((digits - 1) * kLog10Of2));
+}
+
+// C17 5.2.4.2.2p11:
+// "number of decimal digits, n, such that any floating-point number with p
+// radix b digits can be rounded to a floating-point number with n decimal
+// digits and back again without change to the value"
+// ceil(1 + p * log10(2));
+constexpr int MaxDigits10FromDigits(int digits) {
+  return static_cast<int>(ConstexprCeil(1.0 + (digits * kLog10Of2)));
+}
+
+// C17 5.2.4.2.2p11:
+// "minimum negative integer such that 10 raised to that power is in the range
+// of normalized floating-point numbers"
+// ceil(log10(2**(emin - 1))) == ceil((emin - 1) * log10(2));
+constexpr int MinExponent10FromMinExponent(int min_exponent) {
+  return static_cast<int>(ConstexprCeil((min_exponent - 1) * kLog10Of2));
+}
+
+// C17 5.2.4.2.2p11:
+// "maximum integer such that 10 raised to that power is in the range of
+// representable finite floating-point numbers"
+// floor(log10((1 - 2**-p) * 2**emax)) == floor(log10(1 - 2**-p) +
+// emax * log10(2))
+constexpr int MaxExponent10FromMaxExponentAndDigits(int max_exponent,
+                                                    int digits) {
+  // We only support digits in {3,4}. This table would grow if we wanted to
+  // handle more values.
+  constexpr double kLog10OfOnePredecessor[] = {
+      // log10(1 - 2**-3)
+      -0.057991946977686754,
+      // log10(1 - 2**-4)
+      -0.028028723600243537,
+  };
+  return static_cast<int>(ConstexprFloor(kLog10OfOnePredecessor[digits - 3] +
+                                         max_exponent * kLog10Of2));
+}
+
 // Structures for use in specializing std::numeric_limits.
 struct numeric_limits_float8_base {
   // NOLINTBEGIN: these names must match std::numeric_limits.
   static inline constexpr const bool is_specialized = true;
   static inline constexpr const bool is_signed = true;
   static inline constexpr const bool is_integer = false;
   static inline constexpr const bool is_exact = false;
@@ -509,133 +481,152 @@
   static inline constexpr const int radix = std::numeric_limits<float>::radix;
   static inline constexpr const bool traps = std::numeric_limits<float>::traps;
   static inline constexpr const bool tinyness_before =
       std::numeric_limits<float>::tinyness_before;
   // NOLINTEND
 };
 
-template <typename Derived>
-struct numeric_limits_float8 {
-  // NOLINTBEGIN: these names must match std::numeric_limits.
-  static inline constexpr const int digits = 0;
-  static inline constexpr const int digits10 = 0;
-  static inline constexpr const int max_digits10 = 0;
-  static inline constexpr const int min_exponent = 0;
-  static inline constexpr const int min_exponent10 = 0;
-  static inline constexpr const int max_exponent = 0;
-  static inline constexpr const int max_exponent10 = 0;
-  static inline constexpr const bool is_iec559 = false;
-  static inline constexpr const bool has_infinity = false;
-  static inline constexpr const bool has_signaling_NaN = false;
-  // NOLINTEND
-};
+struct numeric_limits_float8_e4m3fn : public numeric_limits_float8_base {
+ private:
+  static inline constexpr const int kExponentBias = 7;
+  static inline constexpr const int kMantissaBits = 3;
 
-template <>
-struct numeric_limits_float8<float8_e4m3fn>
-    : public numeric_limits_float8_base {
+ public:
   // NOLINTBEGIN: these names must match std::numeric_limits.
-  static inline constexpr const int digits = 4;
-  static inline constexpr const int digits10 = 0;      // floor(3 * log10(2));
-  static inline constexpr const int max_digits10 = 3;  // ceil(4 * log10(2) + 1)
-  static inline constexpr const int min_exponent = -5;
-  static inline constexpr const int min_exponent10 = -1;
-  static inline constexpr const int max_exponent = 9;  // Extended format.
-  static inline constexpr const int max_exponent10 = 2;
+  static inline constexpr const int digits = kMantissaBits + 1;
+  static inline constexpr const int digits10 = Digits10FromDigits(digits);
+  static inline constexpr const int max_digits10 =
+      MaxDigits10FromDigits(digits);
+  static inline constexpr const int min_exponent = (1 - kExponentBias) + 1;
+  static inline constexpr const int min_exponent10 =
+      MinExponent10FromMinExponent(min_exponent);
+  static inline constexpr const int max_exponent =
+      (0b1111 - 7) + 1;  // Extended format.
+  static inline constexpr const int max_exponent10 =
+      MaxExponent10FromMaxExponentAndDigits(max_exponent, digits);
   static inline constexpr const bool is_iec559 = false;
   static inline constexpr const bool has_infinity = false;
   static inline constexpr const bool has_signaling_NaN = false;
   // NOLINTEND
 
-  static constexpr float8_e4m3fn min() { return float8_e4m3fn::FromRep(0x08); }
+  // 1.0 * 2^(0b0001 - 7) = 1.0 * 2^-6 = 0.015625
+  static constexpr float8_e4m3fn min() {
+    return float8_e4m3fn::FromRep(0b0'0001 << kMantissaBits);
+  }
+  // -(1 + 0b110 * 2^-3) * 2^(0b1111 - 7) = -1.75 * 2^8 = 448
   static constexpr float8_e4m3fn lowest() {
-    return float8_e4m3fn::FromRep(0xFE);
+    return float8_e4m3fn::FromRep(0b1'1111'110);
   }
-  static constexpr float8_e4m3fn max() { return float8_e4m3fn::FromRep(0x7E); }
+  // (1 + 0b110 * 2^-3) * 2**(0b1111 - 7) = 1.75 * 2^8 = 448
+  static constexpr float8_e4m3fn max() {
+    return float8_e4m3fn::FromRep(0b0'1111'110);
+  }
+  // 1.0 * 2^-3 = 0.125
   static constexpr float8_e4m3fn epsilon() {
-    return float8_e4m3fn::FromRep(0x20);
+    return float8_e4m3fn::FromRep((-kMantissaBits + kExponentBias)
+                                  << kMantissaBits);
   }
+  // 1.0 * 2^-1 = 0.5
   static constexpr float8_e4m3fn round_error() {
-    return float8_e4m3fn::FromRep(0x30);
+    return float8_e4m3fn::FromRep((-1 + kExponentBias) << kMantissaBits);
   }
   static constexpr float8_e4m3fn infinity() {
-    return float8_e4m3fn::FromRep(0x7F);
-  }  // NaN.
+    return float8_e4m3fn::FromRep(0b0'1111'111);
+  }
+  // NaN.
   static constexpr float8_e4m3fn quiet_NaN() {
-    return float8_e4m3fn::FromRep(0x7F);
+    return float8_e4m3fn::FromRep(0b0'1111'111);
   }
   static constexpr float8_e4m3fn signaling_NaN() {
-    return float8_e4m3fn::FromRep(0x7F);
+    return float8_e4m3fn::FromRep(0b0'1111'111);
   }
+  // 1.0 * 2^(-7 - 3 + 1) = 1.0 * 2^-9 = 0.001953125
   static constexpr float8_e4m3fn denorm_min() {
-    return float8_e4m3fn::FromRep(0x01);
+    return float8_e4m3fn::FromRep(0b0'0000'001);
   }
 };
 
-template <>
-struct numeric_limits_float8<float8_e4m3b11>
-    : public numeric_limits_float8_base {
+struct numeric_limits_float8_e4m3b11fnuz : public numeric_limits_float8_base {
+ private:
+  static inline constexpr const int kExponentBias = 11;
+  static inline constexpr const int kMantissaBits = 3;
+
+ public:
   // NOLINTBEGIN: these names must match std::numeric_limits.
-  static inline constexpr const int digits = 4;
-  static inline constexpr const int digits10 = 0;      // floor(3 * log10(2));
-  static inline constexpr const int max_digits10 = 3;  // ceil(4 * log10(2) + 1)
-  static inline constexpr const int min_exponent = (1 - 11) + 1;
-  static inline constexpr const int min_exponent10 = -2;
+  static inline constexpr const int digits = kMantissaBits + 1;
+  static inline constexpr const int digits10 = Digits10FromDigits(digits);
+  static inline constexpr const int max_digits10 =
+      MaxDigits10FromDigits(digits);
+  static inline constexpr const int min_exponent = (1 - kExponentBias) + 1;
+  static inline constexpr const int min_exponent10 =
+      MinExponent10FromMinExponent(min_exponent);
   static inline constexpr const int max_exponent =
-      (0b1111 - 11) + 1;  // Extended format.
-  static inline constexpr const int max_exponent10 = 1;
+      (0b1111 - kExponentBias) + 1;  // Extended format.
+  static inline constexpr const int max_exponent10 =
+      MaxExponent10FromMaxExponentAndDigits(max_exponent, digits);
   static inline constexpr const bool is_iec559 = false;
   static inline constexpr const bool has_infinity = false;
   static inline constexpr const bool has_signaling_NaN = false;
   // NOLINTEND
 
-  static constexpr float8_e4m3b11 min() {
-    return float8_e4m3b11::FromRep(0x08);
+  // 1.0 * 2^(0b0001 - 11) = 1.0 * 2^-10 = 0.0009765625
+  static constexpr float8_e4m3b11fnuz min() {
+    return float8_e4m3b11fnuz::FromRep(1 << kMantissaBits);
   }
-  static constexpr float8_e4m3b11 lowest() {
-    return float8_e4m3b11::FromRep(0xFF);
+  // -(1 + 0b111 * 2^-3) * 2^(0b1111 - 11) = -1.875 * 2^4 = -30
+  static constexpr float8_e4m3b11fnuz lowest() {
+    return float8_e4m3b11fnuz::FromRep(0b1'1111'111);
   }
-  static constexpr float8_e4m3b11 max() {
-    return float8_e4m3b11::FromRep(0x7F);
+  // (1 + 0b111 * 2^-3) * 2^(0b1111 - 11) = 1.875 * 2^4 = 30
+  static constexpr float8_e4m3b11fnuz max() {
+    return float8_e4m3b11fnuz::FromRep(0b0'1111'111);
   }
-  static constexpr float8_e4m3b11 epsilon() {
-    constexpr int kExponentBias = 11;
-    constexpr int kMantissaBits = 3;
-    return float8_e4m3b11::FromRep((kExponentBias - kMantissaBits)
-                                   << kMantissaBits);
-  }
-  static constexpr float8_e4m3b11 round_error() {
-    constexpr int kExponentBias = 11;
-    constexpr int kMantissaBits = 3;
-    return float8_e4m3b11::FromRep((kExponentBias - 1) << kMantissaBits);
+  // 1.0 * 2^-3 = 0.125
+  static constexpr float8_e4m3b11fnuz epsilon() {
+    return float8_e4m3b11fnuz::FromRep((-kMantissaBits + kExponentBias)
+                                       << kMantissaBits);
   }
-  static constexpr float8_e4m3b11 infinity() {
-    return float8_e4m3b11::FromRep(0x80);
-  }  // NaN.
-  static constexpr float8_e4m3b11 quiet_NaN() {
-    return float8_e4m3b11::FromRep(0x80);
+  // 1.0 * 2^-1 = 0.5
+  static constexpr float8_e4m3b11fnuz round_error() {
+    return float8_e4m3b11fnuz::FromRep((-1 + kExponentBias) << kMantissaBits);
+  }
+  static constexpr float8_e4m3b11fnuz infinity() {
+    return float8_e4m3b11fnuz::FromRep(0b1'0000'000);
   }
-  static constexpr float8_e4m3b11 signaling_NaN() {
-    return float8_e4m3b11::FromRep(0x80);
+  // NaN.
+  static constexpr float8_e4m3b11fnuz quiet_NaN() {
+    return float8_e4m3b11fnuz::FromRep(0b1'0000'000);
   }
-  static constexpr float8_e4m3b11 denorm_min() {
-    return float8_e4m3b11::FromRep(0x01);
+  static constexpr float8_e4m3b11fnuz signaling_NaN() {
+    return float8_e4m3b11fnuz::FromRep(0b1'0000'000);
+  }
+  // 1.0 * 2^(-11 - 3 + 1) = 1.0 * 2^-13 = 0.0001220703125
+  static constexpr float8_e4m3b11fnuz denorm_min() {
+    return float8_e4m3b11fnuz::FromRep(0b0'0000'001);
   }
 };
 
-template <>
-struct numeric_limits_float8<float8_e4m3fnuz>
-    : public numeric_limits_float8_base {
+struct numeric_limits_float8_e4m3fnuz : public numeric_limits_float8_base {
+ private:
+  static inline constexpr const int kExponentBias = 8;
+  static inline constexpr const int kMantissaBits = 3;
+
+ public:
   // NOLINTBEGIN: these names must match std::numeric_limits.
-  static inline constexpr const int digits = 4;
-  static inline constexpr const int digits10 = 0;      // floor(3 * log10(2));
-  static inline constexpr const int max_digits10 = 3;  // ceil(4 * log10(2) + 1)
-  static inline constexpr const int min_exponent = -6;
-  static inline constexpr const int min_exponent10 = -2;
-  static inline constexpr const int max_exponent = 7;
-  static inline constexpr const int max_exponent10 = 2;
+  static inline constexpr const int digits = kMantissaBits + 1;
+  static inline constexpr const int digits10 = Digits10FromDigits(digits);
+  static inline constexpr const int max_digits10 =
+      MaxDigits10FromDigits(digits);
+  static inline constexpr const int min_exponent = (1 - kExponentBias) + 1;
+  static inline constexpr const int min_exponent10 =
+      MinExponent10FromMinExponent(min_exponent);
+  static inline constexpr const int max_exponent =
+      (0b1111 - kExponentBias) + 1;  // Extended format.
+  static inline constexpr const int max_exponent10 =
+      MaxExponent10FromMaxExponentAndDigits(max_exponent, digits);
   static inline constexpr const bool is_iec559 = false;
   static inline constexpr const bool has_infinity = false;
   static inline constexpr const bool has_signaling_NaN = false;
   // NOLINTEND
 
   static constexpr float8_e4m3fnuz min() {
     return float8_e4m3fnuz::FromRep(0x08);
@@ -643,23 +634,19 @@
   static constexpr float8_e4m3fnuz lowest() {
     return float8_e4m3fnuz::FromRep(0xFF);
   }
   static constexpr float8_e4m3fnuz max() {
     return float8_e4m3fnuz::FromRep(0x7F);
   }
   static constexpr float8_e4m3fnuz epsilon() {
-    constexpr int kExponentBias = 8;
-    constexpr int kMantissaBits = 3;
-    return float8_e4m3fnuz::FromRep((kExponentBias - kMantissaBits)
+    return float8_e4m3fnuz::FromRep((-kMantissaBits + kExponentBias)
                                     << kMantissaBits);
   }
   static constexpr float8_e4m3fnuz round_error() {
-    constexpr int kExponentBias = 8;
-    constexpr int kMantissaBits = 3;
-    return float8_e4m3fnuz::FromRep((kExponentBias - 1) << kMantissaBits);
+    return float8_e4m3fnuz::FromRep((-1 + kExponentBias) << kMantissaBits);
   }
   static constexpr float8_e4m3fnuz infinity() {
     return float8_e4m3fnuz::FromRep(0x80);
   }  // NaN.
   static constexpr float8_e4m3fnuz quiet_NaN() {
     return float8_e4m3fnuz::FromRep(0x80);
   }
@@ -667,83 +654,116 @@
     return float8_e4m3fnuz::FromRep(0x80);
   }
   static constexpr float8_e4m3fnuz denorm_min() {
     return float8_e4m3fnuz::FromRep(0x01);
   }
 };
 
-template <>
-struct numeric_limits_float8<float8_e5m2> : public numeric_limits_float8_base {
+struct numeric_limits_float8_e5m2 : public numeric_limits_float8_base {
+ private:
+  static inline constexpr const int kExponentBias = 15;
+  static inline constexpr const int kMantissaBits = 2;
+
+ public:
   // NOLINTBEGIN: these names must match std::numeric_limits.
-  static inline constexpr const int digits = 3;
-  static inline constexpr const int digits10 = 0;      // floor(2 * log10(2))
-  static inline constexpr const int max_digits10 = 2;  // ceil(3 * log10(2) + 1)
-  static inline constexpr const int min_exponent = -13;
-  static inline constexpr const int min_exponent10 = -4;
-  static inline constexpr const int max_exponent = 16;
-  static inline constexpr const int max_exponent10 = 4;
+  static inline constexpr const int digits = kMantissaBits + 1;
+  static inline constexpr const int digits10 = Digits10FromDigits(digits);
+  static inline constexpr const int max_digits10 =
+      MaxDigits10FromDigits(digits);
+  static inline constexpr const int min_exponent = (1 - kExponentBias) + 1;
+  static inline constexpr const int min_exponent10 =
+      MinExponent10FromMinExponent(min_exponent);
+  static inline constexpr const int max_exponent = 0b11111 - kExponentBias;
+  static inline constexpr const int max_exponent10 =
+      MaxExponent10FromMaxExponentAndDigits(max_exponent, digits);
   static inline constexpr const bool is_iec559 = true;
   static inline constexpr const bool has_infinity = true;
   static inline constexpr const bool has_signaling_NaN = true;
   // NOLINTEND
 
-  static constexpr float8_e5m2 min() { return float8_e5m2::FromRep(0x04); }
-  static constexpr float8_e5m2 lowest() { return float8_e5m2::FromRep(0xFB); }
-  static constexpr float8_e5m2 max() { return float8_e5m2::FromRep(0x7B); }
-  static constexpr float8_e5m2 epsilon() { return float8_e5m2::FromRep(0x34); }
+  // 1.0 * 2^(0b00001 - 15) = 1.0 * 2^-14 = 0.00006103515625
+  static constexpr float8_e5m2 min() {
+    return float8_e5m2::FromRep(1 << kMantissaBits);
+  }
+  // -(1 + 0b11 * 2^-2) * 2^(0b11110 - 15) = -1.75 * 2^15 = -57344
+  static constexpr float8_e5m2 lowest() {
+    return float8_e5m2::FromRep(0b1'11110'11);
+  }
+  // (1 + 0b11 * 2^-2) * 2^(0b11110 - 15) = 1.75 * 2^15 = 57344
+  static constexpr float8_e5m2 max() {
+    return float8_e5m2::FromRep(0b0'11110'11);
+  }
+  // 1.0 * 2^-2 = 0.25
+  static constexpr float8_e5m2 epsilon() {
+    return float8_e5m2::FromRep((-kMantissaBits + kExponentBias)
+                                << kMantissaBits);
+  }
+  // 1.0 * 2^-1 = 0.5
   static constexpr float8_e5m2 round_error() {
-    return float8_e5m2::FromRep(0x38);
+    return float8_e5m2::FromRep((-1 + kExponentBias) << kMantissaBits);
+  }
+  static constexpr float8_e5m2 infinity() {
+    return float8_e5m2::FromRep(0b0'11111'00);
   }
-  static constexpr float8_e5m2 infinity() { return float8_e5m2::FromRep(0x7C); }
   static constexpr float8_e5m2 quiet_NaN() {
-    return float8_e5m2::FromRep(0x7F);
+    // IEEE 754-2019 6.2.1: "All binary NaN bit strings have the sign bit S set
+    // to 0 or 1 and all the bits of the biased exponent field E set to 1
+    // (see 3.4). A quiet NaN bit string should be encoded with the first bit
+    // (d1) of the trailing significand field T being 1."
+    return float8_e5m2::FromRep(0b0'11111'10);
   }
   static constexpr float8_e5m2 signaling_NaN() {
-    return float8_e5m2::FromRep(0x7D);
+    // IEEE 754-2019 6.2.1: "A signaling NaN bit string should be encoded with
+    // the first bit of the trailing significand field being 0."
+    return float8_e5m2::FromRep(0b0'11111'01);
   }
+  // 1.0 * 2^(-15 - 2 + 1) = 1.0 * 2^-16 = 0.0000152587890625
   static constexpr float8_e5m2 denorm_min() {
-    return float8_e5m2::FromRep(0x01);
+    return float8_e5m2::FromRep(0b0'00000'01);
   }
 };
 
-template <>
-struct numeric_limits_float8<float8_e5m2fnuz>
-    : public numeric_limits_float8_base {
+struct numeric_limits_float8_e5m2fnuz : public numeric_limits_float8_base {
+ private:
+  static inline constexpr const int kExponentBias = 16;
+  static inline constexpr const int kMantissaBits = 2;
+
+ public:
   // NOLINTBEGIN: these names must match std::numeric_limits.
-  static inline constexpr const int digits = 3;
-  static inline constexpr const int digits10 = 0;      // floor(2 * log10(2))
-  static inline constexpr const int max_digits10 = 2;  // ceil(3 * log10(2) + 1)
-  static inline constexpr const int min_exponent = -14;
-  static inline constexpr const int min_exponent10 = -4;
-  static inline constexpr const int max_exponent = 16;
-  static inline constexpr const int max_exponent10 = 4;
+  static inline constexpr const int digits = kMantissaBits + 1;
+  static inline constexpr const int digits10 = Digits10FromDigits(digits);
+  static inline constexpr const int max_digits10 =
+      MaxDigits10FromDigits(digits);
+  static inline constexpr const int min_exponent = (1 - kExponentBias) + 1;
+  static inline constexpr const int min_exponent10 =
+      MinExponent10FromMinExponent(min_exponent);
+  static inline constexpr const int max_exponent =
+      (0b11111 - kExponentBias) + 1;
+  static inline constexpr const int max_exponent10 =
+      MaxExponent10FromMaxExponentAndDigits(max_exponent, digits);
   static inline constexpr const bool is_iec559 = false;
   static inline constexpr const bool has_infinity = false;
   static inline constexpr const bool has_signaling_NaN = false;
   // NOLINTEND
 
   static constexpr float8_e5m2fnuz min() {
-    return float8_e5m2fnuz::FromRep(0x08);
+    return float8_e5m2fnuz::FromRep(0x04);
   }
   static constexpr float8_e5m2fnuz lowest() {
     return float8_e5m2fnuz::FromRep(0xFF);
   }
   static constexpr float8_e5m2fnuz max() {
     return float8_e5m2fnuz::FromRep(0x7F);
   }
   static constexpr float8_e5m2fnuz epsilon() {
-    constexpr int kExponentBias = 16;
-    constexpr int kMantissaBits = 2;
-    return float8_e5m2fnuz::FromRep((kExponentBias - kMantissaBits)
+    return float8_e5m2fnuz::FromRep((-kMantissaBits + kExponentBias)
                                     << kMantissaBits);
   }
   static constexpr float8_e5m2fnuz round_error() {
-    constexpr int kExponentBias = 16;
-    constexpr int kMantissaBits = 2;
-    return float8_e5m2fnuz::FromRep((kExponentBias - 1) << kMantissaBits);
+    return float8_e5m2fnuz::FromRep((-1 + kExponentBias) << kMantissaBits);
   }
   static constexpr float8_e5m2fnuz infinity() {
     return float8_e5m2fnuz::FromRep(0x80);
   }  // NaN.
   static constexpr float8_e5m2fnuz quiet_NaN() {
     return float8_e5m2fnuz::FromRep(0x80);
   }
@@ -758,156 +778,109 @@
 }  // namespace float8_internal
 }  // namespace ml_dtypes
 
 namespace std {
 // Standard-library overrides.  Note that these are picked up by Eigen as well.
 template <>
 struct numeric_limits<ml_dtypes::float8_internal::float8_e4m3fn>
-    : public ml_dtypes::float8_internal::numeric_limits_float8<
-          ml_dtypes::float8_internal::float8_e4m3fn> {};
+    : public ml_dtypes::float8_internal::numeric_limits_float8_e4m3fn {};
 
 template <>
-struct numeric_limits<ml_dtypes::float8_internal::float8_e4m3b11>
-    : public ml_dtypes::float8_internal::numeric_limits_float8<
-          ml_dtypes::float8_internal::float8_e4m3b11> {};
+struct numeric_limits<ml_dtypes::float8_internal::float8_e4m3b11fnuz>
+    : public ml_dtypes::float8_internal::numeric_limits_float8_e4m3b11fnuz {};
 
 template <>
 struct numeric_limits<ml_dtypes::float8_internal::float8_e4m3fnuz>
-    : public ml_dtypes::float8_internal::numeric_limits_float8<
-          ml_dtypes::float8_internal::float8_e4m3fnuz> {};
+    : public ml_dtypes::float8_internal::numeric_limits_float8_e4m3fnuz {};
 
 template <>
 struct numeric_limits<ml_dtypes::float8_internal::float8_e5m2>
-    : public ml_dtypes::float8_internal::numeric_limits_float8<
-          ml_dtypes::float8_internal::float8_e5m2> {};
+    : public ml_dtypes::float8_internal::numeric_limits_float8_e5m2 {};
 
 template <>
 struct numeric_limits<ml_dtypes::float8_internal::float8_e5m2fnuz>
-    : public ml_dtypes::float8_internal::numeric_limits_float8<
-          ml_dtypes::float8_internal::float8_e5m2fnuz> {};
+    : public ml_dtypes::float8_internal::numeric_limits_float8_e5m2fnuz {};
 }  // namespace std
 
 namespace ml_dtypes {
 namespace float8_internal {
 
 // Free-functions for use with ADL and in Eigen.
 constexpr inline float8_e4m3fn abs(const float8_e4m3fn& a) {
-  return float8_e4m3fn::FromRep(a.rep() & 0x7F);
+  return float8_e4m3fn::FromRep(a.rep() & 0b0'1111'111);
 }
 
-constexpr inline bool isnan(const float8_e4m3fn& a) {
-  return (a.rep() & 0x7F) == 0x7F;
+constexpr inline bool(isnan)(const float8_e4m3fn& a) {
+  return abs(a).rep() == std::numeric_limits<float8_e4m3fn>::quiet_NaN().rep();
 }
 
-constexpr inline bool isinf(const float8_e4m3fn& a) {
-  return false;  // No inf representation.
+constexpr inline float8_e4m3b11fnuz abs(const float8_e4m3b11fnuz& a) {
+  return (a.rep() & 0b0'1111'111) == 0
+             ? float8_e4m3b11fnuz::FromRep(a.rep())
+             : float8_e4m3b11fnuz::FromRep(a.rep() & 0b0'1111'111);
 }
 
-constexpr inline bool isfinite(const float8_e4m3fn& a) {
-  return !isnan(a) && !isinf(a);
-}
-
-constexpr inline float8_e4m3b11 abs(const float8_e4m3b11& a) {
-  return (a.rep() & 0x7F) == 0 ? float8_e4m3b11::FromRep(a.rep())
-                               : float8_e4m3b11::FromRep(a.rep() & 0x7F);
-}
-
-constexpr inline bool isnan(const float8_e4m3b11& a) { return a.rep() == 0x80; }
-
-constexpr inline bool isinf(const float8_e4m3b11& a) {
-  return false;  // No inf representation.
-}
-
-constexpr inline bool isfinite(const float8_e4m3b11& a) {
-  return !isnan(a) && !isinf(a);
+constexpr inline bool(isnan)(const float8_e4m3b11fnuz& a) {
+  return a.rep() == std::numeric_limits<float8_e4m3b11fnuz>::quiet_NaN().rep();
 }
 
 constexpr inline float8_e4m3fnuz abs(const float8_e4m3fnuz& a) {
   return (a.rep() & 0x7F) == 0 ? float8_e4m3fnuz::FromRep(a.rep())
                                : float8_e4m3fnuz::FromRep(a.rep() & 0x7F);
 }
 
-constexpr inline bool isnan(const float8_e4m3fnuz& a) {
-  return a.rep() == 0x80;
-}
-
-constexpr inline bool isinf(const float8_e4m3fnuz& a) {
-  return false;  // No inf representation.
-}
-
-constexpr inline bool isfinite(const float8_e4m3fnuz& a) {
-  return !isnan(a) && !isinf(a);
+constexpr inline bool(isnan)(const float8_e4m3fnuz& a) {
+  return abs(a).rep() ==
+         std::numeric_limits<float8_e4m3fnuz>::quiet_NaN().rep();
 }
 
 constexpr inline float8_e5m2 abs(const float8_e5m2& a) {
-  return float8_e5m2::FromRep(a.rep() & 0x7F);
+  return float8_e5m2::FromRep(a.rep() & 0b0'11111'11);
 }
 
-constexpr inline bool isnan(const float8_e5m2& a) {
-  return (a.rep() & 0x7F) > 0x7C;
-}
-
-constexpr inline bool isinf(const float8_e5m2& a) {
-  return (a.rep() & 0x7F) == 0x7C;
-}
-
-constexpr inline bool isfinite(const float8_e5m2& a) {
-  return !isnan(a) && !isinf(a);
+constexpr inline bool(isnan)(const float8_e5m2& a) {
+  return abs(a).rep() > std::numeric_limits<float8_e5m2>::infinity().rep();
 }
 
 constexpr inline float8_e5m2fnuz abs(const float8_e5m2fnuz& a) {
   return (a.rep() & 0x7F) == 0 ? float8_e5m2fnuz::FromRep(a.rep())
                                : float8_e5m2fnuz::FromRep(a.rep() & 0x7F);
 }
 
 constexpr inline bool isnan(const float8_e5m2fnuz& a) {
   return a.rep() == 0x80;
 }
 
-constexpr inline bool isinf(const float8_e5m2fnuz& a) {
-  return false;  // No inf representation.
+template <typename Float8>
+constexpr inline bool(isinf)(const float8_base<Float8>& a) {
+  return std::numeric_limits<Float8>::has_infinity
+             ? abs(a.derived()).rep() ==
+                   std::numeric_limits<Float8>::infinity().rep()
+             : false;  // No inf representation.
 }
 
-constexpr inline bool isfinite(const float8_e5m2fnuz& a) {
-  return !isnan(a) && !isinf(a);
+template <typename Float8>
+constexpr inline bool(isfinite)(const float8_base<Float8>& a) {
+  return !isnan(a.derived()) && !isinf(a.derived());
 }
 
 template <typename Float8>
 std::ostream& operator<<(std::ostream& os, const float8_base<Float8>& f8) {
   os << static_cast<float>(f8.derived());
   return os;
 }
 
 //==============================================================================
 // Inline conversion routines between float8 and other types.
 //==============================================================================
 
-// Helper struct for getting a bit representation provided a byte size.
+// Helper for getting a bit representation provided a byte size.
 template <int kNumBytes>
-struct GetUnsignedInteger;
-
-template <>
-struct GetUnsignedInteger<1> {
-  using type = uint8_t;
-};
-
-template <>
-struct GetUnsignedInteger<2> {
-  using type = uint16_t;
-};
-
-template <>
-struct GetUnsignedInteger<4> {
-  using type = uint32_t;
-};
-
-template <>
-struct GetUnsignedInteger<8> {
-  using type = uint64_t;
-};
+using GetUnsignedInteger =
+    typename Eigen::numext::get_integer_by_size<kNumBytes>::unsigned_type;
 
 // Converts between two floating-point types.
 template <typename From, typename To, bool kSaturate, bool kTruncate,
           typename EnableIf = void>
 struct ConvertImpl;
 
 // Convert to same type.  We need explicit specializations for all combinations
@@ -930,110 +903,44 @@
                    /*EnableIf=*/void> : public IdentityConversion<Scalar> {};
 template <typename Scalar>
 struct ConvertImpl<Scalar, Scalar, /*kSaturate=*/true, /*kTruncate=*/true,
                    /*EnableIf=*/void> : public IdentityConversion<Scalar> {};
 
 template <typename Float>
 struct TraitsBase {
-  using BitsType = typename GetUnsignedInteger<sizeof(Float)>::type;
+  using BitsType = GetUnsignedInteger<sizeof(Float)>;
   static constexpr int kBits = sizeof(Float) * CHAR_BIT;
   static constexpr int kMantissaBits = Eigen::NumTraits<Float>::digits() - 1;
   static constexpr int kExponentBits = kBits - kMantissaBits - 1;
   static constexpr BitsType kExponentMask = ((BitsType{1} << kExponentBits) - 1)
                                             << kMantissaBits;
   static constexpr BitsType kMantissaMask = (BitsType{1} << kMantissaBits) - 1;
+  static constexpr int kExponentBias = (1 << (kExponentBits - 1)) - 1;
 };
 
 template <typename Float>
-struct Traits : public TraitsBase<Float> {
-  using Base = TraitsBase<Float>;
-  static constexpr int kExponentBias = (1 << (Base::kExponentBits - 1)) - 1;
-  static EIGEN_DEVICE_FUNC Float ConstructFromSignAndBits(
-      typename Base::BitsType sign, typename Base::BitsType bits) {
-    return Eigen::numext::bit_cast<Float>(
-        static_cast<typename Base::BitsType>(bits | sign));
-  }
-};
+struct Traits : public TraitsBase<Float> {};
 
 template <>
-struct Traits<float8_e4m3b11> : public TraitsBase<float8_e4m3b11> {
-  using Base = TraitsBase<float8_e4m3b11>;
+struct Traits<float8_e4m3b11fnuz> : public TraitsBase<float8_e4m3b11fnuz> {
   static constexpr int kExponentBias = 11;
-  static EIGEN_DEVICE_FUNC float8_e4m3b11 ConstructFromSignAndBits(
-      typename Base::BitsType sign, typename Base::BitsType bits) {
-    // float8_e4m3b11 does not support signed zero, ignore the sign if we try to
-    // make one.
-    if (bits == 0) {
-      sign = 0;
-    }
-    return Eigen::numext::bit_cast<float8_e4m3b11>(
-        static_cast<typename Base::BitsType>(bits | sign));
-  }
 };
 
 template <>
 struct Traits<float8_e4m3fnuz> : public TraitsBase<float8_e4m3fnuz> {
   using Base = TraitsBase<float8_e4m3fnuz>;
-  static constexpr int kExponentBias = 8;
-  static EIGEN_DEVICE_FUNC float8_e4m3fnuz ConstructFromSignAndBits(
-      typename Base::BitsType sign, typename Base::BitsType bits) {
-    // float8_e4m3fnuz does not support signed zero, ignore the sign if we try
-    // to make one.
-    if (bits == 0) {
-      sign = 0;
-    }
-    return Eigen::numext::bit_cast<float8_e4m3fnuz>(
-        static_cast<typename Base::BitsType>(bits | sign));
-  }
+  static constexpr int kExponentBias = Base::kExponentBias + 1;
 };
 
 template <>
 struct Traits<float8_e5m2fnuz> : public TraitsBase<float8_e5m2fnuz> {
   using Base = TraitsBase<float8_e5m2fnuz>;
-  static constexpr int kExponentBias = 16;
-  static EIGEN_DEVICE_FUNC float8_e5m2fnuz ConstructFromSignAndBits(
-      typename Base::BitsType sign, typename Base::BitsType bits) {
-    // float8_e5m2fnuz does not support signed zero, ignore the sign if we try
-    // to make one.
-    if (bits == 0) {
-      sign = 0;
-    }
-    return Eigen::numext::bit_cast<float8_e5m2fnuz>(
-        static_cast<typename Base::BitsType>(bits | sign));
-  }
+  static constexpr int kExponentBias = Base::kExponentBias + 1;
 };
 
-// Shift bits in the appropriate directions and add the exponent offset
-// to convert between bit representations.  The input `in` must be a
-// positive normalized value.
-template <typename From, typename To,
-          typename FromBits = typename Traits<From>::BitsType,
-          typename ToBits = typename Traits<To>::BitsType>
-constexpr FromBits ToFromBits(ToBits in) {
-  using FromTraits = Traits<From>;
-  constexpr int kFromMantissaBits = FromTraits::kMantissaBits;
-  constexpr int kFromExponentBias = FromTraits::kExponentBias;
-
-  using ToTraits = Traits<To>;
-  constexpr int kToMantissaBits = ToTraits::kMantissaBits;
-  constexpr int kToExponentBias = ToTraits::kExponentBias;
-
-  constexpr int kExponentOffset = kFromExponentBias - kToExponentBias;
-  constexpr int kDigitShift = kFromMantissaBits - kToMantissaBits;
-
-  FromBits out = static_cast<FromBits>(in);
-  if constexpr (kDigitShift > 0) {
-    out <<= kDigitShift;
-  } else if constexpr (kDigitShift < 0) {
-    out >>= -kDigitShift;
-  }
-  out += static_cast<FromBits>(kExponentOffset) << kFromMantissaBits;
-  return out;
-}
-
 template <typename Bits>
 constexpr inline Bits RoundBitsToNearestEven(Bits bits, int roundoff) {
   // Round to nearest even by adding a bias term.
   // Consider a bit pattern
   //   FFF...FLRTT...T,
   // where bits RTT...T need to be rounded-off.  We add a bias term to the
   // bit pattern s.t. a carry is introduced to round up only if
@@ -1043,18 +950,17 @@
   Bits bias = roundoff == 0
                   ? 0
                   : ((bits >> roundoff) & 1) + (Bits{1} << (roundoff - 1)) - 1;
   return bits + bias;
 }
 
 #if (defined(__cpp_lib_bitops) && __cpp_lib_bitops >= 201907L)
-#include <bit>
 using countl_zero = std::countl_zero;
 #else
-static inline int countl_zero(uint64_t x) {
+static constexpr inline int countl_zero(uint64_t x) {
   int zeroes = 60;
   if (x >> 32) {
     zeroes -= 32;
     x >>= 32;
   }
   if (x >> 16) {
     zeroes -= 16;
@@ -1066,15 +972,15 @@
   }
   if (x >> 4) {
     zeroes -= 4;
     x >>= 4;
   }
   return "\4\3\2\2\1\1\1\1\0\0\0\0\0\0\0"[x] + zeroes;
 }
-static inline int countl_zero(uint32_t x) {
+static constexpr inline int countl_zero(uint32_t x) {
   int zeroes = 28;
   if (x >> 16) {
     zeroes -= 16;
     x >>= 16;
   }
   if (x >> 8) {
     zeroes -= 8;
@@ -1082,247 +988,268 @@
   }
   if (x >> 4) {
     zeroes -= 4;
     x >>= 4;
   }
   return "\4\3\2\2\1\1\1\1\0\0\0\0\0\0\0"[x] + zeroes;
 }
-static inline int countl_zero(uint16_t x) {
+static constexpr inline int countl_zero(uint16_t x) {
   int zeroes = 12;
   if (x >> 8) {
     zeroes -= 8;
     x >>= 8;
   }
   if (x >> 4) {
     zeroes -= 4;
     x >>= 4;
   }
   return "\4\3\2\2\1\1\1\1\0\0\0\0\0\0\0"[x] + zeroes;
 }
-static inline int countl_zero(uint8_t x) {
+static constexpr inline int countl_zero(uint8_t x) {
   int zeroes = 4;
   if (x >> 4) {
     zeroes -= 4;
     x >>= 4;
   }
   return "\4\3\2\2\1\1\1\1\0\0\0\0\0\0\0"[x] + zeroes;
 }
 #endif
 
 template <typename From, typename To, bool kSaturate, bool kTruncate>
 struct ConvertImpl<From, To, kSaturate, kTruncate,
                    std::enable_if_t<!std::is_same_v<From, To>>> {
   using FromTraits = Traits<From>;
-  using FromBits = typename GetUnsignedInteger<sizeof(From)>::type;
+  using FromBits = typename FromTraits::BitsType;
   static constexpr int kFromBits = FromTraits::kBits;
   static constexpr int kFromMantissaBits = FromTraits::kMantissaBits;
   static constexpr int kFromExponentBits = FromTraits::kExponentBits;
   static constexpr int kFromExponentBias = FromTraits::kExponentBias;
   static constexpr FromBits kFromExponentMask = FromTraits::kExponentMask;
 
   using ToTraits = Traits<To>;
-  using ToBits = typename GetUnsignedInteger<sizeof(To)>::type;
+  using ToBits = typename ToTraits::BitsType;
   static constexpr int kToBits = ToTraits::kBits;
   static constexpr int kToMantissaBits = ToTraits::kMantissaBits;
   static constexpr int kToExponentBits = ToTraits::kExponentBits;
   static constexpr int kToExponentBias = ToTraits::kExponentBias;
   static constexpr ToBits kToExponentMask = ToTraits::kExponentMask;
 
+  // `WideBits` is wide enough to accommodate the largest exponent and mantissa
+  // in either `From` or `To`.
+  static constexpr int kWideBits =
+      (std::max(kToMantissaBits, kFromMantissaBits)) +  // Max significand.
+      (std::max(kToExponentBits, kFromExponentBits));   // Max exponent.
+  static constexpr int kWideBytes = (kWideBits + (CHAR_BIT - 1)) / CHAR_BIT;
+  using WideBits = GetUnsignedInteger<kWideBytes>;
   static constexpr int kExponentOffset = kToExponentBias - kFromExponentBias;
   static constexpr int kDigitShift = kToMantissaBits - kFromMantissaBits;
-  static constexpr int kSignShift = kToBits - kFromBits;
 
   static EIGEN_DEVICE_FUNC inline To run(const From& from) {
     // Shift bits to destination type, without sign bit.
-    FromBits from_bits = Eigen::numext::bit_cast<FromBits>(from);
-    const FromBits from_sign =
-        from_bits ^ Eigen::numext::bit_cast<FromBits>(Eigen::numext::abs(from));
-    ToBits sign;
-    if constexpr (kSignShift >= 0) {
-      sign = ToBits{from_sign} << kSignShift;
-    } else if constexpr (kSignShift < 0) {
-      sign = static_cast<ToBits>(from_sign >> -kSignShift);
-    }
-    from_bits ^= from_sign;  // Zeros sign bit to obtain absolute value.
+    const bool from_sign_bit =
+        Eigen::numext::bit_cast<FromBits>(from) >> (kFromBits - 1);
+    const FromBits from_bits =
+        Eigen::numext::bit_cast<FromBits>(Eigen::numext::abs(from));
 
     // Special values, preserving sign.
     if (Eigen::numext::isinf(from)) {
-      return sign != 0 ? -Eigen::NumTraits<To>::infinity()
-                       : Eigen::NumTraits<To>::infinity();
+      return from_sign_bit ? -Eigen::NumTraits<To>::infinity()
+                           : Eigen::NumTraits<To>::infinity();
     }
     if (Eigen::numext::isnan(from)) {
-      return sign != 0 ? -Eigen::NumTraits<To>::quiet_NaN()
-                       : Eigen::NumTraits<To>::quiet_NaN();
+      return from_sign_bit ? -Eigen::NumTraits<To>::quiet_NaN()
+                           : Eigen::NumTraits<To>::quiet_NaN();
     }
     if (from_bits == 0) {
-      return ToTraits::ConstructFromSignAndBits(/*sign=*/sign, /*bits=*/0);
+      return from_sign_bit ? -To{} : To{};
     }
 
-    // Adjust mantissa.
-    FromBits rounded_from_bits = from_bits;
-    if constexpr (kDigitShift < 0) {
-      if constexpr (!kTruncate) {
-        rounded_from_bits = RoundBitsToNearestEven(from_bits, -kDigitShift);
-      }
-      // Zero-out tail bits.
-      rounded_from_bits &= ~((FromBits{1} << (-kDigitShift)) - 1);
-    }
+    const int biased_from_exponent = from_bits >> kFromMantissaBits;
 
-    if constexpr (kExponentOffset > 0) {
-      if ((from.rep() & kFromExponentMask) == 0) {
+    // `To` supports more exponents near zero which means that some subnormal
+    // values in `From` may become normal.
+    if constexpr (std::numeric_limits<To>::min_exponent <
+                  std::numeric_limits<From>::min_exponent) {
+      if (biased_from_exponent == 0) {
         // Subnormals.
-        ToBits bits = from_bits;
+        WideBits bits = from_bits;
 
-        // All subnormals become normalized when casting to a type with a larger
-        // number of exponent bits.  We do this by setting the normalized
-        // mantissa bits in the source type, shifting it up to the destination
-        // type, then inserting the exponent bits.
+        // Determine exponent in target type.
         const int normalization_factor =
             countl_zero(from_bits) - (kFromBits - kFromMantissaBits) + 1;
-        // Shift the mantissa to account for the number of leading zeros.
-        bits <<= normalization_factor + kDigitShift;
-        // Clear the hidden bit.
-        bits &= ~(ToBits{1} << kToMantissaBits);
-        // Insert the exponent bits.
-        bits |= static_cast<ToBits>(kExponentOffset - normalization_factor + 1)
-                << kToMantissaBits;
-        return ToTraits::ConstructFromSignAndBits(/*sign=*/sign, /*bits=*/bits);
-      }
-    } else if constexpr (kExponentOffset < 0) {
-      // Check for overflows.
+        const int biased_exponent = kExponentOffset - normalization_factor + 1;
+        if (biased_exponent <= 0) {
+          // Result is subnormal.  Adjust the subnormal bits to account for
+          // the difference in exponent bias.
+          if constexpr (kExponentOffset < sizeof(WideBits) * CHAR_BIT) {
+            bits <<= kExponentOffset;
+          }
+        } else {
+          // Result is normal. Shift the mantissa to account for the number of
+          // leading zero digits, and clear the hidden bit.
+          bits <<= normalization_factor;
+          bits &= ~(WideBits{1} << kFromMantissaBits);
+          // Insert the exponent bits.
+          bits |= static_cast<WideBits>(biased_exponent) << kFromMantissaBits;
+        }
 
-      // Shift up exponent and mantissa, add offset to adjust exponent to
-      // source type.
-      constexpr ToBits kToHighest = Eigen::NumTraits<To>::highest().rep();
-      constexpr FromBits kHighest = ToFromBits<From, To>(kToHighest);
-
-      if (rounded_from_bits > kHighest) {
-        ToBits bits =
-            kSaturate ? kToHighest : Eigen::NumTraits<To>::infinity().rep();
-        return ToTraits::ConstructFromSignAndBits(/*sign=*/sign, /*bits=*/bits);
+        // Truncate/round mantissa if necessary.
+        if constexpr (kDigitShift > 0) {
+          bits <<= kDigitShift;
+        } else {
+          if constexpr (!kTruncate) {
+            bits = RoundBitsToNearestEven(bits, -kDigitShift);
+          }
+          bits >>= -kDigitShift;
+        }
+        To to = Eigen::numext::bit_cast<To>(static_cast<ToBits>(bits));
+        return from_sign_bit ? -to : to;
       }
-
+    }
+    // `To` supports fewer exponents near zero which means that some values in
+    // `From` may become subnormal.
+    if constexpr (std::numeric_limits<To>::min_exponent >
+                  std::numeric_limits<From>::min_exponent) {
+      const int unbiased_exponent = biased_from_exponent - kFromExponentBias;
+      const int biased_to_exponent = unbiased_exponent + kToExponentBias;
       // Subnormals and zero.
-      constexpr FromBits kLowestNormal =
-          ToFromBits<From, To>(std::numeric_limits<To>::min().rep());
-      if (rounded_from_bits < kLowestNormal) {
+      if (biased_to_exponent <= 0) {
         // Round and shift mantissa down.
-        int exponent = ((from_bits >> kFromMantissaBits) - kFromExponentBias);
-        int exponent_shift = -kDigitShift - exponent - kToExponentBias + 1;
-
-        // Insert the implicit leading 1 bit on the mantissa.  This assumes
-        // the input is normalized.  If it is not, then the mantissa bits -
-        // including the implicit one - will be shifted to zero.
-        // NOTE: we need to round again from the original from_bits, otherwise
-        // the lower precision bits may already be lost.  There is an edge-case
-        // where rounding to a normalized value would normally round down,
-        // but for a subnormal, we need to round up.
-        rounded_from_bits = ((from_bits & FromTraits::kMantissaMask) |
-                             (FromBits{1} << kFromMantissaBits));
+        FromBits from_has_leading_one = (biased_from_exponent > 0 ? 1 : 0);
+        int exponent_shift =
+            -kDigitShift - biased_to_exponent + from_has_leading_one;
+        // Insert the implicit leading 1 bit on the mantissa for normalized
+        // inputs.
+        FromBits rounded_from_bits =
+            (from_bits & FromTraits::kMantissaMask) |
+            (from_has_leading_one << kFromMantissaBits);
         ToBits bits = 0;
         // To avoid UB, limit rounding and shifting to the full mantissa plus
         // leading 1.
         if (exponent_shift <= kFromMantissaBits + 1) {
           if constexpr (!kTruncate) {
+            // NOTE: we need to round again from the original from_bits,
+            // otherwise the lower precision bits may already be lost.  There is
+            // an edge-case where rounding to a normalized value would normally
+            // round down, but for a subnormal, we need to round up.
             rounded_from_bits =
                 RoundBitsToNearestEven(rounded_from_bits, exponent_shift);
           }
           bits = (rounded_from_bits >> exponent_shift);
         }
         // Insert sign and return.
-        return ToTraits::ConstructFromSignAndBits(/*sign=*/sign, /*bits=*/bits);
+        To to = Eigen::numext::bit_cast<To>(bits);
+        return from_sign_bit ? -to : to;
       }
     }
 
-    // Shift bits.
+    // Round the mantissa if it is shrinking.
+    WideBits rounded_from_bits = from_bits;
+    if constexpr (kDigitShift < 0) {
+      if constexpr (!kTruncate) {
+        rounded_from_bits = RoundBitsToNearestEven(from_bits, -kDigitShift);
+      }
+      // Zero-out tail bits.
+      rounded_from_bits &= ~((WideBits{1} << (-kDigitShift)) - 1);
+    }
+
+    // Re-bias the exponent.
+    rounded_from_bits += static_cast<WideBits>(kExponentOffset)
+                         << kFromMantissaBits;
+
     ToBits bits;
+    // Check for overflows by aligning the significands. We always align the
+    // narrower significand to the wider significand.
+    const WideBits kToHighestRep =
+        Eigen::numext::bit_cast<ToBits>(Eigen::NumTraits<To>::highest());
+    WideBits aligned_highest{kToHighestRep};
     if constexpr (kDigitShift < 0) {
+      aligned_highest <<= -kDigitShift;
+      // Shift down, all dropped bits should already be zero.
       bits = static_cast<ToBits>(rounded_from_bits >> -kDigitShift);
     } else if constexpr (kDigitShift >= 0) {
-      bits = ToBits{rounded_from_bits} << kDigitShift;
+      // Shift up, inserting zeros in the newly created digits.
+      rounded_from_bits <<= kDigitShift;
+      bits = ToBits{rounded_from_bits};
     }
-    // Increase exponent by offset difference.
-    bits += static_cast<ToBits>(kExponentOffset) << kToMantissaBits;
 
+    To to = Eigen::numext::bit_cast<To>(bits);
+    // `From` supports larger values than `To`, we may overflow.
+    if constexpr (std::make_pair(std::numeric_limits<To>::max_exponent,
+                                 std::numeric_limits<To>::digits) <
+                  std::make_pair(std::numeric_limits<From>::max_exponent,
+                                 std::numeric_limits<From>::digits)) {
+      if (rounded_from_bits > aligned_highest) {
+        // Overflowed values map to highest or infinity depending on kSaturate.
+        to = kSaturate ? Eigen::NumTraits<To>::highest()
+                       : Eigen::NumTraits<To>::infinity();
+      }
+    }
     // Insert sign bit.
-    return ToTraits::ConstructFromSignAndBits(/*sign=*/sign, /*bits=*/bits);
+    return from_sign_bit ? -to : to;
   }
 };
 
 // Saturation has no impact when casting e4m3 to e5m2.
 template <bool kTruncate>
 struct ConvertImpl<float8_e4m3fn, float8_e5m2, true, kTruncate> {
   static EIGEN_DEVICE_FUNC inline float8_e5m2 run(const float8_e4m3fn& from) {
     return ConvertImpl<float8_e4m3fn, float8_e5m2, false, kTruncate>::run(from);
   }
 };
 
-template <bool kTruncate>
-struct ConvertImpl<Eigen::half, float8_e5m2, kTruncate, false> {
+template <bool kSaturate, bool kTruncate>
+struct ConvertImpl<Eigen::half, float8_e5m2, kSaturate, kTruncate> {
   static EIGEN_DEVICE_FUNC inline float8_e5m2 run(const Eigen::half& from) {
     uint16_t from_bits = Eigen::numext::bit_cast<uint16_t>(from);
 
     // Special values (Inf or NaN).
     uint16_t abs_bits = from_bits & 0x7FFF;
     if (abs_bits == 0x7C00) {
       return float8_e5m2::FromRep(from_bits >> 8);
     } else if (abs_bits > 0x7C00) {
-      return float8_e5m2::FromRep((from_bits >> 8) | 0x01);
+      // IEEE 754-2019 6.2.1: "A quiet NaN bit string should be encoded with the
+      // first bit (d1) of the trailing significand field T being 1."
+      // IEEE 754-2019 6.2.3: "Conversion of a quiet NaN to a floating-point
+      // format of the same or a different radix that does not allow the payload
+      // to be preserved, shall return a quiet NaN [...]"
+      return float8_e5m2::FromRep((from_bits >> 8) | 0b0'00000'10);
     }
 
     if constexpr (!kTruncate) {
       from_bits = RoundBitsToNearestEven(from_bits, 8);
+      // Rounding can cause an overflow to infinity. Clamp to the largest finite
+      // value if saturation is requested.
+      if constexpr (kSaturate) {
+        const float8_e5m2 kHighest = Eigen::NumTraits<float8_e5m2>::highest();
+        if ((from_bits & 0x7F00) > static_cast<uint16_t>(kHighest.rep()) << 8) {
+          const bool from_sign_bit = from_bits >> 15;
+          return from_sign_bit ? -kHighest : kHighest;
+        }
+      }
     }
     return float8_e5m2::FromRep(from_bits >> 8);
   }
 };
 
-template <bool kTruncate, bool kSaturate>
-struct ConvertImpl<Eigen::half, float8_e5m2fnuz, kTruncate, kSaturate> {
-  static EIGEN_DEVICE_FUNC inline float8_e5m2fnuz run(const Eigen::half& from) {
-    // Cast via float because float8_e5m2fnuz and Eigen::half have overlapping
-    // subnormal range.
-    return ConvertImpl<float, float8_e5m2fnuz, kTruncate, kSaturate>::run(from);
-  }
-};
-
-template <bool kTruncate, bool kSaturate>
-struct ConvertImpl<float8_e5m2fnuz, Eigen::half, kTruncate, kSaturate> {
-  static EIGEN_DEVICE_FUNC inline Eigen::half run(const float8_e5m2fnuz& from) {
-    // Cast via float because float8_e5m2fnuz and Eigen::half have overlapping
-    // subnormal range.
-    return static_cast<Eigen::half>(
-        ConvertImpl<float8_e5m2fnuz, float, kTruncate, kSaturate>::run(from));
-  }
-};
-
-// Saturation has no impact when casting Eigen::half to e5m2.
-template <bool kTruncate>
-struct ConvertImpl<Eigen::half, float8_e5m2, /*kSaturate=*/true, kTruncate> {
-  static EIGEN_DEVICE_FUNC inline float8_e5m2 run(const Eigen::half& from) {
-    return ConvertImpl<Eigen::half, float8_e5m2, /*kSaturate=*/false,
-                       kTruncate>::run(from);
-  }
-};
-
 template <>
 struct ConvertImpl<float8_e5m2, Eigen::half, /*kSaturate=*/false,
                    /*kTruncate=*/false> {
   static EIGEN_DEVICE_FUNC inline Eigen::half run(const float8_e5m2& from) {
     return Eigen::numext::bit_cast<Eigen::half>(
         static_cast<uint16_t>(static_cast<uint16_t>(from.rep()) << 8));
   }
 };
 
-// Saturation and truncation have no impact when casting e5m2 to Eigen::half.
+// Direct casts of e5m2 to Eigen::half simply shifts bits over.
 template <bool kSaturate, bool kTruncate>
 struct ConvertImpl<float8_e5m2, Eigen::half, kSaturate, kTruncate> {
   static EIGEN_DEVICE_FUNC inline Eigen::half run(const float8_e5m2& from) {
-    return ConvertImpl<float8_e5m2, Eigen::half, /*kSaturate=*/false,
-                       /*kTruncate=*/false>::run(from);
+    return Eigen::numext::bit_cast<Eigen::half>(
+        static_cast<uint16_t>(static_cast<uint16_t>(from.rep()) << 8));
   }
 };
 
 template <typename Derived>
 template <bool kSaturate, bool kTruncate, typename From>
 EIGEN_DEVICE_FUNC Derived float8_base<Derived>::ConvertFrom(const From& from) {
   return ConvertImpl<From, Derived, kSaturate, kTruncate>::run(from);
@@ -1335,15 +1262,15 @@
 }
 
 }  // namespace float8_internal
 
 // Exported types.
 using float8_e4m3fn = float8_internal::float8_e4m3fn;
 using float8_e4m3fnuz = float8_internal::float8_e4m3fnuz;
-using float8_e4m3b11 = float8_internal::float8_e4m3b11;
+using float8_e4m3b11fnuz = float8_internal::float8_e4m3b11fnuz;
 using float8_e5m2 = float8_internal::float8_e5m2;
 using float8_e5m2fnuz = float8_internal::float8_e5m2fnuz;
 
 }  // namespace ml_dtypes
 
 // Eigen-specific overrides.
 namespace Eigen {
@@ -1381,16 +1308,16 @@
 template <>
 EIGEN_DEVICE_FUNC inline bool isinf_impl<ml_dtypes::float8_e4m3fn>(
     const ml_dtypes::float8_e4m3fn& x) {
   return ml_dtypes::float8_internal::isinf(x);
 }
 
 template <>
-EIGEN_DEVICE_FUNC inline bool isinf_impl<ml_dtypes::float8_e4m3b11>(
-    const ml_dtypes::float8_e4m3b11& x) {
+EIGEN_DEVICE_FUNC inline bool isinf_impl<ml_dtypes::float8_e4m3b11fnuz>(
+    const ml_dtypes::float8_e4m3b11fnuz& x) {
   return ml_dtypes::float8_internal::isinf(x);
 }
 
 template <>
 EIGEN_DEVICE_FUNC inline bool isinf_impl<ml_dtypes::float8_e4m3fnuz>(
     const ml_dtypes::float8_e4m3fnuz& x) {
   return ml_dtypes::float8_internal::isinf(x);
@@ -1411,16 +1338,16 @@
 template <>
 EIGEN_DEVICE_FUNC inline bool isnan_impl<ml_dtypes::float8_e4m3fn>(
     const ml_dtypes::float8_e4m3fn& x) {
   return ml_dtypes::float8_internal::isnan(x);
 }
 
 template <>
-EIGEN_DEVICE_FUNC inline bool isnan_impl<ml_dtypes::float8_e4m3b11>(
-    const ml_dtypes::float8_e4m3b11& x) {
+EIGEN_DEVICE_FUNC inline bool isnan_impl<ml_dtypes::float8_e4m3b11fnuz>(
+    const ml_dtypes::float8_e4m3b11fnuz& x) {
   return ml_dtypes::float8_internal::isnan(x);
 }
 
 template <>
 EIGEN_DEVICE_FUNC inline bool isnan_impl<ml_dtypes::float8_e4m3fnuz>(
     const ml_dtypes::float8_e4m3fnuz& x) {
   return ml_dtypes::float8_internal::isnan(x);
@@ -1441,16 +1368,16 @@
 template <>
 EIGEN_DEVICE_FUNC inline bool isfinite_impl<ml_dtypes::float8_e4m3fn>(
     const ml_dtypes::float8_e4m3fn& x) {
   return ml_dtypes::float8_internal::isfinite(x);
 }
 
 template <>
-EIGEN_DEVICE_FUNC inline bool isfinite_impl<ml_dtypes::float8_e4m3b11>(
-    const ml_dtypes::float8_e4m3b11& x) {
+EIGEN_DEVICE_FUNC inline bool isfinite_impl<ml_dtypes::float8_e4m3b11fnuz>(
+    const ml_dtypes::float8_e4m3b11fnuz& x) {
   return ml_dtypes::float8_internal::isfinite(x);
 }
 
 template <>
 EIGEN_DEVICE_FUNC inline bool isfinite_impl<ml_dtypes::float8_e4m3fnuz>(
     const ml_dtypes::float8_e4m3fnuz& x) {
   return ml_dtypes::float8_internal::isfinite(x);
```

### Comparing `ml_dtypes-0.1.0/ml_dtypes/_src/numpy.cc` & `ml_dtypes-0.2.0/ml_dtypes/_src/numpy.cc`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/ml_dtypes/_src/numpy.h` & `ml_dtypes-0.2.0/ml_dtypes/_src/numpy.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/ml_dtypes/tests/custom_float_test.py` & `ml_dtypes-0.2.0/ml_dtypes/tests/custom_float_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from absl.testing import parameterized
 
 import ml_dtypes
 
 import numpy as np
 
 bfloat16 = ml_dtypes.bfloat16
-float8_e4m3b11 = ml_dtypes.float8_e4m3b11
+float8_e4m3b11fnuz = ml_dtypes.float8_e4m3b11fnuz
 float8_e4m3fn = ml_dtypes.float8_e4m3fn
 float8_e4m3fnuz = ml_dtypes.float8_e4m3fnuz
 float8_e5m2 = ml_dtypes.float8_e5m2
 float8_e5m2fnuz = ml_dtypes.float8_e5m2fnuz
 
 
 @contextlib.contextmanager
@@ -98,15 +98,15 @@
   except (OverflowError, ValueError):
     pass
   return is_inf
 
 
 FLOAT_DTYPES = [
     bfloat16,
-    float8_e4m3b11,
+    float8_e4m3b11fnuz,
     float8_e4m3fn,
     float8_e4m3fnuz,
     float8_e5m2,
     float8_e5m2fnuz,
 ]
 
 # Values that should round trip exactly to float and back.
@@ -136,15 +136,15 @@
     ]
     for dtype in FLOAT_DTYPES
 }
 
 # Values that should round trip exactly to integer and back.
 INT_VALUES = {
     bfloat16: [0, 1, 2, 10, 34, 47, 128, 255, 256, 512],
-    float8_e4m3b11: [*range(16), *range(16, 30, 2)],
+    float8_e4m3b11fnuz: [*range(16), *range(16, 30, 2)],
     float8_e4m3fn: list(
         itertools.chain.from_iterable(
             range(1 << n, 2 << n, 1 << max(0, n - 3)) for n in range(9)
         )
     )[:-1],
     float8_e4m3fnuz: list(
         itertools.chain.from_iterable(
@@ -161,15 +161,15 @@
             range(1 << n, 2 << n, 1 << max(0, n - 2)) for n in range(16)
         )
     ),
 }
 
 BITS_TYPE = {
     bfloat16: np.uint16,
-    float8_e4m3b11: np.uint8,
+    float8_e4m3b11fnuz: np.uint8,
     float8_e4m3fn: np.uint8,
     float8_e4m3fnuz: np.uint8,
     float8_e5m2: np.uint8,
     float8_e5m2fnuz: np.uint8,
 }
 
 
@@ -655,14 +655,17 @@
         self.assertEqual(
             (float_type, d) in allowed_casts, np.can_cast(float_type, d)
         )
         self.assertEqual(
             (d, float_type) in allowed_casts, np.can_cast(d, float_type)
         )
 
+  @ignore_warning(
+      category=RuntimeWarning, message="invalid value encountered in cast"
+  )
   def testCasts(self, float_type):
     for dtype in [
         np.float16,
         np.float32,
         np.float64,
         np.longdouble,
         np.int8,
```

### Comparing `ml_dtypes-0.1.0/ml_dtypes/tests/finfo_test.py` & `ml_dtypes-0.2.0/ml_dtypes/tests/finfo_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 from absl.testing import absltest
 from absl.testing import parameterized
 import ml_dtypes
 import numpy as np
 
 ALL_DTYPES = [
     ml_dtypes.bfloat16,
-    ml_dtypes.float8_e4m3b11,
+    ml_dtypes.float8_e4m3b11fnuz,
     ml_dtypes.float8_e4m3fn,
     ml_dtypes.float8_e4m3fnuz,
     ml_dtypes.float8_e5m2,
     ml_dtypes.float8_e5m2fnuz,
 ]
 
 DTYPES_WITH_NO_INFINITY = [
-    ml_dtypes.float8_e4m3b11,
+    ml_dtypes.float8_e4m3b11fnuz,
     ml_dtypes.float8_e4m3fn,
     ml_dtypes.float8_e4m3fnuz,
     ml_dtypes.float8_e5m2fnuz,
 ]
 
 UINT_TYPES = {
     8: np.uint8,
```

### Comparing `ml_dtypes-0.1.0/ml_dtypes/tests/metadata_test.py` & `ml_dtypes-0.2.0/ml_dtypes/tests/metadata_test.py`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/ml_dtypes.egg-info/PKG-INFO` & `ml_dtypes-0.2.0/ml_dtypes.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-dtypes
-Version: 0.1.0
+Version: 0.2.0
 Author-email: ml_dtypes authors <ml_dtypes@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,27 +220,28 @@
 
 # ml_dtypes
 
 [![Unittests](https://github.com/jax-ml/ml_dtypes/actions/workflows/test.yml/badge.svg)](https://github.com/jax-ml/ml_dtypes/actions/workflows/test.yml)
 [![Wheel Build](https://github.com/jax-ml/ml_dtypes/actions/workflows/wheels.yml/badge.svg)](https://github.com/jax-ml/ml_dtypes/actions/workflows/wheels.yml)
 [![PyPI version](https://badge.fury.io/py/ml_dtypes.svg)](https://badge.fury.io/py/ml_dtypes)
 
-*This is not an officially supported Google product.*
-
 `ml_dtypes` is a stand-alone implementation of several NumPy dtype extensions used in machine learning libraries, including:
 
 - [`bfloat16`](https://en.wikipedia.org/wiki/Bfloat16_floating-point_format):
   an alternative to the standard [`float16`](https://en.wikipedia.org/wiki/Half-precision_floating-point_format) format
 - `float8_*`: several experimental 8-bit floating point representations
   including:
-  * `float8_e4m3b11`
+  * `float8_e4m3b11fnuz`
   * `float8_e4m3fn`
   * `float8_e4m3fnuz`
   * `float8_e5m2`
   * `float8_e5m2fnuz`
+- `int4` and `uint4`: low precision integer types.
+
+See below for specifications of these number formats.
 
 ## Installation
 
 The `ml_dtypes` package is tested with Python versions 3.8-3.11, and can be installed
 with the following command:
 ```
 pip install ml_dtypes
@@ -270,13 +271,121 @@
 ```python
 >>> np.dtype('bfloat16')
 dtype(bfloat16)
 >>> np.dtype('float8_e5m2')
 dtype(float8_e5m2)
 ```
 
+## Specifications of implemented floating point formats
+
+### `bfloat16`
+
+A `bfloat16` number is a single-precision float truncated at 16 bits.
+
+Exponent: 8, Mantissa: 7, exponent bias: 127. IEEE 754, with NaN and inf.
+
+### `float8_e4m3b11fnuz`
+
+Exponent: 4, Mantissa: 3, bias: 11.
+
+Extended range: no inf, NaN represented by 0b1000'0000.
+
+### `float8_e4m3fn`
+
+Exponent: 4, Mantissa: 3, bias: 7.
+
+Extended range: no inf, NaN represented by 0bS111'1111.
+
+The `fn` suffix is for consistency with the corresponding LLVM/MLIR type, signaling this type is not consistent with IEEE-754.  The `f` indicates it is finite values only. The `n` indicates it includes NaNs, but only at the outer range.
+
+### `float8_e4m3fnuz`
+
+8-bit floating point with 3 bit mantissa.
+
+An 8-bit floating point type with 1 sign bit, 4 bits exponent and 3 bits mantissa. The suffix `fnuz` is consistent with LLVM/MLIR naming and is derived from the differences to IEEE floating point conventions. `F` is for "finite" (no infinities), `N` for with special NaN encoding, `UZ` for unsigned zero.
+
+This type has the following characteristics:
+ * bit encoding: S1E4M3 - `0bSEEEEMMM`
+ * exponent bias: 8
+ * infinities: Not supported
+ * NaNs: Supported with sign bit set to 1, exponent bits and mantissa bits set to all 0s - `0b10000000`
+ * denormals when exponent is 0
+
+### `float8_e5m2`
+
+Exponent: 5, Mantissa: 2, bias: 15. IEEE 754, with NaN and inf.
+
+### `float8_e5m2fnuz`
+
+8-bit floating point with 2 bit mantissa.
+
+An 8-bit floating point type with 1 sign bit, 5 bits exponent and 2 bits mantissa. The suffix `fnuz` is consistent with LLVM/MLIR naming and is derived from the differences to IEEE floating point conventions. `F` is for "finite" (no infinities), `N` for with special NaN encoding, `UZ` for unsigned zero.
+
+This type has the following characteristics:
+ * bit encoding: S1E5M2 - `0bSEEEEEMM`
+ * exponent bias: 16
+ * infinities: Not supported
+ * NaNs: Supported with sign bit set to 1, exponent bits and mantissa bits set to all 0s - `0b10000000`
+ * denormals when exponent is 0
+
+## `int4` and `uint4`
+
+4-bit integer types, where each element is represented unpacked (i.e., padded up
+to a byte in memory).
+
+NumPy does not support types smaller than a single byte. For example, the
+distance between adjacent elements in an array (`.strides`) is expressed in
+bytes. Relaxing this restriction would be a considerable engineering project.
+The `int4` and `uint4` types therefore use an unpacked representation, where
+each element of the array is padded up to a byte in memory. The lower four bits
+of each byte contain the representation of the number, whereas the upper four
+bits are ignored.
+
+## Quirks of low-precision Arithmetic
+
+If you're exploring the use of low-precision dtypes in your code, you should be
+careful to anticipate when the precision loss might lead to surprising results.
+One example is the behavior of aggregations like `sum`; consider this `bfloat16`
+summation in NumPy (run with version 1.24.2):
+```python
+>>> from ml_dtypes import bfloat16
+>>> import numpy as np
+>>> rng = np.random.default_rng(seed=0)
+>>> vals = rng.uniform(size=10000).astype(bfloat16)
+>>> vals.sum()
+256
+```
+The true sum should be close to 5000, but numpy returns exactly 256: this is
+because `bfloat16` does not have the precision to increment `256` by values less than
+`1`:
+```python
+>>> bfloat16(256) + bfloat16(1)
+256
+```
+After 256, the next representable value in bfloat16 is 258:
+```python
+>>> np.nextafter(bfloat16(256), bfloat16(np.inf))
+258
+```
+For better results you can specify that the accumulation should happen in a
+higher-precision type like `float32`:
+```python
+>>> vals.sum(dtype='float32').astype(bfloat16)
+4992
+```
+In contrast to NumPy, projects like [JAX](http://jax.readthedocs.io/) which support
+low-precision arithmetic more natively will often do these kinds of higher-precision
+accumulations automatically:
+```python
+>>> import jax.numpy as jnp
+>>> jnp.array(vals).sum()
+Array(4992, dtype=bfloat16)
+```
+
 ## License
 
+*This is not an officially supported Google product.*
+
 The `ml_dtypes` source code is licensed under the Apache 2.0 license
 (see [LICENSE](LICENSE)). Pre-compiled wheels are built with the
 [EIGEN](https://eigen.tuxfamily.org/) project, which is released under the
 MPL 2.0 license (see [LICENSE.eigen](LICENSE.eigen)).
```

### Comparing `ml_dtypes-0.1.0/ml_dtypes.egg-info/SOURCES.txt` & `ml_dtypes-0.2.0/ml_dtypes.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,33 @@
 LICENSE.eigen
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 ml_dtypes/__init__.py
 ml_dtypes/_finfo.py
+ml_dtypes/_iinfo.py
 ml_dtypes/py.typed
 ml_dtypes.egg-info/PKG-INFO
 ml_dtypes.egg-info/SOURCES.txt
 ml_dtypes.egg-info/dependency_links.txt
 ml_dtypes.egg-info/requires.txt
 ml_dtypes.egg-info/top_level.txt
+ml_dtypes/_src/common.h
 ml_dtypes/_src/custom_float.h
 ml_dtypes/_src/dtypes.cc
-ml_dtypes/_src/float8.h
+ml_dtypes/_src/int4.h
 ml_dtypes/_src/numpy.cc
 ml_dtypes/_src/numpy.h
+ml_dtypes/_src/ufuncs.h
+ml_dtypes/include/float8.h
 ml_dtypes/tests/custom_float_test.py
 ml_dtypes/tests/finfo_test.py
+ml_dtypes/tests/iinfo_test.py
+ml_dtypes/tests/int4_test.py
 ml_dtypes/tests/metadata_test.py
 third_party/eigen/Eigen/Core
 third_party/eigen/Eigen/src/Core/ArithmeticSequence.h
 third_party/eigen/Eigen/src/Core/Array.h
 third_party/eigen/Eigen/src/Core/ArrayBase.h
 third_party/eigen/Eigen/src/Core/ArrayWrapper.h
 third_party/eigen/Eigen/src/Core/Assign.h
```

### Comparing `ml_dtypes-0.1.0/pyproject.toml` & `ml_dtypes-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ml_dtypes"
-version = "0.1.0"  # Keep in sync with ml_dtypes/__init__.py:__version__
+version = "0.2.0"  # Keep in sync with ml_dtypes/__init__.py:__version__
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [{name = "ml_dtypes authors", email="ml_dtypes@google.com"}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ml_dtypes-0.1.0/setup.py` & `ml_dtypes-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,17 @@
         Pybind11Extension(
             "ml_dtypes._custom_floats",
             [
                 "ml_dtypes/_src/dtypes.cc",
                 "ml_dtypes/_src/numpy.cc",
             ],
             include_dirs=[
-                "third_party",
+                "third_party/eigen",
                 "ml_dtypes",
                 np.get_include(),
             ],
             extra_compile_args=COMPILE_ARGS,
         )
     ],
-    include_package_data=False,
+    include_package_data=True,  # Export headers.
     cmdclass={"build_py": build_py},
 )
```

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/Core` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/Core`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Array.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArrayBase.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArrayWrapper.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Assign.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/AssignEvaluator.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Assign_MKL.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/BandMatrix.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Block.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CommaInitializer.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ConditionEstimator.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CoreEvaluators.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CoreIterators.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseBase.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseStorage.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Diagonal.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DiagonalProduct.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Dot.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/EigenBase.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Fuzzy.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GeneralProduct.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GenericPacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GlobalFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/IO.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/IndexedView.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Inverse.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Map.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MapBase.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Matrix.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MatrixBase.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NestByValue.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NoAlias.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NumTraits.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PermutationMatrix.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PlainObjectBase.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Product.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ProductEvaluators.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Random.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Redux.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Ref.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Replicate.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Reshaped.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ReturnByValue.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Reverse.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Select.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SelfAdjointView.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Solve.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SolveTriangular.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SolverBase.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/StableNorm.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/StlIterators.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Stride.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Swap.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Transpose.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Transpositions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/TriangularMatrix.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/VectorBlock.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/VectorwiseOp.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Visitor.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/Half.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/Parallelizer.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Assert.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Assert.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/BlasUtil.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Constants.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/MKL_support.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Macros.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Memory.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Meta.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Serializer.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/Serializer.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/StaticAssert.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/XprHelper.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/BlockMethods.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h` & `ml_dtypes-0.2.0/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

