# Comparing `tmp/tensorflow_federated-0.7.0-py2.py3-none-any.whl.zip` & `tmp/tensorflow_federated-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,108 +1,123 @@
-Zip file size: 308696 bytes, number of entries: 106
--rw-rw-r--  2.0 unx     4056 b- defN 19-Jul-12 04:46 tensorflow_federated/__init__.py
--rw-rw-r--  2.0 unx      618 b- defN 19-Jul-12 04:46 tensorflow_federated/proto/__init__.py
--rw-rw-r--  2.0 unx      618 b- defN 19-Jul-12 04:46 tensorflow_federated/proto/v0/__init__.py
--rw-rw-r--  2.0 unx    66868 b- defN 19-Jul-12 04:46 tensorflow_federated/proto/v0/computation_pb2.py
--rw-rw-r--  2.0 unx       83 b- defN 19-Jul-12 04:46 tensorflow_federated/proto/v0/computation_pb2_grpc.py
--rw-rw-r--  2.0 unx    31793 b- defN 19-Jul-12 04:46 tensorflow_federated/proto/v0/executor_pb2.py
--rw-rw-r--  2.0 unx     7042 b- defN 19-Jul-12 04:46 tensorflow_federated/proto/v0/executor_pb2_grpc.py
--rw-rw-r--  2.0 unx      618 b- defN 19-Jul-12 04:46 tensorflow_federated/python/__init__.py
--rw-rw-r--  2.0 unx      699 b- defN 19-Jul-12 04:46 tensorflow_federated/python/common_libs/__init__.py
--rw-rw-r--  2.0 unx    14346 b- defN 19-Jul-12 04:46 tensorflow_federated/python/common_libs/anonymous_tuple.py
--rw-rw-r--  2.0 unx     7347 b- defN 19-Jul-12 04:46 tensorflow_federated/python/common_libs/py_typecheck.py
--rw-rw-r--  2.0 unx     2013 b- defN 19-Jul-12 04:46 tensorflow_federated/python/common_libs/serialization_utils.py
--rw-rw-r--  2.0 unx     3120 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/__init__.py
--rw-rw-r--  2.0 unx     2879 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/api/__init__.py
--rw-rw-r--  2.0 unx     1434 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/api/computation_base.py
--rw-rw-r--  2.0 unx    20387 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/api/computation_types.py
--rw-rw-r--  2.0 unx     8441 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/api/computations.py
--rw-rw-r--  2.0 unx    16053 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/api/intrinsics.py
--rw-rw-r--  2.0 unx     1091 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/api/placements.py
--rw-rw-r--  2.0 unx     1127 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/api/typed_object.py
--rw-rw-r--  2.0 unx     2977 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/api/value_base.py
--rw-rw-r--  2.0 unx     3047 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/api/values.py
--rw-rw-r--  2.0 unx     7452 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/framework/__init__.py
--rw-rw-r--  2.0 unx      694 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/__init__.py
--rw-rw-r--  2.0 unx    53517 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/compiled_computation_transforms.py
--rw-rw-r--  2.0 unx     3738 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/compiler_pipeline.py
--rw-rw-r--  2.0 unx     1790 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/computation_building_block_utils.py
--rw-rw-r--  2.0 unx    51156 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/computation_building_blocks.py
--rw-rw-r--  2.0 unx    68812 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/computation_constructing_utils.py
--rw-rw-r--  2.0 unx     3569 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/computation_impl.py
--rw-rw-r--  2.0 unx    18681 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/computation_wrapper.py
--rw-rw-r--  2.0 unx     4103 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/computation_wrapper_instances.py
--rw-rw-r--  2.0 unx     2676 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/concurrent_executor.py
--rw-rw-r--  2.0 unx     3656 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/context_base.py
--rw-rw-r--  2.0 unx     1853 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/context_stack_base.py
--rw-rw-r--  2.0 unx     2458 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/context_stack_impl.py
--rw-rw-r--  2.0 unx      954 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/dtype_utils.py
--rw-rw-r--  2.0 unx    18424 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/eager_executor.py
--rw-rw-r--  2.0 unx     4421 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/execution_context.py
--rw-rw-r--  2.0 unx     3960 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/executor_base.py
--rw-rw-r--  2.0 unx     8354 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/executor_service.py
--rw-rw-r--  2.0 unx     8047 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/executor_service_utils.py
--rw-rw-r--  2.0 unx     2159 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/executor_stacks.py
--rw-rw-r--  2.0 unx     1549 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/executor_value_base.py
--rw-rw-r--  2.0 unx     3461 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/federated_computation_context.py
--rw-rw-r--  2.0 unx     3825 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/federated_computation_utils.py
--rw-rw-r--  2.0 unx    32327 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/federated_executor.py
--rw-rw-r--  2.0 unx    28783 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/function_utils.py
--rw-rw-r--  2.0 unx    54128 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/graph_utils.py
--rw-rw-r--  2.0 unx    13656 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/intrinsic_bodies.py
--rw-rw-r--  2.0 unx    19970 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/intrinsic_defs.py
--rw-rw-r--  2.0 unx    26457 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/intrinsic_factory.py
--rw-rw-r--  2.0 unx     2327 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/intrinsic_reductions.py
--rw-rw-r--  2.0 unx    12435 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/intrinsic_utils.py
--rw-rw-r--  2.0 unx    18827 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/lambda_executor.py
--rw-rw-r--  2.0 unx     2525 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/placement_literals.py
--rw-rw-r--  2.0 unx    51963 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/reference_executor.py
--rw-rw-r--  2.0 unx     5044 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/remote_executor.py
--rw-rw-r--  2.0 unx     1519 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/set_default_executor.py
--rw-rw-r--  2.0 unx     6154 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/tensorflow_deserialization.py
--rw-rw-r--  2.0 unx    14775 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/tensorflow_serialization.py
--rw-rw-r--  2.0 unx     2177 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/tf_computation_context.py
--rw-rw-r--  2.0 unx    41804 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/transformation_utils.py
--rw-rw-r--  2.0 unx    69203 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/transformations.py
--rw-rw-r--  2.0 unx     3568 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/transforming_executor.py
--rw-rw-r--  2.0 unx     3399 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/type_constructors.py
--rw-rw-r--  2.0 unx     6574 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/type_serialization.py
--rw-rw-r--  2.0 unx    59467 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/type_utils.py
--rw-rw-r--  2.0 unx    17373 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/value_impl.py
--rw-rw-r--  2.0 unx     2653 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/impl/value_utils.py
--rw-rw-r--  2.0 unx     2143 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/utils/__init__.py
--rw-rw-r--  2.0 unx    11655 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/utils/computation_utils.py
--rw-rw-r--  2.0 unx     5076 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/utils/federated_aggregations.py
--rw-rw-r--  2.0 unx     5122 b- defN 19-Jul-12 04:46 tensorflow_federated/python/core/utils/tf_computation_utils.py
--rw-rw-r--  2.0 unx      618 b- defN 19-Jul-12 04:46 tensorflow_federated/python/examples/__init__.py
--rw-rw-r--  2.0 unx      969 b- defN 19-Jul-12 04:46 tensorflow_federated/python/examples/mnist/__init__.py
--rw-rw-r--  2.0 unx     4464 b- defN 19-Jul-12 04:46 tensorflow_federated/python/examples/mnist/models.py
--rw-rw-r--  2.0 unx     2084 b- defN 19-Jul-12 04:46 tensorflow_federated/python/learning/__init__.py
--rw-rw-r--  2.0 unx     6929 b- defN 19-Jul-12 04:46 tensorflow_federated/python/learning/federated_averaging.py
--rw-rw-r--  2.0 unx     3125 b- defN 19-Jul-12 04:46 tensorflow_federated/python/learning/federated_evaluation.py
--rw-rw-r--  2.0 unx     8002 b- defN 19-Jul-12 04:46 tensorflow_federated/python/learning/federated_sgd.py
--rw-rw-r--  2.0 unx    19168 b- defN 19-Jul-12 04:46 tensorflow_federated/python/learning/keras_utils.py
--rw-rw-r--  2.0 unx     8542 b- defN 19-Jul-12 04:46 tensorflow_federated/python/learning/model.py
--rw-rw-r--  2.0 unx     6303 b- defN 19-Jul-12 04:46 tensorflow_federated/python/learning/model_utils.py
--rw-rw-r--  2.0 unx     1544 b- defN 19-Jul-12 04:46 tensorflow_federated/python/learning/framework/__init__.py
--rw-rw-r--  2.0 unx    18608 b- defN 19-Jul-12 04:46 tensorflow_federated/python/learning/framework/optimizer_utils.py
--rw-rw-r--  2.0 unx     1538 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/__init__.py
--rw-rw-r--  2.0 unx     3837 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/client_data.py
--rw-rw-r--  2.0 unx     3469 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/file_per_user_client_data.py
--rw-rw-r--  2.0 unx     2269 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/from_tensor_slices_client_data.py
--rw-rw-r--  2.0 unx     3080 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/hdf5_client_data.py
--rw-rw-r--  2.0 unx     5863 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/transforming_client_data.py
--rw-rw-r--  2.0 unx     1031 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/datasets/__init__.py
--rw-rw-r--  2.0 unx     1172 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/datasets/emnist/__init__.py
--rw-rw-r--  2.0 unx     9992 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/datasets/emnist/load_data.py
--rw-rw-r--  2.0 unx    19403 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/datasets/emnist/synthetic.py
--rw-rw-r--  2.0 unx      960 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/datasets/shakespeare/__init__.py
--rw-rw-r--  2.0 unx     3051 b- defN 19-Jul-12 04:46 tensorflow_federated/python/simulation/datasets/shakespeare/load_data.py
--rw-rw-r--  2.0 unx      618 b- defN 19-Jul-12 04:46 tensorflow_federated/python/tensorflow_libs/__init__.py
--rw-rw-r--  2.0 unx     1167 b- defN 19-Jul-12 04:46 tensorflow_federated/python/tensorflow_libs/graph_keys.py
--rw-rw-r--  2.0 unx    13608 b- defN 19-Jul-12 04:46 tensorflow_federated/python/tensorflow_libs/graph_merge.py
--rw-rw-r--  2.0 unx     5818 b- defN 19-Jul-12 04:46 tensorflow_federated/python/tensorflow_libs/tensor_utils.py
--rw-rw-r--  2.0 unx     3214 b- defN 19-Jul-12 04:46 tensorflow_federated-0.7.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 19-Jul-12 04:46 tensorflow_federated-0.7.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       21 b- defN 19-Jul-12 04:46 tensorflow_federated-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    11980 b- defN 19-Jul-12 04:46 tensorflow_federated-0.7.0.dist-info/RECORD
-106 files, 1169627 bytes uncompressed, 288662 bytes compressed:  75.3%
+Zip file size: 387504 bytes, number of entries: 121
+-rw-r-----  2.0 unx     4218 b- defN 19-Oct-07 20:04 tensorflow_federated/__init__.py
+-rw-r-----  2.0 unx      787 b- defN 19-Oct-07 20:04 tensorflow_federated/version.py
+-rw-r-----  2.0 unx      618 b- defN 19-Oct-07 20:04 tensorflow_federated/proto/__init__.py
+-rw-r-----  2.0 unx      618 b- defN 19-Oct-07 20:04 tensorflow_federated/proto/v0/__init__.py
+-rw-r-----  2.0 unx    65974 b- defN 19-Oct-07 20:04 tensorflow_federated/proto/v0/computation_pb2.py
+-rw-r-----  2.0 unx    47745 b- defN 19-Oct-07 20:04 tensorflow_federated/proto/v0/executor_pb2.py
+-rw-r-----  2.0 unx     7996 b- defN 19-Oct-07 20:04 tensorflow_federated/proto/v0/executor_pb2_grpc.py
+-rw-r-----  2.0 unx      618 b- defN 19-Oct-07 20:04 tensorflow_federated/python/__init__.py
+-rw-r-----  2.0 unx      699 b- defN 19-Oct-07 20:04 tensorflow_federated/python/common_libs/__init__.py
+-rw-r-----  2.0 unx    16820 b- defN 19-Oct-07 20:04 tensorflow_federated/python/common_libs/anonymous_tuple.py
+-rw-r-----  2.0 unx     7751 b- defN 19-Oct-07 20:04 tensorflow_federated/python/common_libs/py_typecheck.py
+-rw-r-----  2.0 unx     2872 b- defN 19-Oct-07 20:04 tensorflow_federated/python/common_libs/serialization_utils.py
+-rw-r-----  2.0 unx     3174 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/__init__.py
+-rw-r-----  2.0 unx     2879 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/api/__init__.py
+-rw-r-----  2.0 unx     1434 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/api/computation_base.py
+-rw-r-----  2.0 unx    20539 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/api/computation_types.py
+-rw-r-----  2.0 unx     8441 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/api/computations.py
+-rw-r-----  2.0 unx    16171 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/api/intrinsics.py
+-rw-r-----  2.0 unx     1100 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/api/placements.py
+-rw-r-----  2.0 unx     1127 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/api/typed_object.py
+-rw-r-----  2.0 unx     2977 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/api/value_base.py
+-rw-r-----  2.0 unx     3047 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/api/values.py
+-rw-r-----  2.0 unx      944 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/backends/__init__.py
+-rw-r-----  2.0 unx     2003 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/backends/mapreduce/__init__.py
+-rw-r-----  2.0 unx    19822 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/backends/mapreduce/canonical_form.py
+-rw-r-----  2.0 unx    32232 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/backends/mapreduce/canonical_form_utils.py
+-rw-r-----  2.0 unx    52094 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/backends/mapreduce/transformations.py
+-rw-r-----  2.0 unx     7937 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/framework/__init__.py
+-rw-r-----  2.0 unx      694 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/__init__.py
+-rw-r-----  2.0 unx    13050 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/caching_executor.py
+-rw-r-----  2.0 unx    53456 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiled_computation_transforms.py
+-rw-r-----  2.0 unx     4129 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler_pipeline.py
+-rw-r-----  2.0 unx    24425 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/composite_executor.py
+-rw-r-----  2.0 unx     3584 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/computation_impl.py
+-rw-r-----  2.0 unx    18687 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/computation_wrapper.py
+-rw-r-----  2.0 unx     4094 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/computation_wrapper_instances.py
+-rw-r-----  2.0 unx     2761 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/concurrent_executor.py
+-rw-r-----  2.0 unx     3656 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/context_base.py
+-rw-r-----  2.0 unx     1853 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/context_stack_base.py
+-rw-r-----  2.0 unx     2458 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/context_stack_impl.py
+-rw-r-----  2.0 unx    18657 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/eager_executor.py
+-rw-r-----  2.0 unx     5923 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/execution_context.py
+-rw-r-----  2.0 unx     3960 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/executor_base.py
+-rw-r-----  2.0 unx     9352 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/executor_service.py
+-rw-r-----  2.0 unx    12722 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/executor_service_utils.py
+-rw-r-----  2.0 unx     7945 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/executor_stacks.py
+-rw-r-----  2.0 unx    11102 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/executor_utils.py
+-rw-r-----  2.0 unx     1549 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/executor_value_base.py
+-rw-r-----  2.0 unx     3446 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/federated_computation_context.py
+-rw-r-----  2.0 unx     3959 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/federated_computation_utils.py
+-rw-r-----  2.0 unx    29494 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/federated_executor.py
+-rw-r-----  2.0 unx    14247 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/intrinsic_bodies.py
+-rw-r-----  2.0 unx    26662 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/intrinsic_factory.py
+-rw-r-----  2.0 unx     2262 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/intrinsic_reductions.py
+-rw-r-----  2.0 unx    18841 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/lambda_executor.py
+-rw-r-----  2.0 unx    50372 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/reference_executor.py
+-rw-r-----  2.0 unx    10769 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/remote_executor.py
+-rw-r-----  2.0 unx     3617 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/runtime_utils.py
+-rw-r-----  2.0 unx     1910 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/set_default_executor.py
+-rw-r-----  2.0 unx     6218 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/tensorflow_deserialization.py
+-rw-r-----  2.0 unx    18601 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/tensorflow_serialization.py
+-rw-r-----  2.0 unx     2177 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/tf_computation_context.py
+-rw-r-----  2.0 unx    71861 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/transformations.py
+-rw-r-----  2.0 unx     3483 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/transforming_executor.py
+-rw-r-----  2.0 unx    58436 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/type_utils.py
+-rw-r-----  2.0 unx    16930 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/value_impl.py
+-rw-r-----  2.0 unx     4388 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/value_transformations.py
+-rw-r-----  2.0 unx     3451 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/value_utils.py
+-rw-r-----  2.0 unx      618 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/__init__.py
+-rw-r-----  2.0 unx     3367 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/building_block_analysis.py
+-rw-r-----  2.0 unx    75043 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/building_block_factory.py
+-rw-r-----  2.0 unx    51222 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/building_blocks.py
+-rw-r-----  2.0 unx    19648 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/intrinsic_defs.py
+-rw-r-----  2.0 unx     2525 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/placement_literals.py
+-rw-r-----  2.0 unx     3070 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/proto_transformations.py
+-rw-r-----  2.0 unx    41536 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/transformation_utils.py
+-rw-r-----  2.0 unx    11927 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/tree_analysis.py
+-rw-r-----  2.0 unx     3399 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/type_factory.py
+-rw-r-----  2.0 unx     6585 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/compiler/type_serialization.py
+-rw-r-----  2.0 unx      618 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/utils/__init__.py
+-rw-r-----  2.0 unx    29687 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/utils/function_utils.py
+-rw-r-----  2.0 unx    52057 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/impl/utils/tensorflow_utils.py
+-rw-r-----  2.0 unx     2607 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/utils/__init__.py
+-rw-r-----  2.0 unx    11596 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/utils/computation_utils.py
+-rw-r-----  2.0 unx     7337 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/utils/differential_privacy.py
+-rw-r-----  2.0 unx    18192 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/utils/encoding_utils.py
+-rw-r-----  2.0 unx     5076 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/utils/federated_aggregations.py
+-rw-r-----  2.0 unx     5452 b- defN 19-Oct-07 20:04 tensorflow_federated/python/core/utils/tf_computation_utils.py
+-rw-r-----  2.0 unx     2084 b- defN 19-Oct-07 20:04 tensorflow_federated/python/learning/__init__.py
+-rw-r-----  2.0 unx     7035 b- defN 19-Oct-07 20:04 tensorflow_federated/python/learning/federated_averaging.py
+-rw-r-----  2.0 unx     3125 b- defN 19-Oct-07 20:04 tensorflow_federated/python/learning/federated_evaluation.py
+-rw-r-----  2.0 unx     8002 b- defN 19-Oct-07 20:04 tensorflow_federated/python/learning/federated_sgd.py
+-rw-r-----  2.0 unx    19216 b- defN 19-Oct-07 20:04 tensorflow_federated/python/learning/keras_utils.py
+-rw-r-----  2.0 unx     8645 b- defN 19-Oct-07 20:04 tensorflow_federated/python/learning/model.py
+-rw-r-----  2.0 unx     6303 b- defN 19-Oct-07 20:04 tensorflow_federated/python/learning/model_utils.py
+-rw-r-----  2.0 unx     2196 b- defN 19-Oct-07 20:04 tensorflow_federated/python/learning/framework/__init__.py
+-rw-r-----  2.0 unx     4814 b- defN 19-Oct-07 20:04 tensorflow_federated/python/learning/framework/encoding_utils.py
+-rw-r-----  2.0 unx    18608 b- defN 19-Oct-07 20:04 tensorflow_federated/python/learning/framework/optimizer_utils.py
+-rw-r-----  2.0 unx     2170 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/__init__.py
+-rw-r-----  2.0 unx     6416 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/client_data.py
+-rw-r-----  2.0 unx     3543 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/file_per_user_client_data.py
+-rw-r-----  2.0 unx     2315 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/from_tensor_slices_client_data.py
+-rw-r-----  2.0 unx     3205 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/hdf5_client_data.py
+-rw-r-----  2.0 unx     2931 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/server_utils.py
+-rw-r-----  2.0 unx     5863 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/transforming_client_data.py
+-rw-r-----  2.0 unx     1527 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/datasets/__init__.py
+-rw-r-----  2.0 unx     3725 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/datasets/dataset_utils.py
+-rw-r-----  2.0 unx    29071 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/datasets/emnist.py
+-rw-r-----  2.0 unx     3051 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/datasets/shakespeare.py
+-rw-r-----  2.0 unx     5688 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/datasets/stackoverflow.py
+-rw-r-----  2.0 unx      929 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/models/__init__.py
+-rw-r-----  2.0 unx     4228 b- defN 19-Oct-07 20:04 tensorflow_federated/python/simulation/models/mnist.py
+-rw-r-----  2.0 unx      618 b- defN 19-Oct-07 20:04 tensorflow_federated/python/tensorflow_libs/__init__.py
+-rw-r-----  2.0 unx     1167 b- defN 19-Oct-07 20:04 tensorflow_federated/python/tensorflow_libs/graph_keys.py
+-rw-r-----  2.0 unx    13608 b- defN 19-Oct-07 20:04 tensorflow_federated/python/tensorflow_libs/graph_merge.py
+-rw-r-----  2.0 unx    44791 b- defN 19-Oct-07 20:04 tensorflow_federated/python/tensorflow_libs/nest.py
+-rw-r-----  2.0 unx     5139 b- defN 19-Oct-07 20:04 tensorflow_federated/python/tensorflow_libs/tensor_utils.py
+-rw-r-----  2.0 unx     3448 b- defN 19-Oct-07 20:04 tensorflow_federated-0.9.0.dist-info/METADATA
+-rw-r-----  2.0 unx      110 b- defN 19-Oct-07 20:04 tensorflow_federated-0.9.0.dist-info/WHEEL
+-rw-r-----  2.0 unx       21 b- defN 19-Oct-07 20:04 tensorflow_federated-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    13783 b- defN 19-Oct-07 20:04 tensorflow_federated-0.9.0.dist-info/RECORD
+121 files, 1476755 bytes uncompressed, 364456 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: tensorflow_federated/__init__.py
 Comment: 
 
+Filename: tensorflow_federated/version.py
+Comment: 
+
 Filename: tensorflow_federated/proto/__init__.py
 Comment: 
 
 Filename: tensorflow_federated/proto/v0/__init__.py
 Comment: 
 
 Filename: tensorflow_federated/proto/v0/computation_pb2.py
 Comment: 
 
-Filename: tensorflow_federated/proto/v0/computation_pb2_grpc.py
-Comment: 
-
 Filename: tensorflow_federated/proto/v0/executor_pb2.py
 Comment: 
 
 Filename: tensorflow_federated/proto/v0/executor_pb2_grpc.py
 Comment: 
 
 Filename: tensorflow_federated/python/__init__.py
@@ -60,33 +60,45 @@
 
 Filename: tensorflow_federated/python/core/api/value_base.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/api/values.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/framework/__init__.py
+Filename: tensorflow_federated/python/core/backends/__init__.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/__init__.py
+Filename: tensorflow_federated/python/core/backends/mapreduce/__init__.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/compiled_computation_transforms.py
+Filename: tensorflow_federated/python/core/backends/mapreduce/canonical_form.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/compiler_pipeline.py
+Filename: tensorflow_federated/python/core/backends/mapreduce/canonical_form_utils.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/computation_building_block_utils.py
+Filename: tensorflow_federated/python/core/backends/mapreduce/transformations.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/computation_building_blocks.py
+Filename: tensorflow_federated/python/core/framework/__init__.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/computation_constructing_utils.py
+Filename: tensorflow_federated/python/core/impl/__init__.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/caching_executor.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/compiled_computation_transforms.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/compiler_pipeline.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/composite_executor.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/computation_impl.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/computation_wrapper.py
 Comment: 
@@ -102,17 +114,14 @@
 
 Filename: tensorflow_federated/python/core/impl/context_stack_base.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/context_stack_impl.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/dtype_utils.py
-Comment: 
-
 Filename: tensorflow_federated/python/core/impl/eager_executor.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/execution_context.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/executor_base.py
@@ -123,114 +132,138 @@
 
 Filename: tensorflow_federated/python/core/impl/executor_service_utils.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/executor_stacks.py
 Comment: 
 
+Filename: tensorflow_federated/python/core/impl/executor_utils.py
+Comment: 
+
 Filename: tensorflow_federated/python/core/impl/executor_value_base.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/federated_computation_context.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/federated_computation_utils.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/federated_executor.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/function_utils.py
-Comment: 
-
-Filename: tensorflow_federated/python/core/impl/graph_utils.py
-Comment: 
-
 Filename: tensorflow_federated/python/core/impl/intrinsic_bodies.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/intrinsic_defs.py
-Comment: 
-
 Filename: tensorflow_federated/python/core/impl/intrinsic_factory.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/intrinsic_reductions.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/intrinsic_utils.py
-Comment: 
-
 Filename: tensorflow_federated/python/core/impl/lambda_executor.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/placement_literals.py
-Comment: 
-
 Filename: tensorflow_federated/python/core/impl/reference_executor.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/remote_executor.py
 Comment: 
 
+Filename: tensorflow_federated/python/core/impl/runtime_utils.py
+Comment: 
+
 Filename: tensorflow_federated/python/core/impl/set_default_executor.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/tensorflow_deserialization.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/tensorflow_serialization.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/tf_computation_context.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/transformation_utils.py
-Comment: 
-
 Filename: tensorflow_federated/python/core/impl/transformations.py
 Comment: 
 
 Filename: tensorflow_federated/python/core/impl/transforming_executor.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/type_constructors.py
+Filename: tensorflow_federated/python/core/impl/type_utils.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/type_serialization.py
+Filename: tensorflow_federated/python/core/impl/value_impl.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/type_utils.py
+Filename: tensorflow_federated/python/core/impl/value_transformations.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/value_impl.py
+Filename: tensorflow_federated/python/core/impl/value_utils.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/impl/value_utils.py
+Filename: tensorflow_federated/python/core/impl/compiler/__init__.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/utils/__init__.py
+Filename: tensorflow_federated/python/core/impl/compiler/building_block_analysis.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/utils/computation_utils.py
+Filename: tensorflow_federated/python/core/impl/compiler/building_block_factory.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/utils/federated_aggregations.py
+Filename: tensorflow_federated/python/core/impl/compiler/building_blocks.py
 Comment: 
 
-Filename: tensorflow_federated/python/core/utils/tf_computation_utils.py
+Filename: tensorflow_federated/python/core/impl/compiler/intrinsic_defs.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/compiler/placement_literals.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/compiler/proto_transformations.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/compiler/transformation_utils.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/compiler/tree_analysis.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/compiler/type_factory.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/compiler/type_serialization.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/utils/__init__.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/utils/function_utils.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/impl/utils/tensorflow_utils.py
 Comment: 
 
-Filename: tensorflow_federated/python/examples/__init__.py
+Filename: tensorflow_federated/python/core/utils/__init__.py
 Comment: 
 
-Filename: tensorflow_federated/python/examples/mnist/__init__.py
+Filename: tensorflow_federated/python/core/utils/computation_utils.py
 Comment: 
 
-Filename: tensorflow_federated/python/examples/mnist/models.py
+Filename: tensorflow_federated/python/core/utils/differential_privacy.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/utils/encoding_utils.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/utils/federated_aggregations.py
+Comment: 
+
+Filename: tensorflow_federated/python/core/utils/tf_computation_utils.py
 Comment: 
 
 Filename: tensorflow_federated/python/learning/__init__.py
 Comment: 
 
 Filename: tensorflow_federated/python/learning/federated_averaging.py
 Comment: 
@@ -249,14 +282,17 @@
 
 Filename: tensorflow_federated/python/learning/model_utils.py
 Comment: 
 
 Filename: tensorflow_federated/python/learning/framework/__init__.py
 Comment: 
 
+Filename: tensorflow_federated/python/learning/framework/encoding_utils.py
+Comment: 
+
 Filename: tensorflow_federated/python/learning/framework/optimizer_utils.py
 Comment: 
 
 Filename: tensorflow_federated/python/simulation/__init__.py
 Comment: 
 
 Filename: tensorflow_federated/python/simulation/client_data.py
@@ -267,53 +303,62 @@
 
 Filename: tensorflow_federated/python/simulation/from_tensor_slices_client_data.py
 Comment: 
 
 Filename: tensorflow_federated/python/simulation/hdf5_client_data.py
 Comment: 
 
+Filename: tensorflow_federated/python/simulation/server_utils.py
+Comment: 
+
 Filename: tensorflow_federated/python/simulation/transforming_client_data.py
 Comment: 
 
 Filename: tensorflow_federated/python/simulation/datasets/__init__.py
 Comment: 
 
-Filename: tensorflow_federated/python/simulation/datasets/emnist/__init__.py
+Filename: tensorflow_federated/python/simulation/datasets/dataset_utils.py
+Comment: 
+
+Filename: tensorflow_federated/python/simulation/datasets/emnist.py
 Comment: 
 
-Filename: tensorflow_federated/python/simulation/datasets/emnist/load_data.py
+Filename: tensorflow_federated/python/simulation/datasets/shakespeare.py
 Comment: 
 
-Filename: tensorflow_federated/python/simulation/datasets/emnist/synthetic.py
+Filename: tensorflow_federated/python/simulation/datasets/stackoverflow.py
 Comment: 
 
-Filename: tensorflow_federated/python/simulation/datasets/shakespeare/__init__.py
+Filename: tensorflow_federated/python/simulation/models/__init__.py
 Comment: 
 
-Filename: tensorflow_federated/python/simulation/datasets/shakespeare/load_data.py
+Filename: tensorflow_federated/python/simulation/models/mnist.py
 Comment: 
 
 Filename: tensorflow_federated/python/tensorflow_libs/__init__.py
 Comment: 
 
 Filename: tensorflow_federated/python/tensorflow_libs/graph_keys.py
 Comment: 
 
 Filename: tensorflow_federated/python/tensorflow_libs/graph_merge.py
 Comment: 
 
+Filename: tensorflow_federated/python/tensorflow_libs/nest.py
+Comment: 
+
 Filename: tensorflow_federated/python/tensorflow_libs/tensor_utils.py
 Comment: 
 
-Filename: tensorflow_federated-0.7.0.dist-info/METADATA
+Filename: tensorflow_federated-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: tensorflow_federated-0.7.0.dist-info/WHEEL
+Filename: tensorflow_federated-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: tensorflow_federated-0.7.0.dist-info/top_level.txt
+Filename: tensorflow_federated-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: tensorflow_federated-0.7.0.dist-info/RECORD
+Filename: tensorflow_federated-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tensorflow_federated/__init__.py

```diff
@@ -14,14 +14,16 @@
 # limitations under the License.
 """TensorFlow Federated Library."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
+from tensorflow_federated.version import __version__  # pylint: disable=g-bad-import-order
+
 from tensorflow_federated.python.core.api.computation_base import Computation
 from tensorflow_federated.python.core.api.computation_types import FederatedType
 from tensorflow_federated.python.core.api.computation_types import FunctionType
 from tensorflow_federated.python.core.api.computation_types import NamedTupleType
 from tensorflow_federated.python.core.api.computation_types import SequenceType
 from tensorflow_federated.python.core.api.computation_types import TensorType
 from tensorflow_federated.python.core.api.computation_types import to_type
@@ -46,25 +48,27 @@
 from tensorflow_federated.python.core.api.typed_object import TypedObject
 from tensorflow_federated.python.core.api.value_base import Value
 from tensorflow_federated.python.core.api.values import to_value
 
 # NOTE: These imports must happen after the API imports.
 # pylint: disable=g-bad-import-order
 from tensorflow_federated.python.core import framework
+from tensorflow_federated.python.core import backends
 from tensorflow_federated.python.core import utils
 # pylint: enable=g-bad-import-order
 
 # NOTE: These imports must happen after the Core imports.
 # pylint: disable=g-bad-import-order
 from tensorflow_federated.python import learning
 from tensorflow_federated.python import simulation
 # pylint: enable=g-bad-import-order,wildcard-import
 
 # Used by doc generation script.
 _allowed_symbols = [
+    "backends",
     "CLIENTS",
     "Computation",
     "FederatedType",
     "FunctionType",
     "NamedTupleType",
     "SERVER",
     "SequenceType",
```

## tensorflow_federated/proto/v0/computation_pb2.py

```diff
@@ -17,15 +17,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='tensorflow_federated/proto/v0/computation.proto',
   package='tensorflow_federated.v0',
   syntax='proto3',
   serialized_options=None,
-  serialized_pb=_b('\n/tensorflow_federated/proto/v0/computation.proto\x12\x17tensorflow_federated.v0\x1a\x19google/protobuf/any.proto\"\xdb\x04\n\x0b\x43omputation\x12+\n\x04type\x18\x01 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\x12\x39\n\ntensorflow\x18\x02 \x01(\x0b\x32#.tensorflow_federated.v0.TensorFlowH\x00\x12\x37\n\tintrinsic\x18\x03 \x01(\x0b\x32\".tensorflow_federated.v0.IntrinsicH\x00\x12-\n\x04\x64\x61ta\x18\n \x01(\x0b\x32\x1d.tensorflow_federated.v0.DataH\x00\x12\x31\n\x06lambda\x18\x04 \x01(\x0b\x32\x1f.tensorflow_federated.v0.LambdaH\x00\x12/\n\x05\x62lock\x18\x05 \x01(\x0b\x32\x1e.tensorflow_federated.v0.BlockH\x00\x12\x37\n\treference\x18\x06 \x01(\x0b\x32\".tensorflow_federated.v0.ReferenceH\x00\x12-\n\x04\x63\x61ll\x18\x07 \x01(\x0b\x32\x1d.tensorflow_federated.v0.CallH\x00\x12/\n\x05tuple\x18\x08 \x01(\x0b\x32\x1e.tensorflow_federated.v0.TupleH\x00\x12\x37\n\tselection\x18\t \x01(\x0b\x32\".tensorflow_federated.v0.SelectionH\x00\x12\x37\n\tplacement\x18\x0b \x01(\x0b\x32\".tensorflow_federated.v0.PlacementH\x00\x42\r\n\x0b\x63omputation\"\xaa\x03\n\x04Type\x12\x39\n\x08\x66unction\x18\x01 \x01(\x0b\x32%.tensorflow_federated.v0.FunctionTypeH\x00\x12\x38\n\x05tuple\x18\x02 \x01(\x0b\x32\'.tensorflow_federated.v0.NamedTupleTypeH\x00\x12\x39\n\x08sequence\x18\x03 \x01(\x0b\x32%.tensorflow_federated.v0.SequenceTypeH\x00\x12\x35\n\x06tensor\x18\x04 \x01(\x0b\x32#.tensorflow_federated.v0.TensorTypeH\x00\x12\x39\n\x08\x61\x62stract\x18\x05 \x01(\x0b\x32%.tensorflow_federated.v0.AbstractTypeH\x00\x12;\n\tplacement\x18\x06 \x01(\x0b\x32&.tensorflow_federated.v0.PlacementTypeH\x00\x12;\n\tfederated\x18\x07 \x01(\x0b\x32&.tensorflow_federated.v0.FederatedTypeH\x00\x42\x06\n\x04type\"o\n\x0c\x46unctionType\x12\x30\n\tparameter\x18\x01 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\x12-\n\x06result\x18\x02 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\"\x99\x01\n\x0eNamedTupleType\x12@\n\x07\x65lement\x18\x01 \x03(\x0b\x32/.tensorflow_federated.v0.NamedTupleType.Element\x1a\x45\n\x07\x45lement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\">\n\x0cSequenceType\x12.\n\x07\x65lement\x18\x01 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\"\xc3\x03\n\nTensorType\x12;\n\x05\x64type\x18\x01 \x01(\x0e\x32,.tensorflow_federated.v0.TensorType.DataType\x12\x0c\n\x04\x64ims\x18\x02 \x03(\x03\x12\x14\n\x0cunknown_rank\x18\x03 \x01(\x08\"\xd3\x02\n\x08\x44\x61taType\x12\x0e\n\nDT_INVALID\x10\x00\x12\x0c\n\x08\x44T_FLOAT\x10\x01\x12\r\n\tDT_DOUBLE\x10\x02\x12\x0c\n\x08\x44T_INT32\x10\x03\x12\x0c\n\x08\x44T_UINT8\x10\x04\x12\x0c\n\x08\x44T_INT16\x10\x05\x12\x0b\n\x07\x44T_INT8\x10\x06\x12\r\n\tDT_STRING\x10\x07\x12\x10\n\x0c\x44T_COMPLEX64\x10\x08\x12\x0c\n\x08\x44T_INT64\x10\t\x12\x0b\n\x07\x44T_BOOL\x10\n\x12\x0c\n\x08\x44T_QINT8\x10\x0b\x12\r\n\tDT_QUINT8\x10\x0c\x12\r\n\tDT_QINT32\x10\r\x12\x0f\n\x0b\x44T_BFLOAT16\x10\x0e\x12\r\n\tDT_QINT16\x10\x0f\x12\x0e\n\nDT_QUINT16\x10\x10\x12\r\n\tDT_UINT16\x10\x11\x12\x11\n\rDT_COMPLEX128\x10\x12\x12\x0b\n\x07\x44T_HALF\x10\x13\x12\r\n\tDT_UINT32\x10\x16\x12\r\n\tDT_UINT64\x10\x17\"\x1d\n\x0c\x41\x62stractType\x12\r\n\x05label\x18\x01 \x01(\t\"\x8b\x01\n\rPlacementSpec\x12\x38\n\x05label\x18\x01 \x01(\x0b\x32\'.tensorflow_federated.v0.PlacementLabelH\x00\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32\".tensorflow_federated.v0.PlacementH\x00\x42\x0b\n\tplacement\"\x1f\n\x0ePlacementLabel\x12\r\n\x05label\x18\x01 \x01(\t\"\x18\n\tPlacement\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\x8c\x01\n\rFederatedType\x12\x39\n\tplacement\x18\x01 \x01(\x0b\x32&.tensorflow_federated.v0.PlacementSpec\x12\x11\n\tall_equal\x18\x02 \x01(\x08\x12-\n\x06member\x18\x03 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\"P\n\rPlacementType\x12?\n\x0einstance_label\x18\x01 \x01(\x0b\x32\'.tensorflow_federated.v0.PlacementLabel\"\xa4\x05\n\nTensorFlow\x12\'\n\tgraph_def\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x15\n\rinitialize_op\x18\x04 \x01(\t\x12>\n\tparameter\x18\x02 \x01(\x0b\x32+.tensorflow_federated.v0.TensorFlow.Binding\x12;\n\x06result\x18\x03 \x01(\x0b\x32+.tensorflow_federated.v0.TensorFlow.Binding\x1a\xea\x01\n\x07\x42inding\x12\x46\n\x05tuple\x18\x01 \x01(\x0b\x32\x35.tensorflow_federated.v0.TensorFlow.NamedTupleBindingH\x00\x12\x43\n\x06tensor\x18\x02 \x01(\x0b\x32\x31.tensorflow_federated.v0.TensorFlow.TensorBindingH\x00\x12G\n\x08sequence\x18\x03 \x01(\x0b\x32\x33.tensorflow_federated.v0.TensorFlow.SequenceBindingH\x00\x42\t\n\x07\x62inding\x1aQ\n\x11NamedTupleBinding\x12<\n\x07\x65lement\x18\x01 \x03(\x0b\x32+.tensorflow_federated.v0.TensorFlow.Binding\x1a\x31\n\rTensorBinding\x12\x15\n\x0btensor_name\x18\x01 \x01(\tH\x00\x42\t\n\x07\x62inding\x1a\x66\n\x0fSequenceBinding\x12)\n\x1biterator_string_handle_name\x18\x01 \x01(\tB\x02\x18\x01H\x00\x12\x1d\n\x13variant_tensor_name\x18\x02 \x01(\tH\x00\x42\t\n\x07\x62inding\"\x18\n\tIntrinsic\x12\x0b\n\x03uri\x18\x01 \x01(\t\"V\n\x06Lambda\x12\x16\n\x0eparameter_name\x18\x01 \x01(\t\x12\x34\n\x06result\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\"\xbe\x01\n\x05\x42lock\x12\x33\n\x05local\x18\x01 \x03(\x0b\x32$.tensorflow_federated.v0.Block.Local\x12\x34\n\x06result\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\x1aJ\n\x05Local\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\"\x19\n\tReference\x12\x0c\n\x04name\x18\x01 \x01(\t\"v\n\x04\x43\x61ll\x12\x36\n\x08\x66unction\x18\x01 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\x12\x36\n\x08\x61rgument\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\"\x8e\x01\n\x05Tuple\x12\x37\n\x07\x65lement\x18\x01 \x03(\x0b\x32&.tensorflow_federated.v0.Tuple.Element\x1aL\n\x07\x45lement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\"o\n\tSelection\x12\x34\n\x06source\x18\x01 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\x12\x0e\n\x04name\x18\x02 \x01(\tH\x00\x12\x0f\n\x05index\x18\x03 \x01(\x05H\x00\x42\x0b\n\tselection\"\x1d\n\x04\x44\x61ta\x12\r\n\x03uri\x18\x01 \x01(\tH\x00\x42\x06\n\x04\x64\x61tab\x06proto3')
+  serialized_pb=_b('\n/tensorflow_federated/proto/v0/computation.proto\x12\x17tensorflow_federated.v0\x1a\x19google/protobuf/any.proto\"\xdb\x04\n\x0b\x43omputation\x12+\n\x04type\x18\x01 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\x12\x39\n\ntensorflow\x18\x02 \x01(\x0b\x32#.tensorflow_federated.v0.TensorFlowH\x00\x12\x37\n\tintrinsic\x18\x03 \x01(\x0b\x32\".tensorflow_federated.v0.IntrinsicH\x00\x12-\n\x04\x64\x61ta\x18\n \x01(\x0b\x32\x1d.tensorflow_federated.v0.DataH\x00\x12\x31\n\x06lambda\x18\x04 \x01(\x0b\x32\x1f.tensorflow_federated.v0.LambdaH\x00\x12/\n\x05\x62lock\x18\x05 \x01(\x0b\x32\x1e.tensorflow_federated.v0.BlockH\x00\x12\x37\n\treference\x18\x06 \x01(\x0b\x32\".tensorflow_federated.v0.ReferenceH\x00\x12-\n\x04\x63\x61ll\x18\x07 \x01(\x0b\x32\x1d.tensorflow_federated.v0.CallH\x00\x12/\n\x05tuple\x18\x08 \x01(\x0b\x32\x1e.tensorflow_federated.v0.TupleH\x00\x12\x37\n\tselection\x18\t \x01(\x0b\x32\".tensorflow_federated.v0.SelectionH\x00\x12\x37\n\tplacement\x18\x0b \x01(\x0b\x32\".tensorflow_federated.v0.PlacementH\x00\x42\r\n\x0b\x63omputation\"\xaa\x03\n\x04Type\x12\x39\n\x08\x66unction\x18\x01 \x01(\x0b\x32%.tensorflow_federated.v0.FunctionTypeH\x00\x12\x38\n\x05tuple\x18\x02 \x01(\x0b\x32\'.tensorflow_federated.v0.NamedTupleTypeH\x00\x12\x39\n\x08sequence\x18\x03 \x01(\x0b\x32%.tensorflow_federated.v0.SequenceTypeH\x00\x12\x35\n\x06tensor\x18\x04 \x01(\x0b\x32#.tensorflow_federated.v0.TensorTypeH\x00\x12\x39\n\x08\x61\x62stract\x18\x05 \x01(\x0b\x32%.tensorflow_federated.v0.AbstractTypeH\x00\x12;\n\tplacement\x18\x06 \x01(\x0b\x32&.tensorflow_federated.v0.PlacementTypeH\x00\x12;\n\tfederated\x18\x07 \x01(\x0b\x32&.tensorflow_federated.v0.FederatedTypeH\x00\x42\x06\n\x04type\"o\n\x0c\x46unctionType\x12\x30\n\tparameter\x18\x01 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\x12-\n\x06result\x18\x02 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\"\x99\x01\n\x0eNamedTupleType\x12@\n\x07\x65lement\x18\x01 \x03(\x0b\x32/.tensorflow_federated.v0.NamedTupleType.Element\x1a\x45\n\x07\x45lement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\">\n\x0cSequenceType\x12.\n\x07\x65lement\x18\x01 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\"\xc3\x03\n\nTensorType\x12;\n\x05\x64type\x18\x01 \x01(\x0e\x32,.tensorflow_federated.v0.TensorType.DataType\x12\x0c\n\x04\x64ims\x18\x02 \x03(\x03\x12\x14\n\x0cunknown_rank\x18\x03 \x01(\x08\"\xd3\x02\n\x08\x44\x61taType\x12\x0e\n\nDT_INVALID\x10\x00\x12\x0c\n\x08\x44T_FLOAT\x10\x01\x12\r\n\tDT_DOUBLE\x10\x02\x12\x0c\n\x08\x44T_INT32\x10\x03\x12\x0c\n\x08\x44T_UINT8\x10\x04\x12\x0c\n\x08\x44T_INT16\x10\x05\x12\x0b\n\x07\x44T_INT8\x10\x06\x12\r\n\tDT_STRING\x10\x07\x12\x10\n\x0c\x44T_COMPLEX64\x10\x08\x12\x0c\n\x08\x44T_INT64\x10\t\x12\x0b\n\x07\x44T_BOOL\x10\n\x12\x0c\n\x08\x44T_QINT8\x10\x0b\x12\r\n\tDT_QUINT8\x10\x0c\x12\r\n\tDT_QINT32\x10\r\x12\x0f\n\x0b\x44T_BFLOAT16\x10\x0e\x12\r\n\tDT_QINT16\x10\x0f\x12\x0e\n\nDT_QUINT16\x10\x10\x12\r\n\tDT_UINT16\x10\x11\x12\x11\n\rDT_COMPLEX128\x10\x12\x12\x0b\n\x07\x44T_HALF\x10\x13\x12\r\n\tDT_UINT32\x10\x16\x12\r\n\tDT_UINT64\x10\x17\"\x1d\n\x0c\x41\x62stractType\x12\r\n\x05label\x18\x01 \x01(\t\"\x8b\x01\n\rPlacementSpec\x12\x38\n\x05label\x18\x01 \x01(\x0b\x32\'.tensorflow_federated.v0.PlacementLabelH\x00\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32\".tensorflow_federated.v0.PlacementH\x00\x42\x0b\n\tplacement\"\x1f\n\x0ePlacementLabel\x12\r\n\x05label\x18\x01 \x01(\t\"\x18\n\tPlacement\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\x8c\x01\n\rFederatedType\x12\x39\n\tplacement\x18\x01 \x01(\x0b\x32&.tensorflow_federated.v0.PlacementSpec\x12\x11\n\tall_equal\x18\x02 \x01(\x08\x12-\n\x06member\x18\x03 \x01(\x0b\x32\x1d.tensorflow_federated.v0.Type\"P\n\rPlacementType\x12?\n\x0einstance_label\x18\x01 \x01(\x0b\x32\'.tensorflow_federated.v0.PlacementLabel\"\xff\x04\n\nTensorFlow\x12\'\n\tgraph_def\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x15\n\rinitialize_op\x18\x04 \x01(\t\x12>\n\tparameter\x18\x02 \x01(\x0b\x32+.tensorflow_federated.v0.TensorFlow.Binding\x12;\n\x06result\x18\x03 \x01(\x0b\x32+.tensorflow_federated.v0.TensorFlow.Binding\x1a\xea\x01\n\x07\x42inding\x12\x46\n\x05tuple\x18\x01 \x01(\x0b\x32\x35.tensorflow_federated.v0.TensorFlow.NamedTupleBindingH\x00\x12\x43\n\x06tensor\x18\x02 \x01(\x0b\x32\x31.tensorflow_federated.v0.TensorFlow.TensorBindingH\x00\x12G\n\x08sequence\x18\x03 \x01(\x0b\x32\x33.tensorflow_federated.v0.TensorFlow.SequenceBindingH\x00\x42\t\n\x07\x62inding\x1aQ\n\x11NamedTupleBinding\x12<\n\x07\x65lement\x18\x01 \x03(\x0b\x32+.tensorflow_federated.v0.TensorFlow.Binding\x1a\x31\n\rTensorBinding\x12\x15\n\x0btensor_name\x18\x01 \x01(\tH\x00\x42\t\n\x07\x62inding\x1a\x41\n\x0fSequenceBinding\x12\x1d\n\x13variant_tensor_name\x18\x02 \x01(\tH\x00\x42\t\n\x07\x62indingJ\x04\x08\x01\x10\x02\"\x18\n\tIntrinsic\x12\x0b\n\x03uri\x18\x01 \x01(\t\"V\n\x06Lambda\x12\x16\n\x0eparameter_name\x18\x01 \x01(\t\x12\x34\n\x06result\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\"\xbe\x01\n\x05\x42lock\x12\x33\n\x05local\x18\x01 \x03(\x0b\x32$.tensorflow_federated.v0.Block.Local\x12\x34\n\x06result\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\x1aJ\n\x05Local\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\"\x19\n\tReference\x12\x0c\n\x04name\x18\x01 \x01(\t\"v\n\x04\x43\x61ll\x12\x36\n\x08\x66unction\x18\x01 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\x12\x36\n\x08\x61rgument\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\"\x8e\x01\n\x05Tuple\x12\x37\n\x07\x65lement\x18\x01 \x03(\x0b\x32&.tensorflow_federated.v0.Tuple.Element\x1aL\n\x07\x45lement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\"o\n\tSelection\x12\x34\n\x06source\x18\x01 \x01(\x0b\x32$.tensorflow_federated.v0.Computation\x12\x0e\n\x04name\x18\x02 \x01(\tH\x00\x12\x0f\n\x05index\x18\x03 \x01(\x05H\x00\x42\x0b\n\tselection\"\x1d\n\x04\x44\x61ta\x12\r\n\x03uri\x18\x01 \x01(\tH\x00\x42\x06\n\x04\x64\x61tab\x06proto3')
   ,
   dependencies=[google_dot_protobuf_dot_any__pb2.DESCRIPTOR,])
 
 
 
 _TENSORTYPE_DATATYPE = _descriptor.EnumDescriptor(
   name='DataType',
@@ -817,22 +817,15 @@
   name='SequenceBinding',
   full_name='tensorflow_federated.v0.TensorFlow.SequenceBinding',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='iterator_string_handle_name', full_name='tensorflow_federated.v0.TensorFlow.SequenceBinding.iterator_string_handle_name', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=_b('\030\001'), file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='variant_tensor_name', full_name='tensorflow_federated.v0.TensorFlow.SequenceBinding.variant_tensor_name', index=1,
+      name='variant_tensor_name', full_name='tensorflow_federated.v0.TensorFlow.SequenceBinding.variant_tensor_name', index=0,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -846,15 +839,15 @@
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='binding', full_name='tensorflow_federated.v0.TensorFlow.SequenceBinding.binding',
       index=0, containing_type=None, fields=[]),
   ],
   serialized_start=2957,
-  serialized_end=3059,
+  serialized_end=3022,
 )
 
 _TENSORFLOW = _descriptor.Descriptor(
   name='TensorFlow',
   full_name='tensorflow_federated.v0.TensorFlow',
   filename=None,
   file=DESCRIPTOR,
@@ -897,15 +890,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=2383,
-  serialized_end=3059,
+  serialized_end=3022,
 )
 
 
 _INTRINSIC = _descriptor.Descriptor(
   name='Intrinsic',
   full_name='tensorflow_federated.v0.Intrinsic',
   filename=None,
@@ -927,16 +920,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3061,
-  serialized_end=3085,
+  serialized_start=3024,
+  serialized_end=3048,
 )
 
 
 _LAMBDA = _descriptor.Descriptor(
   name='Lambda',
   full_name='tensorflow_federated.v0.Lambda',
   filename=None,
@@ -965,16 +958,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3087,
-  serialized_end=3173,
+  serialized_start=3050,
+  serialized_end=3136,
 )
 
 
 _BLOCK_LOCAL = _descriptor.Descriptor(
   name='Local',
   full_name='tensorflow_federated.v0.Block.Local',
   filename=None,
@@ -1003,16 +996,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3292,
-  serialized_end=3366,
+  serialized_start=3255,
+  serialized_end=3329,
 )
 
 _BLOCK = _descriptor.Descriptor(
   name='Block',
   full_name='tensorflow_federated.v0.Block',
   filename=None,
   file=DESCRIPTOR,
@@ -1040,16 +1033,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3176,
-  serialized_end=3366,
+  serialized_start=3139,
+  serialized_end=3329,
 )
 
 
 _REFERENCE = _descriptor.Descriptor(
   name='Reference',
   full_name='tensorflow_federated.v0.Reference',
   filename=None,
@@ -1071,16 +1064,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3368,
-  serialized_end=3393,
+  serialized_start=3331,
+  serialized_end=3356,
 )
 
 
 _CALL = _descriptor.Descriptor(
   name='Call',
   full_name='tensorflow_federated.v0.Call',
   filename=None,
@@ -1109,16 +1102,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3395,
-  serialized_end=3513,
+  serialized_start=3358,
+  serialized_end=3476,
 )
 
 
 _TUPLE_ELEMENT = _descriptor.Descriptor(
   name='Element',
   full_name='tensorflow_federated.v0.Tuple.Element',
   filename=None,
@@ -1147,16 +1140,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3582,
-  serialized_end=3658,
+  serialized_start=3545,
+  serialized_end=3621,
 )
 
 _TUPLE = _descriptor.Descriptor(
   name='Tuple',
   full_name='tensorflow_federated.v0.Tuple',
   filename=None,
   file=DESCRIPTOR,
@@ -1177,16 +1170,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3516,
-  serialized_end=3658,
+  serialized_start=3479,
+  serialized_end=3621,
 )
 
 
 _SELECTION = _descriptor.Descriptor(
   name='Selection',
   full_name='tensorflow_federated.v0.Selection',
   filename=None,
@@ -1225,16 +1218,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='selection', full_name='tensorflow_federated.v0.Selection.selection',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=3660,
-  serialized_end=3771,
+  serialized_start=3623,
+  serialized_end=3734,
 )
 
 
 _DATA = _descriptor.Descriptor(
   name='Data',
   full_name='tensorflow_federated.v0.Data',
   filename=None,
@@ -1259,16 +1252,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='tensorflow_federated.v0.Data.data',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=3773,
-  serialized_end=3802,
+  serialized_start=3736,
+  serialized_end=3765,
 )
 
 _COMPUTATION.fields_by_name['type'].message_type = _TYPE
 _COMPUTATION.fields_by_name['tensorflow'].message_type = _TENSORFLOW
 _COMPUTATION.fields_by_name['intrinsic'].message_type = _INTRINSIC
 _COMPUTATION.fields_by_name['data'].message_type = _DATA
 _COMPUTATION.fields_by_name['lambda'].message_type = _LAMBDA
@@ -1372,17 +1365,14 @@
 _TENSORFLOW_NAMEDTUPLEBINDING.containing_type = _TENSORFLOW
 _TENSORFLOW_TENSORBINDING.containing_type = _TENSORFLOW
 _TENSORFLOW_TENSORBINDING.oneofs_by_name['binding'].fields.append(
   _TENSORFLOW_TENSORBINDING.fields_by_name['tensor_name'])
 _TENSORFLOW_TENSORBINDING.fields_by_name['tensor_name'].containing_oneof = _TENSORFLOW_TENSORBINDING.oneofs_by_name['binding']
 _TENSORFLOW_SEQUENCEBINDING.containing_type = _TENSORFLOW
 _TENSORFLOW_SEQUENCEBINDING.oneofs_by_name['binding'].fields.append(
-  _TENSORFLOW_SEQUENCEBINDING.fields_by_name['iterator_string_handle_name'])
-_TENSORFLOW_SEQUENCEBINDING.fields_by_name['iterator_string_handle_name'].containing_oneof = _TENSORFLOW_SEQUENCEBINDING.oneofs_by_name['binding']
-_TENSORFLOW_SEQUENCEBINDING.oneofs_by_name['binding'].fields.append(
   _TENSORFLOW_SEQUENCEBINDING.fields_by_name['variant_tensor_name'])
 _TENSORFLOW_SEQUENCEBINDING.fields_by_name['variant_tensor_name'].containing_oneof = _TENSORFLOW_SEQUENCEBINDING.oneofs_by_name['binding']
 _TENSORFLOW.fields_by_name['graph_def'].message_type = google_dot_protobuf_dot_any__pb2._ANY
 _TENSORFLOW.fields_by_name['parameter'].message_type = _TENSORFLOW_BINDING
 _TENSORFLOW.fields_by_name['result'].message_type = _TENSORFLOW_BINDING
 _LAMBDA.fields_by_name['result'].message_type = _COMPUTATION
 _BLOCK_LOCAL.fields_by_name['value'].message_type = _COMPUTATION
@@ -1627,9 +1617,8 @@
   'DESCRIPTOR' : _DATA,
   '__module__' : 'tensorflow_federated.proto.v0.computation_pb2'
   # @@protoc_insertion_point(class_scope:tensorflow_federated.v0.Data)
   })
 _sym_db.RegisterMessage(Data)
 
 
-_TENSORFLOW_SEQUENCEBINDING.fields_by_name['iterator_string_handle_name']._options = None
 # @@protoc_insertion_point(module_scope)
```

## tensorflow_federated/proto/v0/executor_pb2.py

```diff
@@ -18,21 +18,145 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='tensorflow_federated/proto/v0/executor.proto',
   package='tensorflow_federated.v0',
   syntax='proto3',
   serialized_options=None,
-  serialized_pb=_b('\n,tensorflow_federated/proto/v0/executor.proto\x12\x17tensorflow_federated.v0\x1a\x19google/protobuf/any.proto\x1a/tensorflow_federated/proto/v0/computation.proto\"C\n\x12\x43reateValueRequest\x12-\n\x05value\x18\x01 \x01(\x0b\x32\x1e.tensorflow_federated.v0.Value\"K\n\x13\x43reateValueResponse\x12\x34\n\tvalue_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"\x85\x01\n\x11\x43reateCallRequest\x12\x37\n\x0c\x66unction_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\x12\x37\n\x0c\x61rgument_ref\x18\x02 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"J\n\x12\x43reateCallResponse\x12\x34\n\tvalue_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"\xa9\x01\n\x12\x43reateTupleRequest\x12\x44\n\x07\x65lement\x18\x01 \x03(\x0b\x32\x33.tensorflow_federated.v0.CreateTupleRequest.Element\x1aM\n\x07\x45lement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x34\n\tvalue_ref\x18\x02 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"K\n\x13\x43reateTupleResponse\x12\x34\n\tvalue_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"}\n\x16\x43reateSelectionRequest\x12\x35\n\nsource_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\x12\x0e\n\x04name\x18\x02 \x01(\tH\x00\x12\x0f\n\x05index\x18\x03 \x01(\x05H\x00\x42\x0b\n\tselection\"O\n\x17\x43reateSelectionResponse\x12\x34\n\tvalue_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"F\n\x0e\x43omputeRequest\x12\x34\n\tvalue_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"@\n\x0f\x43omputeResponse\x12-\n\x05value\x18\x01 \x01(\x0b\x32\x1e.tensorflow_federated.v0.Value\"F\n\x0e\x44isposeRequest\x12\x34\n\tvalue_ref\x18\x01 \x03(\x0b\x32!.tensorflow_federated.v0.ValueRef\"\x11\n\x0f\x44isposeResponse\"\xbd\x02\n\x05Value\x12&\n\x06tensor\x18\x01 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x12;\n\x0b\x63omputation\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.ComputationH\x00\x12\x35\n\x05tuple\x18\x03 \x01(\x0b\x32$.tensorflow_federated.v0.Value.TupleH\x00\x1a\x8e\x01\n\x05Tuple\x12=\n\x07\x65lement\x18\x01 \x03(\x0b\x32,.tensorflow_federated.v0.Value.Tuple.Element\x1a\x46\n\x07\x45lement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.tensorflow_federated.v0.ValueB\x07\n\x05value\"\x16\n\x08ValueRef\x12\n\n\x02id\x18\x01 \x01(\t2\x83\x05\n\x08\x45xecutor\x12j\n\x0b\x43reateValue\x12+.tensorflow_federated.v0.CreateValueRequest\x1a,.tensorflow_federated.v0.CreateValueResponse\"\x00\x12g\n\nCreateCall\x12*.tensorflow_federated.v0.CreateCallRequest\x1a+.tensorflow_federated.v0.CreateCallResponse\"\x00\x12j\n\x0b\x43reateTuple\x12+.tensorflow_federated.v0.CreateTupleRequest\x1a,.tensorflow_federated.v0.CreateTupleResponse\"\x00\x12v\n\x0f\x43reateSelection\x12/.tensorflow_federated.v0.CreateSelectionRequest\x1a\x30.tensorflow_federated.v0.CreateSelectionResponse\"\x00\x12^\n\x07\x43ompute\x12\'.tensorflow_federated.v0.ComputeRequest\x1a(.tensorflow_federated.v0.ComputeResponse\"\x00\x12^\n\x07\x44ispose\x12\'.tensorflow_federated.v0.DisposeRequest\x1a(.tensorflow_federated.v0.DisposeResponse\"\x00\x62\x06proto3')
+  serialized_pb=_b('\n,tensorflow_federated/proto/v0/executor.proto\x12\x17tensorflow_federated.v0\x1a\x19google/protobuf/any.proto\x1a/tensorflow_federated/proto/v0/computation.proto\"\xf1\x02\n\x0e\x45xecuteRequest\x12\x43\n\x0c\x63reate_value\x18\x01 \x01(\x0b\x32+.tensorflow_federated.v0.CreateValueRequestH\x00\x12\x41\n\x0b\x63reate_call\x18\x02 \x01(\x0b\x32*.tensorflow_federated.v0.CreateCallRequestH\x00\x12\x43\n\x0c\x63reate_tuple\x18\x03 \x01(\x0b\x32+.tensorflow_federated.v0.CreateTupleRequestH\x00\x12K\n\x10\x63reate_selection\x18\x04 \x01(\x0b\x32/.tensorflow_federated.v0.CreateSelectionRequestH\x00\x12:\n\x07\x63ompute\x18\x05 \x01(\x0b\x32\'.tensorflow_federated.v0.ComputeRequestH\x00\x42\t\n\x07request\"\xf8\x02\n\x0f\x45xecuteResponse\x12\x44\n\x0c\x63reate_value\x18\x01 \x01(\x0b\x32,.tensorflow_federated.v0.CreateValueResponseH\x00\x12\x42\n\x0b\x63reate_call\x18\x02 \x01(\x0b\x32+.tensorflow_federated.v0.CreateCallResponseH\x00\x12\x44\n\x0c\x63reate_tuple\x18\x03 \x01(\x0b\x32,.tensorflow_federated.v0.CreateTupleResponseH\x00\x12L\n\x10\x63reate_selection\x18\x04 \x01(\x0b\x32\x30.tensorflow_federated.v0.CreateSelectionResponseH\x00\x12;\n\x07\x63ompute\x18\x05 \x01(\x0b\x32(.tensorflow_federated.v0.ComputeResponseH\x00\x42\n\n\x08response\"C\n\x12\x43reateValueRequest\x12-\n\x05value\x18\x01 \x01(\x0b\x32\x1e.tensorflow_federated.v0.Value\"K\n\x13\x43reateValueResponse\x12\x34\n\tvalue_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"\x85\x01\n\x11\x43reateCallRequest\x12\x37\n\x0c\x66unction_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\x12\x37\n\x0c\x61rgument_ref\x18\x02 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"J\n\x12\x43reateCallResponse\x12\x34\n\tvalue_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"\xa9\x01\n\x12\x43reateTupleRequest\x12\x44\n\x07\x65lement\x18\x01 \x03(\x0b\x32\x33.tensorflow_federated.v0.CreateTupleRequest.Element\x1aM\n\x07\x45lement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x34\n\tvalue_ref\x18\x02 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"K\n\x13\x43reateTupleResponse\x12\x34\n\tvalue_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"}\n\x16\x43reateSelectionRequest\x12\x35\n\nsource_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\x12\x0e\n\x04name\x18\x02 \x01(\tH\x00\x12\x0f\n\x05index\x18\x03 \x01(\x05H\x00\x42\x0b\n\tselection\"O\n\x17\x43reateSelectionResponse\x12\x34\n\tvalue_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"F\n\x0e\x43omputeRequest\x12\x34\n\tvalue_ref\x18\x01 \x01(\x0b\x32!.tensorflow_federated.v0.ValueRef\"@\n\x0f\x43omputeResponse\x12-\n\x05value\x18\x01 \x01(\x0b\x32\x1e.tensorflow_federated.v0.Value\"F\n\x0e\x44isposeRequest\x12\x34\n\tvalue_ref\x18\x01 \x03(\x0b\x32!.tensorflow_federated.v0.ValueRef\"\x11\n\x0f\x44isposeResponse\"\x93\x05\n\x05Value\x12&\n\x06tensor\x18\x01 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x12;\n\x0b\x63omputation\x18\x02 \x01(\x0b\x32$.tensorflow_federated.v0.ComputationH\x00\x12\x35\n\x05tuple\x18\x03 \x01(\x0b\x32$.tensorflow_federated.v0.Value.TupleH\x00\x12;\n\x08sequence\x18\x04 \x01(\x0b\x32\'.tensorflow_federated.v0.Value.SequenceH\x00\x12=\n\tfederated\x18\x05 \x01(\x0b\x32(.tensorflow_federated.v0.Value.FederatedH\x00\x1a\x8e\x01\n\x05Tuple\x12=\n\x07\x65lement\x18\x01 \x03(\x0b\x32,.tensorflow_federated.v0.Value.Tuple.Element\x1a\x46\n\x07\x45lement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.tensorflow_federated.v0.Value\x1a\x66\n\x08Sequence\x12\x1c\n\x12zipped_saved_model\x18\x01 \x01(\x0cH\x00\x12\x33\n\x0c\x65lement_type\x18\x02 \x01(\x0b\x32\x1d.tensorflow_federated.v0.TypeB\x07\n\x05value\x1ap\n\tFederated\x12\x34\n\x04type\x18\x01 \x01(\x0b\x32&.tensorflow_federated.v0.FederatedType\x12-\n\x05value\x18\x02 \x03(\x0b\x32\x1e.tensorflow_federated.v0.ValueB\x07\n\x05value\"\x16\n\x08ValueRef\x12\n\n\x02id\x18\x01 \x01(\t2\xe7\x05\n\x08\x45xecutor\x12j\n\x0b\x43reateValue\x12+.tensorflow_federated.v0.CreateValueRequest\x1a,.tensorflow_federated.v0.CreateValueResponse\"\x00\x12g\n\nCreateCall\x12*.tensorflow_federated.v0.CreateCallRequest\x1a+.tensorflow_federated.v0.CreateCallResponse\"\x00\x12j\n\x0b\x43reateTuple\x12+.tensorflow_federated.v0.CreateTupleRequest\x1a,.tensorflow_federated.v0.CreateTupleResponse\"\x00\x12v\n\x0f\x43reateSelection\x12/.tensorflow_federated.v0.CreateSelectionRequest\x1a\x30.tensorflow_federated.v0.CreateSelectionResponse\"\x00\x12^\n\x07\x43ompute\x12\'.tensorflow_federated.v0.ComputeRequest\x1a(.tensorflow_federated.v0.ComputeResponse\"\x00\x12^\n\x07\x44ispose\x12\'.tensorflow_federated.v0.DisposeRequest\x1a(.tensorflow_federated.v0.DisposeResponse\"\x00\x12\x62\n\x07\x45xecute\x12\'.tensorflow_federated.v0.ExecuteRequest\x1a(.tensorflow_federated.v0.ExecuteResponse\"\x00(\x01\x30\x01\x62\x06proto3')
   ,
   dependencies=[google_dot_protobuf_dot_any__pb2.DESCRIPTOR,tensorflow__federated_dot_proto_dot_v0_dot_computation__pb2.DESCRIPTOR,])
 
 
 
 
+_EXECUTEREQUEST = _descriptor.Descriptor(
+  name='ExecuteRequest',
+  full_name='tensorflow_federated.v0.ExecuteRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='create_value', full_name='tensorflow_federated.v0.ExecuteRequest.create_value', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='create_call', full_name='tensorflow_federated.v0.ExecuteRequest.create_call', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='create_tuple', full_name='tensorflow_federated.v0.ExecuteRequest.create_tuple', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='create_selection', full_name='tensorflow_federated.v0.ExecuteRequest.create_selection', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='compute', full_name='tensorflow_federated.v0.ExecuteRequest.compute', index=4,
+      number=5, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='request', full_name='tensorflow_federated.v0.ExecuteRequest.request',
+      index=0, containing_type=None, fields=[]),
+  ],
+  serialized_start=150,
+  serialized_end=519,
+)
+
+
+_EXECUTERESPONSE = _descriptor.Descriptor(
+  name='ExecuteResponse',
+  full_name='tensorflow_federated.v0.ExecuteResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='create_value', full_name='tensorflow_federated.v0.ExecuteResponse.create_value', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='create_call', full_name='tensorflow_federated.v0.ExecuteResponse.create_call', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='create_tuple', full_name='tensorflow_federated.v0.ExecuteResponse.create_tuple', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='create_selection', full_name='tensorflow_federated.v0.ExecuteResponse.create_selection', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='compute', full_name='tensorflow_federated.v0.ExecuteResponse.compute', index=4,
+      number=5, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='response', full_name='tensorflow_federated.v0.ExecuteResponse.response',
+      index=0, containing_type=None, fields=[]),
+  ],
+  serialized_start=522,
+  serialized_end=898,
+)
+
+
 _CREATEVALUEREQUEST = _descriptor.Descriptor(
   name='CreateValueRequest',
   full_name='tensorflow_federated.v0.CreateValueRequest',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
@@ -51,16 +175,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=149,
-  serialized_end=216,
+  serialized_start=900,
+  serialized_end=967,
 )
 
 
 _CREATEVALUERESPONSE = _descriptor.Descriptor(
   name='CreateValueResponse',
   full_name='tensorflow_federated.v0.CreateValueResponse',
   filename=None,
@@ -82,16 +206,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=218,
-  serialized_end=293,
+  serialized_start=969,
+  serialized_end=1044,
 )
 
 
 _CREATECALLREQUEST = _descriptor.Descriptor(
   name='CreateCallRequest',
   full_name='tensorflow_federated.v0.CreateCallRequest',
   filename=None,
@@ -120,16 +244,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=296,
-  serialized_end=429,
+  serialized_start=1047,
+  serialized_end=1180,
 )
 
 
 _CREATECALLRESPONSE = _descriptor.Descriptor(
   name='CreateCallResponse',
   full_name='tensorflow_federated.v0.CreateCallResponse',
   filename=None,
@@ -151,16 +275,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=431,
-  serialized_end=505,
+  serialized_start=1182,
+  serialized_end=1256,
 )
 
 
 _CREATETUPLEREQUEST_ELEMENT = _descriptor.Descriptor(
   name='Element',
   full_name='tensorflow_federated.v0.CreateTupleRequest.Element',
   filename=None,
@@ -189,16 +313,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=600,
-  serialized_end=677,
+  serialized_start=1351,
+  serialized_end=1428,
 )
 
 _CREATETUPLEREQUEST = _descriptor.Descriptor(
   name='CreateTupleRequest',
   full_name='tensorflow_federated.v0.CreateTupleRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -219,16 +343,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=508,
-  serialized_end=677,
+  serialized_start=1259,
+  serialized_end=1428,
 )
 
 
 _CREATETUPLERESPONSE = _descriptor.Descriptor(
   name='CreateTupleResponse',
   full_name='tensorflow_federated.v0.CreateTupleResponse',
   filename=None,
@@ -250,16 +374,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=679,
-  serialized_end=754,
+  serialized_start=1430,
+  serialized_end=1505,
 )
 
 
 _CREATESELECTIONREQUEST = _descriptor.Descriptor(
   name='CreateSelectionRequest',
   full_name='tensorflow_federated.v0.CreateSelectionRequest',
   filename=None,
@@ -298,16 +422,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='selection', full_name='tensorflow_federated.v0.CreateSelectionRequest.selection',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=756,
-  serialized_end=881,
+  serialized_start=1507,
+  serialized_end=1632,
 )
 
 
 _CREATESELECTIONRESPONSE = _descriptor.Descriptor(
   name='CreateSelectionResponse',
   full_name='tensorflow_federated.v0.CreateSelectionResponse',
   filename=None,
@@ -329,16 +453,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=883,
-  serialized_end=962,
+  serialized_start=1634,
+  serialized_end=1713,
 )
 
 
 _COMPUTEREQUEST = _descriptor.Descriptor(
   name='ComputeRequest',
   full_name='tensorflow_federated.v0.ComputeRequest',
   filename=None,
@@ -360,16 +484,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=964,
-  serialized_end=1034,
+  serialized_start=1715,
+  serialized_end=1785,
 )
 
 
 _COMPUTERESPONSE = _descriptor.Descriptor(
   name='ComputeResponse',
   full_name='tensorflow_federated.v0.ComputeResponse',
   filename=None,
@@ -391,16 +515,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1036,
-  serialized_end=1100,
+  serialized_start=1787,
+  serialized_end=1851,
 )
 
 
 _DISPOSEREQUEST = _descriptor.Descriptor(
   name='DisposeRequest',
   full_name='tensorflow_federated.v0.DisposeRequest',
   filename=None,
@@ -422,16 +546,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1102,
-  serialized_end=1172,
+  serialized_start=1853,
+  serialized_end=1923,
 )
 
 
 _DISPOSERESPONSE = _descriptor.Descriptor(
   name='DisposeResponse',
   full_name='tensorflow_federated.v0.DisposeResponse',
   filename=None,
@@ -446,16 +570,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1174,
-  serialized_end=1191,
+  serialized_start=1925,
+  serialized_end=1942,
 )
 
 
 _VALUE_TUPLE_ELEMENT = _descriptor.Descriptor(
   name='Element',
   full_name='tensorflow_federated.v0.Value.Tuple.Element',
   filename=None,
@@ -484,16 +608,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1432,
-  serialized_end=1502,
+  serialized_start=2307,
+  serialized_end=2377,
 )
 
 _VALUE_TUPLE = _descriptor.Descriptor(
   name='Tuple',
   full_name='tensorflow_federated.v0.Value.Tuple',
   filename=None,
   file=DESCRIPTOR,
@@ -514,16 +638,93 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1360,
-  serialized_end=1502,
+  serialized_start=2235,
+  serialized_end=2377,
+)
+
+_VALUE_SEQUENCE = _descriptor.Descriptor(
+  name='Sequence',
+  full_name='tensorflow_federated.v0.Value.Sequence',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='zipped_saved_model', full_name='tensorflow_federated.v0.Value.Sequence.zipped_saved_model', index=0,
+      number=1, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b(""),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='element_type', full_name='tensorflow_federated.v0.Value.Sequence.element_type', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='value', full_name='tensorflow_federated.v0.Value.Sequence.value',
+      index=0, containing_type=None, fields=[]),
+  ],
+  serialized_start=2379,
+  serialized_end=2481,
+)
+
+_VALUE_FEDERATED = _descriptor.Descriptor(
+  name='Federated',
+  full_name='tensorflow_federated.v0.Value.Federated',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='tensorflow_federated.v0.Value.Federated.type', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='tensorflow_federated.v0.Value.Federated.value', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2483,
+  serialized_end=2595,
 )
 
 _VALUE = _descriptor.Descriptor(
   name='Value',
   full_name='tensorflow_federated.v0.Value',
   filename=None,
   file=DESCRIPTOR,
@@ -546,31 +747,45 @@
     _descriptor.FieldDescriptor(
       name='tuple', full_name='tensorflow_federated.v0.Value.tuple', index=2,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='sequence', full_name='tensorflow_federated.v0.Value.sequence', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='federated', full_name='tensorflow_federated.v0.Value.federated', index=4,
+      number=5, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
-  nested_types=[_VALUE_TUPLE, ],
+  nested_types=[_VALUE_TUPLE, _VALUE_SEQUENCE, _VALUE_FEDERATED, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='value', full_name='tensorflow_federated.v0.Value.value',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=1194,
-  serialized_end=1511,
+  serialized_start=1945,
+  serialized_end=2604,
 )
 
 
 _VALUEREF = _descriptor.Descriptor(
   name='ValueRef',
   full_name='tensorflow_federated.v0.ValueRef',
   filename=None,
@@ -592,18 +807,58 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1513,
-  serialized_end=1535,
+  serialized_start=2606,
+  serialized_end=2628,
 )
 
+_EXECUTEREQUEST.fields_by_name['create_value'].message_type = _CREATEVALUEREQUEST
+_EXECUTEREQUEST.fields_by_name['create_call'].message_type = _CREATECALLREQUEST
+_EXECUTEREQUEST.fields_by_name['create_tuple'].message_type = _CREATETUPLEREQUEST
+_EXECUTEREQUEST.fields_by_name['create_selection'].message_type = _CREATESELECTIONREQUEST
+_EXECUTEREQUEST.fields_by_name['compute'].message_type = _COMPUTEREQUEST
+_EXECUTEREQUEST.oneofs_by_name['request'].fields.append(
+  _EXECUTEREQUEST.fields_by_name['create_value'])
+_EXECUTEREQUEST.fields_by_name['create_value'].containing_oneof = _EXECUTEREQUEST.oneofs_by_name['request']
+_EXECUTEREQUEST.oneofs_by_name['request'].fields.append(
+  _EXECUTEREQUEST.fields_by_name['create_call'])
+_EXECUTEREQUEST.fields_by_name['create_call'].containing_oneof = _EXECUTEREQUEST.oneofs_by_name['request']
+_EXECUTEREQUEST.oneofs_by_name['request'].fields.append(
+  _EXECUTEREQUEST.fields_by_name['create_tuple'])
+_EXECUTEREQUEST.fields_by_name['create_tuple'].containing_oneof = _EXECUTEREQUEST.oneofs_by_name['request']
+_EXECUTEREQUEST.oneofs_by_name['request'].fields.append(
+  _EXECUTEREQUEST.fields_by_name['create_selection'])
+_EXECUTEREQUEST.fields_by_name['create_selection'].containing_oneof = _EXECUTEREQUEST.oneofs_by_name['request']
+_EXECUTEREQUEST.oneofs_by_name['request'].fields.append(
+  _EXECUTEREQUEST.fields_by_name['compute'])
+_EXECUTEREQUEST.fields_by_name['compute'].containing_oneof = _EXECUTEREQUEST.oneofs_by_name['request']
+_EXECUTERESPONSE.fields_by_name['create_value'].message_type = _CREATEVALUERESPONSE
+_EXECUTERESPONSE.fields_by_name['create_call'].message_type = _CREATECALLRESPONSE
+_EXECUTERESPONSE.fields_by_name['create_tuple'].message_type = _CREATETUPLERESPONSE
+_EXECUTERESPONSE.fields_by_name['create_selection'].message_type = _CREATESELECTIONRESPONSE
+_EXECUTERESPONSE.fields_by_name['compute'].message_type = _COMPUTERESPONSE
+_EXECUTERESPONSE.oneofs_by_name['response'].fields.append(
+  _EXECUTERESPONSE.fields_by_name['create_value'])
+_EXECUTERESPONSE.fields_by_name['create_value'].containing_oneof = _EXECUTERESPONSE.oneofs_by_name['response']
+_EXECUTERESPONSE.oneofs_by_name['response'].fields.append(
+  _EXECUTERESPONSE.fields_by_name['create_call'])
+_EXECUTERESPONSE.fields_by_name['create_call'].containing_oneof = _EXECUTERESPONSE.oneofs_by_name['response']
+_EXECUTERESPONSE.oneofs_by_name['response'].fields.append(
+  _EXECUTERESPONSE.fields_by_name['create_tuple'])
+_EXECUTERESPONSE.fields_by_name['create_tuple'].containing_oneof = _EXECUTERESPONSE.oneofs_by_name['response']
+_EXECUTERESPONSE.oneofs_by_name['response'].fields.append(
+  _EXECUTERESPONSE.fields_by_name['create_selection'])
+_EXECUTERESPONSE.fields_by_name['create_selection'].containing_oneof = _EXECUTERESPONSE.oneofs_by_name['response']
+_EXECUTERESPONSE.oneofs_by_name['response'].fields.append(
+  _EXECUTERESPONSE.fields_by_name['compute'])
+_EXECUTERESPONSE.fields_by_name['compute'].containing_oneof = _EXECUTERESPONSE.oneofs_by_name['response']
 _CREATEVALUEREQUEST.fields_by_name['value'].message_type = _VALUE
 _CREATEVALUERESPONSE.fields_by_name['value_ref'].message_type = _VALUEREF
 _CREATECALLREQUEST.fields_by_name['function_ref'].message_type = _VALUEREF
 _CREATECALLREQUEST.fields_by_name['argument_ref'].message_type = _VALUEREF
 _CREATECALLRESPONSE.fields_by_name['value_ref'].message_type = _VALUEREF
 _CREATETUPLEREQUEST_ELEMENT.fields_by_name['value_ref'].message_type = _VALUEREF
 _CREATETUPLEREQUEST_ELEMENT.containing_type = _CREATETUPLEREQUEST
@@ -620,26 +875,44 @@
 _COMPUTEREQUEST.fields_by_name['value_ref'].message_type = _VALUEREF
 _COMPUTERESPONSE.fields_by_name['value'].message_type = _VALUE
 _DISPOSEREQUEST.fields_by_name['value_ref'].message_type = _VALUEREF
 _VALUE_TUPLE_ELEMENT.fields_by_name['value'].message_type = _VALUE
 _VALUE_TUPLE_ELEMENT.containing_type = _VALUE_TUPLE
 _VALUE_TUPLE.fields_by_name['element'].message_type = _VALUE_TUPLE_ELEMENT
 _VALUE_TUPLE.containing_type = _VALUE
+_VALUE_SEQUENCE.fields_by_name['element_type'].message_type = tensorflow__federated_dot_proto_dot_v0_dot_computation__pb2._TYPE
+_VALUE_SEQUENCE.containing_type = _VALUE
+_VALUE_SEQUENCE.oneofs_by_name['value'].fields.append(
+  _VALUE_SEQUENCE.fields_by_name['zipped_saved_model'])
+_VALUE_SEQUENCE.fields_by_name['zipped_saved_model'].containing_oneof = _VALUE_SEQUENCE.oneofs_by_name['value']
+_VALUE_FEDERATED.fields_by_name['type'].message_type = tensorflow__federated_dot_proto_dot_v0_dot_computation__pb2._FEDERATEDTYPE
+_VALUE_FEDERATED.fields_by_name['value'].message_type = _VALUE
+_VALUE_FEDERATED.containing_type = _VALUE
 _VALUE.fields_by_name['tensor'].message_type = google_dot_protobuf_dot_any__pb2._ANY
 _VALUE.fields_by_name['computation'].message_type = tensorflow__federated_dot_proto_dot_v0_dot_computation__pb2._COMPUTATION
 _VALUE.fields_by_name['tuple'].message_type = _VALUE_TUPLE
+_VALUE.fields_by_name['sequence'].message_type = _VALUE_SEQUENCE
+_VALUE.fields_by_name['federated'].message_type = _VALUE_FEDERATED
 _VALUE.oneofs_by_name['value'].fields.append(
   _VALUE.fields_by_name['tensor'])
 _VALUE.fields_by_name['tensor'].containing_oneof = _VALUE.oneofs_by_name['value']
 _VALUE.oneofs_by_name['value'].fields.append(
   _VALUE.fields_by_name['computation'])
 _VALUE.fields_by_name['computation'].containing_oneof = _VALUE.oneofs_by_name['value']
 _VALUE.oneofs_by_name['value'].fields.append(
   _VALUE.fields_by_name['tuple'])
 _VALUE.fields_by_name['tuple'].containing_oneof = _VALUE.oneofs_by_name['value']
+_VALUE.oneofs_by_name['value'].fields.append(
+  _VALUE.fields_by_name['sequence'])
+_VALUE.fields_by_name['sequence'].containing_oneof = _VALUE.oneofs_by_name['value']
+_VALUE.oneofs_by_name['value'].fields.append(
+  _VALUE.fields_by_name['federated'])
+_VALUE.fields_by_name['federated'].containing_oneof = _VALUE.oneofs_by_name['value']
+DESCRIPTOR.message_types_by_name['ExecuteRequest'] = _EXECUTEREQUEST
+DESCRIPTOR.message_types_by_name['ExecuteResponse'] = _EXECUTERESPONSE
 DESCRIPTOR.message_types_by_name['CreateValueRequest'] = _CREATEVALUEREQUEST
 DESCRIPTOR.message_types_by_name['CreateValueResponse'] = _CREATEVALUERESPONSE
 DESCRIPTOR.message_types_by_name['CreateCallRequest'] = _CREATECALLREQUEST
 DESCRIPTOR.message_types_by_name['CreateCallResponse'] = _CREATECALLRESPONSE
 DESCRIPTOR.message_types_by_name['CreateTupleRequest'] = _CREATETUPLEREQUEST
 DESCRIPTOR.message_types_by_name['CreateTupleResponse'] = _CREATETUPLERESPONSE
 DESCRIPTOR.message_types_by_name['CreateSelectionRequest'] = _CREATESELECTIONREQUEST
@@ -648,14 +921,28 @@
 DESCRIPTOR.message_types_by_name['ComputeResponse'] = _COMPUTERESPONSE
 DESCRIPTOR.message_types_by_name['DisposeRequest'] = _DISPOSEREQUEST
 DESCRIPTOR.message_types_by_name['DisposeResponse'] = _DISPOSERESPONSE
 DESCRIPTOR.message_types_by_name['Value'] = _VALUE
 DESCRIPTOR.message_types_by_name['ValueRef'] = _VALUEREF
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
+ExecuteRequest = _reflection.GeneratedProtocolMessageType('ExecuteRequest', (_message.Message,), {
+  'DESCRIPTOR' : _EXECUTEREQUEST,
+  '__module__' : 'tensorflow_federated.proto.v0.executor_pb2'
+  # @@protoc_insertion_point(class_scope:tensorflow_federated.v0.ExecuteRequest)
+  })
+_sym_db.RegisterMessage(ExecuteRequest)
+
+ExecuteResponse = _reflection.GeneratedProtocolMessageType('ExecuteResponse', (_message.Message,), {
+  'DESCRIPTOR' : _EXECUTERESPONSE,
+  '__module__' : 'tensorflow_federated.proto.v0.executor_pb2'
+  # @@protoc_insertion_point(class_scope:tensorflow_federated.v0.ExecuteResponse)
+  })
+_sym_db.RegisterMessage(ExecuteResponse)
+
 CreateValueRequest = _reflection.GeneratedProtocolMessageType('CreateValueRequest', (_message.Message,), {
   'DESCRIPTOR' : _CREATEVALUEREQUEST,
   '__module__' : 'tensorflow_federated.proto.v0.executor_pb2'
   # @@protoc_insertion_point(class_scope:tensorflow_federated.v0.CreateValueRequest)
   })
 _sym_db.RegisterMessage(CreateValueRequest)
 
@@ -755,21 +1042,37 @@
       })
     ,
     'DESCRIPTOR' : _VALUE_TUPLE,
     '__module__' : 'tensorflow_federated.proto.v0.executor_pb2'
     # @@protoc_insertion_point(class_scope:tensorflow_federated.v0.Value.Tuple)
     })
   ,
+
+  'Sequence' : _reflection.GeneratedProtocolMessageType('Sequence', (_message.Message,), {
+    'DESCRIPTOR' : _VALUE_SEQUENCE,
+    '__module__' : 'tensorflow_federated.proto.v0.executor_pb2'
+    # @@protoc_insertion_point(class_scope:tensorflow_federated.v0.Value.Sequence)
+    })
+  ,
+
+  'Federated' : _reflection.GeneratedProtocolMessageType('Federated', (_message.Message,), {
+    'DESCRIPTOR' : _VALUE_FEDERATED,
+    '__module__' : 'tensorflow_federated.proto.v0.executor_pb2'
+    # @@protoc_insertion_point(class_scope:tensorflow_federated.v0.Value.Federated)
+    })
+  ,
   'DESCRIPTOR' : _VALUE,
   '__module__' : 'tensorflow_federated.proto.v0.executor_pb2'
   # @@protoc_insertion_point(class_scope:tensorflow_federated.v0.Value)
   })
 _sym_db.RegisterMessage(Value)
 _sym_db.RegisterMessage(Value.Tuple)
 _sym_db.RegisterMessage(Value.Tuple.Element)
+_sym_db.RegisterMessage(Value.Sequence)
+_sym_db.RegisterMessage(Value.Federated)
 
 ValueRef = _reflection.GeneratedProtocolMessageType('ValueRef', (_message.Message,), {
   'DESCRIPTOR' : _VALUEREF,
   '__module__' : 'tensorflow_federated.proto.v0.executor_pb2'
   # @@protoc_insertion_point(class_scope:tensorflow_federated.v0.ValueRef)
   })
 _sym_db.RegisterMessage(ValueRef)
@@ -778,16 +1081,16 @@
 
 _EXECUTOR = _descriptor.ServiceDescriptor(
   name='Executor',
   full_name='tensorflow_federated.v0.Executor',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=1538,
-  serialized_end=2181,
+  serialized_start=2631,
+  serialized_end=3374,
   methods=[
   _descriptor.MethodDescriptor(
     name='CreateValue',
     full_name='tensorflow_federated.v0.Executor.CreateValue',
     index=0,
     containing_service=None,
     input_type=_CREATEVALUEREQUEST,
@@ -835,13 +1138,22 @@
     full_name='tensorflow_federated.v0.Executor.Dispose',
     index=5,
     containing_service=None,
     input_type=_DISPOSEREQUEST,
     output_type=_DISPOSERESPONSE,
     serialized_options=None,
   ),
+  _descriptor.MethodDescriptor(
+    name='Execute',
+    full_name='tensorflow_federated.v0.Executor.Execute',
+    index=6,
+    containing_service=None,
+    input_type=_EXECUTEREQUEST,
+    output_type=_EXECUTERESPONSE,
+    serialized_options=None,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_EXECUTOR)
 
 DESCRIPTOR.services_by_name['Executor'] = _EXECUTOR
 
 # @@protoc_insertion_point(module_scope)
```

## tensorflow_federated/proto/v0/executor_pb2_grpc.py

```diff
@@ -40,14 +40,19 @@
         response_deserializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.ComputeResponse.FromString,
         )
     self.Dispose = channel.unary_unary(
         '/tensorflow_federated.v0.Executor/Dispose',
         request_serializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.DisposeRequest.SerializeToString,
         response_deserializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.DisposeResponse.FromString,
         )
+    self.Execute = channel.stream_stream(
+        '/tensorflow_federated.v0.Executor/Execute',
+        request_serializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.ExecuteRequest.SerializeToString,
+        response_deserializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.ExecuteResponse.FromString,
+        )
 
 
 class ExecutorServicer(object):
   """A service interface to be implemented by executors.
   """
 
   def CreateValue(self, request, context):
@@ -96,14 +101,21 @@
     Causes one or more values in the executor to get disposed of (no longer
     available for future calls).
     """
     context.set_code(grpc.StatusCode.UNIMPLEMENTED)
     context.set_details('Method not implemented!')
     raise NotImplementedError('Method not implemented!')
 
+  def Execute(self, request_iterator, context):
+    """Establishes a bidirectional stream with an Executor instance.
+    """
+    context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+    context.set_details('Method not implemented!')
+    raise NotImplementedError('Method not implemented!')
+
 
 def add_ExecutorServicer_to_server(servicer, server):
   rpc_method_handlers = {
       'CreateValue': grpc.unary_unary_rpc_method_handler(
           servicer.CreateValue,
           request_deserializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.CreateValueRequest.FromString,
           response_serializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.CreateValueResponse.SerializeToString,
@@ -129,11 +141,16 @@
           response_serializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.ComputeResponse.SerializeToString,
       ),
       'Dispose': grpc.unary_unary_rpc_method_handler(
           servicer.Dispose,
           request_deserializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.DisposeRequest.FromString,
           response_serializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.DisposeResponse.SerializeToString,
       ),
+      'Execute': grpc.stream_stream_rpc_method_handler(
+          servicer.Execute,
+          request_deserializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.ExecuteRequest.FromString,
+          response_serializer=tensorflow__federated_dot_proto_dot_v0_dot_executor__pb2.ExecuteResponse.SerializeToString,
+      ),
   }
   generic_handler = grpc.method_handlers_generic_handler(
       'tensorflow_federated.v0.Executor', rpc_method_handlers)
   server.add_generic_rpc_handlers((generic_handler,))
```

## tensorflow_federated/python/common_libs/anonymous_tuple.py

```diff
@@ -33,15 +33,15 @@
 
   Anonymous tuples are similar to named tuples, in that their elements can be
   accessed by name or by index, but unlike `collections.namedtuple`, they can
   be instantiated without having to explicitly construct a new class for each
   instance, which incurs unnecessary overhead. Anonymous tuples are thus
   related to `collections.namedtuples` much in the same way anonymous lambdas
   are related to named functions explicitly declared with `def`. One of the
-  intended uses of annoymous tuples is to represent structured parameters in
+  intended uses of anonymous tuples is to represent structured parameters in
   computations defined as Python functions or TF defuns.
 
   Example:
 
   ```python
   x = AnonymousTuple([('foo', 10), (None, 20), ('bar', 30)])
 
@@ -57,15 +57,15 @@
 
   Note that in general, naming the members of these tuples is optional. Thus,
   an `AnonymousTuple` can be used just like an ordinary positional tuple.
 
   Also note that the user will not be creating such tuples. They are a hidden
   part of the impementation designed to work together with function decorators.
   """
-  __slots__ = ('_hash', '_element_array', '_name_to_index')
+  __slots__ = ('_hash', '_element_array', '_name_to_index', '_name_array')
 
   # TODO(b/113112108): Define more magic methods for convenience in handling
   # anonymous tuples. Possibly move out to a more generic location or replace
   # with pre-existing type if a sufficiently widely used one can be found.
   def __init__(self, elements):
     """Constructs a new anonymous named tuple with the given elements.
 
@@ -79,28 +79,33 @@
         the list is not a pair with a string at the first position.
     """
     py_typecheck.check_type(elements, list)
     for e in elements:
       if not py_typecheck.is_name_value_pair(e, name_required=False):
         raise TypeError(
             'Expected every item on the list to be a pair in which the first '
-            'element is a string, found {}.'.format(repr(e)))
+            'element is a string, found {!r}.'.format(e))
 
     self._element_array = tuple(e[1] for e in elements)
     self._name_to_index = {}
+    self._name_array = []
+    reserved_names = ('_asdict',) + AnonymousTuple.__slots__
     for idx, e in enumerate(elements):
       name = e[0]
+      self._name_array.append(name)
       if name is None:
         continue
-      if name == '_asdict':
-        raise ValueError('The name "_asdict" is reserved for a method, '
-                         'as with namedtuples.')
+      if name in reserved_names:
+        raise ValueError(
+            'The names in {} are reserved. You passed the name {}.'.format(
+                reserved_names, name))
       elif name in self._name_to_index:
-        raise ValueError('AnonymousTuple does not support duplicated '
-                         'names, but found ' + str([e[0] for e in elements]))
+        raise ValueError(
+            'AnonymousTuple does not support duplicated names, but found {}'
+            .format([e[0] for e in elements]))
       self._name_to_index[name] = idx
     self._hash = None
 
   def __len__(self):
     return len(self._element_array)
 
   def __iter__(self):
@@ -119,56 +124,70 @@
 
   def __getitem__(self, key):
     py_typecheck.check_type(key, (int, slice))
     if isinstance(key, int):
       if key < 0 or key >= len(self._element_array):
         raise IndexError(
             'Element index {} is out of range, tuple has {} elements.'.format(
-                str(key), str(len(self._element_array))))
+                key, len(self._element_array)))
     return self._element_array[key]
 
   def __getattr__(self, name):
     if name not in self._name_to_index:
       raise AttributeError(
-          'The tuple of length {:d} does not have named field "{!s}".'
-          'Names (only first 10): {!s}'.format(
+          'The tuple of length {:d} does not have named field "{!s}". '
+          'Fields (up to first 10): {!s}'.format(
               len(self._element_array), name,
               list(self._name_to_index.keys())[:10]))
     return self._element_array[self._name_to_index[name]]
 
   def __eq__(self, other):
+    if self is other:
+      return True
     # pylint: disable=protected-access
     return (isinstance(other, AnonymousTuple) and
             (self._element_array == other._element_array) and
-            (self._name_to_index == other._name_to_index))
+            (self._name_array == other._name_array))
     # pylint: enable=protected-access
 
   def __ne__(self, other):
     return not self == other
 
   def __repr__(self):
     return 'AnonymousTuple([{}])'.format(', '.join(
-        '({}, {})'.format(e[0], repr(e[1])) for e in to_elements(self)))
+        '({!r}, {!r})'.format(n, v) for n, v in to_elements(self)))
 
   def __str__(self):
-    return '<{}>'.format(','.join(
-        ('{}={}'.format(e[0], str(e[1])) if e[0] is not None else str(e[1]))
-        for e in to_elements(self)))
+
+    def _element_str(element):
+      name, value = element
+      if name is not None:
+        return '{}={}'.format(name, value)
+      return str(value)
+
+    return '<{}>'.format(','.join(_element_str(e) for e in to_elements(self)))
 
   def __hash__(self):
     if self._hash is None:
       self._hash = hash((
           'anonymous_tuple',  # salting to avoid type mismatch.
           self._element_array,
-          tuple(self._name_to_index.items())))
+          tuple(self._name_array)))
     return self._hash
 
-  def _asdict(self):
-    """Returns an OrderedDict which maps field names to their values."""
-    return to_odict(self)
+  def _asdict(self, recursive=False):
+    """Returns an OrderedDict which maps field names to their values.
+
+    Args:
+      recursive: Whether to convert nested AnonymousTuples recursively.
+
+    Returns:
+      An `OrderedDict`.
+    """
+    return to_odict(self, recursive=recursive)
 
 
 def to_elements(an_anonymous_tuple):
   """Retrieves the list of (name, value) pairs from an anonymous tuple.
 
   Modeled as a module function rather than a method of `AnonymousTuple` to avoid
   naming conflicts with the tuple attributes, and so as not to expose the user
@@ -182,42 +201,71 @@
     the format that's accepted by the tuple constructor.
 
   Raises:
     TypeError: if the argument is not an `AnonymousTuple`.
   """
   py_typecheck.check_type(an_anonymous_tuple, AnonymousTuple)
   # pylint: disable=protected-access
-  index_to_name = {
-      idx: name
-      for name, idx in six.iteritems(an_anonymous_tuple._name_to_index)
-  }
-  return [(index_to_name.get(idx), val)
-          for idx, val in enumerate(an_anonymous_tuple._element_array)]
+  return list(
+      zip(an_anonymous_tuple._name_array, an_anonymous_tuple._element_array))
+  # pylint: enable=protected-access
+
+
+def iter_elements(an_anonymous_tuple):
+  """Generates the list of (name, value) pairs from an anonymous tuple.
+
+  Modeled as a module function rather than a method of `AnonymousTuple` to avoid
+  naming conflicts with the tuple attributes, and so as not to expose the user
+  to this implementation-oriented functionality.
+
+  Args:
+    an_anonymous_tuple: An instance of `AnonymousTuple`.
+
+  Yields:
+    A 2-tuple of name, value pairs, representing the elements of
+      `an_anonymous_tuple`.
+
+  Raises:
+    TypeError: if the argument is not an `AnonymousTuple`.
+  """
+  py_typecheck.check_type(an_anonymous_tuple, AnonymousTuple)
+  # pylint: disable=protected-access
+  for name, val in zip(an_anonymous_tuple._name_array,
+                       an_anonymous_tuple._element_array):
+    yield (name, val)
   # pylint: enable=protected-access
 
 
-def to_odict(anon_tuple):
+def to_odict(anon_tuple, recursive=False):
   """Returns anon_tuple as an `OrderedDict`, if possible.
 
   Args:
     anon_tuple: An `AnonymousTuple`.
+    recursive: Whether to convert nested AnonymousTuples recursively.
 
   Raises:
     ValueError: If the anonymous tuple contains unnamed elements.
 
   Returns:
     An `OrderedDict`.
   """
   py_typecheck.check_type(anon_tuple, AnonymousTuple)
-  elements = to_elements(anon_tuple)
-  for name, _ in elements:
-    if name is None:
-      raise ValueError('Can\'t convert an AnonymousTuple with unnamed '
-                       'entries to an OrderedDict:\n' + str(anon_tuple))
-  return collections.OrderedDict(elements)
+
+  def _to_odict(elements):
+    for name, _ in elements:
+      if name is None:
+        raise ValueError(
+            'Can\'t convert an AnonymousTuple with unnamed entries to an '
+            'OrderedDict: {}'.format(anon_tuple))
+    return collections.OrderedDict(elements)
+
+  if recursive:
+    return to_container_recursive(anon_tuple, _to_odict)
+  else:
+    return _to_odict(to_elements(anon_tuple))
 
 
 def flatten(structure):
   """Returns a list of values in a possibly recursively nested tuple.
 
   N.B. This implementation is not compatible with the approach of
   `tf.nest.flatten`, which enforces lexical order for `OrderedDict`s.
@@ -413,7 +461,40 @@
       raise TypeError('Unable to convert a Python object of type {} into '
                       'an `AnonymousTuple`.'.format(
                           py_typecheck.type_string(type(value))))
     else:
       return value
 
   return _convert(value, recursive, must_be_container=True)
+
+
+def to_container_recursive(value, container_fn):
+  """Recursively converts the AnonymousTuple `value` to a new container type.
+
+  This function is always recursive, since the non-recursive version would
+  be just `container_fn(value)`.
+
+  Note this function will only recurse through `AnonymousTuple`s, so if called
+  on the input
+  `AnonymousTuple([('a', 1), ('b', {'c': AnonymousTuple(...)})])`
+  the inner `AnonymousTuple` will not be converted, because we do not
+  recurse through Python dictionaries.
+
+  Args:
+    value: An `AnonymousTuple`, possibly nested.
+    container_fn: A function that takes a `list` of `(name, value)` tuples ( the
+      elements of an `AnonymousTuple`), and returns a new container holding the
+      same values.
+
+  Returns:
+    A nested container of the type returned by `container_fn`.
+  """
+  py_typecheck.check_type(value, AnonymousTuple)
+  py_typecheck.check_callable(container_fn)
+
+  def recurse(v):
+    if isinstance(v, AnonymousTuple):
+      return to_container_recursive(v, container_fn)
+    else:
+      return v
+
+  return container_fn([(k, recurse(v)) for k, v in to_elements(value)])
```

## tensorflow_federated/python/common_libs/py_typecheck.py

```diff
@@ -225,7 +225,23 @@
     return False
   if ((name_required or element[0] is not None) and
       not isinstance(element[0], six.string_types)):
     return False
   if value_type is not None and not isinstance(element[1], value_type):
     return False
   return True
+
+
+def check_len(target, length):
+  """Checks that the length of `target` is equal to `length`.
+
+  Args:
+    target: The object to check.
+    length: The expected length.
+
+  Raises:
+    ValueError: If the lengths do not match.
+  """
+  if len(target) != length:
+    raise ValueError(
+        'Expected an argument of length {}, got one of length {} ({}).'.format(
+            length, len(target), target))
```

## tensorflow_federated/python/common_libs/serialization_utils.py

```diff
@@ -19,14 +19,32 @@
 from __future__ import print_function
 
 import tensorflow as tf
 
 from google.protobuf import any_pb2
 from tensorflow_federated.python.common_libs import py_typecheck
 
+# The default seed below matches the seed in
+# `tensorflow/python/framework/random_seed.py`; this is an unexported symbol, so
+# replicating here. If this seed is broken, likely something major has changed
+# in TensorFlow, so it may be preferable to contact TensorFlow before attempting
+# serious debugging.
+DEFAULT_GRAPH_SEED = 87654321
+
+
+def _check_no_graph_level_seed(graph_def):
+  for x in graph_def.node:
+    seed_attr = x.attr.get('seed')
+    seed2_attr = x.attr.get('seed2')
+    if seed_attr is not None and not (seed_attr.i == DEFAULT_GRAPH_SEED or
+                                      (seed_attr.i == 0 and seed2_attr.i == 0)):
+      raise ValueError(
+          'TFF disallows the setting of a graph-level random seed. See the '
+          'FAQ for more details on reasoning and preferred randomness in TFF.')
+
 
 def pack_graph_def(graph_def):
   """Pack a `tf.compat.v1.GraphDef` into a proto3 `Any` message.
 
   Args:
     graph_def: the `tf.compat.v1.GraphDef` to pack into a protocol buffer
       message.
@@ -34,14 +52,15 @@
   Returns:
     A `google.protobuf.Any` protocol buffer message.
 
   Raises:
     TypeError: if `graph_def` is not a `tf.compat.v1.GraphDef`.
   """
   py_typecheck.check_type(graph_def, tf.compat.v1.GraphDef)
+  _check_no_graph_level_seed(graph_def)
   any_pb = any_pb2.Any()
   any_pb.Pack(graph_def)
   return any_pb
 
 
 def unpack_graph_def(any_pb):
   """Unpacks a proto3 `Any` message to a `tf.compat.v1.GraphDef`.
```

## tensorflow_federated/python/core/__init__.py

```diff
@@ -46,9 +46,10 @@
 from tensorflow_federated.python.core.api.typed_object import TypedObject
 from tensorflow_federated.python.core.api.value_base import Value
 from tensorflow_federated.python.core.api.values import to_value
 
 # NOTE: These imports must happen after the API imports.
 # pylint: disable=g-bad-import-order
 from tensorflow_federated.python.core import framework
+from tensorflow_federated.python.core import backends
 from tensorflow_federated.python.core import utils
 # pylint: enable=g-bad-import-order
```

## tensorflow_federated/python/core/api/computation_types.py

```diff
@@ -23,30 +23,38 @@
 
 import attr
 import six
 import tensorflow as tf
 
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
-from tensorflow_federated.python.core.impl import placement_literals
+from tensorflow_federated.python.core.impl.compiler import placement_literals
 from tensorflow_federated.python.tensorflow_libs import tensor_utils
 
 
 @six.add_metaclass(abc.ABCMeta)
 class Type(object):
   """An abstract interface for all classes that represent TFF types."""
 
+  def compact_representation(self):
+    """Returns the compact string representation of this type."""
+    return _string_representation(self, formatted=False)
+
+  def formatted_representation(self):
+    """Returns the formatted string representation of this type."""
+    return _string_representation(self, formatted=True)
+
   @abc.abstractmethod
   def __repr__(self):
     """Returns a full-form representation of this type."""
     raise NotImplementedError
 
   def __str__(self):
     """Returns a concise representation of this type."""
-    return compact_representation(self)
+    return self.compact_representation()
 
   @abc.abstractmethod
   def __eq__(self, other):
     """Determines whether two type definitions are identical.
 
     Note that this notion of equality is stronger than equivalence. Two types
     with equivalent definitions may not be identical, e.g., if they represent
@@ -74,15 +82,16 @@
   def __init__(self, dtype, shape=None):
     """Constructs a new instance from the given `dtype` and `shape`.
 
     Args:
       dtype: An instance of `tf.DType`.
       shape: An optional instance of `tf.TensorShape` or an argument that can be
         passed to its constructor (such as a `list` or a `tuple`), or `None` for
-        the default scalar shape. Unspecified shapes are not supported.
+        the default scalar shape. TensorShapes with unknown rank are not
+        supported.
 
     Raises:
       TypeError: if arguments are of the wrong types.
     """
     py_typecheck.check_type(dtype, tf.DType)
     self._dtype = dtype
     # TODO(b/123764922): If we are passed a shape of `TensorShape(None)`, which
@@ -106,28 +115,32 @@
 
   @property
   def shape(self):
     return self._shape
 
   def __repr__(self):
     if self._shape.ndims is None:
-      return 'TensorType({}, {})'.format(repr(self._dtype), None)
+      return 'TensorType({!r}, {})'.format(self._dtype, None)
     elif self._shape.ndims > 0:
-      values = repr([dim.value for dim in self._shape.dims])
-      return 'TensorType({}, {})'.format(repr(self._dtype), values)
+      values = [dim.value for dim in self._shape.dims]
+      return 'TensorType({!r}, {!r})'.format(self._dtype, values)
     else:
-      return 'TensorType({})'.format(repr(self._dtype))
+      return 'TensorType({!r})'.format(self._dtype)
 
   def __eq__(self, other):
     return (isinstance(other, TensorType) and self._dtype == other.dtype and
             tensor_utils.same_shape(self._shape, other.shape))
 
 
 class NamedTupleType(anonymous_tuple.AnonymousTuple, Type):
-  """An implementation of `tff.Type` representing named tuple types in TFF."""
+  """An implementation of `tff.Type` representing named tuple types in TFF.
+
+  Elements initialized by name can be accessed as `foo.name`, and otherwise by
+  index, `foo[index]`.
+  """
 
   def __init__(self, elements):
     """Constructs a new instance from the given element types.
 
     Args:
       elements: Element specifications, in the format of a `list`, `tuple`, or
         `collections.OrderedDict`. Each element specification is either a type
@@ -159,22 +172,22 @@
     else:
       elements = [_map_element(e) for e in elements]
 
     anonymous_tuple.AnonymousTuple.__init__(self, elements)
 
   def __repr__(self):
 
-    def _element_repr(e):
-      if e[0] is not None:
-        return '(\'{}\', {})'.format(e[0], repr(e[1]))
-      else:
-        return repr(e[1])
+    def _element_repr(element):
+      name, value = element
+      if name is not None:
+        return '(\'{}\', {!r})'.format(name, value)
+      return repr(value)
 
     return 'NamedTupleType([{}])'.format(', '.join(
-        [_element_repr(e) for e in anonymous_tuple.to_elements(self)]))
+        _element_repr(e) for e in anonymous_tuple.iter_elements(self)))
 
   def __eq__(self, other):
     return (isinstance(other, NamedTupleType) and
             super(NamedTupleType, self).__eq__(other))
 
 
 # While this lives in the `api` diretory, `NamedTupleTypeWithPyContainerType` is
@@ -205,29 +218,30 @@
     self._element = to_type(element)
 
   @property
   def element(self):
     return self._element
 
   def __repr__(self):
-    return 'SequenceType({})'.format(repr(self._element))
+    return 'SequenceType({!r})'.format(self._element)
 
   def __eq__(self, other):
     return isinstance(other, SequenceType) and self._element == other.element
 
 
 class FunctionType(Type):
   """An implementation of `tff.Type` representing functional types in TFF."""
 
   def __init__(self, parameter, result):
     """Constructs a new instance from the given `parameter` and `result` types.
 
     Args:
       parameter: A specification of the parameter type, either an instance of
-        `tff.Type` or something convertible to it by `tff.to_type`.
+        `tff.Type` or something convertible to it by `tff.to_type`. Multiple
+        input arguments can be specified as a single `tff.NamedTupleType`.
       result: A specification of the result type, either an instance of
         `tff.Type` or something convertible to it by `tff.to_type`.
     """
     self._parameter = to_type(parameter)
     self._result = to_type(result)
 
   @property
@@ -235,16 +249,15 @@
     return self._parameter
 
   @property
   def result(self):
     return self._result
 
   def __repr__(self):
-    return 'FunctionType({}, {})'.format(
-        repr(self._parameter), repr(self._result))
+    return 'FunctionType({!r}, {!r})'.format(self._parameter, self._result)
 
   def __eq__(self, other):
     return (isinstance(other, FunctionType) and
             self._parameter == other.parameter and self._result == other.result)
 
 
 class AbstractType(Type):
@@ -331,16 +344,17 @@
     return self._placement
 
   @property
   def all_equal(self):
     return self._all_equal
 
   def __repr__(self):
-    return 'FederatedType({}, {}, {})'.format(
-        repr(self._member), repr(self._placement), repr(self._all_equal))
+    return 'FederatedType({!r}, {!r}, {!r})'.format(self._member,
+                                                    self._placement,
+                                                    self._all_equal)
 
   def __eq__(self, other):
     return (isinstance(other, FederatedType) and
             self._member == other.member and
             self._placement == other.placement and
             self._all_equal == other.all_equal)
 
@@ -413,53 +427,35 @@
     return NamedTupleTypeWithPyContainerType(
         attr.asdict(spec, dict_factory=collections.OrderedDict, recurse=False),
         type(spec))
   elif isinstance(spec, collections.Mapping):
     # This is an unsupported mapping, likely a `dict`. NamedTupleType adds an
     # ordering, which the original container did not have.
     raise TypeError(
-        'Unsupported mapping type {}. Use collections.OrderedDict for'
+        'Unsupported mapping type {}. Use collections.OrderedDict for '
         'mappings.'.format(py_typecheck.type_string(type(spec))))
   else:
     raise TypeError(
         'Unable to interpret an argument of type {} as a type spec.'.format(
             py_typecheck.type_string(type(spec))))
 
 
-def compact_representation(type_spec):
-  """Returns the compact string representation of a TFF `Type`.
-
-  Args:
-    type_spec: An instance of a TFF `Type`.
-  """
-  return _string_representation(type_spec, formatted=False)
-
-
-def formatted_representation(type_spec):
-  """Returns the formatted string representation of a TFF `Type`.
-
-  Args:
-    type_spec: An instance of a TFF `Type`.
-  """
-  return _string_representation(type_spec, formatted=True)
-
-
 def _string_representation(type_spec, formatted):
   """Returns the string representation of a TFF `Type`.
 
-  This functions creates a `list` of strings representing the given `type_spec`;
+  This function creates a `list` of strings representing the given `type_spec`;
   combines the strings in either a formatted or un-formatted representation; and
-  returns the resulting string represetnation.
+  returns the resulting string representation.
 
   Args:
     type_spec: An instance of a TFF `Type`.
     formatted: A boolean indicating if the returned string should be formatted.
 
   Raises:
-    TypeError: If `type_spec` has an unepxected type.
+    TypeError: If `type_spec` has an unexpected type.
   """
   py_typecheck.check_type(type_spec, Type)
 
   def _combine(components):
     """Returns a `list` of strings by combining `components`.
 
     This function creates and returns a `list` of strings by combining a `list`
@@ -556,15 +552,15 @@
     elif isinstance(type_spec, PlacementType):
       return ['placement']
     elif isinstance(type_spec, SequenceType):
       element_lines = _lines_for_type(type_spec.element, formatted)
       return _combine([element_lines, ['*']])
     elif isinstance(type_spec, TensorType):
       if type_spec.shape.ndims is None:
-        return ['{}[{}]'.format(repr(type_spec.dtype), None)]
+        return ['{!r}[{}]'.format(type_spec.dtype, None)]
       elif type_spec.shape.ndims > 0:
 
         def _value_string(value):
           return str(value) if value is not None else '?'
 
         value_strings = [_value_string(e.value) for e in type_spec.shape.dims]
         values_strings = ','.join(value_strings)
```

## tensorflow_federated/python/core/api/intrinsics.py

```diff
@@ -99,14 +99,17 @@
   factory = intrinsic_factory.IntrinsicFactory(context_stack_impl.context_stack)
   return factory.federated_apply(fn, arg)
 
 
 def federated_mean(value, weight=None):
   """Computes a `tff.SERVER` mean of `value` placed on `tff.CLIENTS`.
 
+  For values `v_1, ..., v_k`, and weights `w_1, ..., w_k`, this means
+  `sum_{i=1}^k (w_i * v_i) / sum_{i=1}^k w_i`.
+
   Args:
     value: The value of which the mean is to be computed. Must be of a TFF
       federated type placed at `tff.CLIENTS`. The value may be structured, e.g.,
       its member constituents can be named tuples. The tensor types that the
       value is composed of must be floating-point or complex.
     weight: An optional weight, a TFF federated integer or floating-point tensor
       value, also placed at `tff.CLIENTS`.
@@ -279,15 +282,15 @@
 def sequence_map(mapping_fn, value):
   """Maps a TFF sequence `value` pointwise using a given function `mapping_fn`.
 
   This function supports two modes of usage:
 
   * When applied to a non-federated sequence, it maps individual elements of
     the sequence pointwise. If the supplied `mapping_fn` is of type `T->U` and
-    the sequence `value` is of type `T*` (a seqeunce of `T`-typed elements),
+    the sequence `value` is of type `T*` (a sequence of `T`-typed elements),
     the result is a sequence of type `U*` (a sequence of `U`-typed elements),
     with each element of the input sequence individually mapped by `mapping_fn`.
     In this mode of usage, `sequence_map` behaves like a compuatation with type
     signature `<T->U,T*> -> U*`.
 
   * When applied to a federated sequence, `sequence_map` behaves as if it were
     individually applied to each member constituent. In this mode of usage, one
```

## tensorflow_federated/python/core/api/placements.py

```diff
@@ -14,14 +14,14 @@
 # limitations under the License.
 """Defines common types of placements for use in defining TFF computations."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-from tensorflow_federated.python.core.impl import placement_literals
+from tensorflow_federated.python.core.impl.compiler import placement_literals
 
 # The collective of all the client devices, a TFF placement constant.
 CLIENTS = placement_literals.CLIENTS
 
 # The single top-level central coordinator, a TFF placement constant.
 SERVER = placement_literals.SERVER
```

## tensorflow_federated/python/core/framework/__init__.py

```diff
@@ -16,46 +16,47 @@
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import six
 
-from tensorflow_federated.python.core.impl.computation_building_block_utils import is_called_intrinsic
-from tensorflow_federated.python.core.impl.computation_building_blocks import Block
-from tensorflow_federated.python.core.impl.computation_building_blocks import Call
-from tensorflow_federated.python.core.impl.computation_building_blocks import CompiledComputation
-from tensorflow_federated.python.core.impl.computation_building_blocks import ComputationBuildingBlock
-from tensorflow_federated.python.core.impl.computation_building_blocks import Intrinsic
-from tensorflow_federated.python.core.impl.computation_building_blocks import Lambda
-from tensorflow_federated.python.core.impl.computation_building_blocks import Placement
-from tensorflow_federated.python.core.impl.computation_building_blocks import Reference
-from tensorflow_federated.python.core.impl.computation_building_blocks import Selection
-from tensorflow_federated.python.core.impl.computation_building_blocks import Tuple
-from tensorflow_federated.python.core.impl.computation_constructing_utils import create_federated_map_all_equal
-from tensorflow_federated.python.core.impl.computation_constructing_utils import create_federated_map_or_apply
-from tensorflow_federated.python.core.impl.computation_constructing_utils import create_federated_zip
-from tensorflow_federated.python.core.impl.computation_constructing_utils import unique_name_generator
+from tensorflow_federated.python.core.impl.compiler.building_block_analysis import is_called_intrinsic
+from tensorflow_federated.python.core.impl.compiler.building_block_factory import create_federated_map_all_equal
+from tensorflow_federated.python.core.impl.compiler.building_block_factory import create_federated_map_or_apply
+from tensorflow_federated.python.core.impl.compiler.building_block_factory import create_federated_zip
+from tensorflow_federated.python.core.impl.compiler.building_block_factory import unique_name_generator
+from tensorflow_federated.python.core.impl.compiler.building_blocks import Block
+from tensorflow_federated.python.core.impl.compiler.building_blocks import Call
+from tensorflow_federated.python.core.impl.compiler.building_blocks import CompiledComputation
+from tensorflow_federated.python.core.impl.compiler.building_blocks import ComputationBuildingBlock
+from tensorflow_federated.python.core.impl.compiler.building_blocks import Intrinsic
+from tensorflow_federated.python.core.impl.compiler.building_blocks import Lambda
+from tensorflow_federated.python.core.impl.compiler.building_blocks import Placement
+from tensorflow_federated.python.core.impl.compiler.building_blocks import Reference
+from tensorflow_federated.python.core.impl.compiler.building_blocks import Selection
+from tensorflow_federated.python.core.impl.compiler.building_blocks import Tuple
+from tensorflow_federated.python.core.impl.compiler.intrinsic_defs import FEDERATED_AGGREGATE
+from tensorflow_federated.python.core.impl.compiler.intrinsic_defs import FEDERATED_APPLY
+from tensorflow_federated.python.core.impl.compiler.intrinsic_defs import FEDERATED_BROADCAST
+from tensorflow_federated.python.core.impl.compiler.intrinsic_defs import FEDERATED_MAP
+from tensorflow_federated.python.core.impl.compiler.intrinsic_defs import FEDERATED_MAP_ALL_EQUAL
+from tensorflow_federated.python.core.impl.compiler.transformation_utils import transform_postorder
+from tensorflow_federated.python.core.impl.compiler.tree_analysis import check_broadcast_not_dependent_on_aggregate
+from tensorflow_federated.python.core.impl.compiler.tree_analysis import check_has_unique_names
+from tensorflow_federated.python.core.impl.compiler.tree_analysis import check_intrinsics_whitelisted_for_reduction
 from tensorflow_federated.python.core.impl.computation_wrapper_instances import building_block_to_computation
-from tensorflow_federated.python.core.impl.intrinsic_defs import FEDERATED_AGGREGATE
-from tensorflow_federated.python.core.impl.intrinsic_defs import FEDERATED_APPLY
-from tensorflow_federated.python.core.impl.intrinsic_defs import FEDERATED_BROADCAST
-from tensorflow_federated.python.core.impl.intrinsic_defs import FEDERATED_MAP
-from tensorflow_federated.python.core.impl.intrinsic_defs import FEDERATED_MAP_ALL_EQUAL
 from tensorflow_federated.python.core.impl.intrinsic_reductions import replace_intrinsics_with_bodies
-from tensorflow_federated.python.core.impl.transformation_utils import transform_postorder
-from tensorflow_federated.python.core.impl.transformations import check_has_unique_names
-from tensorflow_federated.python.core.impl.transformations import check_intrinsics_whitelisted_for_reduction
 from tensorflow_federated.python.core.impl.transformations import get_map_of_unbound_references
 from tensorflow_federated.python.core.impl.transformations import inline_block_locals
 from tensorflow_federated.python.core.impl.transformations import insert_called_tf_identity_at_leaves
 from tensorflow_federated.python.core.impl.transformations import merge_tuple_intrinsics
+from tensorflow_federated.python.core.impl.transformations import remove_lambdas_and_blocks
 from tensorflow_federated.python.core.impl.transformations import remove_mapped_or_applied_identity
 from tensorflow_federated.python.core.impl.transformations import replace_called_lambda_with_block
-from tensorflow_federated.python.core.impl.transformations import replace_selection_from_tuple_with_element
 from tensorflow_federated.python.core.impl.transformations import TFParser
 from tensorflow_federated.python.core.impl.transformations import uniquify_reference_names
 from tensorflow_federated.python.core.impl.transformations import unwrap_placement
 from tensorflow_federated.python.core.impl.type_utils import are_equivalent_types
 from tensorflow_federated.python.core.impl.type_utils import is_assignable_from
 from tensorflow_federated.python.core.impl.type_utils import is_tensorflow_compatible_type
 from tensorflow_federated.python.core.impl.type_utils import transform_type_postorder
@@ -66,34 +67,39 @@
 # and dependent on targets are are not currently included in the open-source
 # build rule.
 # TODO(b/134543154): Modify the OSS build rule to conditionally include these
 # new targets if possible.
 if six.PY3:
   # pylint: disable=g-import-not-at-top
   try:
+    from tensorflow_federated.python.core.impl.caching_executor import CachingExecutor
+    from tensorflow_federated.python.core.impl.composite_executor import CompositeExecutor
     from tensorflow_federated.python.core.impl.concurrent_executor import ConcurrentExecutor
     from tensorflow_federated.python.core.impl.eager_executor import EagerExecutor
     from tensorflow_federated.python.core.impl.executor_base import Executor
     from tensorflow_federated.python.core.impl.executor_service import ExecutorService
     from tensorflow_federated.python.core.impl.executor_stacks import create_local_executor
+    from tensorflow_federated.python.core.impl.executor_stacks import create_worker_pool_executor
     from tensorflow_federated.python.core.impl.executor_value_base import ExecutorValue
     from tensorflow_federated.python.core.impl.federated_executor import FederatedExecutor
     from tensorflow_federated.python.core.impl.lambda_executor import LambdaExecutor
     from tensorflow_federated.python.core.impl.remote_executor import RemoteExecutor
     from tensorflow_federated.python.core.impl.set_default_executor import set_default_executor
     from tensorflow_federated.python.core.impl.transforming_executor import TransformingExecutor
   except ModuleNotFoundError:
     pass
   # pylint: enable=g-import-not-at-top
 
 # Used by doc generation script.
 _allowed_symbols = [
     "Block",
+    "CachingExecutor",
     "Call",
     "CompiledComputation",
+    "CompositeExecutor",
     "ComputationBuildingBlock",
     "ConcurrentExecutor",
     "EagerExecutor",
     "Executor",
     "ExecutorService",
     "ExecutorValue",
     "FEDERATED_AGGREGATE",
@@ -116,25 +122,26 @@
     "building_block_to_computation",
     "check_has_unique_names",
     "check_intrinsics_whitelisted_for_reduction",
     "create_federated_map_all_equal",
     "create_federated_map_or_apply",
     "create_federated_zip",
     "create_local_executor",
+    "create_worker_pool_executor",
     "get_map_of_unbound_references",
     "inline_block_locals",
     "insert_called_tf_identity_at_leaves",
     "is_assignable_from",
     "is_called_intrinsic",
     "is_tensorflow_compatible_type",
     "merge_tuple_intrinsics",
+    "remove_lambdas_and_blocks",
     "remove_mapped_or_applied_identity",
     "replace_called_lambda_with_block",
     "replace_intrinsics_with_bodies",
-    "replace_selection_from_tuple_with_element",
     "set_default_executor",
     "transform_postorder",
     "transform_type_postorder",
     "type_from_tensors",
     "type_to_tf_tensor_specs",
     "unique_name_generator",
     "uniquify_reference_names",
```

## tensorflow_federated/python/core/impl/compiled_computation_transforms.py

```diff
@@ -24,26 +24,27 @@
 import tensorflow as tf
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.common_libs import serialization_utils
 from tensorflow_federated.python.core.api import computation_types
-from tensorflow_federated.python.core.impl import computation_building_blocks
-from tensorflow_federated.python.core.impl import computation_constructing_utils
-from tensorflow_federated.python.core.impl import graph_utils
-from tensorflow_federated.python.core.impl import transformation_utils
-from tensorflow_federated.python.core.impl import type_serialization
+from tensorflow_federated.python.core.impl.compiler import building_block_factory
+from tensorflow_federated.python.core.impl.compiler import building_blocks
+from tensorflow_federated.python.core.impl.compiler import proto_transformations
+from tensorflow_federated.python.core.impl.compiler import transformation_utils
+from tensorflow_federated.python.core.impl.compiler import type_serialization
+from tensorflow_federated.python.core.impl.utils import tensorflow_utils
 from tensorflow_federated.python.tensorflow_libs import graph_merge
 
 
 def select_graph_output(comp, name=None, index=None):
   r"""Makes `CompiledComputation` with same input as `comp` and output `output`.
 
-  Given an instance of `computation_building_blocks.CompiledComputation` `comp`
+  Given an instance of `building_blocks.CompiledComputation` `comp`
   with type signature (T -> <U, ...,V>), `select_output` returns a
   `CompiledComputation` representing the logic of calling `comp` and then
   selecting `name` or `index` from the resulting `tuple`. Notice that only one
   of `name` or `index` can be specified, and one of them must be specified.
 
   At the level of a TFF AST, `select_graph_output` is necessary to transform
   the structure below:
@@ -58,27 +59,27 @@
 
                                 Call
                                /    \
   select_graph_output(Graph, x)      Comp
 
 
   Args:
-    comp: Instance of `computation_building_blocks.CompiledComputation` which
-      must have result type `computation_types.NamedTupleType`, the function
-      from which to select `output`.
+    comp: Instance of `building_blocks.CompiledComputation` which must have
+      result type `computation_types.NamedTupleType`, the function from which to
+      select `output`.
     name: Instance of `str`, the name of the field to select from the output of
       `comp`. Optional, but one of `name` or `index` must be specified.
     index: Instance of `index`, the index of the field to select from the output
       of `comp`. Optional, but one of `name` or `index` must be specified.
 
   Returns:
-    An instance of `computation_building_blocks.CompiledComputation` as
+    An instance of `building_blocks.CompiledComputation` as
     described, the result of selecting the appropriate output from `comp`.
   """
-  py_typecheck.check_type(comp, computation_building_blocks.CompiledComputation)
+  py_typecheck.check_type(comp, building_blocks.CompiledComputation)
   if index and name:
     raise ValueError(
         'Please specify at most one of `name` or `index` to `select_outputs`.')
   if index is not None:
     py_typecheck.check_type(index, int)
   elif name is not None:
     py_typecheck.check_type(name, str)
@@ -95,52 +96,53 @@
   proto_type = type_serialization.deserialize_type(proto.type)
   py_typecheck.check_type(proto_type.result, computation_types.NamedTupleType)
   if name is None:
     result = [x for x in graph_result_binding.tuple.element][index]
     result_type = proto_type.result[index]
   else:
     type_names_list = [
-        x[0] for x in anonymous_tuple.to_elements(proto_type.result)
+        x[0] for x in anonymous_tuple.iter_elements(proto_type.result)
     ]
     index = type_names_list.index(name)
     result = [x for x in graph_result_binding.tuple.element][index]
     result_type = proto_type.result[index]
   serialized_type = type_serialization.serialize_type(
       computation_types.FunctionType(proto_type.parameter, result_type))
   selected_proto = pb.Computation(
       type=serialized_type,
       tensorflow=pb.TensorFlow(
           graph_def=proto.tensorflow.graph_def,
           initialize_op=proto.tensorflow.initialize_op,
           parameter=proto.tensorflow.parameter,
           result=result))
-  return computation_building_blocks.CompiledComputation(selected_proto)
+  proto_pruned = proto_transformations.prune_tensorflow_proto(selected_proto)
+  return building_blocks.CompiledComputation(proto_pruned)
 
 
 def permute_graph_inputs(comp, input_permutation):
   r"""Remaps input indices of `comp` to match the `input_permutation`.
 
   Changes the order of the parameters `comp`, an instance of
-  `computation_building_blocks.CompiledComputation`. Accepts a permutation
+  `building_blocks.CompiledComputation`. Accepts a permutation
   of the input tuple by index, and applies this permutation to the input
   bindings of `comp`. For example, given a `comp` which accepts a 3-tuple of
   types `[tf.int32, tf.float32, tf.bool]` as its parameter, passing in the
   input permutation
 
                           [2, 0, 1]
 
   would change the order of the parameter bindings accepted, so that
   `permute_graph_inputs` returns a
-  `computation_building_blocks.CompiledComputation`
+  `building_blocks.CompiledComputation`
   accepting a 3-tuple of types `[tf.bool, tf.int32, tf.float32]`. Notice that
   we use one-line notation for our permutations, with beginning index 0
   (https://en.wikipedia.org/wiki/Permutation#One-line_notation).
 
   At the AST structural level, this is a no-op, as it simply takes in one
-  instance of `computation_building_blocks.CompiledComputation` and returns
+  instance of `building_blocks.CompiledComputation` and returns
   another. However, it is necessary to make a replacement such as transforming:
 
                           Call
                          /    \
                     Graph      Tuple
                               / ... \
                   Selection(i)       Selection(j)
@@ -149,30 +151,30 @@
 
   into:
                                      Call
                                     /    \
   permute_graph_inputs(Graph, [...])      Comp
 
   Args:
-    comp: Instance of `computation_building_blocks.CompiledComputation` whose
-      parameter bindings we wish to permute.
+    comp: Instance of `building_blocks.CompiledComputation` whose parameter
+      bindings we wish to permute.
     input_permutation: The permutation we wish to apply to the parameter
       bindings of `comp` in 0-indexed one-line permutation notation. This can be
       a Python `list` or `tuple` of `int`s.
 
   Returns:
-    An instance of `computation_building_blocks.CompiledComputation` whose
+    An instance of `building_blocks.CompiledComputation` whose
     parameter bindings represent the same as the result of applying
     `input_permutation` to the parameter bindings of `comp`.
 
   Raises:
     TypeError: If the types specified in the args section do not match.
   """
 
-  py_typecheck.check_type(comp, computation_building_blocks.CompiledComputation)
+  py_typecheck.check_type(comp, building_blocks.CompiledComputation)
   py_typecheck.check_type(input_permutation, (tuple, list))
   permutation_length = len(input_permutation)
   for index in input_permutation:
     py_typecheck.check_type(index, int)
   proto = comp.proto
   graph_parameter_binding = proto.tensorflow.parameter
   proto_type = type_serialization.deserialize_type(proto.type)
@@ -218,42 +220,43 @@
       tensorflow=pb.TensorFlow(
           graph_def=proto.tensorflow.graph_def,
           initialize_op=proto.tensorflow.initialize_op,
           parameter=pb.TensorFlow.Binding(
               tuple=pb.TensorFlow.NamedTupleBinding(
                   element=new_parameter_bindings)),
           result=proto.tensorflow.result))
-  return computation_building_blocks.CompiledComputation(permuted_proto)
+  proto_pruned = proto_transformations.prune_tensorflow_proto(permuted_proto)
+  return building_blocks.CompiledComputation(proto_pruned)
 
 
 def bind_graph_parameter_as_tuple(comp, name=None):
   """Wraps the parameter of `comp` in a tuple binding.
 
   `bind_graph_parameter_as_tuple` is intended as a preprocessing step
   to `pad_graph_inputs_to_match_type`, so that `pad_graph_inputs_to_match_type`
   can
   make the assumption that its argument `comp` always has a tuple binding,
   instead of dealing with the possibility of an unwrapped tensor or sequence
   binding.
 
   Args:
-    comp: Instance of `computation_building_blocks.CompiledComputation` whose
-      parameter we wish to wrap in a tuple binding.
+    comp: Instance of `building_blocks.CompiledComputation` whose parameter we
+      wish to wrap in a tuple binding.
     name: Optional string argument, the name to assign to the element type in
       the constructed tuple. Defaults to `None`.
 
   Returns:
     A transformed version of comp representing exactly the same computation,
     but accepting a tuple containing one element--the parameter of `comp`.
 
   Raises:
     TypeError: If `comp` is not a
-      `computation_building_blocks.CompiledComputation`.
+      `building_blocks.CompiledComputation`.
   """
-  py_typecheck.check_type(comp, computation_building_blocks.CompiledComputation)
+  py_typecheck.check_type(comp, building_blocks.CompiledComputation)
   if name is not None:
     py_typecheck.check_type(name, six.string_types)
   proto = comp.proto
   proto_type = type_serialization.deserialize_type(proto.type)
 
   parameter_binding = [proto.tensorflow.parameter]
   parameter_type_list = [(name, proto_type.parameter)]
@@ -267,43 +270,44 @@
   input_padded_proto = pb.Computation(
       type=serialized_type,
       tensorflow=pb.TensorFlow(
           graph_def=proto.tensorflow.graph_def,
           initialize_op=proto.tensorflow.initialize_op,
           parameter=new_parameter_binding,
           result=proto.tensorflow.result))
-
-  return computation_building_blocks.CompiledComputation(input_padded_proto)
+  proto_pruned = proto_transformations.prune_tensorflow_proto(
+      input_padded_proto)
+  return building_blocks.CompiledComputation(proto_pruned)
 
 
 def bind_graph_result_as_tuple(comp, name=None):
   """Wraps the result of `comp` in a tuple binding.
 
   `bind_graph_result_as_tuple` is used when a
-  `computation_building_blocks.Tuple` of length 1 containing a called graph is
+  `building_blocks.Tuple` of length 1 containing a called graph is
   encountered; this is an equivalent construct to simply calling the graph
   with the same argument, but wrapping the result in as a tuple. This can
   be accomplished purely by manipulating proto bindings, which is the purpose
   of this function.
 
   Args:
-    comp: Instance of `computation_building_blocks.CompiledComputation` whose
-      parameter we wish to wrap in a tuple binding.
+    comp: Instance of `building_blocks.CompiledComputation` whose parameter we
+      wish to wrap in a tuple binding.
     name: Optional string argument, the name to assign to the element type in
       the constructed tuple. Defaults to `None`.
 
   Returns:
     A transformed version of comp representing exactly the same computation,
     but returning a tuple containing one element--the parameter of `comp`.
 
   Raises:
     TypeError: If `comp` is not a
-      `computation_building_blocks.CompiledComputation`.
+      `building_blocks.CompiledComputation`.
   """
-  py_typecheck.check_type(comp, computation_building_blocks.CompiledComputation)
+  py_typecheck.check_type(comp, building_blocks.CompiledComputation)
   if name is not None:
     py_typecheck.check_type(name, six.string_types)
   proto = comp.proto
   proto_type = type_serialization.deserialize_type(proto.type)
 
   result_binding = [proto.tensorflow.result]
   result_type_list = [(name, proto_type.result)]
@@ -317,16 +321,17 @@
   result_as_tuple_proto = pb.Computation(
       type=serialized_type,
       tensorflow=pb.TensorFlow(
           graph_def=proto.tensorflow.graph_def,
           initialize_op=proto.tensorflow.initialize_op,
           parameter=proto.tensorflow.parameter,
           result=new_result_binding))
-
-  return computation_building_blocks.CompiledComputation(result_as_tuple_proto)
+  proto_pruned = proto_transformations.prune_tensorflow_proto(
+      result_as_tuple_proto)
+  return building_blocks.CompiledComputation(proto_pruned)
 
 
 def pad_graph_inputs_to_match_type(comp, type_signature):
   r"""Pads the parameter bindings of `comp` to match `type_signature`.
 
   The padded parameters here are in effect dummy bindings--they are not
   plugged in elsewhere in `comp`. This pattern is necessary to transform TFF
@@ -357,37 +362,36 @@
   parameter permutation via `permute_graph_inputs`.
 
   Notice also that the existing parameter bindings of `comp` must match the
   first elements of `type_signature`. This is to ensure that we are attempting
   to pad only compatible `CompiledComputation`s to a given type signature.
 
   Args:
-    comp: Instance of `computation_building_blocks.CompiledComputation`
-      representing the graph whose inputs we want to pad to match
-      `type_signature`.
+    comp: Instance of `building_blocks.CompiledComputation` representing the
+      graph whose inputs we want to pad to match `type_signature`.
     type_signature: Instance of `computation_types.NamedTupleType` representing
       the type signature we wish to pad `comp` to accept as a parameter.
 
   Returns:
     A transformed version of `comp`, instance of
-    `computation_building_blocks.CompiledComputation` which takes an argument
+    `building_blocks.CompiledComputation` which takes an argument
     of type `type_signature` and executes the same logic as `comp`. In
     particular, this transformed version will have the same return type as
     the original `comp`.
 
   Raises:
     TypeError: If the proto underlying `comp` has a parameter type which
       is not of `NamedTupleType`, the `type_signature` argument is not of type
       `NamedTupleType`, or there is a type mismatch between the declared
       parameters of `comp` and the requested `type_signature`.
     ValueError: If the requested `type_signature` is shorter than the
       parameter type signature declared by `comp`.
   """
   py_typecheck.check_type(type_signature, computation_types.NamedTupleType)
-  py_typecheck.check_type(comp, computation_building_blocks.CompiledComputation)
+  py_typecheck.check_type(comp, building_blocks.CompiledComputation)
   proto = comp.proto
   graph_def = proto.tensorflow.graph_def
   graph_parameter_binding = proto.tensorflow.parameter
   proto_type = type_serialization.deserialize_type(proto.type)
   binding_oneof = graph_parameter_binding.WhichOneof('binding')
   if binding_oneof != 'tuple':
     raise TypeError(
@@ -426,15 +430,15 @@
   elems_to_stamp = anonymous_tuple.to_elements(
       type_signature)[len(parameter_bindings):]
   for name, type_spec in elems_to_stamp:
     if name is None:
       stamp_name = 'name'
     else:
       stamp_name = name
-    _, stamped_binding = graph_utils.stamp_parameter_in_graph(
+    _, stamped_binding = tensorflow_utils.stamp_parameter_in_graph(
         stamp_name, type_spec, g)
     parameter_bindings.append(stamped_binding)
     parameter_type_elements.append((name, type_spec))
 
   new_parameter_binding = pb.TensorFlow.Binding(
       tuple=pb.TensorFlow.NamedTupleBinding(element=parameter_bindings))
   new_graph_def = g.as_graph_def()
@@ -446,16 +450,17 @@
   input_padded_proto = pb.Computation(
       type=serialized_type,
       tensorflow=pb.TensorFlow(
           graph_def=serialization_utils.pack_graph_def(new_graph_def),
           initialize_op=proto.tensorflow.initialize_op,
           parameter=new_parameter_binding,
           result=proto.tensorflow.result))
-
-  return computation_building_blocks.CompiledComputation(input_padded_proto)
+  proto_pruned = proto_transformations.prune_tensorflow_proto(
+      input_padded_proto)
+  return building_blocks.CompiledComputation(proto_pruned)
 
 
 def _unpack_proto_into_graph_spec(tf_block_proto):
   """Packs a TF proto into a `graph_merge.GraphSpec`.
 
   Args:
     tf_block_proto: Instance of `computation_pb2.Computation` with `tensorflow`
@@ -470,19 +475,19 @@
   graph_init_op_name = tf_block_proto.tensorflow.initialize_op
   if not graph_init_op_name:
     graph_init_op_name = None
   graph_parameter_binding = tf_block_proto.tensorflow.parameter
   graph_result_binding = tf_block_proto.tensorflow.result
 
   if graph_parameter_binding.WhichOneof('binding') is not None:
-    graph_parameter_list = graph_utils.extract_tensor_names_from_binding(
+    graph_parameter_list = tensorflow_utils.extract_tensor_names_from_binding(
         graph_parameter_binding)
   else:
     graph_parameter_list = []
-  graph_result_list = graph_utils.extract_tensor_names_from_binding(
+  graph_result_list = tensorflow_utils.extract_tensor_names_from_binding(
       graph_result_binding)
   return graph_merge.GraphSpec(graph, graph_init_op_name, graph_parameter_list,
                                graph_result_list)
 
 
 def _repack_binding_with_new_name(binding, name_map):
   """Constructs new binding via `name_map`.
@@ -517,23 +522,22 @@
   elif binding.WhichOneof('binding') == 'tuple':
     return pb.TensorFlow.Binding(
         tuple=pb.TensorFlow.NamedTupleBinding(element=[
             _repack_binding_with_new_name(e, name_map)
             for e in binding.tuple.element
         ]))
   elif binding.WhichOneof('binding') == 'sequence':
-    handle_name = binding.sequence.iterator_string_handle_name
-    if handle_name:
-      return pb.TensorFlow.Binding(
-          sequence=pb.TensorFlow.SequenceBinding(
-              iterator_string_handle_name=name_map[handle_name]))
-    else:
+    sequence_oneof = binding.sequence.WhichOneof('binding')
+    if sequence_oneof == 'variant_tensor_name':
       return pb.TensorFlow.Binding(
           sequence=pb.TensorFlow.SequenceBinding(variant_tensor_name=name_map[
               binding.sequence.variant_tensor_name]))
+    else:
+      raise ValueError(
+          'Unsupported sequence binding \'{}\'.'.format(sequence_oneof))
   else:
     raise TypeError
 
 
 def _pack_concatenated_bindings(old_bindings, tensor_name_maps):
   """Maps the old TFF bindings to the correct new names.
 
@@ -573,15 +577,15 @@
 
   This logic is explained in the docstring of `concatenate_tensorflow_blocks`.
 
   Args:
     type_list: Python `list` or `tuple` of `computation_types.Type`s, which we
       want to use to construct a new parameter or result type for a computation
       representing concatenation of inputs and outputs of two
-      `computation_building_blocks.CompiledComputation`s.
+      `building_blocks.CompiledComputation`s.
 
   Returns:
     Instance of `computation_types.Type` representing the appropriate
     parameter or result type, or `None` if `type_list` contains no non-`None`
     types.
   """
   non_none_type_list = [x for x in type_list if x is not None]
@@ -592,36 +596,36 @@
   return computation_types.NamedTupleType(non_none_type_list)
 
 
 def concatenate_tensorflow_blocks(tf_comp_list, output_name_list):
   """Concatenates inputs and outputs of its argument to a single TF block.
 
   Takes a Python `list` or `tuple` of instances of
-  `computation_building_blocks.CompiledComputation`, and constructs a single
+  `building_blocks.CompiledComputation`, and constructs a single
   instance of the same building block representing the computations present
   in this list concatenated side-by-side.
 
   There is one important convention here for callers to be aware of.
   `concatenate_tensorflow_blocks` does not perform any more packing into tuples
   than necessary. That is, if `tf_comp_list` contains only a single TF
   computation which declares a parameter, the parameter type of the resulting
   computation is exactly this single parameter type. Since all TF blocks declare
   a result, this is only of concern for parameters, and we will always return a
   function with a tuple for its result value.
 
   Args:
     tf_comp_list: Python `list` or `tuple` of
-      `computation_building_blocks.CompiledComputation`s, whose inputs and
-      outputs we wish to concatenate.
+      `building_blocks.CompiledComputation`s, whose inputs and outputs we wish
+      to concatenate.
     output_name_list: A list list or tuple of names to give to the result types
       in the concatenated TF computations. The elements of this list or tuple
       must be either string types or None
 
   Returns:
-    A single instance of `computation_building_blocks.CompiledComputation`,
+    A single instance of `building_blocks.CompiledComputation`,
     representing all the computations in `tf_comp_list` concatenated
     side-by-side.
 
   Raises:
     ValueError: If we are passed less than 1 computation in `tf_comp_list`.
       Also raises if `output_name_list` and `tf_comp_list` have different
       lengths.
@@ -645,16 +649,15 @@
                      'fully specified output names, even if the names are '
                      '`None`.')
   for name in output_name_list:
     if name is not None:
       py_typecheck.check_type(name, six.string_types)
   tf_proto_list = []
   for comp in tf_comp_list:
-    py_typecheck.check_type(comp,
-                            computation_building_blocks.CompiledComputation)
+    py_typecheck.check_type(comp, building_blocks.CompiledComputation)
     tf_proto_list.append(comp.proto)
 
   (merged_graph, init_op_name, parameter_name_maps,
    result_name_maps) = graph_merge.concatenate_inputs_and_outputs(
        [_unpack_proto_into_graph_spec(x) for x in tf_proto_list])
 
   concatenated_parameter_bindings = _pack_concatenated_bindings(
@@ -681,33 +684,34 @@
   return_type = [(output_name_list[i], x.type_signature.result)
                  for i, x in enumerate(tf_comp_list)]
   function_type = computation_types.FunctionType(parameter_type, return_type)
   serialized_function_type = type_serialization.serialize_type(function_type)
 
   constructed_proto = pb.Computation(
       type=serialized_function_type, tensorflow=tf_result_proto)
-  return computation_building_blocks.CompiledComputation(constructed_proto)
+  proto_pruned = proto_transformations.prune_tensorflow_proto(constructed_proto)
+  return building_blocks.CompiledComputation(proto_pruned)
 
 
 def compose_tensorflow_blocks(tf_comps):
   """Composes TensorFlow blocks from `tf_comps`.
 
   Args:
     tf_comps: List or tuple of instances of
-      `computation_building_blocks.CompiledComputation` representing the
-      functions we wish to compose. Notice that these must obey a certain
-      invariant; the result type of computation k in this list must be identical
-      to the parameter type of computation k-1. Notice also that the order of
-      this list is quite important, as composition is completely noncommutative.
-      This function represents the standard mathematical convention for
-      composition; IE, compose(f1, f2) represents the function which first calls
-      f2 on its argument, then f1 on the result of this call.
+      `building_blocks.CompiledComputation` representing the functions we wish
+      to compose. Notice that these must obey a certain invariant; the result
+      type of computation k in this list must be identical to the parameter type
+      of computation k-1. Notice also that the order of this list is quite
+      important, as composition is completely noncommutative. This function
+      represents the standard mathematical convention for composition; IE,
+      compose(f1, f2) represents the function which first calls f2 on its
+      argument, then f1 on the result of this call.
 
   Returns:
-    Instance of `computation_building_blocks.CompiledComputation` representing
+    Instance of `building_blocks.CompiledComputation` representing
     the composition of the functions in `tf_comps`.
 
   Raises:
     TypeError: If `tf_comps` is not a `tuple` or `list`, or if the parameter
       and return types of `tf_comps` do not respect the invariant mentioned
       in the args section of this docstring.
     ValueError: If we are passed a `tf_comps` with fewer than 2 elements;
@@ -717,16 +721,15 @@
   if len(tf_comps) < 2:
     raise ValueError('Encountered a `tf_comps` of fewer than 2 elements; '
                      'in this case, likely you do not want '
                      '`compose_tensorflow_blocks`.')
   tf_protos = []
   previous_param_type = None
   for comp in tf_comps:
-    py_typecheck.check_type(comp,
-                            computation_building_blocks.CompiledComputation)
+    py_typecheck.check_type(comp, building_blocks.CompiledComputation)
     if previous_param_type is not None:
       if previous_param_type != comp.type_signature.result:
         raise TypeError('The result type of computation k should match the '
                         'parameter type of computation k-1 in `tf_comps`, '
                         'as we are attempting to compose; we have encountered '
                         'a result of type {} attempting to match a parameter '
                         'of type {}'.format(comp.type_signature.result,
@@ -765,34 +768,34 @@
   return_type = tf_comps[0].type_signature.result
 
   function_type = computation_types.FunctionType(parameter_type, return_type)
   serialized_function_type = type_serialization.serialize_type(function_type)
 
   constructed_proto = pb.Computation(
       type=serialized_function_type, tensorflow=tf_result_proto)
-  return computation_building_blocks.CompiledComputation(constructed_proto)
+  proto_pruned = proto_transformations.prune_tensorflow_proto(constructed_proto)
+  return building_blocks.CompiledComputation(proto_pruned)
 
 
 class CalledCompositionOfTensorFlowBlocks(transformation_utils.TransformSpec):
   """`TransformSpec` representing a composition of TF blocks."""
 
   def should_transform(self, comp):
-    return (isinstance(comp, computation_building_blocks.Call) and isinstance(
-        comp.function, computation_building_blocks.CompiledComputation) and
-            isinstance(comp.argument, computation_building_blocks.Call) and
-            isinstance(comp.argument.function,
-                       computation_building_blocks.CompiledComputation))
+    return (isinstance(comp, building_blocks.Call) and
+            isinstance(comp.function, building_blocks.CompiledComputation) and
+            isinstance(comp.argument, building_blocks.Call) and isinstance(
+                comp.argument.function, building_blocks.CompiledComputation))
 
   def transform(self, comp):
     if self.should_transform(comp):
       bottom_arg = comp.argument.argument
       function_1 = comp.function
       function_2 = comp.argument.function
       composed_fn = compose_tensorflow_blocks([function_1, function_2])
-      return computation_building_blocks.Call(composed_fn, bottom_arg), True
+      return building_blocks.Call(composed_fn, bottom_arg), True
     return comp, False
 
 
 class CalledGraphOnReplicatedArg(transformation_utils.TransformSpec):
   r"""`TransformSpec` representing a called graph with replicated argument.
 
   Transforms the pattern:
@@ -809,39 +812,37 @@
 
   This is necessary for preserving the invariant that we are always passing
   called graphs up the tree; concatenating a tuple of called graphs necessarily
   calls into this function to preserve this invariant.
   """
 
   def should_transform(self, comp):
-    if not isinstance(comp, computation_building_blocks.Call):
+    if not isinstance(comp, building_blocks.Call):
       return False
     function = comp.function
     argument = comp.argument
-    if not isinstance(function,
-                      computation_building_blocks.CompiledComputation):
+    if not isinstance(function, building_blocks.CompiledComputation):
       return False
-    if not (isinstance(argument, computation_building_blocks.Tuple) and all(
-        isinstance(x, computation_building_blocks.Reference)
-        for x in argument)):
+    if not (isinstance(argument, building_blocks.Tuple) and
+            all(isinstance(x, building_blocks.Reference) for x in argument)):
       return False
     first_ref_name = argument[0].name
     return all(x.name == first_ref_name for x in argument)
 
   def transform(self, comp):
     if not self.should_transform(comp):
       return comp, False
-    preprocess_arg_comp = computation_constructing_utils.create_compiled_input_replication(
+    preprocess_arg_comp = building_block_factory.create_compiled_input_replication(
         comp.argument[0].type_signature, len(comp.argument))
     logic_of_tf_comp = comp.function
     composed_tf = compose_tensorflow_blocks(
         [logic_of_tf_comp, preprocess_arg_comp])
-    single_arg = computation_building_blocks.Reference(
-        comp.argument[0].name, comp.argument[0].type_signature)
-    called_tf = computation_building_blocks.Call(composed_tf, single_arg)
+    single_arg = building_blocks.Reference(comp.argument[0].name,
+                                           comp.argument[0].type_signature)
+    called_tf = building_blocks.Call(composed_tf, single_arg)
     return called_tf, True
 
 
 class SelectionFromCalledTensorFlowBlock(transformation_utils.TransformSpec):
   r"""`TransformSpec` representing a selection from the result of a TF block.
 
   That is, parses the pattern:
@@ -858,26 +859,26 @@
                              /    \
           CompiledComputation      Argument
 
   While preserving semantics.
   """
 
   def should_transform(self, comp):
-    return (isinstance(comp, computation_building_blocks.Selection) and
-            isinstance(comp.source, computation_building_blocks.Call) and
-            isinstance(comp.source.function,
-                       computation_building_blocks.CompiledComputation))
+    return (isinstance(comp, building_blocks.Selection) and
+            isinstance(comp.source, building_blocks.Call) and isinstance(
+                comp.source.function, building_blocks.CompiledComputation))
 
   def transform(self, comp):
     if not self.should_transform(comp):
       return comp, False
-    return computation_building_blocks.Call(
-        select_graph_output(
-            comp.source.function, index=comp.index, name=comp.name),
-        comp.source.argument), True
+    selected = select_graph_output(
+        comp.source.function, index=comp.index, name=comp.name)
+    pruned = building_blocks.CompiledComputation(
+        proto_transformations.prune_tensorflow_proto(selected.proto))
+    return building_blocks.Call(pruned, comp.source.argument), True
 
 
 class LambdaWrappingGraph(transformation_utils.TransformSpec):
   r"""`TransformSpec` representing a lambda wrapping a call to a TF graph.
 
   Transforms the pattern:
 
@@ -892,20 +893,18 @@
                       CompiledComputation
 
   While preserving semantics. This represents the final stage of parsing TFF
   into TF.
   """
 
   def should_transform(self, comp):
-    return (isinstance(comp, computation_building_blocks.Lambda) and
-            isinstance(comp.result, computation_building_blocks.Call) and
-            isinstance(comp.result.function,
-                       computation_building_blocks.CompiledComputation) and
-            isinstance(comp.result.argument,
-                       computation_building_blocks.Reference) and
+    return (isinstance(comp, building_blocks.Lambda) and
+            isinstance(comp.result, building_blocks.Call) and isinstance(
+                comp.result.function, building_blocks.CompiledComputation) and
+            isinstance(comp.result.argument, building_blocks.Reference) and
             comp.result.argument.name == comp.parameter_name)
 
   def transform(self, comp):
     if not self.should_transform(comp):
       return comp, False
     return comp.result.function, True
 
@@ -929,44 +928,44 @@
                                   / ... \
                                 Arg1    Argn
 
   While preserving semantics.
   """
 
   def should_transform(self, comp):
-    return (isinstance(comp, computation_building_blocks.Tuple) and all(
-        isinstance(x, computation_building_blocks.Call) for x in comp) and all(
-            isinstance(x.function,
-                       computation_building_blocks.CompiledComputation)
-            for x in comp))
+    return (isinstance(comp, building_blocks.Tuple) and
+            all(isinstance(x, building_blocks.Call) for x in comp) and all(
+                isinstance(x.function, building_blocks.CompiledComputation)
+                for x in comp))
 
   def transform(self, comp):
     if not self.should_transform(comp):
       return comp, False
     if len(comp) == 0:  # pylint: disable=g-explicit-length-test
-      return computation_constructing_utils.create_compiled_empty_tuple(), True
+      return building_block_factory.create_compiled_empty_tuple(), True
     compiled_computation_list = []
     arg_list = []
-    name_list = [x[0] for x in anonymous_tuple.to_elements(comp.type_signature)]
+    name_list = [
+        x[0] for x in anonymous_tuple.iter_elements(comp.type_signature)
+    ]
     for k in range(len(comp.type_signature)):
       compiled_computation_list.append(comp[k].function)
       arg_list.append(comp[k].argument)
 
     concatenated_tf = concatenate_tensorflow_blocks(compiled_computation_list,
                                                     name_list)
     non_none_arg_list = [x for x in arg_list if x is not None]
     if not non_none_arg_list:
       arg = None
     elif len(non_none_arg_list) == 1:
       arg = non_none_arg_list[0]
-      return computation_building_blocks.Call(concatenated_tf, arg), True
+      return building_blocks.Call(concatenated_tf, arg), True
     else:
-      arg = computation_building_blocks.Tuple(non_none_arg_list)
-    called_tf_on_concatenated_arg = computation_building_blocks.Call(
-        concatenated_tf, arg)
+      arg = building_blocks.Tuple(non_none_arg_list)
+    called_tf_on_concatenated_arg = building_blocks.Call(concatenated_tf, arg)
     replicated_arg_check = CalledGraphOnReplicatedArg()
     return replicated_arg_check.transform(
         called_tf_on_concatenated_arg)[0], True
 
 
 def _construct_padding(list_of_indices, tuple_type):
   """Constructs padding for `_remap_graph_inputs`.
@@ -976,15 +975,15 @@
   `_construct_padding` is present in the global scope only to ease its
   testing; one could consider it to be private to `_remap_graph_inputs`.
 
   Args:
     list_of_indices: Python `list` containing integers between 0 and the length
       of `tuple_type`.
     tuple_type: Instance of `computation_types.NamedTupleType` as described in
-      the docstring o `_remap_graph_inputs`.
+      the docstring of `_remap_graph_inputs`.
 
   Returns:
     An instance of `computation_types.NamedTupleType` containing
     prefix identical to that constructed from selecting `list_of_indices` in
     order from `tuple_type`, with the remaining elements being the remaining
     elements of `tuple_type` in order.
   """
@@ -1078,36 +1077,35 @@
   `_construct_padding` will recover `tuple_type`.
 
   These invariants are utilized in `_remap_graph_inputs` to construct a
   TensorFlow computation with the same semantics as `graph`, but accepting
   a parameter of type `tuple_type`.
 
   Args:
-    graph: Instance of `computation_building_blocks.CompiledComputation` whose
-      parameter type we are trying to match with `tuple_type` if possible.
+    graph: Instance of `building_blocks.CompiledComputation` whose parameter
+      type we are trying to match with `tuple_type` if possible.
     list_of_indices: Python `list` containing integers between 0 and the length
       of `tuple_type`.
     tuple_type: Instance of `computation_types.NamedTupleType` as described
       above.
 
   Returns:
-    An instance of `computation_building_blocks.CompiledComputation` which
+    An instance of `building_blocks.CompiledComputation` which
     contains the same logic as the input `graph`, but accepts an argument of
     type `tuple_type`.
 
   Raises:
     TypeError: If `tuple_type` is not a `computation_types.NamedTupleType` or
     `list_of_indices` is not a `list`.
     ValueError: If `list_of_indices` contains an index less than 0 or out of
     range for the `tuple_type`.
   """
   # TODO(b/133328350): Extend _remap_graph_inputs to allow for multiple reuse of
   # selections.
-  py_typecheck.check_type(graph,
-                          computation_building_blocks.CompiledComputation)
+  py_typecheck.check_type(graph, building_blocks.CompiledComputation)
   py_typecheck.check_type(graph.type_signature.parameter,
                           computation_types.NamedTupleType)
   py_typecheck.check_type(tuple_type, computation_types.NamedTupleType)
   py_typecheck.check_type(list_of_indices, list)
   tuple_type_len = len(tuple_type)
   if len(set(list_of_indices)) != len(list_of_indices):
     raise ValueError('Support for repeated indices is not yet implemented.')
@@ -1143,24 +1141,22 @@
 
   Notice that we cannot simply transform the logic strictly under the
   Lambda before encountering the Lambda, as we must still bind the
   Reference to the parameter of the Lambda.
   """
 
   def should_transform(self, comp):
-    return (isinstance(comp, computation_building_blocks.Lambda) and isinstance(
-        comp.parameter_type, computation_types.NamedTupleType) and
-            isinstance(comp.result, computation_building_blocks.Call) and
-            isinstance(comp.result.function,
-                       computation_building_blocks.CompiledComputation) and
-            isinstance(comp.result.argument,
-                       computation_building_blocks.Selection) and
-            isinstance(comp.result.argument.source,
-                       computation_building_blocks.Reference) and
-            comp.result.argument.source.name == comp.parameter_name)
+    return (
+        isinstance(comp, building_blocks.Lambda) and
+        isinstance(comp.parameter_type, computation_types.NamedTupleType) and
+        isinstance(comp.result, building_blocks.Call) and isinstance(
+            comp.result.function, building_blocks.CompiledComputation) and
+        isinstance(comp.result.argument, building_blocks.Selection) and
+        isinstance(comp.result.argument.source, building_blocks.Reference) and
+        comp.result.argument.source.name == comp.parameter_name)
 
   def transform(self, comp):
     if not self.should_transform(comp):
       return comp, False
     parameter_type_elements = anonymous_tuple.to_elements(comp.parameter_type)
     if comp.result.argument.name is None:
       index_of_selection = comp.result.argument.index
@@ -1168,16 +1164,19 @@
       index_of_selection = [x[0] for x in parameter_type_elements
                            ].index(comp.result.argument.name)
 
     name = parameter_type_elements[index_of_selection][0]
 
     graph_with_wrapped_parameter = bind_graph_parameter_as_tuple(
         comp.result.function, name=name)
-    return _remap_graph_inputs(graph_with_wrapped_parameter,
-                               [index_of_selection], comp.parameter_type), True
+    remapped = _remap_graph_inputs(graph_with_wrapped_parameter,
+                                   [index_of_selection], comp.parameter_type)
+    pruned = building_blocks.CompiledComputation(
+        proto_transformations.prune_tensorflow_proto(remapped.proto))
+    return pruned, True
 
 
 class LambdaToCalledTupleOfSelectionsFromArg(transformation_utils.TransformSpec
                                             ):
   r"""Identifies a lambda to a called graph on a tuple of selections.
 
   Notice the selections here must be selections from the argument of the
@@ -1187,43 +1186,43 @@
 
                               Lambda(arg)
                                   |
                                 Call
                                /    \
             CompiledComputation(x)   Tuple
                                     / ... \
-                          Selection(x)     Selection(y)
+                          Selection(a)     Selection(b)
                                |                |
                             Ref(arg)           Ref(arg)
 
   into:
 
                        CompiledComputation
 
   By pushing the selection and tuple creation logic into the
   CompiledComputation.
   """
 
   def should_transform(self, comp):
-    if not (isinstance(comp, computation_building_blocks.Lambda) and
+    if not (isinstance(comp, building_blocks.Lambda) and
             isinstance(comp.parameter_type, computation_types.NamedTupleType)):
       return False
     result = comp.result
-    if not (isinstance(result, computation_building_blocks.Call) and isinstance(
-        result.function, computation_building_blocks.CompiledComputation)):
+    if not (isinstance(result, building_blocks.Call) and
+            isinstance(result.function, building_blocks.CompiledComputation)):
       return False
     compiled_comp_arg = result.argument
-    if not isinstance(compiled_comp_arg, computation_building_blocks.Tuple):
+    if not isinstance(compiled_comp_arg, building_blocks.Tuple):
       return False
     if not all(
-        isinstance(tuple_elem, computation_building_blocks.Selection)
+        isinstance(tuple_elem, building_blocks.Selection)
         for tuple_elem in compiled_comp_arg):
       return False
     if not all(
-        isinstance(tuple_elem.source, computation_building_blocks.Reference)
+        isinstance(tuple_elem.source, building_blocks.Reference)
         for tuple_elem in compiled_comp_arg):
       return False
     if not all(tuple_elem.source.name == comp.parameter_name
                for tuple_elem in compiled_comp_arg):
       return False
     return True
 
@@ -1235,17 +1234,20 @@
                        'we cannot ask a TF computation to forget about '
                        'any of its inputs. You have tried to replace a TF '
                        'computation accepting {} arguments with one '
                        ' {} arguments.'.format(
                            len(comp.result.argument.type_signature),
                            len(comp.parameter_type)))
     parameter_names = [
-        x[0] for x in anonymous_tuple.to_elements(comp.parameter_type)
+        x[0] for x in anonymous_tuple.iter_elements(comp.parameter_type)
     ]
     parameter_map = []
     for sel in comp.result.argument:
       if sel.index is not None:
         parameter_map.append(sel.index)
       else:
         parameter_map.append(parameter_names.index(sel.name))
-    return _remap_graph_inputs(comp.result.function, parameter_map,
-                               comp.parameter_type), True
+    inputs_mapped = _remap_graph_inputs(comp.result.function, parameter_map,
+                                        comp.parameter_type)
+    pruned = building_blocks.CompiledComputation(
+        proto_transformations.prune_tensorflow_proto(inputs_mapped.proto))
+    return pruned, True
```

## tensorflow_federated/python/core/impl/compiler_pipeline.py

```diff
@@ -17,18 +17,19 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_base
-from tensorflow_federated.python.core.impl import computation_building_blocks
 from tensorflow_federated.python.core.impl import computation_impl
 from tensorflow_federated.python.core.impl import context_stack_base
 from tensorflow_federated.python.core.impl import transformations
+from tensorflow_federated.python.core.impl import value_transformations
+from tensorflow_federated.python.core.impl.compiler import building_blocks
 
 
 class CompilerPipeline(object):
   """The compiler pipeline.
 
   This pipeline will eventually be made configurable, and driven largely by what
   the targeted backend can support. The set of conversions that are currently
@@ -57,33 +58,37 @@
     Returns:
       An instance of `computation_base.Computation` that repeesents the result.
     """
     py_typecheck.check_type(computation_to_compile,
                             computation_base.Computation)
     computation_proto = computation_impl.ComputationImpl.get_proto(
         computation_to_compile)
+    py_typecheck.check_type(computation_proto, pb.Computation)
+    comp = building_blocks.ComputationBuildingBlock.from_proto(
+        computation_proto)
 
     # TODO(b/113123410): Add a compiler options argument that characterizes the
     # desired form of the output. To be driven by what the specific backend the
     # pipeline is targeting is able to understand. Pending a more fleshed out
     # design of the backend API.
 
-    py_typecheck.check_type(computation_proto, pb.Computation)
-    comp = computation_building_blocks.ComputationBuildingBlock.from_proto(
-        computation_proto)
-
     # Replace intrinsics with their bodies, for now manually in a fixed order.
     # TODO(b/113123410): Replace this with a more automated implementation that
     # does not rely on manual maintenance.
-    comp, _ = transformations.replace_all_intrinsics_with_bodies(
+    comp, _ = value_transformations.replace_all_intrinsics_with_bodies(
         comp, self._context_stack)
 
     # Replaces called lambdas with LET constructs with a single local symbol.
     comp, _ = transformations.replace_called_lambda_with_block(comp)
-    # TODO(b/113123410): Add more transformations to simplify and optimize the
-    # structure, e.g., such as:
-    # * removing unnecessary lambdas,
-    # * flatteting the structure,
-    # * merging TensorFlow blocks where appropriate,
-    # * ...and so on.
+
+    # Removes maped or applied identities.
+    comp, _ = transformations.remove_mapped_or_applied_identity(comp)
+
+    # Remove duplicate computations. This is important! otherwise the semantics
+    # non-deterministic computations (e.g. a `tff.tf_computation` depending on
+    # `tf.random`) will give unexpected behavior. Additionally, this may reduce
+    # the amount of calls into TF for some ASTs.
+    comp, _ = transformations.uniquify_reference_names(comp)
+    comp, _ = transformations.extract_computations(comp)
+    comp, _ = transformations.remove_duplicate_computations(comp)
 
     return computation_impl.ComputationImpl(comp.proto, self._context_stack)
```

## tensorflow_federated/python/core/impl/computation_impl.py

```diff
@@ -18,17 +18,17 @@
 from __future__ import division
 from __future__ import print_function
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.impl import context_stack_base
-from tensorflow_federated.python.core.impl import function_utils
-from tensorflow_federated.python.core.impl import type_serialization
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import type_serialization
+from tensorflow_federated.python.core.impl.utils import function_utils
 
 
 class ComputationImpl(function_utils.ConcreteFunction):
   """An implementation of the base interface cb.Computation."""
 
   @classmethod
   def get_proto(cls, value):
```

## tensorflow_federated/python/core/impl/computation_wrapper.py

```diff
@@ -18,16 +18,16 @@
 from __future__ import division
 from __future__ import print_function
 
 import types
 
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
-from tensorflow_federated.python.core.impl import function_utils
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.utils import function_utils
 
 
 def _wrap(fn, parameter_type, wrapper_fn):
   """Wrap a given `fn` with a given `parameter_type` using `wrapper_fn`.
 
   This method does not handle the multiple modes of usage as wrapper/decorator,
   as those are handled by ComputationWrapper below. It focused on the simple
```

## tensorflow_federated/python/core/impl/computation_wrapper_instances.py

```diff
@@ -15,22 +15,22 @@
 """Definitions of specific computation wrapper instances."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 from tensorflow_federated.python.common_libs import py_typecheck
-from tensorflow_federated.python.core.impl import computation_building_blocks
 from tensorflow_federated.python.core.impl import computation_impl
 from tensorflow_federated.python.core.impl import computation_wrapper
 from tensorflow_federated.python.core.impl import context_stack_impl
 from tensorflow_federated.python.core.impl import federated_computation_utils
-from tensorflow_federated.python.core.impl import function_utils
 from tensorflow_federated.python.core.impl import tensorflow_serialization
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import building_blocks
+from tensorflow_federated.python.core.impl.utils import function_utils
 
 
 def _tf_wrapper_fn(target_fn, parameter_type, unpack, name=None):
   """Wrapper function to plug Tensorflow logic in to TFF framework."""
   del name  # Unused.
   target_fn = function_utils.wrap_as_zero_or_one_arg_callable(
       target_fn, parameter_type, unpack)
@@ -82,10 +82,10 @@
 federated_computation_wrapper = computation_wrapper.ComputationWrapper(
     _federated_computation_wrapper_fn)
 
 
 def building_block_to_computation(building_block):
   """Converts a computation building block to a computation impl."""
   py_typecheck.check_type(building_block,
-                          computation_building_blocks.ComputationBuildingBlock)
+                          building_blocks.ComputationBuildingBlock)
   return computation_impl.ComputationImpl(building_block.proto,
                                           context_stack_impl.context_stack)
```

## tensorflow_federated/python/core/impl/concurrent_executor.py

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A concurrent executor that does work asynchronously in multiple threads."""
 
 import asyncio
 import functools
 import threading
+import weakref
 
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.impl import executor_base
 
 
 class ConcurrentExecutor(executor_base.Executor):
   """The concurrent executor delegates work to a separate thread.
@@ -45,20 +46,22 @@
     self._event_loop = asyncio.new_event_loop()
 
     def run_loop(loop):
       loop.run_forever()
       loop.close()
 
     self._thread = threading.Thread(
-        target=functools.partial(run_loop, self._event_loop))
+        target=functools.partial(run_loop, self._event_loop), daemon=True)
     self._thread.start()
 
-  def __del__(self):
-    self._event_loop.call_soon_threadsafe(self._event_loop.stop)
-    self._thread.join()
+    def finalizer(loop, thread):
+      loop.call_soon_threadsafe(loop.stop)
+      thread.join()
+
+    weakref.finalize(self, finalizer, self._event_loop, self._thread)
 
   def _delegate(self, coro):
     return asyncio.wrap_future(
         asyncio.run_coroutine_threadsafe(coro, self._event_loop))
 
   async def create_value(self, value, type_spec=None):
     return await self._delegate(
```

## tensorflow_federated/python/core/impl/eager_executor.py

```diff
@@ -23,17 +23,17 @@
 from tensorflow_federated.python.common_libs import serialization_utils
 from tensorflow_federated.python.core.api import computation_base
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.api import typed_object
 from tensorflow_federated.python.core.impl import computation_impl
 from tensorflow_federated.python.core.impl import executor_base
 from tensorflow_federated.python.core.impl import executor_value_base
-from tensorflow_federated.python.core.impl import graph_utils
-from tensorflow_federated.python.core.impl import type_serialization
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import type_serialization
+from tensorflow_federated.python.core.impl.utils import tensorflow_utils
 from tensorflow_federated.python.tensorflow_libs import graph_merge
 
 
 def embed_tensorflow_computation(comp, type_spec=None, device=None):
   """Embeds a TensorFlow computation for use in the eager context.
 
   Args:
@@ -45,28 +45,25 @@
     Either a one-argument or a zero-argument callable that executes the
     computation in eager mode.
 
   Raises:
     TypeError: If arguments are of the wrong types, e.g., in `comp` is not a
       TensorFlow computation.
   """
-  # TODO(b/134543154): Decide whether this belongs in `graph_utils.py` since
-  # it deals exclusively with eager mode. Incubate here, and potentially move
-  # there, once stable.
-
-  if device is not None:
-    raise NotImplementedError('Unable to embed TF code on a specific device.')
+  # TODO(b/134543154): Decide whether this belongs in `tensorflow_utils.py`
+  # since it deals exclusively with eager mode. Incubate here, and potentially
+  # move there, once stable.
 
   py_typecheck.check_type(comp, pb.Computation)
   comp_type = type_serialization.deserialize_type(comp.type)
   type_spec = computation_types.to_type(type_spec)
   if type_spec is not None:
     if not type_utils.are_equivalent_types(type_spec, comp_type):
       raise TypeError('Expected a computation of type {}, got {}.'.format(
-          str(type_spec), str(comp_type)))
+          type_spec, comp_type))
   else:
     type_spec = comp_type
   which_computation = comp.WhichOneof('computation')
   if which_computation != 'tensorflow':
     raise TypeError('Expected a TensorFlow computation, found {}.'.format(
         which_computation))
 
@@ -74,34 +71,43 @@
     param_type = type_spec.parameter
     result_type = type_spec.result
   else:
     param_type = None
     result_type = type_spec
 
   if param_type is not None:
-    input_tensor_names = graph_utils.extract_tensor_names_from_binding(
+    input_tensor_names = tensorflow_utils.extract_tensor_names_from_binding(
         comp.tensorflow.parameter)
   else:
     input_tensor_names = []
 
-  output_tensor_names = graph_utils.extract_tensor_names_from_binding(
+  output_tensor_names = tensorflow_utils.extract_tensor_names_from_binding(
       comp.tensorflow.result)
 
   def function_to_wrap(*args):  # pylint: disable=missing-docstring
     if len(args) != len(input_tensor_names):
       raise RuntimeError('Expected {} arguments, found {}.'.format(
-          str(len(input_tensor_names)), str(len(args))))
+          len(input_tensor_names), len(args)))
     graph_def = serialization_utils.unpack_graph_def(comp.tensorflow.graph_def)
     init_op = comp.tensorflow.initialize_op
     if init_op:
-      graph_def = graph_utils.add_control_deps_for_init_op(graph_def, init_op)
-    return tf.import_graph_def(
-        graph_merge.uniquify_shared_names(graph_def),
-        input_map=dict(list(zip(input_tensor_names, args))),
-        return_elements=output_tensor_names)
+      graph_def = tensorflow_utils.add_control_deps_for_init_op(
+          graph_def, init_op)
+
+    def _import_fn():
+      return tf.import_graph_def(
+          graph_merge.uniquify_shared_names(graph_def),
+          input_map=dict(list(zip(input_tensor_names, args))),
+          return_elements=output_tensor_names)
+
+    if device is not None:
+      with tf.device(device):
+        return _import_fn()
+    else:
+      return _import_fn()
 
   signature = []
   param_fns = []
   if param_type is not None:
     for spec in anonymous_tuple.flatten(type_spec.parameter):
       if isinstance(spec, computation_types.TensorType):
         signature.append(tf.TensorSpec(spec.shape, spec.dtype))
@@ -128,38 +134,49 @@
 
   def _fn_to_return(arg, param_fns, wrapped_fn):  # pylint:disable=missing-docstring
     param_elements = []
     if arg is not None:
       arg_parts = anonymous_tuple.flatten(arg)
       if len(arg_parts) != len(param_fns):
         raise RuntimeError('Expected {} arguments, found {}.'.format(
-            str(len(param_fns)), str(len(arg_parts))))
+            len(param_fns), len(arg_parts)))
       for arg_part, param_fn in zip(arg_parts, param_fns):
         param_elements.append(param_fn(arg_part))
     result_parts = wrapped_fn(*param_elements)
     result_elements = []
     for result_part, result_fn in zip(result_parts, result_fns):
       result_elements.append(result_fn(result_part))
     return anonymous_tuple.pack_sequence_as(result_type, result_elements)
 
   fn_to_return = lambda arg, p=param_fns, w=wrapped_fn: _fn_to_return(arg, p, w)
+
+  if device is not None:
+    old_fn_to_return = fn_to_return
+
+    # pylint: disable=function-redefined
+    def fn_to_return(x):
+      with tf.device(device):
+        return old_fn_to_return(x)
+
+    # pylint: enable=function-redefined
+
   if param_type is not None:
     return lambda arg: fn_to_return(arg)  # pylint: disable=unnecessary-lambda
   else:
     return lambda: fn_to_return(None)
 
 
 def to_representation_for_type(value, type_spec=None, device=None):
   """Verifies or converts the `value` to an eager objct matching `type_spec`.
 
   WARNING: This function is only partially implemented. It does not support
   data sets at this point.
 
   The output of this function is always an eager tensor, eager dataset, a
-  representation of a TensorFlow computtion, or a nested structure of those
+  representation of a TensorFlow computation, or a nested structure of those
   that matches `type_spec`, and when `device` has been specified, everything
   is placed on that device on a best-effort basis.
 
   TensorFlow computations are represented here as zero- or one-argument Python
   callables that accept their entire argument bundle as a single Python object.
 
   Args:
@@ -171,73 +188,73 @@
 
   Returns:
     Either `value` itself, or a modified version of it.
 
   Raises:
     TypeError: If the `value` is not compatible with `type_spec`.
   """
-  if device is not None:
-    py_typecheck.check_type(device, str)
-    with tf.device(device):
-      return to_representation_for_type(value, type_spec=type_spec, device=None)
   type_spec = type_utils.reconcile_value_with_type_spec(value, type_spec)
-  if isinstance(value, EagerValue):
-    return value.internal_representation
-  if isinstance(value, executor_value_base.ExecutorValue):
-    raise TypeError(
-        'Cannot accept a value embedded within a non-eager executor.')
   if isinstance(value, computation_base.Computation):
     return to_representation_for_type(
         computation_impl.ComputationImpl.get_proto(value), type_spec, device)
-  if isinstance(value, pb.Computation):
+  elif isinstance(value, pb.Computation):
     return embed_tensorflow_computation(value, type_spec, device)
-  if isinstance(type_spec, computation_types.TensorType):
-    if not isinstance(value, tf.Tensor):
-      if isinstance(value, np.ndarray):
-        value = tf.constant(value, dtype=type_spec.dtype)
-      else:
-        value = tf.constant(value, dtype=type_spec.dtype, shape=type_spec.shape)
-    value_type = (
-        computation_types.TensorType(value.dtype.base_dtype, value.shape))
-    if not type_utils.is_assignable_from(type_spec, value_type):
-      raise TypeError(
-          'The apparent type {} of a tensor {} does not match the expected '
-          'type {}.'.format(str(value_type), str(value), str(type_spec)))
-    return value
   elif isinstance(type_spec, computation_types.NamedTupleType):
     type_elem = anonymous_tuple.to_elements(type_spec)
     value_elem = (
         anonymous_tuple.to_elements(anonymous_tuple.from_container(value)))
     result_elem = []
     if len(type_elem) != len(value_elem):
       raise TypeError('Expected a {}-element tuple, found {} elements.'.format(
-          str(len(type_elem)), str(len(value_elem))))
+          len(type_elem), len(value_elem)))
     for (t_name, el_type), (v_name, el_val) in zip(type_elem, value_elem):
       if t_name != v_name:
         raise TypeError(
             'Mismatching element names in type vs. value: {} vs. {}.'.format(
                 t_name, v_name))
       el_repr = to_representation_for_type(el_val, el_type, device)
       result_elem.append((t_name, el_repr))
     return anonymous_tuple.AnonymousTuple(result_elem)
+  elif device is not None:
+    py_typecheck.check_type(device, str)
+    with tf.device(device):
+      return to_representation_for_type(value, type_spec=type_spec, device=None)
+  elif isinstance(value, EagerValue):
+    return value.internal_representation
+  elif isinstance(value, executor_value_base.ExecutorValue):
+    raise TypeError(
+        'Cannot accept a value embedded within a non-eager executor.')
+  elif isinstance(type_spec, computation_types.TensorType):
+    if not isinstance(value, tf.Tensor):
+      if isinstance(value, np.ndarray):
+        value = tf.constant(value, dtype=type_spec.dtype)
+      else:
+        value = tf.constant(value, dtype=type_spec.dtype, shape=type_spec.shape)
+    value_type = (
+        computation_types.TensorType(value.dtype.base_dtype, value.shape))
+    if not type_utils.is_assignable_from(type_spec, value_type):
+      raise TypeError(
+          'The apparent type {} of a tensor {} does not match the expected '
+          'type {}.'.format(value_type, value, type_spec))
+    return value
   elif isinstance(type_spec, computation_types.SequenceType):
     if isinstance(value, list):
-      value = graph_utils.make_data_set_from_elements(None, value,
-                                                      type_spec.element)
+      value = tensorflow_utils.make_data_set_from_elements(
+          None, value, type_spec.element)
     py_typecheck.check_type(
         value,
         (tf.data.Dataset, tf.compat.v1.data.Dataset, tf.compat.v2.data.Dataset))
     element_type = type_utils.tf_dtypes_and_shapes_to_type(
         tf.compat.v1.data.get_output_types(value),
         tf.compat.v1.data.get_output_shapes(value))
     value_type = computation_types.SequenceType(element_type)
     type_utils.check_assignable_from(type_spec, value_type)
     return value
   else:
-    raise TypeError('Unexpected type {}.'.format(str(type_spec)))
+    raise TypeError('Unexpected type {}.'.format(type_spec))
 
 
 class EagerValue(executor_value_base.ExecutorValue):
   """A representation of an eager value managed by the eager executor."""
 
   def __init__(self, value, type_spec=None, device=None):
     """Creates an instance of a value in this executor.
@@ -368,15 +385,15 @@
       TypeError: If the arguments are of the wrong types.
     """
     py_typecheck.check_type(comp, EagerValue)
     if arg is not None:
       py_typecheck.check_type(arg, EagerValue)
     if not isinstance(comp.type_signature, computation_types.FunctionType):
       raise TypeError('Expected a functional type, found {}'.format(
-          str(comp.type_signature)))
+          comp.type_signature))
     if comp.type_signature.parameter is not None:
       return EagerValue(
           comp.internal_representation(arg.internal_representation),
           comp.type_signature.result, self._device)
     elif arg is None:
       return EagerValue(comp.internal_representation(),
                         comp.type_signature.result, self._device)
@@ -426,16 +443,16 @@
                             computation_types.NamedTupleType)
     py_typecheck.check_type(source.internal_representation,
                             anonymous_tuple.AnonymousTuple)
     if index is not None:
       py_typecheck.check_type(index, int)
       if name is not None:
         raise ValueError(
-            'Cannot simulatenously specify name {} and index {}.'.format(
-                str(name), str(index)))
+            'Cannot simultaneously specify name {} and index {}.'.format(
+                name, index))
       else:
         return EagerValue(source.internal_representation[index],
                           source.type_signature[index])
     elif name is not None:
       py_typecheck.check_type(name, str)
       return EagerValue(
           getattr(source.internal_representation, str(name)),
```

## tensorflow_federated/python/core/impl/execution_context.py

```diff
@@ -17,29 +17,48 @@
 import asyncio
 
 import tensorflow as tf
 
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
+from tensorflow_federated.python.core.api import typed_object
 from tensorflow_federated.python.core.impl import context_base
 from tensorflow_federated.python.core.impl import executor_base
 from tensorflow_federated.python.core.impl import executor_value_base
+from tensorflow_federated.python.core.impl import runtime_utils
 from tensorflow_federated.python.core.impl import type_utils
 
 
 def _unwrap(value):
   if isinstance(value, tf.Tensor):
     return value.numpy()
   elif isinstance(value, anonymous_tuple.AnonymousTuple):
     return anonymous_tuple.map_structure(_unwrap, value)
   else:
     return value
 
 
+class ExecutionContextValue(typed_object.TypedObject):
+  """Wrapper class for values produced by `ExecutionContext`."""
+
+  def __init__(self, value, type_spec):
+    py_typecheck.check_type(type_spec, computation_types.Type)
+    self._value = value
+    self._type_spec = type_spec
+
+  @property
+  def type_signature(self):
+    return self._type_spec
+
+  @property
+  def value(self):
+    return self._value
+
+
 async def _ingest(executor, val, type_spec):
   """A coroutine that handles ingestion.
 
   Args:
     executor: An instance of `executor_base.Executor`.
     val: The first argument to `context_base.Context.ingest()`.
     type_spec: The second argument to `context_base.Context.ingest()`.
@@ -55,15 +74,15 @@
   elif (isinstance(val, anonymous_tuple.AnonymousTuple) and
         not isinstance(type_spec, computation_types.FederatedType)):
     py_typecheck.check_type(type_spec, computation_types.NamedTupleType)
     v_elem = anonymous_tuple.to_elements(val)
     t_elem = anonymous_tuple.to_elements(type_spec)
     if ([k for k, _ in v_elem] != [k for k, _ in t_elem]):
       raise ValueError('Value {} does not match type {}.'.format(
-          str(val), str(type_spec)))
+          val, type_spec))
     ingested = []
     for (_, v), (_, t) in zip(v_elem, t_elem):
       ingested.append(_ingest(executor, v, t))
     ingested = await asyncio.gather(*ingested)
     return await executor.create_tuple(
         anonymous_tuple.AnonymousTuple([
             (name, val) for (name, _), val in zip(t_elem, ingested)
@@ -93,28 +112,48 @@
   result_val = _unwrap(await result.compute())
   if type_utils.is_anon_tuple_with_py_container(result_val, result_type):
     return type_utils.convert_to_py_container(result_val, result_type)
   else:
     return result_val
 
 
+def _unwrap_execution_context_value(val):
+  """Recursively removes wrapping from `val` under anonymous tuples."""
+  if isinstance(val, anonymous_tuple.AnonymousTuple):
+    return anonymous_tuple.map_structure(_unwrap_execution_context_value, val)
+  elif isinstance(val, ExecutionContextValue):
+    return _unwrap_execution_context_value(val.value)
+  else:
+    return val
+
+
 class ExecutionContext(context_base.Context):
   """Represents an execution context backed by an `executor_base.Executor`."""
 
-  def __init__(self, executor):
-    """Constructs a new execution context backed by `executor`.
+  def __init__(self, executor_fn):
+    """Initializes execution context.
 
     Args:
-      executor: An instance of `executor_base.Executor`.
+      executor_fn: Callable taking a dict of `placement_literals.Placement` keys
+        and integer values to an instance of `executor_base.Executor`.
     """
-    py_typecheck.check_type(executor, executor_base.Executor)
-    self._executor = executor
+    # TODO(b/140112504): Follow up with an ExecutorFactory abstract class.
+    py_typecheck.check_callable(executor_fn)
+    self._executor_factory = executor_fn
 
   def ingest(self, val, type_spec):
-    result = asyncio.get_event_loop().run_until_complete(
-        _ingest(self._executor, val, type_spec))
-    py_typecheck.check_type(result, executor_value_base.ExecutorValue)
-    return result
+    return ExecutionContextValue(val, type_spec)
 
   def invoke(self, comp, arg):
+    executor = self._executor_factory({})
+    py_typecheck.check_type(executor, executor_base.Executor)
+    if arg:
+      py_typecheck.check_type(arg, ExecutionContextValue)
+      unwrapped_arg = _unwrap_execution_context_value(arg)
+      cardinalities = runtime_utils.infer_cardinalities(unwrapped_arg,
+                                                        arg.type_signature)
+      executor = self._executor_factory(cardinalities)
+      py_typecheck.check_type(executor, executor_base.Executor)
+      arg = asyncio.get_event_loop().run_until_complete(
+          _ingest(executor, unwrapped_arg, arg.type_signature))
     return asyncio.get_event_loop().run_until_complete(
-        _invoke(self._executor, comp, arg))
+        _invoke(executor, comp, arg))
```

## tensorflow_federated/python/core/impl/executor_service.py

```diff
@@ -15,14 +15,15 @@
 """A service wrapper around an executor that makes it accessible over gRPC."""
 
 import asyncio
 import functools
 import threading
 import traceback
 import uuid
+import weakref
 
 from absl import logging
 import grpc
 
 from tensorflow_federated.proto.v0 import executor_pb2
 from tensorflow_federated.proto.v0 import executor_pb2_grpc
 from tensorflow_federated.python.common_libs import anonymous_tuple
@@ -52,20 +53,43 @@
 
     def run_loop(loop):
       loop.run_forever()
       loop.close()
 
     self._event_loop = asyncio.new_event_loop()
     self._thread = threading.Thread(
-        target=functools.partial(run_loop, self._event_loop))
+        target=functools.partial(run_loop, self._event_loop), daemon=True)
     self._thread.start()
 
-  def __del__(self):
-    self._event_loop.call_soon_threadsafe(self._event_loop.stop)
-    self._thread.join()
+    def finalize(loop, thread):
+      loop.call_soon_threadsafe(loop.stop)
+      thread.join()
+
+    weakref.finalize(self, finalize, self._event_loop, self._thread)
+
+  def Execute(self, request_iter, context):
+    for v in request_iter:
+      which = v.WhichOneof('request')
+      if not which:
+        raise RuntimeError('Must set a request type')
+      if which == 'create_value':
+        yield executor_pb2.ExecuteResponse(
+            create_value=self.CreateValue(v.create_value, context))
+      elif which == 'create_call':
+        yield executor_pb2.ExecuteResponse(
+            create_call=self.CreateCall(v.create_call, context))
+      elif which == 'create_tuple':
+        yield executor_pb2.ExecuteResponse(
+            create_tuple=self.CreateTuple(v.create_tuple, context))
+      elif which == 'create_selection':
+        yield executor_pb2.ExecuteResponse(
+            create_selection=self.CreateSelection(v.create_selection, context))
+      elif which == 'compute':
+        yield executor_pb2.ExecuteResponse(
+            compute=self.Compute(v.compute, context))
 
   def CreateValue(self, request, context):
     """Creates a value embedded in the executor.
 
     Args:
       request: An instance of `executor_pb2.CreateValueRequest`.
       context: An instance of `grpc.ServicerContext`.
```

## tensorflow_federated/python/core/impl/executor_service_utils.py

```diff
@@ -20,16 +20,18 @@
 from google.protobuf import any_pb2
 from tensorflow_federated.proto.v0 import computation_pb2
 from tensorflow_federated.proto.v0 import executor_pb2
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.impl import computation_impl
-from tensorflow_federated.python.core.impl import type_serialization
+from tensorflow_federated.python.core.impl import tensorflow_serialization
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import type_serialization
+from tensorflow_federated.python.core.impl.utils import tensorflow_utils
 
 
 def serialize_tensor_value(value, type_spec=None):
   """Serializes a tensor value into `executor_pb2.Value`.
 
   Args:
     value: A Numpy array or other object understood by `tf.make_tensor_proto`.
@@ -110,14 +112,75 @@
   value_type = computation_types.TensorType(
       dtype=tf.DType(tensor_proto.dtype),
       shape=tf.TensorShape(tensor_proto.tensor_shape))
 
   return tensor_value, value_type
 
 
+def serialize_sequence_value(value):
+  """Serializes a `tf.data.Dataset` value into `executor_pb2.Value`.
+
+  Args:
+    value: A `tf.data.Dataset`, or equivalent.
+
+  Returns:
+    A tuple `(value_proto, type_spec)` in which `value_proto` is an instance
+    of `executor_pb2.Value` with the serialized content of `value`, and
+    `type_spec` is the type of the serialized value.
+  """
+  py_typecheck.check_type(value, tensorflow_utils.DATASET_REPRESENTATION_TYPES)
+  # TFF must store the type spec here because TF will lose the ordering of the
+  # names for `tf.data.Dataset` that return elements of `collections.Mapping`
+  # type. This allows TFF to preserve and restore the key ordering upon
+  # deserialization.
+  element_type = computation_types.to_type(
+      tf.data.experimental.get_structure(value))
+  return executor_pb2.Value(
+      sequence=executor_pb2.Value.Sequence(
+          zipped_saved_model=tensorflow_serialization.serialize_dataset(value),
+          element_type=type_serialization.serialize_type(element_type)))
+
+
+def deserialize_sequence_value(sequence_value_proto):
+  """Deserializes a `tf.data.Dataset`.
+
+  Args:
+    sequence_value_proto: `Sequence` protocol buffer message.
+
+  Returns:
+    A tuple of `(tf.data.Dataset, tff.Type)`.
+  """
+  py_typecheck.check_type(sequence_value_proto, executor_pb2.Value.Sequence)
+
+  which_value = sequence_value_proto.WhichOneof('value')
+  if which_value == 'zipped_saved_model':
+    ds = tensorflow_serialization.deserialize_dataset(
+        sequence_value_proto.zipped_saved_model)
+  else:
+    raise NotImplementedError(
+        'Deserializing Sequences enocded as {!s} has not been implemented'
+        .format(which_value))
+
+  element_type = type_serialization.deserialize_type(
+      sequence_value_proto.element_type)
+
+  # If a serialized dataset had elements of nested structes of tensors (e.g.
+  # `dict`, `OrderedDict`), the deserialized dataset will return `dict`,
+  # `tuple`, or `namedtuple` (loses `collections.OrderedDict` in a conversion).
+  #
+  # Since the dataset will only be used inside TFF, we wrap the dictionary
+  # coming from TF in an `OrderedDict` when necessary (a type that both TF and
+  # TFF understand), using the field order stored in the TFF type stored during
+  # serialization.
+  ds = tensorflow_utils.coerce_dataset_elements_to_tff_type_spec(
+      ds, element_type)
+
+  return ds, computation_types.SequenceType(element=element_type)
+
+
 def serialize_value(value, type_spec=None):
   """Serializes a value into `executor_pb2.Value`.
 
   Args:
     value: A value to be serialized.
     type_spec: Optional type spec, a `tff.Type` or something convertible to it.
 
@@ -151,14 +214,45 @@
       e_proto, _ = serialize_value(e_val, e_type)
       tup_elems.append(
           executor_pb2.Value.Tuple.Element(
               name=e_name if e_name else None, value=e_proto))
     result_proto = (
         executor_pb2.Value(tuple=executor_pb2.Value.Tuple(element=tup_elems)))
     return result_proto, type_spec
+  elif isinstance(type_spec, computation_types.SequenceType):
+    if not isinstance(value, tensorflow_utils.DATASET_REPRESENTATION_TYPES):
+      raise TypeError(
+          'Cannot serialize Python type {!s} as TFF type {!s}.'.format(
+              py_typecheck.type_string(type(value)),
+              type_spec if type_spec is not None else 'unknown'))
+
+    value_type = computation_types.SequenceType(
+        computation_types.to_type(tf.data.experimental.get_structure(value)))
+    if not type_utils.is_assignable_from(type_spec, value_type):
+      raise TypeError(
+          'Cannot serialize dataset with elements of type {!s} as TFF type {!s}.'
+          .format(value_type,
+                  type_spec if type_spec is not None else 'unknown'))
+
+    return serialize_sequence_value(value), type_spec
+  elif isinstance(type_spec, computation_types.FederatedType):
+    if type_spec.all_equal:
+      value = [value]
+    else:
+      py_typecheck.check_type(value, list)
+    items = []
+    for v in value:
+      it, it_type = serialize_value(v, type_spec.member)
+      type_utils.check_assignable_from(type_spec.member, it_type)
+      items.append(it)
+    result_proto = executor_pb2.Value(
+        federated=executor_pb2.Value.Federated(
+            type=type_serialization.serialize_type(type_spec).federated,
+            value=items))
+    return result_proto, type_spec
   else:
     raise ValueError(
         'Unable to serialize value with Python type {} and {} TFF type.'.format(
             str(py_typecheck.type_string(type(value))),
             str(type_spec) if type_spec is not None else 'unknown'))
 
 
@@ -191,10 +285,28 @@
     for e in value_proto.tuple.element:
       name = e.name if e.name else None
       e_val, e_type = deserialize_value(e.value)
       val_elems.append((name, e_val))
       type_elems.append((name, e_type) if name else e_type)
     return (anonymous_tuple.AnonymousTuple(val_elems),
             computation_types.NamedTupleType(type_elems))
+  elif which_value == 'sequence':
+    return deserialize_sequence_value(value_proto.sequence)
+  elif which_value == 'federated':
+    type_spec = type_serialization.deserialize_type(
+        computation_pb2.Type(federated=value_proto.federated.type))
+    value = []
+    for item in value_proto.federated.value:
+      item_value, item_type = deserialize_value(item)
+      type_utils.check_assignable_from(type_spec.member, item_type)
+      value.append(item_value)
+    if type_spec.all_equal:
+      if len(value) == 1:
+        value = value[0]
+      else:
+        raise ValueError(
+            'Return an all_equal value with {} member consatituents.'.format(
+                len(value)))
+    return value, type_spec
   else:
     raise ValueError(
         'Unable to deserialize a value of type {}.'.format(which_value))
```

## tensorflow_federated/python/core/impl/executor_stacks.py

```diff
@@ -10,44 +10,201 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A collection of constructors for basic types of executor stacks."""
 
+import six
+
 from tensorflow_federated.python.common_libs import py_typecheck
+from tensorflow_federated.python.core.impl import caching_executor
+from tensorflow_federated.python.core.impl import composite_executor
 from tensorflow_federated.python.core.impl import concurrent_executor
 from tensorflow_federated.python.core.impl import eager_executor
+from tensorflow_federated.python.core.impl import executor_base
 from tensorflow_federated.python.core.impl import federated_executor
 from tensorflow_federated.python.core.impl import lambda_executor
-from tensorflow_federated.python.core.impl import placement_literals
+from tensorflow_federated.python.core.impl.compiler import placement_literals
 
 
-def create_local_executor(num_clients):
-  """Constructs an executor to execute computations on the local machine.
+def _complete_stack(ex):
+  return lambda_executor.LambdaExecutor(
+      caching_executor.CachingExecutor(
+          concurrent_executor.ConcurrentExecutor(ex)))
 
-  The initial temporary implementation requires that the number of clients be
-  specified in advance. This limitation will be removed in the near future.
 
-  NOTE: This function is only available in Python 3.
+def _create_bottom_stack():
+  return _complete_stack(eager_executor.EagerExecutor())
+
+
+def _create_federated_stack(num_clients):
+  executor_dict = {
+      placement_literals.CLIENTS: [
+          _create_bottom_stack() for _ in range(num_clients)
+      ],
+      placement_literals.SERVER: _create_bottom_stack(),
+      None: _create_bottom_stack()
+  }
+  return _complete_stack(federated_executor.FederatedExecutor(executor_dict))
+
+
+def _create_composite_stack(children):
+  return _complete_stack(
+      composite_executor.CompositeExecutor(_create_bottom_stack(), children))
+
+
+def _aggregate_stacks(executors, max_fanout):
+  """Aggregates multiple stacks into a single composite executor.
 
   Args:
-    num_clients: The number of clients.
+    executors: Executors to aggregate as a `list`.
+    max_fanout: The max fanout (see below).
 
   Returns:
-    An instance of `tff.framework.Executor` for single-machine use only.
+    An executor stack, potentially multi-level, that spans all `executors`.
+
+  Raises:
+    RuntimeError: If it can't create composite executors.
   """
-  # TODO(b/134543154): We should not have to specif the number of clients; this
-  # needs to go away once we flesh out all the remaining bits ad pieces.
+  py_typecheck.check_type(executors, list)
+  py_typecheck.check_type(max_fanout, int)
+  for ex in executors:
+    py_typecheck.check_type(ex, executor_base.Executor)
+  # Recursively construct as many levels as it takes to support all clients,
+  # reducing by the factor of `max_fanout` in each iteration, for up to
+  # `log(len(address_list)) / log(max_fanout)` iterations.
+  while len(executors) > 1:
+    new_executors = []
+    offset = 0
+    while offset < len(executors):
+      new_offset = offset + max_fanout
+      new_executors.append(
+          _create_composite_stack(executors[offset:new_offset]))
+      offset = new_offset
+    executors = new_executors
+  if len(executors) != 1:
+    raise RuntimeError('Expected 1 executor, got {}.'.format(len(executors)))
+  return executors[0]
+
+
+def _create_full_stack(num_clients, max_fanout):
+  """Creates a full executor stack.
+
+  Args:
+    num_clients: The number of clients to support. Must be 0 or larger.
+    max_fanout: The maximum fanout at any point in the hierarchy. Must be 1 or
+      larger.
 
+  Returns:
+    An executor stack, potentially multi-level, that spans all clients.
+
+  Raises:
+    ValueError: If the number of clients or fanout are not as specified.
+    RuntimeError: If the stack construction fails.
+  """
   py_typecheck.check_type(num_clients, int)
-  bottom_ex = lambda_executor.LambdaExecutor(eager_executor.EagerExecutor())
+  py_typecheck.check_type(max_fanout, int)
+  if num_clients < 0:
+    raise ValueError('Number of clients cannot be negative.')
+  if max_fanout < 1:
+    raise ValueError('Max fanout must be positive.')
+  if num_clients < 1:
+    return _create_federated_stack(0)
+  else:
+    executors = []
+    while num_clients > 0:
+      n = min(num_clients, max_fanout)
+      executors.append(_create_federated_stack(n))
+      num_clients -= n
+    return _aggregate_stacks(executors, max_fanout)
+
+
+def _create_explicit_cardinality_executor_fn(num_clients, max_fanout):
+  """Creates executor function with fixed cardinality."""
+
+  def _return_executor(_):
+    return _create_full_stack(num_clients, max_fanout)
+
+  return _return_executor
+
+
+def _create_inferred_cardinality_executor_fn(max_fanout):
+  """Creates executor function with variable cardinality."""
+
+  def _create_variable_clients_executors(cardinalities):
+    """Constructs executor stacks from `dict` argument."""
+    py_typecheck.check_type(cardinalities, dict)
+    for k, v in six.iteritems(cardinalities):
+      py_typecheck.check_type(k, placement_literals.PlacementLiteral)
+      if k not in [placement_literals.CLIENTS, placement_literals.SERVER]:
+        raise ValueError('Unsupported placement: {}.'.format(k))
+      if v <= 0:
+        raise ValueError(
+            'Cardinality must be at '
+            'least one; you have passed {} for placement {}.'.format(v, k))
 
-  def _make(n):
-    return [concurrent_executor.ConcurrentExecutor(bottom_ex) for _ in range(n)]
+    return _create_full_stack(
+        cardinalities.get(placement_literals.CLIENTS, 0), max_fanout)
 
-  return lambda_executor.LambdaExecutor(
-      federated_executor.FederatedExecutor({
-          None: _make(1),
-          placement_literals.SERVER: _make(1),
-          placement_literals.CLIENTS: _make(num_clients)
-      }))
+  return _create_variable_clients_executors
+
+
+def create_local_executor(num_clients=None, max_fanout=100):
+  """Constructs an executor to execute computations on the local machine.
+
+  NOTE: This function is only available in Python 3.
+
+  Args:
+    num_clients: The number of clients. If specified, the executor factory
+      function returned by `create_local_executor` will be configured to have
+      exactly `num_clients` clients. If unspecified (`None`), then the function
+      returned will attempt to infer cardinalities of all placements for which
+      it is passed values.
+    max_fanout: The maximum fanout at any point in the aggregation hierarchy.
+      If `num_clients > max_fanout`, the constructed executor stack will consist
+      of multiple levels of aggregators. The height of the stack will be on the
+      order of `log(num_clients) / log(max_fanout)`.
+
+  Returns:
+    An executor factory function which returns a
+    `tff.framework.Executor` upon invocation with a dict mapping placements
+    to positive integers.
+
+  Raises:
+    ValueError: If the number of clients is specified and not one or larger.
+  """
+  # TODO(b/140112504): Follow up with an ExecutorFactory abstract class.
+
+  if num_clients is not None:
+    py_typecheck.check_type(num_clients, int)
+    if num_clients <= 0:
+      raise ValueError('If specifying `num_clients`, cardinality must be at '
+                       'least one; you have passed {}.'.format(num_clients))
+    return _create_explicit_cardinality_executor_fn(num_clients, max_fanout)
+  else:
+    return _create_inferred_cardinality_executor_fn(max_fanout)
+
+
+def create_worker_pool_executor(executors, max_fanout=100):
+  """Create an executor backed by a worker pool.
+
+  Args:
+    executors: A list of `tff.framework.Executor` instances that forward work to
+      workers in the worker pool. These can be any type of executors, but in
+      most scenarios, they will be instances of `tff.framework.RemoteExecutor`.
+    max_fanout: The maximum fanout at any point in the aggregation hierarchy. If
+      `num_clients > max_fanout`, the constructed executor stack will consist of
+      multiple levels of aggregators. The height of the stack will be on the
+      order of `log(num_clients) / log(max_fanout)`.
+
+  Returns:
+    An instance of `tff.framework.Executor`.
+  """
+  py_typecheck.check_type(executors, list)
+  py_typecheck.check_type(max_fanout, int)
+  if not executors:
+    raise ValueError('The list executors cannot be empty.')
+  if max_fanout < 1:
+    raise ValueError('Max fanout must be positive.')
+  executors = [_complete_stack(e) for e in executors]
+  return _aggregate_stacks(executors, max_fanout)
```

## tensorflow_federated/python/core/impl/federated_computation_context.py

```diff
@@ -55,15 +55,15 @@
     while ancestor is not None:
       ancestor_names.add(ancestor.name)
       ancestor = ancestor.parent
     name = suggested_name
     name_count = 0
     while name in ancestor_names:
       name_count = name_count + 1
-      name = '{}_{}'.format(suggested_name, str(name_count))
+      name = '{}_{}'.format(suggested_name, name_count)
     self._context_stack = context_stack
     self._parent = parent
     self._name = name
 
   @property
   def name(self):
     return self._name
@@ -85,11 +85,11 @@
         ret_val = fn(arg)
       else:
         ret_val = fn()
       type_utils.check_type(ret_val, fn.type_signature.result)
       return ret_val
     elif arg is not None:
       raise ValueError(
-          'A computation of type {} does not expect any arguments, '
-          'but got an argument {}.'.format(str(fn.type_signature), str(arg)))
+          'A computation of type {} does not expect any arguments, but got an '
+          'argument {}.'.format(fn.type_signature, arg))
     else:
       return fn
```

## tensorflow_federated/python/core/impl/federated_computation_utils.py

```diff
@@ -17,18 +17,18 @@
 from __future__ import division
 from __future__ import print_function
 
 import six
 
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
-from tensorflow_federated.python.core.impl import computation_building_blocks
 from tensorflow_federated.python.core.impl import context_stack_base
 from tensorflow_federated.python.core.impl import federated_computation_context
 from tensorflow_federated.python.core.impl import value_impl
+from tensorflow_federated.python.core.impl.compiler import building_blocks
 
 
 def zero_or_one_arg_fn_to_building_block(fn,
                                          parameter_name,
                                          parameter_type,
                                          context_stack,
                                          suggested_name=None):
@@ -43,15 +43,15 @@
     context_stack: The context stack to use.
     suggested_name: The optional suggested name to use for the federated context
       that will be used to serialize this function's body (ideally the name of
       the underlying Python function). It might be modified to avoid conflicts.
       If not `None`, it must be a string.
 
   Returns:
-    An instance of `computation_building_blocks.ComputationBuildingBlock` that
+    An instance of `building_blocks.ComputationBuildingBlock` that
     contains the logic from `fn`.
 
   Raises:
     ValueError: if `fn` is incompatible with `parameter_type`.
   """
   py_typecheck.check_callable(fn)
   py_typecheck.check_type(context_stack, context_stack_base.ContextStack)
@@ -68,19 +68,22 @@
   if parameter_name is not None:
     py_typecheck.check_type(parameter_name, six.string_types)
     parameter_name = '{}_{}'.format(context.name, str(parameter_name))
   with context_stack.install(context):
     if parameter_type is not None:
       result = fn(
           value_impl.ValueImpl(
-              computation_building_blocks.Reference(parameter_name,
-                                                    parameter_type),
+              building_blocks.Reference(parameter_name, parameter_type),
               context_stack))
     else:
       result = fn()
+    if result is None:
+      raise ValueError(
+          'The function defined on line {} of file {} has returned a '
+          '`NoneType`, but all TFF functions must return some non-`None` '
+          'value.'.format(fn.__code__.co_firstlineno, fn.__code__.co_filename))
     result = value_impl.to_value(result, None, context_stack)
     result_comp = value_impl.ValueImpl.get_comp(result)
     if parameter_type is None:
       return result_comp
     else:
-      return computation_building_blocks.Lambda(parameter_name, parameter_type,
-                                                result_comp)
+      return building_blocks.Lambda(parameter_name, parameter_type, result_comp)
```

## tensorflow_federated/python/core/impl/federated_executor.py

```diff
@@ -18,24 +18,23 @@
 
 import tensorflow as tf
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
-from tensorflow_federated.python.core.impl import computation_constructing_utils
 from tensorflow_federated.python.core.impl import computation_impl
 from tensorflow_federated.python.core.impl import executor_base
+from tensorflow_federated.python.core.impl import executor_utils
 from tensorflow_federated.python.core.impl import executor_value_base
-from tensorflow_federated.python.core.impl import intrinsic_defs
-from tensorflow_federated.python.core.impl import intrinsic_utils
-from tensorflow_federated.python.core.impl import placement_literals
-from tensorflow_federated.python.core.impl import type_constructors
-from tensorflow_federated.python.core.impl import type_serialization
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import intrinsic_defs
+from tensorflow_federated.python.core.impl.compiler import placement_literals
+from tensorflow_federated.python.core.impl.compiler import type_factory
+from tensorflow_federated.python.core.impl.compiler import type_serialization
 
 
 class FederatedExecutorValue(executor_value_base.ExecutorValue):
   """Represents a value embedded in the federated executor."""
 
   def __init__(self, value, type_spec):
     """Creates an embedded instance of a value in this executor.
@@ -97,19 +96,29 @@
         py_typecheck.check_type(v, executor_value_base.ExecutorValue)
         results.append(v.compute())
       results = await asyncio.gather(*results)
       if self._type_signature.all_equal:
         return results[0]
       else:
         return results
+    elif isinstance(self._value, anonymous_tuple.AnonymousTuple):
+      value_elements = anonymous_tuple.to_elements(self._value)
+      type_elements = anonymous_tuple.to_elements(self._type_signature)
+      gathered_values = await asyncio.gather(*[
+          FederatedExecutorValue(v, t).compute()
+          for (_, v), (_, t) in zip(value_elements, type_elements)
+      ])
+      return anonymous_tuple.AnonymousTuple([
+          (k, v) for (k, _), v in zip(type_elements, gathered_values)
+      ])
     else:
-      raise RuntimeError('Computing values of type {} represented as {} is not '
-                         'supported in this executor.'.format(
-                             str(self._type_signature),
-                             py_typecheck.type_string(type(self._value))))
+      raise RuntimeError(
+          'Computing values of type {} represented as {} is not supported in '
+          'this executor.'.format(self._type_signature,
+                                  py_typecheck.type_string(type(self._value))))
 
 
 class FederatedExecutor(executor_base.Executor):
   """The federated executor orchestrates federated computations.
 
   NOTE: This component is only available in Python 3.
 
@@ -180,23 +189,23 @@
         self._target_executors[k] = v
     for pl in [None, placement_literals.SERVER]:
       if pl in self._target_executors:
         pl_cardinality = len(self._target_executors[pl])
         if pl_cardinality != 1:
           raise ValueError(
               'Unsupported cardinality for placement "{}": {}.'.format(
-                  str(pl), str(pl_cardinality)))
+                  pl, pl_cardinality))
 
   async def create_value(self, value, type_spec=None):
     type_spec = computation_types.to_type(type_spec)
     if isinstance(value, intrinsic_defs.IntrinsicDef):
       if not type_utils.is_concrete_instance_of(type_spec,
                                                 value.type_signature):
         raise TypeError('Incompatible type {} used with intrinsic {}.'.format(
-            str(type_spec), value.uri))
+            type_spec, value.uri))
       else:
         return FederatedExecutorValue(value, type_spec)
     if isinstance(value, placement_literals.PlacementLiteral):
       if type_spec is not None:
         py_typecheck.check_type(type_spec, computation_types.PlacementType)
       return FederatedExecutorValue(value, computation_types.PlacementType())
     elif isinstance(value, computation_impl.ComputationImpl):
@@ -258,36 +267,38 @@
         raise ValueError(
             'Unsupported computation building block of type "{}".'.format(
                 which_computation))
     else:
       py_typecheck.check_type(type_spec, computation_types.Type)
       if isinstance(type_spec, computation_types.FunctionType):
         raise ValueError(
-            'Uncountered a value of a functional TFF type {} and Python type '
+            'Encountered a value of a functional TFF type {} and Python type '
             '{} that is not of one of the recognized representations.'.format(
-                str(type_spec), py_typecheck.type_string(type(value))))
+                type_spec, py_typecheck.type_string(type(value))))
       elif isinstance(type_spec, computation_types.FederatedType):
         children = self._target_executors.get(type_spec.placement)
         if not children:
           raise ValueError(
               'Placement "{}" is not configured in this executor.'.format(
-                  str(type_spec.placement)))
+                  type_spec.placement))
         py_typecheck.check_type(children, list)
         if not type_spec.all_equal:
-          py_typecheck.check_type(value, list)
+          py_typecheck.check_type(value, (list, tuple, set, frozenset))
+          if not isinstance(value, list):
+            value = list(value)
         elif isinstance(value, list):
           raise ValueError(
               'An all_equal value should be passed directly, not as a list.')
         else:
           value = [value for _ in children]
         if len(value) != len(children):
           raise ValueError(
               'Federated value contains {} items, but the placement {} in this '
               'executor is configured with {} participants.'.format(
-                  len(value), str(type_spec.placement), len(children)))
+                  len(value), type_spec.placement, len(children)))
         child_vals = await asyncio.gather(*[
             c.create_value(v, type_spec.member)
             for v, c in zip(value, children)
         ])
         return FederatedExecutorValue(child_vals, type_spec)
       else:
         child = self._target_executors.get(None)
@@ -309,26 +320,25 @@
     if isinstance(comp.internal_representation, pb.Computation):
       which_computation = comp.internal_representation.WhichOneof('computation')
       if which_computation == 'tensorflow':
         child = self._target_executors[None][0]
         embedded_comp = await child.create_value(comp.internal_representation,
                                                  comp.type_signature)
         if arg is not None:
-          embedded_arg = await self._delegate(child,
-                                              arg.internal_representation,
-                                              arg.type_signature)
+          embedded_arg = await executor_utils.delegate_entirely_to_executor(
+              arg.internal_representation, arg.type_signature, child)
         else:
           embedded_arg = None
         result = await child.create_call(embedded_comp, embedded_arg)
         return FederatedExecutorValue(result, result.type_signature)
       else:
         raise ValueError(
             'Directly calling computations of type {} is unsupported.'.format(
                 which_computation))
-    if isinstance(comp.internal_representation, intrinsic_defs.IntrinsicDef):
+    elif isinstance(comp.internal_representation, intrinsic_defs.IntrinsicDef):
       coro = getattr(
           self,
           '_compute_intrinsic_{}'.format(comp.internal_representation.uri))
       if coro is not None:
         return await coro(arg)
       else:
         raise NotImplementedError(
@@ -347,51 +357,47 @@
             (k, v.internal_representation) for k, v in elem
         ]),
         computation_types.NamedTupleType([
             (k, v.type_signature) if k else v.type_signature for k, v in elem
         ]))
 
   async def create_selection(self, source, index=None, name=None):
-    raise NotImplementedError
-
-  async def _delegate(self, executor, arg, arg_type):
-    """Delegates a non-federated `arg` in its entirety to the target executor.
-
-    Args:
-      executor: The target executor to use.
-      arg: The object to delegate to the target executor.
-      arg_type: The type of this object.
-
-    Returns:
-      An instance of `executor_value_base.ExecutorValue` that represents the
-      result of delegation.
-
-    Raises:
-      TypeError: If the arguments are of the wrong types.
-    """
-    py_typecheck.check_type(arg_type, computation_types.Type)
-    if isinstance(arg_type, computation_types.FederatedType):
-      raise TypeError(
-          'Cannot delegate an argument of a federated type {}.'.format(
-              str(arg_type)))
-    if isinstance(arg, executor_value_base.ExecutorValue):
-      return arg
-    elif isinstance(arg, anonymous_tuple.AnonymousTuple):
-      v_elem = anonymous_tuple.to_elements(arg)
-      t_elem = anonymous_tuple.to_elements(arg_type)
-      vals = await asyncio.gather(*[
-          self._delegate(executor, v, t)
-          for (_, v), (_, t) in zip(v_elem, t_elem)
-      ])
-      return await executor.create_tuple(
-          anonymous_tuple.AnonymousTuple(
-              list(zip([k for k, _ in t_elem], vals))))
+    py_typecheck.check_type(source, FederatedExecutorValue)
+    py_typecheck.check_type(source.type_signature,
+                            computation_types.NamedTupleType)
+    if name is not None:
+      name_to_index = dict((n, i) for i, (
+          n,
+          t) in enumerate(anonymous_tuple.to_elements(source.type_signature)))
+      index = name_to_index[name]
+    if isinstance(source.internal_representation,
+                  anonymous_tuple.AnonymousTuple):
+      val = source.internal_representation
+      selected = val[index]
+      return FederatedExecutorValue(selected, source.type_signature[index])
+    elif isinstance(source.internal_representation,
+                    executor_value_base.ExecutorValue):
+      if type_utils.type_tree_contains_types(source.type_signature,
+                                             computation_types.FederatedType):
+        raise ValueError('FederatedExecutorValue {} has violated its contract; '
+                         'it is embedded in another executor and yet its type '
+                         'has placement. The embedded value is {}, with type '
+                         'signature {}.'.format(source,
+                                                source.internal_representation,
+                                                source.type_signature))
+      val = source.internal_representation
+      child = self._target_executors[None][0]
+      return FederatedExecutorValue(
+          await child.create_selection(val, index=index),
+          source.type_signature[index])
     else:
-      py_typecheck.check_type(arg, pb.Computation)
-      return await executor.create_value(arg, arg_type)
+      raise ValueError('Unexpected internal representation while creating '
+                       'selection. Expected one of `AnonymousTuple` or value '
+                       'embedded in target executor, received {}'.format(
+                           source.internal_representation))
 
   async def _place(self, arg, placement):
     py_typecheck.check_type(placement, placement_literals.PlacementLiteral)
     children = self._target_executors[placement]
     val = await arg.internal_representation.compute()
     return FederatedExecutorValue(
         await asyncio.gather(
@@ -450,15 +456,15 @@
     new_vals = await asyncio.gather(
         *[c.create_tuple(x) for c, x in zip(children, new_vals)])
     return FederatedExecutorValue(
         new_vals,
         computation_types.FederatedType(
             computation_types.NamedTupleType([
                 (k, v.member) if k else v.member
-                for k, v in anonymous_tuple.to_elements(arg.type_signature)
+                for k, v in anonymous_tuple.iter_elements(arg.type_signature)
             ]),
             placement,
             all_equal=all_equal))
 
   async def _compute_intrinsic_federated_value_at_server(self, arg):
     return await self._place(arg, placement_literals.SERVER)
 
@@ -480,16 +486,15 @@
       raise ValueError(
           'Cannot broadcast a with a non-singleton representation.')
     val = await arg.internal_representation[0].compute()
     return FederatedExecutorValue(
         await asyncio.gather(*[
             c.create_value(val, arg.type_signature.member)
             for c in self._target_executors[placement_literals.CLIENTS]
-        ]),
-        type_constructors.at_clients(arg.type_signature.member, all_equal=True))
+        ]), type_factory.at_clients(arg.type_signature.member, all_equal=True))
 
   async def _compute_intrinsic_federated_zip_at_server(self, arg):
     return await self._zip(arg, placement_literals.SERVER, all_equal=True)
 
   async def _compute_intrinsic_federated_zip_at_clients(self, arg):
     return await self._zip(arg, placement_literals.CLIENTS, all_equal=False)
 
@@ -505,63 +510,47 @@
 
     val_type = arg.type_signature[0]
     py_typecheck.check_type(val_type, computation_types.FederatedType)
     item_type = val_type.member
     zero_type = arg.type_signature[1]
     op_type = arg.type_signature[2]
     type_utils.check_equivalent_types(
-        op_type, type_constructors.reduction_op(zero_type, item_type))
+        op_type, type_factory.reduction_op(zero_type, item_type))
 
     val = arg.internal_representation[0]
     py_typecheck.check_type(val, list)
     child = self._target_executors[placement_literals.SERVER][0]
 
     async def _move(v):
       return await child.create_value(await v.compute(), item_type)
 
     items = await asyncio.gather(*[_move(v) for v in val])
 
     zero = await child.create_value(
-        await arg.internal_representation[1].compute(), zero_type)
+        await (await self.create_selection(arg, index=1)).compute(), zero_type)
     op = await child.create_value(arg.internal_representation[2], op_type)
 
     result = zero
     for item in items:
       result = await child.create_call(
           op, await child.create_tuple(
               anonymous_tuple.AnonymousTuple([(None, result), (None, item)])))
     return FederatedExecutorValue([result],
                                   computation_types.FederatedType(
                                       result.type_signature,
                                       placement_literals.SERVER,
                                       all_equal=True))
 
   async def _compute_intrinsic_federated_aggregate(self, arg):
-    py_typecheck.check_type(arg.type_signature,
-                            computation_types.NamedTupleType)
+    val_type, zero_type, accumulate_type, _, report_type = (
+        executor_utils.parse_federated_aggregate_argument_types(
+            arg.type_signature))
     py_typecheck.check_type(arg.internal_representation,
                             anonymous_tuple.AnonymousTuple)
-    if len(arg.internal_representation) != 5:
-      raise ValueError(
-          'Expected 5 elements in the `federated_aggregate()` argument tuple, '
-          'found {}.'.format(len(arg.internal_representation)))
-
-    val_type = arg.type_signature[0]
-    py_typecheck.check_type(val_type, computation_types.FederatedType)
-    item_type = val_type.member
-    zero_type = arg.type_signature[1]
-    accumulate_type = arg.type_signature[2]
-    type_utils.check_equivalent_types(
-        accumulate_type, type_constructors.reduction_op(zero_type, item_type))
-    merge_type = arg.type_signature[3]
-    type_utils.check_equivalent_types(merge_type,
-                                      type_constructors.binary_op(zero_type))
-    report_type = arg.type_signature[4]
-    py_typecheck.check_type(report_type, computation_types.FunctionType)
-    type_utils.check_equivalent_types(report_type.parameter, zero_type)
+    py_typecheck.check_len(arg.internal_representation, 5)
 
     # NOTE: This is a simple initial implementation that simply forwards this
     # to `federated_reduce()`. The more complete implementation would be able
     # to take advantage of the parallelism afforded by `merge` to reduce the
     # cost from liner (with respect to the number of clients) to sub-linear.
 
     # TODO(b/134543154): Expand this implementation to take advantage of the
@@ -589,18 +578,21 @@
                 (None, report), (None, pre_report.internal_representation)
             ]),
             computation_types.NamedTupleType(
                 [report_type, pre_report.type_signature])))
 
   async def _compute_intrinsic_federated_sum(self, arg):
     py_typecheck.check_type(arg.type_signature, computation_types.FederatedType)
-    zero, plus = tuple(await asyncio.gather(*[
-        _embed_tf_scalar_constant(self, arg.type_signature.member, 0),
-        _embed_tf_binary_operator(self, arg.type_signature.member, tf.add)
-    ]))
+    zero, plus = tuple(await
+                       asyncio.gather(*[
+                           executor_utils.embed_tf_scalar_constant(
+                               self, arg.type_signature.member, 0),
+                           executor_utils.embed_tf_binary_operator(
+                               self, arg.type_signature.member, tf.add)
+                       ]))
     return await self._compute_intrinsic_federated_reduce(
         FederatedExecutorValue(
             anonymous_tuple.AnonymousTuple([
                 (None, arg.internal_representation),
                 (None, zero.internal_representation),
                 (None, plus.internal_representation)
             ]),
@@ -612,101 +604,37 @@
     arg_sum = await self._compute_intrinsic_federated_sum(arg)
     member_type = arg_sum.type_signature.member
     count = float(len(arg.internal_representation))
     if count < 1.0:
       raise RuntimeError('Cannot compute a federated mean over an empty group.')
     child = self._target_executors[placement_literals.SERVER][0]
     factor, multiply = tuple(await asyncio.gather(*[
-        _embed_tf_scalar_constant(child, member_type, float(1.0 / count)),
-        _embed_tf_binary_operator(child, member_type, tf.multiply)
+        executor_utils.embed_tf_scalar_constant(child, member_type,
+                                                float(1.0 / count)),
+        executor_utils.embed_tf_binary_operator(child, member_type, tf.multiply)
     ]))
     multiply_arg = await child.create_tuple(
         anonymous_tuple.AnonymousTuple([(None,
                                          arg_sum.internal_representation[0]),
                                         (None, factor)]))
     result = await child.create_call(multiply, multiply_arg)
     return FederatedExecutorValue([result], arg_sum.type_signature)
 
   async def _compute_intrinsic_federated_weighted_mean(self, arg):
-    type_utils.check_valid_federated_weighted_mean_argument_tuple_type(
-        arg.type_signature)
-    zipped_arg = await self._compute_intrinsic_federated_zip_at_clients(arg)
-    # TODO(b/134543154): Replace with something that produces a section of
-    # plain TensorFlow code instead of constructing a lambda (so that this
-    # can be executed directly on top of a plain TensorFlow-based executor).
-    multiply_blk = intrinsic_utils.create_binary_operator_with_upcast(
-        zipped_arg.type_signature.member, tf.multiply)
-    sum_of_products = await self._compute_intrinsic_federated_sum(
-        await self._compute_intrinsic_federated_map(
-            FederatedExecutorValue(
-                anonymous_tuple.AnonymousTuple([
-                    (None, multiply_blk.proto),
-                    (None, zipped_arg.internal_representation)
-                ]),
-                computation_types.NamedTupleType(
-                    [multiply_blk.type_signature, zipped_arg.type_signature]))))
-    total_weight = await self._compute_intrinsic_federated_sum(
-        FederatedExecutorValue(arg.internal_representation[1],
-                               arg.type_signature[1]))
-    divide_arg = await self._compute_intrinsic_federated_zip_at_server(
-        await self.create_tuple(
-            anonymous_tuple.AnonymousTuple([(None, sum_of_products),
-                                            (None, total_weight)])))
-    divide_blk = intrinsic_utils.create_binary_operator_with_upcast(
-        divide_arg.type_signature.member, tf.divide)
-    return await self._compute_intrinsic_federated_apply(
-        FederatedExecutorValue(
-            anonymous_tuple.AnonymousTuple([
-                (None, divide_blk.proto),
-                (None, divide_arg.internal_representation)
-            ]),
-            computation_types.NamedTupleType(
-                [divide_blk.type_signature, divide_arg.type_signature])))
-
+    return await executor_utils.compute_federated_weighted_mean(self, arg)
 
-async def _embed_tf_scalar_constant(executor, type_spec, val):
-  """Embeds a constant `val` of TFF type `type_spec` in `executor`.
-
-  Args:
-    executor: An instance of `tff.framework.Executor`.
-    type_spec: An instance of `tff.Type`.
-    val: A scalar value.
-
-  Returns:
-    An instance of `tff.framework.ExecutorValue` containing an embedded value.
-  """
-  # TODO(b/134543154): Perhaps graduate this and the function below it into a
-  # separate library, so that it can be used in other places.
-  py_typecheck.check_type(executor, executor_base.Executor)
-  fn_building_block = (
-      computation_constructing_utils.create_tensorflow_constant(type_spec, val))
-  embedded_val = await executor.create_call(await executor.create_value(
-      fn_building_block.function.proto,
-      fn_building_block.function.type_signature))
-  type_utils.check_equivalent_types(embedded_val.type_signature, type_spec)
-  return embedded_val
-
-
-async def _embed_tf_binary_operator(executor, type_spec, op):
-  """Embeds a binary operator `op` on `type_spec`-typed values in `executor`.
-
-  Args:
-    executor: An instance of `tff.framework.Executor`.
-    type_spec: An instance of `tff.Type` of the type of values that the binary
-      operator accepts as input and returns as output.
-    op: An operator function (such as `tf.add` or `tf.multiply`) to apply to the
-      tensor-level constituents of the values, pointwise.
-
-  Returns:
-    An instance of `tff.framework.ExecutorValue` representing the operator in
-    a form embedded into the executor.
-  """
-  # TODO(b/134543154): There is an opportunity here to import something more
-  # in line with the usage (no building block wrapping, etc.)
-  fn_building_block = (
-      computation_constructing_utils.create_tensorflow_binary_operator(
-          type_spec, op))
-  embedded_val = await executor.create_value(fn_building_block.proto,
-                                             fn_building_block.type_signature)
-  type_utils.check_equivalent_types(embedded_val.type_signature,
-                                    type_constructors.binary_op(type_spec))
-  return embedded_val
+  async def _compute_intrinsic_federated_collect(self, arg):
+    py_typecheck.check_type(arg.type_signature, computation_types.FederatedType)
+    type_utils.check_federated_type(
+        arg.type_signature, placement=placement_literals.CLIENTS)
+    val = arg.internal_representation
+    py_typecheck.check_type(val, list)
+    member_type = arg.type_signature.member
+    child = self._target_executors[placement_literals.SERVER][0]
+    collected_items = await child.create_value(
+        await asyncio.gather(*[v.compute() for v in val]),
+        computation_types.SequenceType(member_type))
+    return FederatedExecutorValue(
+        [collected_items],
+        computation_types.FederatedType(
+            computation_types.SequenceType(member_type),
+            placement_literals.SERVER))
```

## tensorflow_federated/python/core/impl/intrinsic_bodies.py

```diff
@@ -22,22 +22,21 @@
 
 from six.moves import range
 import tensorflow as tf
 
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
-from tensorflow_federated.python.core.impl import computation_building_blocks
-from tensorflow_federated.python.core.impl import computation_constructing_utils
 from tensorflow_federated.python.core.impl import context_stack_base
-from tensorflow_federated.python.core.impl import intrinsic_defs
 from tensorflow_federated.python.core.impl import intrinsic_factory
-from tensorflow_federated.python.core.impl import intrinsic_utils
 from tensorflow_federated.python.core.impl import type_utils
 from tensorflow_federated.python.core.impl import value_impl
+from tensorflow_federated.python.core.impl.compiler import building_block_factory
+from tensorflow_federated.python.core.impl.compiler import building_blocks
+from tensorflow_federated.python.core.impl.compiler import intrinsic_defs
 
 
 def get_intrinsic_bodies(context_stack):
   """Returns a `collections.OrderedDict` of intrinsic bodies.
 
   This dictionary respects the invariant that no body may refer to an intrinsic
   whose body appears previously in the `dict`.
@@ -68,46 +67,40 @@
   # - FEDERATED_COLLECT(x) := GENERIC_COLLECT(x, SERVER)
   #
   # - FEDERATED_MAP(f, x) := GENERIC_MAP(f, x)
   #
   # - FEDERATED_VALUE_AT_CLIENTS(x) := GENERIC_PLACE(x, CLIENTS)
   #
   # - FEDERATED_VALUE_AT_SERVER(x) := GENERIC_PLACE(x, SERVER)
-  #
-  # - FEDERATED_MEAN(x) := FEDERATED_WEIGHTED_MEAN(
-  #     x, FEDERATED_VALUE_AT_CLIENTS(GENERIC_ONE))
-  #
-  # - FEDERATED_WEIGHTED_MEAN(x, w) :=
-  #     GENERIC_DIVIDE(FEDERATED_SUM(GENERIC_MULTIPLY(x, w)), w)
 
   def _pack_binary_operator_args(x, y):
     """Packs arguments to binary operator into a single arg."""
 
     def _only_tuple_or_tensor(value):
       return type_utils.type_tree_contains_only(
           value.type_signature,
           (computation_types.NamedTupleType, computation_types.TensorType))
 
     if _only_tuple_or_tensor(x) and _only_tuple_or_tensor(y):
       arg = value_impl.ValueImpl(
-          computation_building_blocks.Tuple([
+          building_blocks.Tuple([
               value_impl.ValueImpl.get_comp(x),
               value_impl.ValueImpl.get_comp(y)
           ]), context_stack)
     elif (isinstance(x.type_signature, computation_types.FederatedType) and
           isinstance(y.type_signature, computation_types.FederatedType) and
           x.type_signature.placement == y.type_signature.placement):
       if not type_utils.is_binary_op_with_upcast_compatible_pair(
           x.type_signature.member, y.type_signature.member):
         raise TypeError(
             'The members of the federated types {} and {} are not division '
             'compatible; see `type_utils.is_binary_op_with_upcast_compatible_pair` '
             'for more details.'.format(x.type_signature, y.type_signature))
       packed_arg = value_impl.ValueImpl(
-          computation_building_blocks.Tuple([
+          building_blocks.Tuple([
               value_impl.ValueImpl.get_comp(x),
               value_impl.ValueImpl.get_comp(y)
           ]), context_stack)
       arg = intrinsics.federated_zip(packed_arg)
     else:
       raise TypeError
     return arg
@@ -142,117 +135,141 @@
             'You have passed first argument of type {} '
             'and second argument of type {}.'.format(op_name, x.type_signature,
                                                      y.type_signature))
 
     top_level_mismatch_string = (
         '{} does not accept arguments of type {} and '
         '{}, as they are mismatched at the top level.'.format(
-            x.type_signature, y.type_signature, op_name))
+            op_name, x.type_signature, y.type_signature))
     if isinstance(x.type_signature, computation_types.FederatedType):
       if (not isinstance(y.type_signature, computation_types.FederatedType) or
           x.type_signature.placement != y.type_signature.placement or
-          x.type_signature.all_equal != y.type_signature.all_equal or
           not type_utils.is_binary_op_with_upcast_compatible_pair(
               x.type_signature.member, y.type_signature.member)):
         raise TypeError(top_level_mismatch_string)
     if isinstance(x.type_signature, computation_types.NamedTupleType):
-      if not isinstance(y.type_signature,
-                        computation_types.NamedTupleType) or dir(
-                            x.type_signature) != dir(x.type_signature):
+      if type_utils.is_binary_op_with_upcast_compatible_pair(
+          x.type_signature, y.type_signature):
+        return None
+      elif not isinstance(y.type_signature,
+                          computation_types.NamedTupleType) or dir(
+                              x.type_signature) != dir(y.type_signature):
         raise TypeError(top_level_mismatch_string)
 
   def federated_weighted_mean(arg):
     w = arg[1]
     multiplied = generic_multiply(arg)
     summed = federated_sum(intrinsics.federated_zip([multiplied, w]))
     return generic_divide(summed)
 
+  def federated_mean(arg):
+    one = value_impl.ValueImpl(
+        building_block_factory.create_generic_constant(arg.type_signature, 1),
+        context_stack)
+    arg = value_impl.to_value([arg, one], None, context_stack)
+    return federated_weighted_mean(arg)
+
   def federated_sum(x):
     zero = value_impl.ValueImpl(
-        intrinsic_utils.create_generic_constant(x.type_signature.member, 0),
-        context_stack)
+        building_block_factory.create_generic_constant(x.type_signature.member,
+                                                       0), context_stack)
     plus_op = value_impl.ValueImpl(
-        intrinsic_utils.create_binary_operator_with_upcast(
+        building_block_factory.create_binary_operator_with_upcast(
             computation_types.NamedTupleType(
                 [x.type_signature.member, x.type_signature.member]), tf.add),
         context_stack)
     return federated_reduce([x, zero, plus_op])
 
   def federated_reduce(arg):
     x = arg[0]
     zero = arg[1]
     op = arg[2]
-    identity = computation_constructing_utils.create_compiled_identity(
+    identity = building_block_factory.create_compiled_identity(
         op.type_signature.result)
     return intrinsics.federated_aggregate(x, zero, op, op, identity)
 
+  def _generic_op_can_be_applied(x, y):
+    return type_utils.is_binary_op_with_upcast_compatible_pair(
+        x.type_signature, y.type_signature) or isinstance(
+            x.type_signature, computation_types.FederatedType)
+
+  def _apply_generic_op(op, x, y):
+    arg = _pack_binary_operator_args(x, y)
+    arg_comp = value_impl.ValueImpl.get_comp(arg)
+    result = building_block_factory.apply_binary_operator_with_upcast(
+        arg_comp, op)
+    return value_impl.ValueImpl(result, context_stack)
+
   def generic_divide(arg):
     """Divides two arguments when possible."""
     x = arg[0]
     y = arg[1]
     _check_top_level_compatibility_with_generic_operators(
         x, y, 'Generic divide')
-    if isinstance(x.type_signature, computation_types.NamedTupleType):
+    if _generic_op_can_be_applied(x, y):
+      return _apply_generic_op(tf.divide, x, y)
+    elif isinstance(x.type_signature, computation_types.NamedTupleType):
       # This case is needed if federated types are nested deeply.
-      names = [t[0] for t in anonymous_tuple.to_elements(x.type_signature)]
+      names = [t[0] for t in anonymous_tuple.iter_elements(x.type_signature)]
       divided = [
           value_impl.ValueImpl.get_comp(generic_divide([x[i], y[i]]))
           for i in range(len(names))
       ]
-      named_divided = computation_constructing_utils.create_named_tuple(
-          computation_building_blocks.Tuple(divided), names)
+      named_divided = building_block_factory.create_named_tuple(
+          building_blocks.Tuple(divided), names)
       return value_impl.ValueImpl(named_divided, context_stack)
-    arg = _pack_binary_operator_args(x, y)
-    arg_comp = value_impl.ValueImpl.get_comp(arg)
-    divided = intrinsic_utils.apply_binary_operator_with_upcast(
-        arg_comp, tf.divide)
-    return value_impl.ValueImpl(divided, context_stack)
+    else:
+      raise TypeError(
+          'Generic divide encountered unexpected type {}, {}'.format(
+              x.type_signature, y.type_signature))
 
   def generic_multiply(arg):
     """Multiplies two arguments when possible."""
     x = arg[0]
     y = arg[1]
     _check_top_level_compatibility_with_generic_operators(
         x, y, 'Generic multiply')
-    if isinstance(x.type_signature, computation_types.NamedTupleType):
+    if _generic_op_can_be_applied(x, y):
+      return _apply_generic_op(tf.multiply, x, y)
+    elif isinstance(x.type_signature, computation_types.NamedTupleType):
       # This case is needed if federated types are nested deeply.
-      names = [t[0] for t in anonymous_tuple.to_elements(x.type_signature)]
+      names = [t[0] for t in anonymous_tuple.iter_elements(x.type_signature)]
       multiplied = [
           value_impl.ValueImpl.get_comp(generic_multiply([x[i], y[i]]))
           for i in range(len(names))
       ]
-      named_multiplied = computation_constructing_utils.create_named_tuple(
-          computation_building_blocks.Tuple(multiplied), names)
+      named_multiplied = building_block_factory.create_named_tuple(
+          building_blocks.Tuple(multiplied), names)
       return value_impl.ValueImpl(named_multiplied, context_stack)
-    arg = _pack_binary_operator_args(x, y)
-    arg_comp = value_impl.ValueImpl.get_comp(arg)
-    multiplied = intrinsic_utils.apply_binary_operator_with_upcast(
-        arg_comp, tf.multiply)
-    return value_impl.ValueImpl(multiplied, context_stack)
+    else:
+      raise TypeError(
+          'Generic multiply encountered unexpected type {}, {}'.format(
+              x.type_signature, y.type_signature))
 
   def generic_plus(arg):
     """Adds two arguments when possible."""
     x = arg[0]
     y = arg[1]
     _check_top_level_compatibility_with_generic_operators(x, y, 'Generic plus')
+    if _generic_op_can_be_applied(x, y):
+      return _apply_generic_op(tf.add, x, y)
     # TODO(b/136587334): Push this logic down a level
-    if isinstance(x.type_signature, computation_types.NamedTupleType):
+    elif isinstance(x.type_signature, computation_types.NamedTupleType):
       # This case is needed if federated types are nested deeply.
-      names = [t[0] for t in anonymous_tuple.to_elements(x.type_signature)]
+      names = [t[0] for t in anonymous_tuple.iter_elements(x.type_signature)]
       added = [
           value_impl.ValueImpl.get_comp(generic_plus([x[i], y[i]]))
           for i in range(len(names))
       ]
-      named_added = computation_constructing_utils.create_named_tuple(
-          computation_building_blocks.Tuple(added), names)
+      named_added = building_block_factory.create_named_tuple(
+          building_blocks.Tuple(added), names)
       return value_impl.ValueImpl(named_added, context_stack)
-    arg = _pack_binary_operator_args(x, y)
-    arg_comp = value_impl.ValueImpl.get_comp(arg)
-    added = intrinsic_utils.apply_binary_operator_with_upcast(arg_comp, tf.add)
-    return value_impl.ValueImpl(added, context_stack)
+    else:
+      raise TypeError('Generic plus encountered unexpected type {}, {}'.format(
+          x.type_signature, y.type_signature))
 
   # - FEDERATED_ZIP(x, y) := GENERIC_ZIP(x, y)
   #
   # - GENERIC_AVERAGE(x: {T}@p, q: placement) :=
   #     GENERIC_WEIGHTED_AVERAGE(x, GENERIC_ONE, q)
   #
   # - GENERIC_WEIGHTED_AVERAGE(x: {T}@p, w: {U}@p, q: placement) :=
@@ -304,13 +321,14 @@
   # - GENERIC_PLUS
   # - GENERIC_ZERO
   # - GENERIC_ZIP
   # - SEQUENCE_MAP
   # - SEQUENCE_REDUCE
 
   return collections.OrderedDict([
+      (intrinsic_defs.FEDERATED_MEAN.uri, federated_mean),
       (intrinsic_defs.FEDERATED_WEIGHTED_MEAN.uri, federated_weighted_mean),
       (intrinsic_defs.FEDERATED_SUM.uri, federated_sum),
       (intrinsic_defs.GENERIC_DIVIDE.uri, generic_divide),
       (intrinsic_defs.GENERIC_MULTIPLY.uri, generic_multiply),
       (intrinsic_defs.GENERIC_PLUS.uri, generic_plus),
   ])
```

## tensorflow_federated/python/core/impl/intrinsic_factory.py

```diff
@@ -19,22 +19,22 @@
 from __future__ import print_function
 
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.api import placements
 from tensorflow_federated.python.core.api import value_base
-from tensorflow_federated.python.core.impl import computation_building_blocks
-from tensorflow_federated.python.core.impl import computation_constructing_utils
 from tensorflow_federated.python.core.impl import context_stack_base
-from tensorflow_federated.python.core.impl import intrinsic_defs
-from tensorflow_federated.python.core.impl import type_constructors
 from tensorflow_federated.python.core.impl import type_utils
 from tensorflow_federated.python.core.impl import value_impl
 from tensorflow_federated.python.core.impl import value_utils
+from tensorflow_federated.python.core.impl.compiler import building_block_factory
+from tensorflow_federated.python.core.impl.compiler import building_blocks
+from tensorflow_federated.python.core.impl.compiler import intrinsic_defs
+from tensorflow_federated.python.core.impl.compiler import type_factory
 
 
 class IntrinsicFactory(object):
   """A factory that can constructs intrinsics over the given context stack."""
 
   # NOTE: Tests for this class currently go to `api/intrinsics_test.py`.
 
@@ -60,36 +60,39 @@
     Returns:
       As in `api/intrinsics.py`.
 
     Raises:
       TypeError: As in `api/intrinsics.py`.
     """
     value = value_impl.to_value(value, None, self._context_stack)
-    type_utils.check_federated_value_placement(value, placements.CLIENTS,
-                                               'value to be aggregated')
+    value_utils.check_federated_value_placement(value, placements.CLIENTS,
+                                                'value to be aggregated')
 
     zero = value_impl.to_value(zero, None, self._context_stack)
     py_typecheck.check_type(zero, value_base.Value)
-
-    # TODO(b/113112108): We need a check here that zero does not have federated
-    # constituents.
-
     accumulate = value_impl.to_value(accumulate, None, self._context_stack)
     merge = value_impl.to_value(merge, None, self._context_stack)
     report = value_impl.to_value(report, None, self._context_stack)
     for op in [accumulate, merge, report]:
       py_typecheck.check_type(op, value_base.Value)
       py_typecheck.check_type(op.type_signature, computation_types.FunctionType)
 
-    accumulate_type_expected = type_constructors.reduction_op(
-        zero.type_signature, value.type_signature.member)
-    merge_type_expected = type_constructors.reduction_op(
-        zero.type_signature, zero.type_signature)
+    if not type_utils.is_assignable_from(accumulate.type_signature.parameter[0],
+                                         zero.type_signature):
+      raise TypeError('Expected `zero` to be assignable to type {}, '
+                      'but was of incompatible type {}.'.format(
+                          accumulate.type_signature.parameter[0],
+                          zero.type_signature))
+
+    accumulate_type_expected = type_factory.reduction_op(
+        accumulate.type_signature.result, value.type_signature.member)
+    merge_type_expected = type_factory.reduction_op(
+        accumulate.type_signature.result, accumulate.type_signature.result)
     report_type_expected = computation_types.FunctionType(
-        zero.type_signature, report.type_signature.result)
+        merge.type_signature.result, report.type_signature.result)
     for op_name, op, type_expected in [
         ('accumulate', accumulate, accumulate_type_expected),
         ('merge', merge, merge_type_expected),
         ('report', report, report_type_expected)
     ]:
       if not type_utils.is_assignable_from(type_expected, op.type_signature):
         raise TypeError(
@@ -97,15 +100,16 @@
             .format(op_name, type_expected, op.type_signature))
 
     value = value_impl.ValueImpl.get_comp(value)
     zero = value_impl.ValueImpl.get_comp(zero)
     accumulate = value_impl.ValueImpl.get_comp(accumulate)
     merge = value_impl.ValueImpl.get_comp(merge)
     report = value_impl.ValueImpl.get_comp(report)
-    comp = computation_constructing_utils.create_federated_aggregate(
+
+    comp = building_block_factory.create_federated_aggregate(
         value, zero, accumulate, merge, report)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def federated_apply(self, fn, arg):
     """Implements `federated_apply` as defined in `api/intrinsics.py`.
 
     Args:
@@ -123,29 +127,29 @@
     py_typecheck.check_type(fn.type_signature, computation_types.FunctionType)
 
     arg = value_impl.to_value(arg, None, self._context_stack)
     if isinstance(arg.type_signature, computation_types.NamedTupleType):
       if len(anonymous_tuple.to_elements(arg.type_signature)) >= 2:
         # We've been passed a value which the user expects to be zipped.
         arg = self.federated_zip(arg)
-    type_utils.check_federated_value_placement(arg, placements.SERVER,
-                                               'the argument')
+    value_utils.check_federated_value_placement(arg, placements.SERVER,
+                                                'the argument')
     if not arg.type_signature.all_equal:
       raise TypeError('The argument should be equal at all locations.')
 
     if not type_utils.is_assignable_from(fn.type_signature.parameter,
                                          arg.type_signature.member):
       raise TypeError(
           'The function to apply expects a parameter of type {}, but member '
           'constituents of the argument are of an incompatible type {}.'.format(
               fn.type_signature.parameter, arg.type_signature.member))
 
     fn = value_impl.ValueImpl.get_comp(fn)
     arg = value_impl.ValueImpl.get_comp(arg)
-    comp = computation_constructing_utils.create_federated_apply(fn, arg)
+    comp = building_block_factory.create_federated_apply(fn, arg)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def federated_broadcast(self, value):
     """Implements `federated_broadcast` as defined in `api/intrinsics.py`.
 
     Args:
       value: As in `api/intrinsics.py`.
@@ -153,22 +157,22 @@
     Returns:
       As in `api/intrinsics.py`.
 
     Raises:
       TypeError: As in `api/intrinsics.py`.
     """
     value = value_impl.to_value(value, None, self._context_stack)
-    type_utils.check_federated_value_placement(value, placements.SERVER,
-                                               'value to be broadcasted')
+    value_utils.check_federated_value_placement(value, placements.SERVER,
+                                                'value to be broadcasted')
 
     if not value.type_signature.all_equal:
       raise TypeError('The broadcasted value should be equal at all locations.')
 
     value = value_impl.ValueImpl.get_comp(value)
-    comp = computation_constructing_utils.create_federated_broadcast(value)
+    comp = building_block_factory.create_federated_broadcast(value)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def federated_collect(self, value):
     """Implements `federated_collect` as defined in `api/intrinsics.py`.
 
     Args:
       value: As in `api/intrinsics.py`.
@@ -176,19 +180,19 @@
     Returns:
       As in `api/intrinsics.py`.
 
     Raises:
       TypeError: As in `api/intrinsics.py`.
     """
     value = value_impl.to_value(value, None, self._context_stack)
-    type_utils.check_federated_value_placement(value, placements.CLIENTS,
-                                               'value to be collected')
+    value_utils.check_federated_value_placement(value, placements.CLIENTS,
+                                                'value to be collected')
 
     value = value_impl.ValueImpl.get_comp(value)
-    comp = computation_constructing_utils.create_federated_collect(value)
+    comp = building_block_factory.create_federated_collect(value)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def federated_map(self, fn, arg):
     """Implements `federated_map` as defined in `api/intrinsics.py`.
 
     Args:
       fn: As in `api/intrinsics.py`.
@@ -207,16 +211,16 @@
     # placement.
 
     arg = value_impl.to_value(arg, None, self._context_stack)
     if isinstance(arg.type_signature, computation_types.NamedTupleType):
       if len(anonymous_tuple.to_elements(arg.type_signature)) >= 2:
         # We've been passed a value which the user expects to be zipped.
         arg = self.federated_zip(arg)
-    type_utils.check_federated_value_placement(arg, placements.CLIENTS,
-                                               'value to be mapped')
+    value_utils.check_federated_value_placement(arg, placements.CLIENTS,
+                                                'value to be mapped')
 
     # TODO(b/113112108): Add support for polymorphic templates auto-instantiated
     # here based on the actual type of the argument.
     fn = value_impl.to_value(fn, None, self._context_stack)
 
     py_typecheck.check_type(fn, value_base.Value)
     py_typecheck.check_type(fn.type_signature, computation_types.FunctionType)
@@ -225,15 +229,15 @@
       raise TypeError(
           'The mapping function expects a parameter of type {}, but member '
           'constituents of the mapped value are of incompatible type {}.'
           .format(fn.type_signature.parameter, arg.type_signature.member))
 
     fn = value_impl.ValueImpl.get_comp(fn)
     arg = value_impl.ValueImpl.get_comp(arg)
-    comp = computation_constructing_utils.create_federated_map(fn, arg)
+    comp = building_block_factory.create_federated_map(fn, arg)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def federated_map_all_equal(self, fn, arg):
     """Implements `federated_map` as defined in `api/intrinsic.py`.
 
     Implements `federated_map` as defined in `api/intrinsic.py` with an argument
     with the `all_equal` bit set.
@@ -255,16 +259,16 @@
     # placement.
 
     arg = value_impl.to_value(arg, None, self._context_stack)
     if isinstance(arg.type_signature, computation_types.NamedTupleType):
       if len(anonymous_tuple.to_elements(arg.type_signature)) >= 2:
         # We've been passed a value which the user expects to be zipped.
         arg = self.federated_zip(arg)
-    type_utils.check_federated_value_placement(arg, placements.CLIENTS,
-                                               'value to be mapped')
+    value_utils.check_federated_value_placement(arg, placements.CLIENTS,
+                                                'value to be mapped')
 
     # TODO(b/113112108): Add support for polymorphic templates auto-instantiated
     # here based on the actual type of the argument.
     fn = value_impl.to_value(fn, None, self._context_stack)
 
     py_typecheck.check_type(fn, value_base.Value)
     py_typecheck.check_type(fn.type_signature, computation_types.FunctionType)
@@ -273,16 +277,15 @@
       raise TypeError(
           'The mapping function expects a parameter of type {}, but member '
           'constituents of the mapped value are of incompatible type {}.'
           .format(fn.type_signature.parameter, arg.type_signature.member))
 
     fn = value_impl.ValueImpl.get_comp(fn)
     arg = value_impl.ValueImpl.get_comp(arg)
-    comp = computation_constructing_utils.create_federated_map_all_equal(
-        fn, arg)
+    comp = building_block_factory.create_federated_map_all_equal(fn, arg)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def federated_mean(self, value, weight):
     """Implements `federated_mean` as defined in `api/intrinsics.py`.
 
     Args:
       value: As in `api/intrinsics.py`.
@@ -303,40 +306,40 @@
     # TODO(b/120439632): Possibly allow the weight to be either structured or
     # non-scalar, e.g., for the case of averaging a convolutional layer, when
     # we would want to use a different weight for every filter, and where it
     # might be cumbersome for users to have to manually slice and assemble a
     # variable.
 
     value = value_impl.to_value(value, None, self._context_stack)
-    type_utils.check_federated_value_placement(value, placements.CLIENTS,
-                                               'value to be averaged')
+    value_utils.check_federated_value_placement(value, placements.CLIENTS,
+                                                'value to be averaged')
     if not type_utils.is_average_compatible(value.type_signature):
       raise TypeError(
           'The value type {} is not compatible with the average operator.'
           .format(value.type_signature))
 
     if weight is not None:
       weight = value_impl.to_value(weight, None, self._context_stack)
-      type_utils.check_federated_value_placement(weight, placements.CLIENTS,
-                                                 'weight to use in averaging')
+      value_utils.check_federated_value_placement(weight, placements.CLIENTS,
+                                                  'weight to use in averaging')
       py_typecheck.check_type(weight.type_signature.member,
                               computation_types.TensorType)
       if weight.type_signature.member.shape.ndims != 0:
         raise TypeError('The weight type {} is not a federated scalar.'.format(
             weight.type_signature))
       if not (weight.type_signature.member.dtype.is_integer or
               weight.type_signature.member.dtype.is_floating):
         raise TypeError(
             'The weight type {} is not a federated integer or floating-point '
             'tensor.'.format(weight.type_signature))
 
     value = value_impl.ValueImpl.get_comp(value)
     if weight is not None:
       weight = value_impl.ValueImpl.get_comp(weight)
-    comp = computation_constructing_utils.create_federated_mean(value, weight)
+    comp = building_block_factory.create_federated_mean(value, weight)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def federated_reduce(self, value, zero, op):
     """Implements `federated_reduce` as defined in `api/intrinsics.py`.
 
     Args:
       value: As in `api/intrinsics.py`.
@@ -350,37 +353,36 @@
       TypeError: As in `api/intrinsics.py`.
     """
     # TODO(b/113112108): Since in most cases, it can be assumed that CLIENTS is
     # a non-empty collective (or else, the computation fails), specifying zero
     # at this level of the API should probably be optional. TBD.
 
     value = value_impl.to_value(value, None, self._context_stack)
-    type_utils.check_federated_value_placement(value, placements.CLIENTS,
-                                               'value to be reduced')
+    value_utils.check_federated_value_placement(value, placements.CLIENTS,
+                                                'value to be reduced')
 
     zero = value_impl.to_value(zero, None, self._context_stack)
     py_typecheck.check_type(zero, value_base.Value)
 
     # TODO(b/113112108): We need a check here that zero does not have federated
     # constituents.
 
     op = value_impl.to_value(op, None, self._context_stack)
     py_typecheck.check_type(op, value_base.Value)
     py_typecheck.check_type(op.type_signature, computation_types.FunctionType)
-    op_type_expected = type_constructors.reduction_op(
-        zero.type_signature, value.type_signature.member)
+    op_type_expected = type_factory.reduction_op(zero.type_signature,
+                                                 value.type_signature.member)
     if not type_utils.is_assignable_from(op_type_expected, op.type_signature):
       raise TypeError('Expected an operator of type {}, got {}.'.format(
           op_type_expected, op.type_signature))
 
     value = value_impl.ValueImpl.get_comp(value)
     zero = value_impl.ValueImpl.get_comp(zero)
     op = value_impl.ValueImpl.get_comp(op)
-    comp = computation_constructing_utils.create_federated_reduce(
-        value, zero, op)
+    comp = building_block_factory.create_federated_reduce(value, zero, op)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def federated_sum(self, value):
     """Implements `federated_sum` as defined in `api/intrinsics.py`.
 
     Args:
       value: As in `api/intrinsics.py`.
@@ -388,24 +390,24 @@
     Returns:
       As in `api/intrinsics.py`.
 
     Raises:
       TypeError: As in `api/intrinsics.py`.
     """
     value = value_impl.to_value(value, None, self._context_stack)
-    type_utils.check_federated_value_placement(value, placements.CLIENTS,
-                                               'value to be summed')
+    value_utils.check_federated_value_placement(value, placements.CLIENTS,
+                                                'value to be summed')
 
     if not type_utils.is_sum_compatible(value.type_signature):
       raise TypeError(
           'The value type {} is not compatible with the sum operator.'.format(
               value.type_signature))
 
     value = value_impl.ValueImpl.get_comp(value)
-    comp = computation_constructing_utils.create_federated_sum(value)
+    comp = building_block_factory.create_federated_sum(value)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def federated_value(self, value, placement):
     """Implements `federated_value` as defined in `api/intrinsics.py`.
 
     Args:
       value: As in `api/intrinsics.py`.
@@ -419,16 +421,15 @@
     """
     # TODO(b/113112108): Verify that neither the value, nor any of its parts
     # are of a federated type.
 
     value = value_impl.to_value(value, None, self._context_stack)
 
     value = value_impl.ValueImpl.get_comp(value)
-    comp = computation_constructing_utils.create_federated_value(
-        value, placement)
+    comp = building_block_factory.create_federated_value(value, placement)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def federated_zip(self, value):
     """Implements `federated_zip` as defined in `api/intrinsics.py`.
 
     Args:
       value: As in `api/intrinsics.py`.
@@ -462,15 +463,15 @@
         raise TypeError(
             'The elements of the named tuple to zip must be placed at {!s}. '
             'Element placements: ({})'.format(
                 first_type_signature.placement,
                 ','.join(str(type.placement) for type in value.type_signature)))
 
     value = value_impl.ValueImpl.get_comp(value)
-    comp = computation_constructing_utils.create_federated_zip(value)
+    comp = building_block_factory.create_federated_zip(value)
     return value_impl.ValueImpl(comp, self._context_stack)
 
   def sequence_map(self, fn, arg):
     """Implements `sequence_map` as defined in `api/intrinsics.py`.
 
     Args:
       fn: As in `api/intrinsics.py`.
@@ -485,23 +486,23 @@
     fn = value_impl.to_value(fn, None, self._context_stack)
     py_typecheck.check_type(fn.type_signature, computation_types.FunctionType)
     arg = value_impl.to_value(arg, None, self._context_stack)
 
     if isinstance(arg.type_signature, computation_types.SequenceType):
       fn = value_impl.ValueImpl.get_comp(fn)
       arg = value_impl.ValueImpl.get_comp(arg)
-      return computation_constructing_utils.create_sequence_map(fn, arg)
+      return building_block_factory.create_sequence_map(fn, arg)
     elif isinstance(arg.type_signature, computation_types.FederatedType):
       parameter_type = computation_types.SequenceType(
           fn.type_signature.parameter)
       result_type = computation_types.SequenceType(fn.type_signature.result)
       intrinsic_type = computation_types.FunctionType(
           (fn.type_signature, parameter_type), result_type)
-      intrinsic = computation_building_blocks.Intrinsic(
-          intrinsic_defs.SEQUENCE_MAP.uri, intrinsic_type)
+      intrinsic = building_blocks.Intrinsic(intrinsic_defs.SEQUENCE_MAP.uri,
+                                            intrinsic_type)
       intrinsic_impl = value_impl.ValueImpl(intrinsic, self._context_stack)
       local_fn = value_utils.get_curried(intrinsic_impl)(fn)
       if arg.type_signature.placement is placements.SERVER:
         return self.federated_apply(local_fn, arg)
       elif arg.type_signature.placement is placements.CLIENTS:
         return self.federated_map(local_fn, arg)
       else:
@@ -533,40 +534,38 @@
       element_type = value.type_signature.element
     else:
       py_typecheck.check_type(value.type_signature,
                               computation_types.FederatedType)
       py_typecheck.check_type(value.type_signature.member,
                               computation_types.SequenceType)
       element_type = value.type_signature.member.element
-    op_type_expected = type_constructors.reduction_op(zero.type_signature,
-                                                      element_type)
+    op_type_expected = type_factory.reduction_op(zero.type_signature,
+                                                 element_type)
     if not type_utils.is_assignable_from(op_type_expected, op.type_signature):
       raise TypeError('Expected an operator of type {}, got {}.'.format(
           op_type_expected, op.type_signature))
 
     value = value_impl.ValueImpl.get_comp(value)
     zero = value_impl.ValueImpl.get_comp(zero)
     op = value_impl.ValueImpl.get_comp(op)
     if isinstance(value.type_signature, computation_types.SequenceType):
-      return computation_constructing_utils.create_sequence_reduce(
-          value, zero, op)
+      return building_block_factory.create_sequence_reduce(value, zero, op)
     else:
       value_type = computation_types.SequenceType(element_type)
       intrinsic_type = computation_types.FunctionType((
           value_type,
           zero.type_signature,
           op.type_signature,
       ), op.type_signature.result)
-      intrinsic = computation_building_blocks.Intrinsic(
-          intrinsic_defs.SEQUENCE_REDUCE.uri, intrinsic_type)
-      ref = computation_building_blocks.Reference('arg', value_type)
-      tup = computation_building_blocks.Tuple((ref, zero, op))
-      call = computation_building_blocks.Call(intrinsic, tup)
-      fn = computation_building_blocks.Lambda(ref.name, ref.type_signature,
-                                              call)
+      intrinsic = building_blocks.Intrinsic(intrinsic_defs.SEQUENCE_REDUCE.uri,
+                                            intrinsic_type)
+      ref = building_blocks.Reference('arg', value_type)
+      tup = building_blocks.Tuple((ref, zero, op))
+      call = building_blocks.Call(intrinsic, tup)
+      fn = building_blocks.Lambda(ref.name, ref.type_signature, call)
       fn_impl = value_impl.ValueImpl(fn, self._context_stack)
       if value.type_signature.placement is placements.SERVER:
         return self.federated_apply(fn_impl, value)
       elif value.type_signature.placement is placements.CLIENTS:
         return self.federated_map(fn_impl, value)
       else:
         raise TypeError('Unsupported placement {}.'.format(
@@ -596,20 +595,20 @@
     if not type_utils.is_sum_compatible(element_type):
       raise TypeError(
           'The value type {} is not compatible with the sum operator.'.format(
               value.type_signature.member))
 
     if isinstance(value.type_signature, computation_types.SequenceType):
       value = value_impl.ValueImpl.get_comp(value)
-      return computation_constructing_utils.create_sequence_sum(value)
+      return building_block_factory.create_sequence_sum(value)
     elif isinstance(value.type_signature, computation_types.FederatedType):
       intrinsic_type = computation_types.FunctionType(
           value.type_signature.member, value.type_signature.member.element)
-      intrinsic = computation_building_blocks.Intrinsic(
-          intrinsic_defs.SEQUENCE_SUM.uri, intrinsic_type)
+      intrinsic = building_blocks.Intrinsic(intrinsic_defs.SEQUENCE_SUM.uri,
+                                            intrinsic_type)
       intrinsic_impl = value_impl.ValueImpl(intrinsic, self._context_stack)
       if value.type_signature.placement is placements.SERVER:
         return self.federated_apply(intrinsic_impl, value)
       elif value.type_signature.placement is placements.CLIENTS:
         return self.federated_map(intrinsic_impl, value)
       else:
         raise TypeError('Unsupported placement {}.'.format(
```

## tensorflow_federated/python/core/impl/intrinsic_reductions.py

```diff
@@ -15,39 +15,38 @@
 """Intrinsic reductions as AST transformations."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 from tensorflow_federated.python.common_libs import py_typecheck
-from tensorflow_federated.python.core.impl import computation_building_blocks
 from tensorflow_federated.python.core.impl import context_stack_impl
-from tensorflow_federated.python.core.impl import transformations
+from tensorflow_federated.python.core.impl import value_transformations
+from tensorflow_federated.python.core.impl.compiler import building_blocks
 
 
 def replace_intrinsics_with_bodies(comp):
   """Reduces intrinsics to their bodies as defined in `intrinsic_bodies.py`.
 
   This function operates on the AST level; meaning, it takes in a
-  `computation_building_blocks.ComputationBuildingBlock` as an argument and
+  `building_blocks.ComputationBuildingBlock` as an argument and
   returns one as well. `replace_intrinsics_with_bodies` is intended to be the
   standard reduction function, which will reduce all currently implemented
   intrinsics to their bodies.
 
   Notice that the success of this function depends on the contract of
   `intrinsic_bodies.get_intrinsic_bodies`, that the dict returned by that
   function is ordered from more complex intrinsic to less complex intrinsics.
 
   Args:
-    comp: Instance of `computation_building_blocks.ComputationBuildingBlock` in
-      which we wish to replace all intrinsics with their bodies.
+    comp: Instance of `building_blocks.ComputationBuildingBlock` in which we
+      wish to replace all intrinsics with their bodies.
 
   Returns:
-    An instance of `computation_building_blocks.ComputationBuildingBlock` with
+    An instance of `building_blocks.ComputationBuildingBlock` with
     all intrinsics defined in `intrinsic_bodies.py` replaced with their bodies.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
   context_stack = context_stack_impl.context_stack
-  comp, _ = transformations.replace_all_intrinsics_with_bodies(
+  comp, _ = value_transformations.replace_all_intrinsics_with_bodies(
       comp, context_stack)
   return comp
```

## tensorflow_federated/python/core/impl/lambda_executor.py

```diff
@@ -16,21 +16,21 @@
 
 import asyncio
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
-from tensorflow_federated.python.core.impl import computation_building_blocks
 from tensorflow_federated.python.core.impl import computation_impl
 from tensorflow_federated.python.core.impl import executor_base
 from tensorflow_federated.python.core.impl import executor_value_base
 from tensorflow_federated.python.core.impl import transformations
-from tensorflow_federated.python.core.impl import type_serialization
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import building_blocks
+from tensorflow_federated.python.core.impl.compiler import type_serialization
 
 
 class LambdaExecutorScope(object):
   """Represents a naming scope for computations in the lambda executor."""
 
   def __init__(self, symbols, parent=None):
     """Constructs a new scope.
@@ -120,15 +120,15 @@
       py_typecheck.check_none(scope)
       py_typecheck.check_type(type_spec, computation_types.FunctionType)
     else:
       py_typecheck.check_type(value, anonymous_tuple.AnonymousTuple)
       py_typecheck.check_none(scope)
       py_typecheck.check_none(type_spec)
       type_elements = []
-      for k, v in anonymous_tuple.to_elements(value):
+      for k, v in anonymous_tuple.iter_elements(value):
         py_typecheck.check_type(v, LambdaExecutorValue)
         type_elements.append((k, v.type_signature))
       type_spec = computation_types.NamedTupleType([
           (k, v) if k is not None else v for k, v in type_elements
       ])
     self._value = value
     self._scope = scope
@@ -254,15 +254,16 @@
     py_typecheck.check_type(comp.type_signature, computation_types.FunctionType)
     param_type = comp.type_signature.parameter
     if param_type is not None:
       py_typecheck.check_type(arg, LambdaExecutorValue)
       if not type_utils.is_assignable_from(param_type, arg.type_signature):
         arg_type = type_utils.get_argument_type(arg.type_signature)
         type_utils.check_assignable_from(param_type, arg_type)
-        return await self.create_call(comp, await self.create_call(arg))
+        arg = await self.create_call(arg)
+        return await self.create_call(comp, arg)
     else:
       py_typecheck.check_none(arg)
     comp_repr = comp.internal_representation
     if isinstance(comp_repr, executor_value_base.ExecutorValue):
       delegated_arg = await self._delegate(arg) if arg is not None else None
       return LambdaExecutorValue(await self._target_executor.create_call(
           comp_repr, delegated_arg))
@@ -419,13 +420,13 @@
   Args:
     comp: An instance of `pb.Computation` to check.
 
   Raises:
     ValueError: If `comp` has unbound references.
   """
   py_typecheck.check_type(comp, pb.Computation)
-  blk = computation_building_blocks.ComputationBuildingBlock.from_proto(comp)
+  blk = building_blocks.ComputationBuildingBlock.from_proto(comp)
   unbound_map = transformations.get_map_of_unbound_references(blk)
   unbound_refs = unbound_map[blk]
   if unbound_refs:
     raise ValueError(
         'The computation contains unbound references: {}.'.format(unbound_refs))
```

## tensorflow_federated/python/core/impl/reference_executor.py

```diff
@@ -35,25 +35,25 @@
 
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_base
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.api import placements
 from tensorflow_federated.python.core.impl import compiler_pipeline
-from tensorflow_federated.python.core.impl import computation_building_blocks
 from tensorflow_federated.python.core.impl import computation_impl
 from tensorflow_federated.python.core.impl import context_base
-from tensorflow_federated.python.core.impl import dtype_utils
-from tensorflow_federated.python.core.impl import graph_utils
-from tensorflow_federated.python.core.impl import intrinsic_defs
-from tensorflow_federated.python.core.impl import placement_literals
+from tensorflow_federated.python.core.impl import runtime_utils
 from tensorflow_federated.python.core.impl import tensorflow_deserialization
 from tensorflow_federated.python.core.impl import transformations
-from tensorflow_federated.python.core.impl import type_constructors
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import building_blocks
+from tensorflow_federated.python.core.impl.compiler import intrinsic_defs
+from tensorflow_federated.python.core.impl.compiler import placement_literals
+from tensorflow_federated.python.core.impl.compiler import type_factory
+from tensorflow_federated.python.core.impl.utils import tensorflow_utils
 
 
 class ComputedValue(object):
   """A container for values computed by the reference executor."""
 
   def __init__(self, value, type_spec):
     """Creates a value with given raw payload `value` and TFF type `type_spec`.
@@ -79,57 +79,57 @@
     return self._type_signature
 
   @property
   def value(self):
     return self._value
 
   def __str__(self):
-    return 'ComputedValue({}, {})'.format(
-        str(self._value), str(self._type_signature))
+    return 'ComputedValue({}, {})'.format(self._value, self._type_signature)
 
 
 def to_representation_for_type(value, type_spec, callable_handler=None):
   """Verifies or converts the `value` representation to match `type_spec`.
 
   This method first tries to determine whether `value` is a valid representation
   of TFF type `type_spec`. If so, it is returned unchanged. If not, but if it
   can be converted into a valid representation, it is converted to such, and the
   valid representation is returned. If no conversion to a valid representation
   is possible, TypeError is raised.
 
   The accepted forms of `value` for vaqrious TFF types as as follows:
 
-  * For TFF tensor types listed in `dtypes.TENSOR_REPRESENTATION_TYPES`.
+  *   For TFF tensor types listed in
+      `tensorflow_utils.TENSOR_REPRESENTATION_TYPES`.
 
-  * For TFF named tuple types, instances of `anonymous_tuple.AnonymousTuple`.
+  *   For TFF named tuple types, instances of `anonymous_tuple.AnonymousTuple`.
 
-  * For TFF sequences, Python lists.
+  *   For TFF sequences, Python lists.
 
-  * For TFF functional types, Python callables that accept a single argument
-    that is an instance of `ComputedValue` (if the function has a parameter)
-    or `None` (otherwise), and return a `ComputedValue` instance as a result.
-    This function only verifies that `value` is a callable.
-
-  * For TFF abstract types, there is no valid representation. The reference
-    executor requires all types in an executable computation to be concrete.
-
-  * For TFF placement types, the valid representations are the placement
-    literals (currently only `tff.SERVER` and `tff.CLIENTS`).
-
-  * For TFF federated types with `all_equal` set to `True`, the representation
-    is the same as the representation of the member constituent (thus, e.g.,
-    a valid representation of `int32@SERVER` is the same as that of `int32`).
-    For those types that have `all_equal_` set to `False`, the representation
-    is a Python list of member constituents.
-
-    NOTE: This function does not attempt at validating that the sizes of lists
-    that represent federated values match the corresponding placemenets. The
-    cardinality analysis is a separate step, handled by the reference executor
-    at a different point. As long as values can be packed into a Python list,
-    they are accepted as they are.
+  *   For TFF functional types, Python callables that accept a single argument
+      that is an instance of `ComputedValue` (if the function has a parameter)
+      or `None` (otherwise), and return a `ComputedValue` instance as a result.
+      This function only verifies that `value` is a callable.
+
+  *   For TFF abstract types, there is no valid representation. The reference
+      executor requires all types in an executable computation to be concrete.
+
+  *   For TFF placement types, the valid representations are the placement
+      literals (currently only `tff.SERVER` and `tff.CLIENTS`).
+
+  *   For TFF federated types with `all_equal` set to `True`, the representation
+      is the same as the representation of the member constituent (thus, e.g.,
+      a valid representation of `int32@SERVER` is the same as that of `int32`).
+      For those types that have `all_equal_` set to `False`, the representation
+      is a Python list of member constituents.
+
+      NOTE: This function does not attempt at validating that the sizes of lists
+      that represent federated values match the corresponding placemenets. The
+      cardinality analysis is a separate step, handled by the reference executor
+      at a different point. As long as values can be packed into a Python list,
+      they are accepted as they are.
 
   Args:
     value: The raw representation of a value to compare against `type_spec` and
       potentially to be converted into a canonical form for the given TFF type.
     type_spec: The TFF type, an instance of `tff.Type` or something convertible
       to it that determines what the valid representation should be.
     callable_handler: The function to invoke to handle TFF functional types. If
@@ -153,20 +153,20 @@
   # NOTE: We do not simply call `type_utils.infer_type()` on `value`, as the
   # representations of values in the reference executor are only a subset of
   # the Python types recognized by that helper function.
 
   if isinstance(type_spec, computation_types.TensorType):
     if tf.executing_eagerly() and isinstance(value, (tf.Tensor, tf.Variable)):
       value = value.numpy()
-    py_typecheck.check_type(value, dtype_utils.TENSOR_REPRESENTATION_TYPES)
+    py_typecheck.check_type(value, tensorflow_utils.TENSOR_REPRESENTATION_TYPES)
     inferred_type_spec = type_utils.infer_type(value)
     if not type_utils.is_assignable_from(type_spec, inferred_type_spec):
       raise TypeError(
           'The tensor type {} of the value representation does not match '
-          'the type spec {}.'.format(str(inferred_type_spec), str(type_spec)))
+          'the type spec {}.'.format(inferred_type_spec, type_spec))
     return value
   elif isinstance(type_spec, computation_types.NamedTupleType):
     type_spec_elements = anonymous_tuple.to_elements(type_spec)
     # Special-casing unodered dictionaries to allow their elements to be fed in
     # the order in which they're defined in the named tuple type.
     if (isinstance(value, dict) and
         (set(value.keys()) == set(k for k, _ in type_spec_elements))):
@@ -175,16 +175,15 @@
       ])
     value = anonymous_tuple.from_container(value)
     value_elements = anonymous_tuple.to_elements(value)
     if len(value_elements) != len(type_spec_elements):
       raise TypeError(
           'The number of elements {} in the value tuple {} does not match the '
           'number of elements {} in the type spec {}.'.format(
-              len(value_elements), str(value), len(type_spec_elements),
-              str(type_spec)))
+              len(value_elements), value, len(type_spec_elements), type_spec))
     result_elements = []
     for index, (type_elem_name, type_elem) in enumerate(type_spec_elements):
       value_elem_name, value_elem = value_elements[index]
       if value_elem_name not in [type_elem_name, None]:
         raise TypeError(
             'Found element named `{}` where `{}` was expected at position {} '
             'in the value tuple. Value: {}. Type: {}'.format(
@@ -227,29 +226,28 @@
     if type_spec.all_equal:
       return to_representation_for_type(value, type_spec.member,
                                         callable_handler)
     elif type_spec.placement is not placements.CLIENTS:
       raise TypeError(
           'Unable to determine a valid value representation for a federated '
           'type with non-equal members placed at {}.'.format(
-              str(type_spec.placement)))
+              type_spec.placement))
     elif not isinstance(value, (list, tuple)):
       raise ValueError('Please pass a list or tuple to any function that'
                        ' expects a federated type placed at {};'
                        ' you passed {}'.format(type_spec.placement, value))
     else:
       return [
           to_representation_for_type(v, type_spec.member, callable_handler)
           for v in value
       ]
   else:
     raise NotImplementedError(
         'Unable to determine valid value representation for {} for what '
-        'is currently an unsupported TFF type {}.'.format(
-            str(value), str(type_spec)))
+        'is currently an unsupported TFF type {}.'.format(value, type_spec))
 
 
 def stamp_computed_value_into_graph(value, graph):
   """Stamps `value` in `graph`.
 
   Args:
     value: An instance of `ComputedValue`.
@@ -288,20 +286,20 @@
       stamped_elements = []
       for idx, (k, v) in enumerate(elements):
         computed_v = ComputedValue(v, type_elements[idx][1])
         stamped_v = stamp_computed_value_into_graph(computed_v, graph)
         stamped_elements.append((k, stamped_v))
       return anonymous_tuple.AnonymousTuple(stamped_elements)
     elif isinstance(value.type_signature, computation_types.SequenceType):
-      return graph_utils.make_data_set_from_elements(
+      return tensorflow_utils.make_data_set_from_elements(
           graph, value.value, value.type_signature.element)
     else:
       raise NotImplementedError(
           'Unable to embed a computed value of type {} in graph.'.format(
-              str(value.type_signature)))
+              value.type_signature))
 
 
 def capture_computed_value_from_graph(value, type_spec):
   """Captures `value` from a TensorFlow graph.
 
   Args:
     value: A Python object made of tensors in `graph`, `tf.data.Dataset`s,
@@ -314,38 +312,39 @@
   """
   type_spec = computation_types.to_type(type_spec)
   py_typecheck.check_type(type_spec, computation_types.Type)
   value = type_utils.to_canonical_value(value)
   return ComputedValue(to_representation_for_type(value, type_spec), type_spec)
 
 
+# TODO(b/139439722): Consolidate implementation to run a TF comp with an arg.
 def run_tensorflow(comp, arg):
   """Runs a compiled TensorFlow computation `comp` with argument `arg`.
 
   Args:
-    comp: An instance of `computation_building_blocks.CompiledComputation` with
-      embedded TensorFlow code.
+    comp: An instance of `building_blocks.CompiledComputation` with embedded
+      TensorFlow code.
     arg: An instance of `ComputedValue` that represents the argument, or `None`
       if the compuation expects no argument.
 
   Returns:
     An instance of `ComputedValue` with the result.
   """
-  py_typecheck.check_type(comp, computation_building_blocks.CompiledComputation)
+  py_typecheck.check_type(comp, building_blocks.CompiledComputation)
   if arg is not None:
     py_typecheck.check_type(arg, ComputedValue)
   with tf.Graph().as_default() as graph:
     stamped_arg = stamp_computed_value_into_graph(arg, graph)
     init_op, result = (
         tensorflow_deserialization.deserialize_and_call_tf_computation(
             comp.proto, stamped_arg, graph))
   with tf.compat.v1.Session(graph=graph) as sess:
     if init_op:
       sess.run(init_op)
-    result_val = graph_utils.fetch_value_in_session(sess, result)
+    result_val = tensorflow_utils.fetch_value_in_session(sess, result)
   return capture_computed_value_from_graph(result_val,
                                            comp.type_signature.result)
 
 
 def numpy_cast(value, dtype, shape):
   """Returns a Numpy representation of `value` for given `dtype` and `shape`.
 
@@ -360,17 +359,19 @@
   Raises:
     TypeError: If the `value` cannot be converted to the given `dtype` and the
       desired `shape`.
   """
   py_typecheck.check_type(dtype, tf.DType)
   py_typecheck.check_type(shape, tf.TensorShape)
   value_as_numpy_array = np.array(value, dtype=dtype.as_numpy_dtype)
-  if list(value_as_numpy_array.shape) != shape.dims:
+  if not (len(value_as_numpy_array.shape) == len(shape.dims) and
+          all(value_as_numpy_array.shape[i] == shape.dims[i] or
+              shape.dims[i].value is None) for i in range(len(shape.dims))):
     raise TypeError('Expected shape {}, found {}.'.format(
-        str(shape.dims), str(value_as_numpy_array.shape)))
+        shape.dims, value_as_numpy_array.shape))
   # NOTE: We don't want to make things more complicated than necessary by
   # returning the result as an array if it's just a plain scalar, so we
   # special-case this by pulling the singleton `np.ndarray`'s element out.
   if len(value_as_numpy_array.shape) > 0:  # pylint: disable=g-explicit-length-test
     return value_as_numpy_array
   else:
     return value_as_numpy_array.flatten()[0]
@@ -402,57 +403,15 @@
           ComputedValue(v, type_elements[idx][1]), multiplier).value
       result_elements.append((k, multiplied_v))
     return ComputedValue(
         anonymous_tuple.AnonymousTuple(result_elements), value.type_signature)
   else:
     raise NotImplementedError(
         'Multiplying vlues of type {} by a scalar is unsupported.'.format(
-            str(value.type_signature)))
-
-
-def get_cardinalities(value):
-  """Get a dictionary mapping placements to their cardinalities from `value`.
-
-  Args:
-    value: An instance of `ComputationValue`.
-
-  Returns:
-    A dictionary from placement literals to the cardinalities of each placement.
-  """
-  py_typecheck.check_type(value, ComputedValue)
-  if isinstance(value.type_signature, computation_types.FederatedType):
-    if value.type_signature.all_equal:
-      return {}
-    else:
-      py_typecheck.check_type(value.value, list)
-      return {value.type_signature.placement: len(value.value)}
-  elif isinstance(
-      value.type_signature,
-      (computation_types.TensorType, computation_types.SequenceType,
-       computation_types.AbstractType, computation_types.FunctionType,
-       computation_types.PlacementType)):
-    return {}
-  elif isinstance(value.type_signature, computation_types.NamedTupleType):
-    py_typecheck.check_type(value.value, anonymous_tuple.AnonymousTuple)
-    result = {}
-    for idx, (_, elem_type) in enumerate(
-        anonymous_tuple.to_elements(value.type_signature)):
-      for k, v in six.iteritems(
-          get_cardinalities(ComputedValue(value.value[idx], elem_type))):
-        if k not in result:
-          result[k] = v
-        elif result[k] != v:
-          raise ValueError(
-              'Mismatching cardinalities for {}: {} vs. {}.'.format(
-                  str(k), str(result[k]), str(v)))
-    return result
-  else:
-    raise NotImplementedError(
-        'Unable to get cardinalities from a value of TFF type {}.'.format(
-            str(value.type_signature)))
+            value.type_signature))
 
 
 class ComputationContext(object):
   """Encapsulates context/state in which computations or parts thereof run."""
 
   def __init__(self,
                parent_context=None,
@@ -516,16 +475,16 @@
     """
     py_typecheck.check_type(placement, placement_literals.PlacementLiteral)
     if self._cardinalities is not None and placement in self._cardinalities:
       return self._cardinalities[placement]
     elif self._parent_context is not None:
       return self._parent_context.get_cardinality(placement)
     else:
-      raise ValueError('Unable to determine the cardinality for {}.'.format(
-          str(placement)))
+      raise ValueError(
+          'Unable to determine the cardinality for {}.'.format(placement))
 
 
 def fit_argument(arg, type_spec, context):
   """Fits the given argument `arg` to match the given parameter `type_spec`.
 
   Args:
     arg: The argument to fit, an instance of `ComputedValue`.
@@ -572,15 +531,15 @@
         return ComputedValue(member_val.value, type_spec)
       else:
         cardinality = context.get_cardinality(type_spec.placement)
         return ComputedValue([member_val.value for _ in range(cardinality)],
                              type_spec)
     elif type_spec.all_equal:
       raise TypeError('Cannot fit a non all-equal {} into all-equal {}.'.format(
-          str(arg.type_signature), str(type_spec)))
+          arg.type_signature, type_spec))
     else:
       py_typecheck.check_type(arg.value, list)
 
       def _fit_member_val(x):
         x_val = ComputedValue(x, arg.type_signature.member)
         return fit_argument(x_val, type_spec.member, context).value
 
@@ -675,15 +634,15 @@
     root_context = ComputationContext(cardinalities=cardinalities)
     computed_comp = self._compute(comp, root_context)
     type_utils.check_assignable_from(comp.type_signature,
                                      computed_comp.type_signature)
     if not isinstance(computed_comp.type_signature,
                       computation_types.FunctionType):
       if arg is not None:
-        raise TypeError('Unexpected argument {}.'.format(str(arg)))
+        raise TypeError('Unexpected argument {}.'.format(arg))
       else:
         value = computed_comp.value
         result_type = fn.type_signature.result
         if type_utils.is_anon_tuple_with_py_container(value, result_type):
           return type_utils.convert_to_py_container(value, result_type)
         return value
     else:
@@ -696,15 +655,17 @@
           return computed_fn.value
 
         computed_arg = ComputedValue(
             to_representation_for_type(arg,
                                        computed_comp.type_signature.parameter,
                                        _handle_callable),
             computed_comp.type_signature.parameter)
-        cardinalities.update(get_cardinalities(computed_arg))
+        cardinalities.update(
+            runtime_utils.infer_cardinalities(computed_arg.value,
+                                              computed_arg.type_signature))
       else:
         computed_arg = None
       result = computed_comp.value(computed_arg)
       py_typecheck.check_type(result, ComputedValue)
       type_utils.check_assignable_from(comp.type_signature.result,
                                        result.type_signature)
       value = result.value
@@ -716,82 +677,80 @@
   def _compile(self, comp):
     """Compiles a `computation_base.Computation` to prepare it for execution.
 
     Args:
       comp: An instance of `computation_base.Computation`.
 
     Returns:
-      An instance of `computation_building_blocks.ComputationBuildingBlock` that
+      An instance of `building_blocks.ComputationBuildingBlock` that
       contains the compiled logic of `comp`.
     """
     py_typecheck.check_type(comp, computation_base.Computation)
     if self._compiler is not None:
       comp = self._compiler.compile(comp)
     comp, _ = transformations.uniquify_compiled_computation_names(
-        computation_building_blocks.ComputationBuildingBlock.from_proto(
+        building_blocks.ComputationBuildingBlock.from_proto(
             computation_impl.ComputationImpl.get_proto(comp)))
     return comp
 
   def _compute(self, comp, context):
     """Computes `comp` and returns the resulting computed value.
 
     Args:
-      comp: An instance of
-        `computation_building_blocks.ComputationBuildingBlock`.
+      comp: An instance of `building_blocks.ComputationBuildingBlock`.
       context: An instance of `ComputationContext`.
 
     Returns:
       The corresponding instance of `ComputedValue` that represents the result
       of `comp`.
 
     Raises:
       TypeError: If type mismatch occurs during the course of computation.
       ValueError: If a malformed value is encountered.
       NotImplementedError: For computation building blocks that are not yet
         supported by this executor.
     """
-    if isinstance(comp, computation_building_blocks.CompiledComputation):
+    if isinstance(comp, building_blocks.CompiledComputation):
       return self._compute_compiled(comp, context)
-    elif isinstance(comp, computation_building_blocks.Call):
+    elif isinstance(comp, building_blocks.Call):
       return self._compute_call(comp, context)
-    elif isinstance(comp, computation_building_blocks.Tuple):
+    elif isinstance(comp, building_blocks.Tuple):
       return self._compute_tuple(comp, context)
-    elif isinstance(comp, computation_building_blocks.Reference):
+    elif isinstance(comp, building_blocks.Reference):
       return self._compute_reference(comp, context)
-    elif isinstance(comp, computation_building_blocks.Selection):
+    elif isinstance(comp, building_blocks.Selection):
       return self._compute_selection(comp, context)
-    elif isinstance(comp, computation_building_blocks.Lambda):
+    elif isinstance(comp, building_blocks.Lambda):
       return self._compute_lambda(comp, context)
-    elif isinstance(comp, computation_building_blocks.Block):
+    elif isinstance(comp, building_blocks.Block):
       return self._compute_block(comp, context)
-    elif isinstance(comp, computation_building_blocks.Intrinsic):
+    elif isinstance(comp, building_blocks.Intrinsic):
       return self._compute_intrinsic(comp, context)
-    elif isinstance(comp, computation_building_blocks.Data):
+    elif isinstance(comp, building_blocks.Data):
       return self._compute_data(comp, context)
-    elif isinstance(comp, computation_building_blocks.Placement):
+    elif isinstance(comp, building_blocks.Placement):
       return self._compute_placement(comp, context)
     else:
       raise NotImplementedError(
           'A computation building block of a type {} not currently recognized '
-          'by the reference executor: {}.'.format(str(type(comp)), str(comp)))
+          'by the reference executor: {}.'.format(type(comp), comp))
 
   def _compute_compiled(self, comp, context):
-    py_typecheck.check_type(comp,
-                            computation_building_blocks.CompiledComputation)
+    py_typecheck.check_type(comp, building_blocks.CompiledComputation)
     computation_oneof = comp.proto.WhichOneof('computation')
     if computation_oneof != 'tensorflow':
       raise ValueError(
           'Expected all parsed compiled computations to be tensorflow, '
           'but found \'{}\' instead.'.format(computation_oneof))
     else:
       return ComputedValue(lambda x: run_tensorflow(comp, x),
                            comp.type_signature)
 
   def _compute_call(self, comp, context):
-    py_typecheck.check_type(comp, computation_building_blocks.Call)
+    py_typecheck.check_type(comp, building_blocks.Call)
     computed_fn = self._compute(comp.function, context)
     py_typecheck.check_type(computed_fn.type_signature,
                             computation_types.FunctionType)
     if comp.argument is not None:
       computed_arg = self._compute(comp.argument, context)
       type_utils.check_assignable_from(computed_fn.type_signature.parameter,
                                        computed_arg.type_signature)
@@ -802,31 +761,31 @@
     result = computed_fn.value(computed_arg)
     py_typecheck.check_type(result, ComputedValue)
     type_utils.check_assignable_from(computed_fn.type_signature.result,
                                      result.type_signature)
     return result
 
   def _compute_tuple(self, comp, context):
-    py_typecheck.check_type(comp, computation_building_blocks.Tuple)
+    py_typecheck.check_type(comp, building_blocks.Tuple)
     result_elements = []
     result_type_elements = []
-    for k, v in anonymous_tuple.to_elements(comp):
+    for k, v in anonymous_tuple.iter_elements(comp):
       computed_v = self._compute(v, context)
       type_utils.check_assignable_from(v.type_signature,
                                        computed_v.type_signature)
       result_elements.append((k, computed_v.value))
       result_type_elements.append((k, computed_v.type_signature))
     return ComputedValue(
         anonymous_tuple.AnonymousTuple(result_elements),
         computation_types.NamedTupleType([
             (k, v) if k else v for k, v in result_type_elements
         ]))
 
   def _compute_selection(self, comp, context):
-    py_typecheck.check_type(comp, computation_building_blocks.Selection)
+    py_typecheck.check_type(comp, building_blocks.Selection)
     source = self._compute(comp.source, context)
     py_typecheck.check_type(source.type_signature,
                             computation_types.NamedTupleType)
     py_typecheck.check_type(source.value, anonymous_tuple.AnonymousTuple)
     if comp.name is not None:
       result_value = getattr(source.value, comp.name)
       result_type = getattr(source.type_signature, comp.name)
@@ -834,45 +793,44 @@
       assert comp.index is not None
       result_value = source.value[comp.index]
       result_type = source.type_signature[comp.index]
     type_utils.check_assignable_from(comp.type_signature, result_type)
     return ComputedValue(result_value, result_type)
 
   def _compute_lambda(self, comp, context):
-    py_typecheck.check_type(comp, computation_building_blocks.Lambda)
+    py_typecheck.check_type(comp, building_blocks.Lambda)
     py_typecheck.check_type(context, ComputationContext)
 
     def _wrap(arg):
       py_typecheck.check_type(arg, ComputedValue)
       if not type_utils.is_assignable_from(comp.parameter_type,
                                            arg.type_signature):
         raise TypeError(
             'Expected the type of argument {} to be {}, found {}.'.format(
-                str(comp.parameter_name), str(comp.parameter_type),
-                str(arg.type_signature)))
+                comp.parameter_name, comp.parameter_type, arg.type_signature))
       return ComputationContext(context, {comp.parameter_name: arg})
 
     return ComputedValue(lambda x: self._compute(comp.result, _wrap(x)),
                          comp.type_signature)
 
   def _compute_reference(self, comp, context):
-    py_typecheck.check_type(comp, computation_building_blocks.Reference)
+    py_typecheck.check_type(comp, building_blocks.Reference)
     py_typecheck.check_type(context, ComputationContext)
     return context.resolve_reference(comp.name)
 
   def _compute_block(self, comp, context):
-    py_typecheck.check_type(comp, computation_building_blocks.Block)
+    py_typecheck.check_type(comp, building_blocks.Block)
     py_typecheck.check_type(context, ComputationContext)
     for local_name, local_comp in comp.locals:
       local_val = self._compute(local_comp, context)
       context = ComputationContext(context, {local_name: local_val})
     return self._compute(comp.result, context)
 
   def _compute_intrinsic(self, comp, context):
-    py_typecheck.check_type(comp, computation_building_blocks.Intrinsic)
+    py_typecheck.check_type(comp, building_blocks.Intrinsic)
     my_method = self._intrinsic_method_dict.get(comp.uri)
     if my_method is not None:
       # The interpretation of `my_method` depends on whether the intrinsic
       # does or does not take arguments. If it does, the method accepts the
       # argument as a `ComputedValue` instance. Otherwise, if the intrinsic
       # is not a function, but a constant (such as `GENERIC_ZERO`), the
       # method accepts the type of the result.
@@ -884,24 +842,25 @@
       else:
         return my_method(comp.type_signature)
     else:
       raise NotImplementedError('Intrinsic {} is currently unsupported.'.format(
           comp.uri))
 
   def _compute_data(self, comp, context):
-    py_typecheck.check_type(comp, computation_building_blocks.Data)
+    py_typecheck.check_type(comp, building_blocks.Data)
     raise NotImplementedError('Data is currently unsupported.')
 
   def _compute_placement(self, comp, context):
-    py_typecheck.check_type(comp, computation_building_blocks.Placement)
+    py_typecheck.check_type(comp, building_blocks.Placement)
     raise NotImplementedError('Placement is currently unsupported.')
 
   def _sequence_sum(self, arg):
+    inferred_type_spec = type_utils.infer_type(arg.value[0])
     py_typecheck.check_type(arg.type_signature, computation_types.SequenceType)
-    total = self._generic_zero(arg.type_signature.element)
+    total = self._generic_zero(inferred_type_spec)
     for v in arg.value:
       total = self._generic_plus(
           ComputedValue(
               anonymous_tuple.AnonymousTuple([(None, total.value), (None, v)]),
               [arg.type_signature.element, arg.type_signature.element]))
     return total
 
@@ -989,49 +948,49 @@
         with tf.compat.v1.Session(graph=graph) as sess:
           zeros_val = sess.run(zeros)
       return ComputedValue(zeros_val, type_spec)
     elif isinstance(type_spec, computation_types.NamedTupleType):
       return ComputedValue(
           anonymous_tuple.AnonymousTuple([
               (k, self._generic_zero(v).value)
-              for k, v in anonymous_tuple.to_elements(type_spec)
+              for k, v in anonymous_tuple.iter_elements(type_spec)
           ]), type_spec)
     elif isinstance(
         type_spec,
         (computation_types.SequenceType, computation_types.FunctionType,
          computation_types.AbstractType, computation_types.PlacementType)):
       raise TypeError(
           'The generic_zero is not well-defined for TFF type {}.'.format(
-              str(type_spec)))
+              type_spec))
     elif isinstance(type_spec, computation_types.FederatedType):
       if type_spec.all_equal:
         return ComputedValue(
             self._generic_zero(type_spec.member).value, type_spec)
       else:
         # TODO(b/113116813): Implement this in terms of the generic placement
         # operator once it's been added to the mix.
         raise NotImplementedError(
             'Generic zero support for non-all_equal federated types is not '
             'implemented yet.')
     else:
       raise NotImplementedError(
           'Generic zero support for {} is not implemented yet.'.format(
-              str(type_spec)))
+              type_spec))
 
   def _generic_plus(self, arg):
     py_typecheck.check_type(arg.type_signature,
                             computation_types.NamedTupleType)
     if len(arg.type_signature) != 2:
       raise TypeError('Generic plus is undefined for tuples of size {}.'.format(
-          str(len(arg.type_signature))))
+          len(arg.type_signature)))
     element_type = arg.type_signature[0]
     if arg.type_signature[1] != element_type:
       raise TypeError('Generic plus is undefined for two-tuples of different '
-                      'types ({} vs. {}).'.format(
-                          str(element_type), str(arg.type_signature[1])))
+                      'types ({} vs. {}).'.format(element_type,
+                                                  arg.type_signature[1]))
     if isinstance(element_type, computation_types.TensorType):
       val = numpy_cast(arg.value[0] + arg.value[1], element_type.dtype,
                        element_type.shape)
       return ComputedValue(val, element_type)
     elif isinstance(element_type, computation_types.NamedTupleType):
       py_typecheck.check_type(arg.value[0], anonymous_tuple.AnonymousTuple)
       py_typecheck.check_type(arg.value[1], anonymous_tuple.AnonymousTuple)
@@ -1111,30 +1070,29 @@
     type_utils.check_federated_type(arg.type_signature, None,
                                     placements.CLIENTS, False)
     py_typecheck.check_type(arg.value, list)
     server_sum = self._federated_sum(arg)
     unplaced_avg = multiply_by_scalar(
         ComputedValue(server_sum.value, server_sum.type_signature.member),
         1.0 / float(len(arg.value)))
-    return ComputedValue(
-        unplaced_avg.value,
-        type_constructors.at_server(unplaced_avg.type_signature))
+    return ComputedValue(unplaced_avg.value,
+                         type_factory.at_server(unplaced_avg.type_signature))
 
   def _federated_zip_at_server(self, arg):
     py_typecheck.check_type(arg.type_signature,
                             computation_types.NamedTupleType)
     for idx in range(len(arg.type_signature)):
       type_utils.check_federated_type(arg.type_signature[idx], None,
                                       placements.SERVER, True)
     return ComputedValue(
         arg.value,
-        type_constructors.at_server(
+        type_factory.at_server(
             computation_types.NamedTupleType([
                 (k, v.member) if k else v.member
-                for k, v in anonymous_tuple.to_elements(arg.type_signature)
+                for k, v in anonymous_tuple.iter_elements(arg.type_signature)
             ])))
 
   def _federated_zip_at_clients(self, arg):
     py_typecheck.check_type(arg.type_signature,
                             computation_types.NamedTupleType)
     py_typecheck.check_type(arg.value, anonymous_tuple.AnonymousTuple)
     zip_args = []
@@ -1145,23 +1103,23 @@
       zip_args.append(val)
       val_type = arg.type_signature[idx]
       type_utils.check_federated_type(val_type, None, placements.CLIENTS, False)
       zip_arg_types.append(val_type.member)
     zipped_val = [anonymous_tuple.from_container(x) for x in zip(*zip_args)]
     return ComputedValue(
         zipped_val,
-        type_constructors.at_clients(
+        type_factory.at_clients(
             computation_types.NamedTupleType(zip_arg_types)))
 
   def _federated_aggregate(self, arg):
     py_typecheck.check_type(arg.type_signature,
                             computation_types.NamedTupleType)
     if len(arg.type_signature) != 5:
       raise TypeError('Expected a 5-tuple, found {}.'.format(
-          str(arg.type_signature)))
+          arg.type_signature))
     root_accumulator = self._federated_reduce(
         ComputedValue(
             anonymous_tuple.from_container([arg.value[k] for k in range(3)]),
             [arg.type_signature[k] for k in range(3)]))
     return self._federated_apply(
         ComputedValue([arg.value[4], root_accumulator.value],
                       [arg.type_signature[4], root_accumulator.type_signature]))
@@ -1172,15 +1130,15 @@
     v_type = arg.type_signature[0].member
     total = sum(arg.value[1])
     products_val = [
         multiply_by_scalar(ComputedValue(v, v_type), w / total).value
         for v, w in zip(arg.value[0], arg.value[1])
     ]
     return self._federated_sum(
-        ComputedValue(products_val, type_constructors.at_clients(v_type)))
+        ComputedValue(products_val, type_factory.at_clients(v_type)))
 
   def _federated_broadcast(self, arg):
     type_utils.check_federated_type(arg.type_signature, None, placements.SERVER,
                                     True)
     return ComputedValue(
         arg.value,
         computation_types.FederatedType(arg.type_signature.member,
```

## tensorflow_federated/python/core/impl/remote_executor.py

```diff
@@ -10,25 +10,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A local proxy for a remote executor service hosted on a separate machine."""
 
+import asyncio
+import logging
+import queue
+import threading
+
 import grpc
 
 from tensorflow_federated.proto.v0 import executor_pb2
 from tensorflow_federated.proto.v0 import executor_pb2_grpc
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.impl import executor_base
 from tensorflow_federated.python.core.impl import executor_service_utils
 from tensorflow_federated.python.core.impl import executor_value_base
 
+_STREAM_CLOSE_WAIT_SECONDS = 10
+
 
 class RemoteValue(executor_value_base.ExecutorValue):
   """A reference to a value embedded in a remotely deployed executor service."""
 
   def __init__(self, value_ref, type_spec, executor):
     """Creates the value.
 
@@ -53,73 +60,204 @@
     return await self._executor._compute(self._value_ref)  # pylint: disable=protected-access
 
   @property
   def value_ref(self):
     return self._value_ref
 
 
+class _BidiStream:
+  """A bidi stream connection to the Executor service's Execute method."""
+
+  def __init__(self, stub, thread_pool_executor):
+    self._request_queue = queue.Queue()
+    self._response_event_queue = queue.Queue()
+    self._stream_closed_event = threading.Event()
+    self._thread_pool_executor = thread_pool_executor
+
+    def request_iter():
+      """Iterator that blocks on the request Queue."""
+      while True:
+        logging.debug('request_iter: waiting for request')
+        val = self._request_queue.get()
+        if val:
+          py_typecheck.check_type(val[0], executor_pb2.ExecuteRequest)
+          py_typecheck.check_type(val[1], threading.Event)
+          logging.debug('request_iter: got request of type %s',
+                        val[0].WhichOneof('request'))
+          self._response_event_queue.put_nowait(val[1])
+          yield val[0]
+        else:
+          logging.debug('request_iter: got None request')
+          # None means we are done processing
+          return
+
+    response_iter = stub.Execute(request_iter())
+
+    def response_thread_fn():
+      """Consumes response iter and exposes the value on corresponding Event."""
+      try:
+        logging.debug('response_thread_fn: waiting for response')
+        for response in response_iter:
+          logging.debug('response_thread_fn: got response of type %s',
+                        response.WhichOneof('response'))
+          # Get the corresponding response Event from the queue
+          response_event = self._response_event_queue.get_nowait()
+          # Attach the response as an attribute on the Event
+          response_event.response = response
+          response_event.set()
+        # Set the event indicating the stream has been closed
+        self._stream_closed_event.set()
+      except grpc.RpcError as error:
+        self._response_event_queue.put(error)
+
+    response_thread = threading.Thread(target=response_thread_fn)
+    response_thread.daemon = True
+    response_thread.start()
+
+  async def send_request(self, request):
+    """Send a request on the bidi stream."""
+    py_typecheck.check_type(request, executor_pb2.ExecuteRequest)
+    request_type = request.WhichOneof('request')
+    response_event = threading.Event()
+    # Enqueue a tuple of request and an Event used to return the response
+    self._request_queue.put((request, response_event))
+    await asyncio.get_event_loop().run_in_executor(self._thread_pool_executor,
+                                                   response_event.wait)
+    response = response_event.response
+    if isinstance(response, Exception):
+      raise response
+    py_typecheck.check_type(response, executor_pb2.ExecuteResponse)
+    response_type = response.WhichOneof('response')
+    if response_type != request_type:
+      raise ValueError('Request had type: {} but response had type: {}'.format(
+          request_type, response_type))
+    return response
+
+  def close(self):
+    self._request_queue.put(None)
+    # Wait for the stream to be closed
+    self._stream_closed_event.wait(_STREAM_CLOSE_WAIT_SECONDS)
+
+
 class RemoteExecutor(executor_base.Executor):
   """The remote executor is a local proxy for a remote executor instance.
 
   NOTE: This component is only available in Python 3.
   """
 
   # TODO(b/134543154): Switch to using an asynchronous gRPC client so we don't
   # have to block on all those calls.
 
-  def __init__(self, channel):
+  def __init__(self,
+               channel,
+               rpc_mode='REQUEST_REPLY',
+               thread_pool_executor=None):
     """Creates a remote executor.
 
     Args:
       channel: An instance of `grpc.Channel` to use for communication with the
         remote executor service.
+      rpc_mode: Optional mode of calling the remote executor. Must be either
+        'REQUEST_REPLY' or 'STREAMING' (defaults to 'REQUEST_REPLY'). This
+        option will be removed after the request-reply interface is deprecated.
+      thread_pool_executor: Optional concurrent.futures.Executor used to wait
+        for the reply to a streaming RPC message. Uses the default Executor if
+        not specified.
     """
     py_typecheck.check_type(channel, grpc.Channel)
+    py_typecheck.check_type(rpc_mode, str)
+    if rpc_mode not in ['REQUEST_REPLY', 'STREAMING']:
+      raise ValueError('Invalid rpc_mode: {}'.format(rpc_mode))
+
     self._stub = executor_pb2_grpc.ExecutorStub(channel)
+    self._bidi_stream = None
+    if rpc_mode == 'STREAMING':
+      self._bidi_stream = _BidiStream(self._stub, thread_pool_executor)
+
+  def __del__(self):
+    if self._bidi_stream:
+      self._bidi_stream.close()
+      del self._bidi_stream
 
   async def create_value(self, value, type_spec=None):
     value_proto, type_spec = (
         executor_service_utils.serialize_value(value, type_spec))
-    response = self._stub.CreateValue(
-        executor_pb2.CreateValueRequest(value=value_proto))
+    create_value_request = executor_pb2.CreateValueRequest(value=value_proto)
+    if not self._bidi_stream:
+      response = self._stub.CreateValue(create_value_request)
+    else:
+      response = (await self._bidi_stream.send_request(
+          executor_pb2.ExecuteRequest(create_value=create_value_request)
+      )).create_value
     py_typecheck.check_type(response, executor_pb2.CreateValueResponse)
     return RemoteValue(response.value_ref, type_spec, self)
 
   async def create_call(self, comp, arg=None):
     py_typecheck.check_type(comp, RemoteValue)
     py_typecheck.check_type(comp.type_signature, computation_types.FunctionType)
     if arg is not None:
       py_typecheck.check_type(arg, RemoteValue)
-    response = self._stub.CreateCall(
-        executor_pb2.CreateCallRequest(
-            function_ref=comp.value_ref,
-            argument_ref=(arg.value_ref if arg is not None else None)))
+    create_call_request = executor_pb2.CreateCallRequest(
+        function_ref=comp.value_ref,
+        argument_ref=(arg.value_ref if arg is not None else None))
+    if not self._bidi_stream:
+      response = self._stub.CreateCall(create_call_request)
+    else:
+      response = (await self._bidi_stream.send_request(
+          executor_pb2.ExecuteRequest(create_call=create_call_request)
+      )).create_call
     py_typecheck.check_type(response, executor_pb2.CreateCallResponse)
     return RemoteValue(response.value_ref, comp.type_signature.result, self)
 
   async def create_tuple(self, elements):
     elem = anonymous_tuple.to_elements(anonymous_tuple.from_container(elements))
     proto_elem = []
     type_elem = []
     for k, v in elem:
       py_typecheck.check_type(v, RemoteValue)
       proto_elem.append(
           executor_pb2.CreateTupleRequest.Element(
               name=(k if k else None), value_ref=v.value_ref))
       type_elem.append((k, v.type_signature) if k else v.type_signature)
     result_type = computation_types.NamedTupleType(type_elem)
-    response = self._stub.CreateTuple(
-        executor_pb2.CreateTupleRequest(element=proto_elem))
+    request = executor_pb2.CreateTupleRequest(element=proto_elem)
+    if not self._bidi_stream:
+      response = self._stub.CreateTuple(request)
+    else:
+      response = (await self._bidi_stream.send_request(
+          executor_pb2.ExecuteRequest(create_tuple=request))).create_tuple
     py_typecheck.check_type(response, executor_pb2.CreateTupleResponse)
     return RemoteValue(response.value_ref, result_type, self)
 
   async def create_selection(self, source, index=None, name=None):
-    # TODO(b/134543154): Implement this.
-    raise NotImplementedError
+    py_typecheck.check_type(source, RemoteValue)
+    py_typecheck.check_type(source.type_signature,
+                            computation_types.NamedTupleType)
+    if index is not None:
+      py_typecheck.check_type(index, int)
+      py_typecheck.check_none(name)
+      result_type = source.type_signature[index]
+    else:
+      py_typecheck.check_type(name, str)
+      result_type = getattr(source.type_signature, name)
+    request = executor_pb2.CreateSelectionRequest(
+        source_ref=source.value_ref, name=name, index=index)
+    if not self._bidi_stream:
+      response = self._stub.CreateSelection(request)
+    else:
+      response = (await self._bidi_stream.send_request(
+          executor_pb2.ExecuteRequest(create_selection=request)
+      )).create_selection
+    py_typecheck.check_type(response, executor_pb2.CreateSelectionResponse)
+    return RemoteValue(response.value_ref, result_type, self)
 
   async def _compute(self, value_ref):
     py_typecheck.check_type(value_ref, executor_pb2.ValueRef)
     request = executor_pb2.ComputeRequest(value_ref=value_ref)
-    response = self._stub.Compute(request)
+    if not self._bidi_stream:
+      response = self._stub.Compute(request)
+    else:
+      response = (await self._bidi_stream.send_request(
+          executor_pb2.ExecuteRequest(compute=request))).compute
     py_typecheck.check_type(response, executor_pb2.ComputeResponse)
     value, _ = executor_service_utils.deserialize_value(response.value)
     return value
```

## tensorflow_federated/python/core/impl/set_default_executor.py

```diff
@@ -22,16 +22,23 @@
 
 def set_default_executor(executor=None):
   """Places an `executor`-backed execution context at the top of the stack.
 
   NOTE: This function is only available in Python 3.
 
   Args:
-    executor: Either an instance of `executor_base.Executor`, or `None` which
-      causes the default reference executor to be installed (as is the default).
+    executor: Either an instance of `executor_base.Executor`, a factory
+      function returning such executors, or `None`. If `executor` is a factory
+      function, the constructed context will infer the number of clients from
+      the data it is passed, if possible. If `None`, causes the default
+      reference executor to be installed (as is the default).
   """
-  if executor is not None:
-    py_typecheck.check_type(executor, executor_base.Executor)
+  # TODO(b/140112504): Follow up here when we implement the ExecutorFactory
+  # interface.
+  if isinstance(executor, executor_base.Executor):
+    context = execution_context.ExecutionContext(lambda x: executor)
+  elif callable(executor):
     context = execution_context.ExecutionContext(executor)
   else:
+    py_typecheck.check_none(executor)
     context = None
   context_stack_impl.context_stack.set_default_context(context)
```

## tensorflow_federated/python/core/impl/tensorflow_deserialization.py

```diff
@@ -27,17 +27,17 @@
 import six
 from six.moves import zip
 import tensorflow as tf
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.common_libs import serialization_utils
-from tensorflow_federated.python.core.impl import graph_utils
-from tensorflow_federated.python.core.impl import type_serialization
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import type_serialization
+from tensorflow_federated.python.core.impl.utils import tensorflow_utils
 
 
 def deserialize_and_call_tf_computation(computation_proto, arg, graph):
   """Deserializes a TF computation and inserts it into `graph`.
 
   This method performs an action that can be considered roughly the opposite of
   what `tensorflow_serialization.serialize_py_fn_as_tf_computation` does. At
@@ -78,33 +78,34 @@
     type_spec = type_serialization.deserialize_type(computation_proto.type)
     if type_spec.parameter is None:
       if arg is None:
         input_map = None
       else:
         raise TypeError(
             'The computation declared no parameters; encountered an unexpected '
-            'argument {}.'.format(str(arg)))
+            'argument {}.'.format(arg))
     elif arg is None:
       raise TypeError(
           'The computation declared a parameter of type {}, but the argument '
-          'was not supplied.'.format(str(type_spec.parameter)))
+          'was not supplied.'.format(type_spec.parameter))
     else:
-      arg_type, arg_binding = graph_utils.capture_result_from_graph(arg, graph)
+      arg_type, arg_binding = tensorflow_utils.capture_result_from_graph(
+          arg, graph)
       if not type_utils.is_assignable_from(type_spec.parameter, arg_type):
         raise TypeError(
             'The computation declared a parameter of type {}, but the argument '
-            'is of a mismatching type {}.'.format(
-                str(type_spec.parameter), str(arg_type)))
+            'is of a mismatching type {}.'.format(type_spec.parameter,
+                                                  arg_type))
       else:
         input_map = {
             k: graph.get_tensor_by_name(v) for k, v in six.iteritems(
-                graph_utils.compute_map_from_bindings(
+                tensorflow_utils.compute_map_from_bindings(
                     computation_proto.tensorflow.parameter, arg_binding))
         }
-    return_elements = graph_utils.extract_tensor_names_from_binding(
+    return_elements = tensorflow_utils.extract_tensor_names_from_binding(
         computation_proto.tensorflow.result)
     orig_init_op_name = computation_proto.tensorflow.initialize_op
     if orig_init_op_name:
       return_elements.append(orig_init_op_name)
     # N. B. Unlike MetaGraphDef, the GraphDef alone contains no information
     # about collections, and hence, when we import a graph with Variables,
     # those Variables are not added to global collections, and hence
@@ -121,10 +122,10 @@
         # somewhat more readable, since _N style de-duplication of graph
         # node names is less likely to be needed.
         name='subcomputation')
 
     output_map = {k: v for k, v in zip(return_elements, output_tensors)}
     new_init_op_name = output_map.pop(orig_init_op_name, None)
     return (new_init_op_name,
-            graph_utils.assemble_result_from_graph(
+            tensorflow_utils.assemble_result_from_graph(
                 type_spec.result, computation_proto.tensorflow.result,
                 output_map))
```

## tensorflow_federated/python/core/impl/tensorflow_serialization.py

```diff
@@ -14,45 +14,54 @@
 # limitations under the License.
 """Utilities for serializing TensorFlow computations."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-import inspect
+import os
+import os.path
 import shutil
+import sys
 import tempfile
 import types
+import zipfile
 
+import six
 import tensorflow as tf
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.common_libs import serialization_utils
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.impl import context_stack_base
-from tensorflow_federated.python.core.impl import function_utils
-from tensorflow_federated.python.core.impl import graph_utils
 from tensorflow_federated.python.core.impl import tf_computation_context
-from tensorflow_federated.python.core.impl import type_serialization
+from tensorflow_federated.python.core.impl.compiler import type_serialization
+from tensorflow_federated.python.core.impl.utils import function_utils
+from tensorflow_federated.python.core.impl.utils import tensorflow_utils
 from tensorflow_federated.python.tensorflow_libs import graph_keys
 
 
+class SerializationError(Exception):
+  """Error raised during value serialization or deserialization."""
+  pass
+
+
 def finalize_binding(binding, tensor_info_map):
   """Mutates binding by filling in actual tensor names.
 
   Args:
     binding: A `pb.Binding` or one of its submessages.
     tensor_info_map: A dict mapping the placeholder `tensor_name`s found in
       `binding` to final tensor names.
   """
   if not binding:
     if tensor_info_map:
-      raise ValueError('Empty binding, but non-empty tensor_info_map {}:\n' +
-                       str(tensor_info_map))
+      raise ValueError('Empty binding, but non-empty tensor_info_map {}'.format(
+          tensor_info_map))
     return
   if isinstance(binding, pb.TensorFlow.Binding):
     sub_binding = getattr(binding, binding.WhichOneof('binding'))
     finalize_binding(sub_binding, tensor_info_map)
 
   elif isinstance(binding, pb.TensorFlow.TensorBinding):
     name = binding.tensor_name
@@ -93,26 +102,26 @@
       parameter type.
   """
   py_typecheck.check_callable(target)
   parameter_type = computation_types.to_type(parameter_type)
   argspec = function_utils.get_argspec(target)
   if argspec.args and parameter_type is None:
     raise ValueError(
-        'Expected the target to declare no parameters, found {}.'.format(
-            repr(argspec.args)))
+        'Expected the target to declare no parameters, found {!r}.'.format(
+            argspec.args))
 
   # In the codepath for TF V1 based serialization (tff.tf_computation),
   # we get the "wrapped" function to serialize. Here, target is the
   # raw function to be wrapped; however, we still need to know if
   # the parameter_type should be unpacked into multiple args and kwargs
   # in order to construct the TensorSpecs to be passed in the call
   # to get_concrete_fn below.
   unpack = function_utils.infer_unpack_needed(target, parameter_type, unpack)
   arg_typespecs, kwarg_typespecs, parameter_binding = (
-      graph_utils.get_tf_typespec_and_binding(
+      tensorflow_utils.get_tf_typespec_and_binding(
           parameter_type, arg_names=argspec.args, unpack=unpack))
 
   # Pseudo-global to be appended to once when target_poly below is traced.
   type_and_binding_slot = []
 
   # N.B. To serialize a tf.function or eager python code,
   # the return type must be a flat list, tuple, or dict. However, the
@@ -124,19 +133,19 @@
   #
   # TODO(b/117428091): The return type limitation is primarily a limitation of
   # SignatureDefs  and therefore of the signatures argument to
   # tf.saved_model.save. tf.functions attached to objects and loaded back with
   # tf.saved_model.load can take/return nests; this might offer a better
   # approach to the one taken here.
 
-  @tf.function(autograph=False)
+  @tf.function
   def target_poly(*args, **kwargs):
     result = target(*args, **kwargs)
     result_dict, result_type, result_binding = (
-        graph_utils.get_tf2_result_dict_and_binding(result))
+        tensorflow_utils.get_tf2_result_dict_and_binding(result))
     assert not type_and_binding_slot
     # A "side channel" python output.
     type_and_binding_slot.append((result_type, result_binding))
     return result_dict
 
   # Triggers tracing so that type_and_binding_slot is filled.
   cc_fn = target_poly.get_concrete_function(*arg_typespecs, **kwarg_typespecs)
@@ -167,16 +176,16 @@
     # to just get the MetaGraphDef directly without saving to a tempfile? This
     # looks like a small change to v2.saved_model.save().
     outdir = tempfile.mkdtemp('savedmodel')
     tf.saved_model.save(saveable, outdir, signatures=cc_fn)
 
     graph = tf.Graph()
     with tf.compat.v1.Session(graph=graph) as sess:
-      mgd = tf.saved_model.loader.load(
-          sess, tags=[tf.saved_model.tag_constants.SERVING], export_dir=outdir)
+      mgd = tf.compat.v1.saved_model.load(
+          sess, tags=[tf.saved_model.SERVING], export_dir=outdir)
   finally:
     shutil.rmtree(outdir)
   sigs = mgd.signature_def
 
   # TODO(b/123102455): Figure out how to support the init_op. The meta graph def
   # contains sigs['__saved_model_init_op'].outputs['__saved_model_init_op']. It
   # probably won't do what we want, because it will want to read from
@@ -240,32 +249,32 @@
   # with keyword args or multiple args corresponding to elements of a tuple.
   # Document all accepted forms with examples in the API, and point to there
   # from here.
 
   py_typecheck.check_type(target, types.FunctionType)
   py_typecheck.check_type(context_stack, context_stack_base.ContextStack)
   parameter_type = computation_types.to_type(parameter_type)
-  argspec = inspect.getargspec(target)  # pylint: disable=deprecated-method
+  argspec = function_utils.get_argspec(target)
 
   with tf.Graph().as_default() as graph:
     args = []
     if parameter_type is not None:
       if len(argspec.args) != 1:
         raise ValueError(
-            'Expected the target to declare exactly one parameter, '
-            'found {}.'.format(repr(argspec.args)))
+            'Expected the target to declare exactly one parameter, found {!r}.'
+            .format(argspec.args))
       parameter_name = argspec.args[0]
-      parameter_value, parameter_binding = graph_utils.stamp_parameter_in_graph(
+      parameter_value, parameter_binding = tensorflow_utils.stamp_parameter_in_graph(
           parameter_name, parameter_type, graph)
       args.append(parameter_value)
     else:
       if argspec.args:
         raise ValueError(
-            'Expected the target to declare no parameters, found {}.'.format(
-                repr(argspec.args)))
+            'Expected the target to declare no parameters, found {!r}.'.format(
+                argspec.args))
       parameter_binding = None
     context = tf_computation_context.TensorFlowComputationContext(graph)
     with context_stack.install(context):
       result = target(*args)
 
       # TODO(b/122081673): This needs to change for TF 2.0. We may also
       # want to allow the person creating a tff.tf_computation to specify
@@ -274,15 +283,15 @@
       # then it is wasteful to initialize them before this.
       #
       # The following is a bit of a work around: the collections below may
       # contain variables more than once, hence we throw into a set. TFF needs
       # to ensure all variables are initialized, but not all variables are
       # always in the collections we expect. tff.learning._KerasModel tries to
       # pull Keras variables (that may or may not be in GLOBAL_VARIABLES) into
-      # TFF_MODEL_VARIABLES for now.
+      # VARS_FOR_TFF_TO_INITIALIZE for now.
       all_variables = set(tf.compat.v1.global_variables() +
                           tf.compat.v1.local_variables() +
                           tf.compat.v1.get_collection(
                               graph_keys.GraphKeys.VARS_FOR_TFF_TO_INITIALIZE))
       if all_variables:
         # Use a readable but not-too-long name for the init_op.
         name = 'init_op_for_' + '_'.join(
@@ -298,22 +307,126 @@
               all_variables, name=name).name
       elif context.init_ops:
         init_op_name = tf.group(
             *context.init_ops, name='subcomputation_init_ops').name
       else:
         init_op_name = None
 
-    result_type, result_binding = graph_utils.capture_result_from_graph(
+    result_type, result_binding = tensorflow_utils.capture_result_from_graph(
         result, graph)
 
   annotated_type = computation_types.FunctionType(parameter_type, result_type)
 
   return pb.Computation(
       type=pb.Type(
           function=pb.FunctionType(
               parameter=type_serialization.serialize_type(parameter_type),
               result=type_serialization.serialize_type(result_type))),
       tensorflow=pb.TensorFlow(
           graph_def=serialization_utils.pack_graph_def(graph.as_graph_def()),
           parameter=parameter_binding,
           result=result_binding,
           initialize_op=init_op_name)), annotated_type
+
+
+# The maximum size allowed for serialized sequence values. Sequence that
+# serialize to values larger than this will result in errors being raised.  This
+# likely occurs when the sequence is dependent on, and thus pulling in, many of
+# variables from the graph.
+DEFAULT_MAX_SERIALIZED_SEQUENCE_SIZE_BYTES = 20 * (1024**2)  # 20 MB
+
+
+# TODO(b/137880330): there is likely opportunity here to share implementation
+# with the serialization happening in
+# `tensorflow_serialization.serialize_tf2_as_tf_computation()`. It would be good
+# to sync with TF team about options for ensuring graph-only (variable-less)
+# serializations.
+def serialize_dataset(
+    dataset,
+    max_serialized_size_bytes=DEFAULT_MAX_SERIALIZED_SEQUENCE_SIZE_BYTES):
+  """Serializes a `tf.data.Dataset` value into a `bytes` object.
+
+  Args:
+    dataset: A `tf.data.Dataset`.
+    max_serialized_size_bytes: An `int` size in bytes designating the threshold
+      on when to raise an error if the resulting serialization is too big.
+
+  Returns:
+    A `bytes` object that can be sent to
+  `tensorflow_serialization.deserialize_dataset` to recover the original
+  `tf.data.Dataset`.
+
+  Raises:
+    SerializationError: if there was an error in TensorFlow during
+      serialization.
+  """
+  py_typecheck.check_type(dataset,
+                          tensorflow_utils.DATASET_REPRESENTATION_TYPES)
+  module = tf.Module()
+  module.dataset = dataset
+  module.dataset_fn = tf.function(lambda: module.dataset, input_signature=())
+
+  temp_dir = tempfile.mkdtemp('dataset')
+  fd, temp_zip = tempfile.mkstemp('zip')
+  os.close(fd)
+  try:
+    tf.saved_model.save(module, temp_dir, signatures={})
+    with zipfile.ZipFile(temp_zip, 'w') as z:
+      for topdir, _, filenames in tf.io.gfile.walk(temp_dir):
+        dest_dir = topdir[len(temp_dir):]
+        for filename in filenames:
+          z.write(
+              os.path.join(topdir, filename), os.path.join(dest_dir, filename))
+    with open(temp_zip, 'rb') as z:
+      zip_bytes = z.read()
+  except Exception as e:  # pylint: disable=broad-except
+    six.reraise(
+        SerializationError,
+        SerializationError('Error serializing tff.Sequence value. '
+                           'Inner error: {!s}'.format(e)),
+        sys.exc_info()[2])
+  finally:
+    tf.io.gfile.rmtree(temp_dir)
+    tf.io.gfile.remove(temp_zip)
+
+  if len(zip_bytes) > max_serialized_size_bytes:
+    raise ValueError('Serialized size of Dataset ({:d} bytes) exceeds maximum '
+                     'allowed ({:d} bytes)'.format(
+                         len(zip_bytes), max_serialized_size_bytes))
+  return zip_bytes
+
+
+def deserialize_dataset(serialized_bytes):
+  """Deserializes a `bytes` object to a `tf.data.Dataset`.
+
+  Args:
+    serialized_bytes: `bytes` object produced by
+      `tensorflow_serialization.serialize_dataset`
+
+  Returns:
+    A `tf.data.Dataset` instance.
+
+  Raises:
+    SerializationError: if there was an error in TensorFlow during
+      serialization.
+  """
+  py_typecheck.check_type(serialized_bytes, bytes)
+  temp_dir = tempfile.mkdtemp('dataset')
+  fd, temp_zip = tempfile.mkstemp('zip')
+  os.close(fd)
+  try:
+    with open(temp_zip, 'wb') as f:
+      f.write(serialized_bytes)
+    with zipfile.ZipFile(temp_zip, 'r') as z:
+      z.extractall(path=temp_dir)
+    loaded = tf.compat.v2.saved_model.load(temp_dir)
+    ds = loaded.dataset_fn()
+  except Exception as e:  # pylint: disable=broad-except
+    six.reraise(
+        SerializationError,
+        SerializationError('Error deserializing tff.Sequence value. '
+                           'Inner error: {!s}'.format(e)),
+        sys.exc_info()[2])
+  finally:
+    tf.io.gfile.rmtree(temp_dir)
+    tf.io.gfile.remove(temp_zip)
+  return ds
```

## tensorflow_federated/python/core/impl/transformations.py

```diff
@@ -24,326 +24,470 @@
 from six.moves import range
 from six.moves import zip
 
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.impl import compiled_computation_transforms
-from tensorflow_federated.python.core.impl import computation_building_block_utils
-from tensorflow_federated.python.core.impl import computation_building_blocks
-from tensorflow_federated.python.core.impl import computation_constructing_utils
-from tensorflow_federated.python.core.impl import context_stack_base
-from tensorflow_federated.python.core.impl import federated_computation_utils
-from tensorflow_federated.python.core.impl import intrinsic_bodies
-from tensorflow_federated.python.core.impl import intrinsic_defs
-from tensorflow_federated.python.core.impl import placement_literals
-from tensorflow_federated.python.core.impl import transformation_utils
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import building_block_analysis
+from tensorflow_federated.python.core.impl.compiler import building_block_factory
+from tensorflow_federated.python.core.impl.compiler import building_blocks
+from tensorflow_federated.python.core.impl.compiler import intrinsic_defs
+from tensorflow_federated.python.core.impl.compiler import transformation_utils
+from tensorflow_federated.python.core.impl.compiler import tree_analysis
+
+
+def _apply_transforms(comp, transforms):
+  """Applies all `transforms` in a single walk of `comp`.
+
+  This function is private for a reason; TFF does not intend to expose the
+  capability to chain arbitrary transformations in this way, since the
+  application of one transformation may cause the resulting AST to violate the
+  assumptions of another. This function should be used quite selectively and
+  considered extensively in order to avoid such subtle issues.
 
+  Args:
+    comp: An instance of `building_blocks.ComputationBuildingBlock` to transform
+      with all elements of `transforms`.
+    transforms: An instance of `transformation_utils.TransformSpec` or iterable
+      thereof, the transformations to apply to `comp`.
 
-def extract_intrinsics(comp):
-  r"""Extracts intrinsics to the scope which binds any variable it depends on.
+  Returns:
+    A transformed version of `comp`, with all transformations in `transforms`
+    applied.
 
-  This transform traverses `comp` postorder, matches the following pattern, and
-  replaces the following computation containing a called intrinsic:
+  Raises:
+    TypeError: If the types don't match.
+  """
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
+  if isinstance(transforms, transformation_utils.TransformSpec):
+    transforms = [transforms]
+  else:
+    for transform in transforms:
+      py_typecheck.check_type(transform, transformation_utils.TransformSpec)
 
-        ...
-           \
-            Call
-           /    \
-  Intrinsic      ...
+  def _transform(comp):
+    modified = False
+    for transform in transforms:
+      comp, transform_modified = transform.transform(comp)
+      modified = modified or transform_modified
+    return comp, modified
 
-  with the following computation containing a block with the extracted called
-  intrinsic:
+  return transformation_utils.transform_postorder(comp, _transform)
 
-                  Block
-                 /     \
-         [x=Call]       ...
-           /    \          \
-  Intrinsic      ...        Ref(x)
-
-  The called intrinsics are extracted to the scope which binds any variable the
-  called intrinsic depends. If the called intrinsic is not bound by any
-  computation in `comp` it will be extracted to the root. Both the
-  `parameter_name` of a `computation_building_blocks.Lambda` and the name of any
-  variable defined by a `computation_building_blocks.Block` can affect the scope
-  in which a reference in called intrinsic is bound.
-
-  NOTE: This function will also extract blocks to the scope in which they are
-  bound because block variables can restrict the scope in which intrinsics are
-  bound.
+
+def remove_lambdas_and_blocks(comp):
+  """Removes any called lambdas and blocks from `comp`.
+
+  This function will rename all the variables in `comp` in a single walk of the
+  AST, then replace called lambdas with blocks in another walk, since this
+  transformation interacts with scope in delicate ways. It will chain inlining
+  the blocks and collapsing the selection-from-tuple pattern together into a
+  final pass.
 
   Args:
-    comp: The computation building block in which to perform the extractions.
-      The names of lambda parameters and block variables in `comp` must be
-      unique.
+    comp: Instance of `building_blocks.ComputationBuildingBlock` from which we
+      want to remove called lambdas and blocks.
 
   Returns:
-    A new computation with the transformation applied or the original `comp`.
+    A transformed version of `comp` which has no called lambdas or blocks, and
+    no extraneous selections from tuples.
+  """
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
+  comp, _ = uniquify_reference_names(comp)
+  comp, _ = replace_called_lambda_with_block(comp)
+  block_inliner = InlineBlock(comp)
+  selection_replacer = ReplaceSelectionFromTuple()
+  transforms = [block_inliner, selection_replacer]
+  symbol_tree = transformation_utils.SymbolTree(
+      transformation_utils.ReferenceCounter)
 
-  Raises:
-    TypeError: If types do not match.
-    ValueError: If `comp` contains variables with non-unique names.
+  def _transform_fn(comp, symbol_tree):
+    """Transform function chaining inlining and collapsing selections.
+
+    This function is inlined here as opposed to factored out and parameterized
+    by the transforms to apply, due to the delicacy of chaining transformations
+    which rely on state. These transformations should be safe if they appear
+    first in the list of transforms, but due to the difficulty of reasoning
+    about the invariants the transforms can rely on in this setting, there is
+    no function exposed which hoists out the internal logic.
+
+    Args:
+      comp: Instance of `building_blocks.ComputationBuildingBlock` we wish to
+        check for inlining and collapsing of selections.
+      symbol_tree: Instance of `building_blocks.SymbolTree` defining the
+        bindings available to `comp`.
+
+    Returns:
+      A transformed version of `comp`.
+    """
+    modified = False
+    for transform in transforms:
+      if transform.global_transform:
+        comp, transform_modified = transform.transform(comp, symbol_tree)
+      else:
+        comp, transform_modified = transform.transform(comp)
+      modified = modified or transform_modified
+    return comp, modified
+
+  return transformation_utils.transform_postorder_with_symbol_bindings(
+      comp, _transform_fn, symbol_tree)
+
+
+class ExtractComputation(transformation_utils.TransformSpec):
+  """Extracts a computation if a variable it depends on is not bound.
+
+  This transforms a computation which matches the `predicate` or is a Block, and
+  replaces the computations with a LET
+  construct if a variable it depends on is not bound by the current scope. Both
+  the `parameter_name` of a `building_blocks.Lambda` and the name of
+  any variable defined by a `building_blocks.Block` can affect the
+  scope in which a reference in computation is bound.
+
+  NOTE: This function extracts `computation_building_block.Block` because block
+  variables can restrict the scope in which computations are bound.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  check_has_unique_names(comp)
-  name_generator = computation_constructing_utils.unique_name_generator(comp)
-  unbound_references = get_map_of_unbound_references(comp)
 
-  def _contains_unbound_reference(comp, names):
+  def __init__(self, comp, predicate):
+    """Constructs a new instance.
+
+    Args:
+      comp: The computation building block in which to perform the extractions.
+        The names of lambda parameters and block variables in `comp` must be
+        unique.
+      predicate: A function that takes a single computation building block as a
+        argument and returns `True` if the computation should be extracted and
+        `False` otherwise.
+
+    Raises:
+      TypeError: If types do not match.
+      ValueError: If `comp` contains variables with non-unique names.
+    """
+    super(ExtractComputation, self).__init__()
+    py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
+    tree_analysis.check_has_unique_names(comp)
+    self._name_generator = building_block_factory.unique_name_generator(comp)
+    self._predicate = predicate
+    self._unbound_references = get_map_of_unbound_references(comp)
+
+  def _contains_unbound_reference(self, comp, names):
     """Returns `True` if `comp` contains unbound references to `names`.
 
-    This function will update the non-local `unbound_references` captured from
+    This function will update the non-local `_unbound_references` captured from
     the parent context if `comp` is not contained in that collection. This can
     happen when new computations are created and added to the AST.
 
     Args:
       comp: The computation building block to test.
       names: A Python string or a list, tuple, or set of Python strings.
     """
     if isinstance(names, six.string_types):
       names = (names,)
-    if comp not in unbound_references:
+    if comp not in self._unbound_references:
       references = get_map_of_unbound_references(comp)
-      unbound_references.update(references)
-    return any(n in unbound_references[comp] for n in names)
+      self._unbound_references.update(references)
+    return any(n in self._unbound_references[comp] for n in names)
 
-  def _is_called_intrinsic_or_block(comp):
-    """Returns `True` if `comp` is a called intrinsic or a block."""
-    return (computation_building_block_utils.is_called_intrinsic(comp) or
-            isinstance(comp, computation_building_blocks.Block))
+  def _passes_test_or_block(self, comp):
+    """Returns `True` if `comp` matches the `predicate` or is a block."""
+    return self._predicate(comp) or isinstance(comp, building_blocks.Block)
 
-  def _should_transform(comp):
+  def should_transform(self, comp):
     """Returns `True` if `comp` should be transformed.
 
     The following `_extract_intrinsic_*` methods all depend on being invoked
-    after `_should_transform` evaluates to `True` for a given `comp`. Because of
+    after `should_transform` evaluates to `True` for a given `comp`. Because of
     this certain assumptions are made:
 
     * transformation functions will transform a given `comp`
     * block variables are guaranteed to not be empty
 
     Args:
       comp: The computation building block in which to test.
     """
-    if isinstance(comp, computation_building_blocks.Block):
-      return (_is_called_intrinsic_or_block(comp.result) or any(
-          isinstance(e, computation_building_blocks.Block)
-          for _, e in comp.locals))
-    elif isinstance(comp, computation_building_blocks.Call):
-      return _is_called_intrinsic_or_block(comp.argument)
-    elif isinstance(comp, computation_building_blocks.Lambda):
-      if computation_building_block_utils.is_called_intrinsic(comp.result):
+    if isinstance(comp, building_blocks.Block):
+      return (self._passes_test_or_block(comp.result) or
+              any(isinstance(e, building_blocks.Block) for _, e in comp.locals))
+    elif isinstance(comp, building_blocks.Call):
+      return (self._passes_test_or_block(comp.function) or
+              self._passes_test_or_block(comp.argument))
+    elif isinstance(comp, building_blocks.Lambda):
+      if self._predicate(comp.result):
         return True
-      if isinstance(comp.result, computation_building_blocks.Block):
+      if isinstance(comp.result, building_blocks.Block):
         for index, (_, variable) in enumerate(comp.result.locals):
           names = [n for n, _ in comp.result.locals[:index]]
-          if (not _contains_unbound_reference(variable, comp.parameter_name) and
-              not _contains_unbound_reference(variable, names)):
+          if (not self._contains_unbound_reference(variable,
+                                                   comp.parameter_name) and
+              not self._contains_unbound_reference(variable, names)):
             return True
-    elif isinstance(comp, computation_building_blocks.Selection):
-      return _is_called_intrinsic_or_block(comp.source)
-    elif isinstance(comp, computation_building_blocks.Tuple):
-      return any(_is_called_intrinsic_or_block(e) for e in comp)
+    elif isinstance(comp, building_blocks.Selection):
+      return self._passes_test_or_block(comp.source)
+    elif isinstance(comp, building_blocks.Tuple):
+      return any(self._passes_test_or_block(e) for e in comp)
     return False
 
-  def _extract_from_block(comp):
+  def _extract_from_block(self, comp):
     """Returns a new computation with all intrinsics extracted."""
-    if computation_building_block_utils.is_called_intrinsic(comp.result):
-      called_intrinsic = comp.result
-      name = six.next(name_generator)
+    if self._predicate(comp.result):
+      name = six.next(self._name_generator)
       variables = comp.locals
-      variables.append((name, called_intrinsic))
-      result = computation_building_blocks.Reference(
-          name, called_intrinsic.type_signature)
-      return computation_building_blocks.Block(variables, result)
-    elif isinstance(comp.result, computation_building_blocks.Block):
-      return computation_building_blocks.Block(comp.locals + comp.result.locals,
-                                               comp.result.result)
+      variables.append((name, comp.result))
+      result = building_blocks.Reference(name, comp.result.type_signature)
+    elif isinstance(comp.result, building_blocks.Block):
+      variables = comp.locals + comp.result.locals
+      result = comp.result.result
     else:
-      variables = []
-      for name, variable in comp.locals:
-        if isinstance(variable, computation_building_blocks.Block):
-          variables.extend(variable.locals)
-          variables.append((name, variable.result))
+      variables = comp.locals
+      result = comp.result
+
+    def _remove_blocks_from_variables(variables):
+      new_variables = []
+      for name, variable in variables:
+        if isinstance(variable, building_blocks.Block):
+          new_variables.extend(variable.locals)
+          new_variables.append((name, variable.result))
         else:
-          variables.append((name, variable))
-      return computation_building_blocks.Block(variables, comp.result)
+          new_variables.append((name, variable))
+      return new_variables
 
-  def _extract_from_call(comp):
+    variables = _remove_blocks_from_variables(variables)
+    return building_blocks.Block(variables, result)
+
+  def _extract_from_call(self, comp):
     """Returns a new computation with all intrinsics extracted."""
-    if computation_building_block_utils.is_called_intrinsic(comp.argument):
-      called_intrinsic = comp.argument
-      name = six.next(name_generator)
-      variables = ((name, called_intrinsic),)
-      result = computation_building_blocks.Reference(
-          name, called_intrinsic.type_signature)
+    variables = []
+    if self._predicate(comp.function):
+      name = six.next(self._name_generator)
+      variables.append((name, comp.function))
+      function = building_blocks.Reference(name, comp.function.type_signature)
+    elif isinstance(comp.function, building_blocks.Block):
+      block = comp.function
+      variables.extend(block.locals)
+      function = block.result
     else:
-      block = comp.argument
-      variables = block.locals
-      result = block.result
-    call = computation_building_blocks.Call(comp.function, result)
-    block = computation_building_blocks.Block(variables, call)
-    return _extract_from_block(block)
+      function = comp.function
+    if comp.argument is not None:
+      if self._predicate(comp.argument):
+        name = six.next(self._name_generator)
+        variables.append((name, comp.argument))
+        argument = building_blocks.Reference(name, comp.argument.type_signature)
+      elif isinstance(comp.argument, building_blocks.Block):
+        block = comp.argument
+        variables.extend(block.locals)
+        argument = block.result
+      else:
+        argument = comp.argument
+    else:
+      argument = None
+    call = building_blocks.Call(function, argument)
+    block = building_blocks.Block(variables, call)
+    return self._extract_from_block(block)
 
-  def _extract_from_lambda(comp):
+  def _extract_from_lambda(self, comp):
     """Returns a new computation with all intrinsics extracted."""
-    if computation_building_block_utils.is_called_intrinsic(comp.result):
-      called_intrinsic = comp.result
-      name = six.next(name_generator)
-      variables = ((name, called_intrinsic),)
-      ref = computation_building_blocks.Reference(
-          name, called_intrinsic.type_signature)
-      if not _contains_unbound_reference(comp.result, comp.parameter_name):
-        fn = computation_building_blocks.Lambda(comp.parameter_name,
-                                                comp.parameter_type, ref)
-        return computation_building_blocks.Block(variables, fn)
+    if self._predicate(comp.result):
+      name = six.next(self._name_generator)
+      variables = [(name, comp.result)]
+      result = building_blocks.Reference(name, comp.result.type_signature)
+      if not self._contains_unbound_reference(comp.result, comp.parameter_name):
+        fn = building_blocks.Lambda(comp.parameter_name, comp.parameter_type,
+                                    result)
+        block = building_blocks.Block(variables, fn)
+        return self._extract_from_block(block)
       else:
-        block = computation_building_blocks.Block(variables, ref)
-        return computation_building_blocks.Lambda(comp.parameter_name,
-                                                  comp.parameter_type, block)
+        block = building_blocks.Block(variables, result)
+        block = self._extract_from_block(block)
+        return building_blocks.Lambda(comp.parameter_name, comp.parameter_type,
+                                      block)
     else:
       block = comp.result
       extracted_variables = []
       retained_variables = []
       for name, variable in block.locals:
         names = [n for n, _ in retained_variables]
-        if (not _contains_unbound_reference(variable, comp.parameter_name) and
-            not _contains_unbound_reference(variable, names)):
+        if (not self._contains_unbound_reference(variable, comp.parameter_name)
+            and not self._contains_unbound_reference(variable, names)):
           extracted_variables.append((name, variable))
         else:
           retained_variables.append((name, variable))
       if retained_variables:
-        result = computation_building_blocks.Block(retained_variables,
-                                                   block.result)
+        result = building_blocks.Block(retained_variables, block.result)
       else:
         result = block.result
-      fn = computation_building_blocks.Lambda(comp.parameter_name,
-                                              comp.parameter_type, result)
-      block = computation_building_blocks.Block(extracted_variables, fn)
-      return _extract_from_block(block)
+      fn = building_blocks.Lambda(comp.parameter_name, comp.parameter_type,
+                                  result)
+      block = building_blocks.Block(extracted_variables, fn)
+      return self._extract_from_block(block)
 
-  def _extract_from_selection(comp):
+  def _extract_from_selection(self, comp):
     """Returns a new computation with all intrinsics extracted."""
-    if computation_building_block_utils.is_called_intrinsic(comp.source):
-      called_intrinsic = comp.source
-      name = six.next(name_generator)
-      variables = ((name, called_intrinsic),)
-      result = computation_building_blocks.Reference(
-          name, called_intrinsic.type_signature)
+    if self._predicate(comp.source):
+      name = six.next(self._name_generator)
+      variables = [(name, comp.source)]
+      source = building_blocks.Reference(name, comp.source.type_signature)
     else:
       block = comp.source
       variables = block.locals
-      result = block.result
-    selection = computation_building_blocks.Selection(
-        result, name=comp.name, index=comp.index)
-    block = computation_building_blocks.Block(variables, selection)
-    return _extract_from_block(block)
+      source = block.result
+    selection = building_blocks.Selection(
+        source, name=comp.name, index=comp.index)
+    block = building_blocks.Block(variables, selection)
+    return self._extract_from_block(block)
 
-  def _extract_from_tuple(comp):
+  def _extract_from_tuple(self, comp):
     """Returns a new computation with all intrinsics extracted."""
     variables = []
     elements = []
-    for name, element in anonymous_tuple.to_elements(comp):
-      if _is_called_intrinsic_or_block(element):
-        variable_name = six.next(name_generator)
+    for name, element in anonymous_tuple.iter_elements(comp):
+      if self._passes_test_or_block(element):
+        variable_name = six.next(self._name_generator)
         variables.append((variable_name, element))
-        ref = computation_building_blocks.Reference(variable_name,
-                                                    element.type_signature)
+        ref = building_blocks.Reference(variable_name, element.type_signature)
         elements.append((name, ref))
       else:
         elements.append((name, element))
-    tup = computation_building_blocks.Tuple(elements)
-    block = computation_building_blocks.Block(variables, tup)
-    return _extract_from_block(block)
+    tup = building_blocks.Tuple(elements)
+    block = building_blocks.Block(variables, tup)
+    return self._extract_from_block(block)
 
-  def _transform(comp):
+  def transform(self, comp):
     """Returns a new transformed computation or `comp`."""
-    if not _should_transform(comp):
+    if not self.should_transform(comp):
       return comp, False
-    if isinstance(comp, computation_building_blocks.Block):
-      comp = _extract_from_block(comp)
-    elif isinstance(comp, computation_building_blocks.Call):
-      comp = _extract_from_call(comp)
-    elif isinstance(comp, computation_building_blocks.Lambda):
-      comp = _extract_from_lambda(comp)
-    elif isinstance(comp, computation_building_blocks.Selection):
-      comp = _extract_from_selection(comp)
-    elif isinstance(comp, computation_building_blocks.Tuple):
-      comp = _extract_from_tuple(comp)
+    if isinstance(comp, building_blocks.Block):
+      comp = self._extract_from_block(comp)
+    elif isinstance(comp, building_blocks.Call):
+      comp = self._extract_from_call(comp)
+    elif isinstance(comp, building_blocks.Lambda):
+      comp = self._extract_from_lambda(comp)
+    elif isinstance(comp, building_blocks.Selection):
+      comp = self._extract_from_selection(comp)
+    elif isinstance(comp, building_blocks.Tuple):
+      comp = self._extract_from_tuple(comp)
     return comp, True
 
-  return transformation_utils.transform_postorder(comp, _transform)
 
+def extract_computations(comp):
+  """Extracts computations to the scope which binds a variable it depends on.
 
-def inline_block_locals(comp, variable_names=None):
-  """Inlines the block variables in `comp` whitelisted by `variable_names`.
+  NOTE: If a computation does not contain a variable that is bound by a
+  computation in `comp` it will be extracted to the root.
 
   Args:
-    comp: The computation building block in which to perform the extractions.
-      The names of lambda parameters and block variables in `comp` must be
-      unique.
-    variable_names: A Python list, tuple, or set representing the whitelist of
-      variable names to inline; or None if all variables should be inlined.
+    comp: The computation building block in which to perform the transformation.
 
   Returns:
     A new computation with the transformation applied or the original `comp`.
+  """
 
-  Raises:
-    ValueError: If `comp` contains variables with non-unique names.
+  def _predicate(comp):
+    return not isinstance(comp, building_blocks.Reference)
+
+  return _apply_transforms(comp, ExtractComputation(comp, _predicate))
+
+
+def extract_intrinsics(comp):
+  """Extracts intrinsics to the scope which binds a variable it depends on.
+
+  NOTE: If an intrinsic does not contain a variable that is bound by a
+  computation in `comp` it will be extracted to the root.
+
+  Args:
+    comp: The computation building block in which to perform the transformation.
+
+  Returns:
+    A new computation with the transformation applied or the original `comp`.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  check_has_unique_names(comp)
-  if variable_names is not None:
-    py_typecheck.check_type(variable_names, (list, tuple, set))
 
-  def _should_inline_variable(name):
-    return variable_names is None or name in variable_names
+  def _predicate(comp):
+    return building_block_analysis.is_called_intrinsic(comp)
 
-  def _should_transform(comp):
-    return ((isinstance(comp, computation_building_blocks.Reference) and
-             _should_inline_variable(comp.name)) or
-            (isinstance(comp, computation_building_blocks.Block) and
-             any(_should_inline_variable(name) for name, _ in comp.locals)))
+  return _apply_transforms(comp, ExtractComputation(comp, _predicate))
 
-  def _transform(comp, symbol_tree):
-    """Returns a new transformed computation or `comp`."""
-    if not _should_transform(comp):
+
+class InlineBlock(transformation_utils.TransformSpec):
+  """Inlines the block variables in `comp` whitelisted by `variable_names`.
+
+  Each invocation of the `transform` method checks for presence of a
+  block-bound `building_blocks.Reference`, and inlines this
+  reference with its appropriate value.
+  """
+
+  def __init__(self, comp, variable_names=None):
+    """Initializes the block inliner.
+
+    Checks that `comp` has unique names, and that `variable_names` is an
+    iterable of string types.
+
+    Args:
+      comp: The top-level computation to inline.
+      variable_names: The variable names to inline. If `None`, inlines all
+        variables.
+
+    Raises:
+      ValueError: If `comp` contains variables with non-unique names.
+      TypeError: If `variable_names` is a non-`list`, `set` or `tuple`, or
+        contains anything other than strings.
+    """
+    super(InlineBlock, self).__init__(global_transform=True)
+    py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
+    tree_analysis.check_has_unique_names(comp)
+    if variable_names is not None:
+      py_typecheck.check_type(variable_names, (list, tuple, set))
+      for name in variable_names:
+        py_typecheck.check_type(name, six.string_types)
+    self._variable_names = variable_names
+
+  def _should_inline_variable(self, name):
+    return self._variable_names is None or name in self._variable_names
+
+  def should_transform(self, comp):
+    return ((isinstance(comp, building_blocks.Reference) and
+             self._should_inline_variable(comp.name)) or
+            (isinstance(comp, building_blocks.Block) and any(
+                self._should_inline_variable(name) for name, _ in comp.locals)))
+
+  def transform(self, comp, symbol_tree):
+    if not self.should_transform(comp):
       return comp, False
-    if isinstance(comp, computation_building_blocks.Reference):
+    if isinstance(comp, building_blocks.Reference):
       try:
         value = symbol_tree.get_payload_with_name(comp.name).value
       except NameError:
         # This reference is unbound
         value = None
       # This identifies a variable bound by a Block as opposed to a Lambda.
       if value is not None:
         return value, True
       return comp, False
-    elif isinstance(comp, computation_building_blocks.Block):
+    elif isinstance(comp, building_blocks.Block):
       variables = [(name, value)
                    for name, value in comp.locals
-                   if not _should_inline_variable(name)]
+                   if not self._should_inline_variable(name)]
       if not variables:
         comp = comp.result
       else:
-        comp = computation_building_blocks.Block(variables, comp.result)
+        comp = building_blocks.Block(variables, comp.result)
       return comp, True
     return comp, False
 
+
+def inline_block_locals(comp, variable_names=None):
+  """Inlines the block variables in `comp` whitelisted by `variable_names`."""
   symbol_tree = transformation_utils.SymbolTree(
       transformation_utils.ReferenceCounter)
+  transform_spec = InlineBlock(comp, variable_names)
   return transformation_utils.transform_postorder_with_symbol_bindings(
-      comp, _transform, symbol_tree)
+      comp, transform_spec.transform, symbol_tree)
 
 
-def merge_chained_blocks(comp):
-  r"""Merges all the chained blocks in `comp` into one block.
+class MergeChainedBlocks(transformation_utils.TransformSpec):
+  r"""Merges chained blocks into one block.
 
   Looks for occurrences of the following pattern:
 
         Block
        /     \
   [...]       Block
              /     \
@@ -351,48 +495,45 @@
 
   And merges them to
 
         Block
        /     \
   [...]       Comp(x)
 
-  Preserving the relative ordering of any locals declarations in a postorder
-  walk, which therefore preserves scoping rules.
+  Preserving the relative ordering of any locals declarations, which preserves
+  scoping rules.
 
   Notice that because TFF Block constructs bind their variables in sequence, it
   is completely safe to add the locals lists together in this implementation,
-
-  Args:
-    comp: The computation building block in which to perform the merges.
-
-  Returns:
-    Transformed version of `comp` with its neighboring blocks merged.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
 
-  def _should_transform(comp):
-    return (isinstance(comp, computation_building_blocks.Block) and
-            isinstance(comp.result, computation_building_blocks.Block))
+  def should_transform(self, comp):
+    """Returns `True` if `comp` is a block and its result is a block."""
+    return (isinstance(comp, building_blocks.Block) and
+            isinstance(comp.result, building_blocks.Block))
 
-  def _transform(comp):
-    if not _should_transform(comp):
+  def transform(self, comp):
+    """Returns a new transformed computation or `comp`."""
+    if not self.should_transform(comp):
       return comp, False
-    transformed_comp = computation_building_blocks.Block(
-        comp.locals + comp.result.locals, comp.result.result)
-    return transformed_comp, True
+    comp = building_blocks.Block(comp.locals + comp.result.locals,
+                                 comp.result.result)
+    return comp, True
 
-  return transformation_utils.transform_postorder(comp, _transform)
+
+def merge_chained_blocks(comp):
+  """Merges chained blocks into one block."""
+  return _apply_transforms(comp, MergeChainedBlocks())
 
 
-def merge_chained_federated_maps_or_applys(comp):
-  r"""Merges all the chained federated maps or federated apply in `comp`.
+class MergeChainedFederatedMapsOrApplys(transformation_utils.TransformSpec):
+  r"""Merges chained federated maps or federated apply into one structure.
 
-  This transform traverses `comp` postorder, matches the following pattern, and
-  replaces the following computation containing two federated map intrinsics:
+  This transform matches the following pattern, and replaces the following
+  computation containing two federated map intrinsics:
 
             Call
            /    \
   Intrinsic      Tuple
                  |
                  [Comp(x), Call]
                           /    \
@@ -422,111 +563,109 @@
                                  /
                           Ref(fn)
 
   intrinsic(<(let fn=<y, x> in (arg -> fn[1](fn[0](arg)))), z>)
 
   The functional computations `x` and `y`, and the argument `z` are retained;
   the other computations are replaced.
+  """
 
-  Args:
-    comp: The computation building block in which to perform the merges.
+  def __init__(self, comp):
+    """Constructs a new instance.
 
-  Returns:
-    A new computation with the transformation applied or the original `comp`.
+    Args:
+      comp: The computation building block in which to perform the merges.
 
-  Raises:
-    TypeError: If types do not match.
-  """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  name_generator = computation_constructing_utils.unique_name_generator(comp)
+    Raises:
+      TypeError: If types do not match.
+    """
+    super(MergeChainedFederatedMapsOrApplys, self).__init__()
+    py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
+    self._name_generator = building_block_factory.unique_name_generator(comp)
 
-  def _should_transform(comp):
+  def should_transform(self, comp):
     """Returns `True` if `comp` is a chained federated map."""
-    if computation_building_block_utils.is_called_intrinsic(
-        comp, (
-            intrinsic_defs.FEDERATED_APPLY.uri,
-            intrinsic_defs.FEDERATED_MAP.uri,
-        )):
+    if building_block_analysis.is_called_intrinsic(comp, (
+        intrinsic_defs.FEDERATED_APPLY.uri,
+        intrinsic_defs.FEDERATED_MAP.uri,
+    )):
       outer_arg = comp.argument[1]
-      if computation_building_block_utils.is_called_intrinsic(
-          outer_arg, comp.function.uri):
+      if building_block_analysis.is_called_intrinsic(outer_arg,
+                                                     comp.function.uri):
         return True
     return False
 
-  def _transform(comp):
-    """Returns a new transformed computation or `comp`."""
-    if not _should_transform(comp):
-      return comp, False
+  def _create_block_to_chained_calls(self, comps):
+    r"""Constructs a transformed block computation from `comps`.
 
-    def _create_block_to_chained_calls(comps):
-      r"""Constructs a transformed block computation from `comps`.
+                   Block
+                  /     \
+        [fn=Tuple]       Lambda(arg)
+            |                       \
+    [Comp(y), Comp(x)]               Call
+                                    /    \
+                              Sel(1)      Call
+                             /           /    \
+                      Ref(fn)      Sel(0)      Ref(arg)
+                                  /
+                           Ref(fn)
 
-                     Block
-                    /     \
-          [fn=Tuple]       Lambda(arg)
-              |                       \
-      [Comp(y), Comp(x)]               Call
-                                      /    \
-                                Sel(1)      Call
-                               /           /    \
-                        Ref(fn)      Sel(0)      Ref(arg)
-                                    /
-                             Ref(fn)
-
-      (let fn=<y, x> in (arg -> fn[1](fn[0](arg)))
-
-      Args:
-        comps: A Python list of computations.
-
-      Returns:
-        A `computation_building_blocks.Block`.
-      """
-      functions = computation_building_blocks.Tuple(comps)
-      functions_name = six.next(name_generator)
-      functions_ref = computation_building_blocks.Reference(
-          functions_name, functions.type_signature)
-      arg_name = six.next(name_generator)
-      arg_type = comps[0].type_signature.parameter
-      arg_ref = computation_building_blocks.Reference(arg_name, arg_type)
-      arg = arg_ref
-      for index, _ in enumerate(comps):
-        fn_sel = computation_building_blocks.Selection(
-            functions_ref, index=index)
-        call = computation_building_blocks.Call(fn_sel, arg)
-        arg = call
-      fn = computation_building_blocks.Lambda(arg_ref.name,
-                                              arg_ref.type_signature, call)
-      return computation_building_blocks.Block(
-          ((functions_ref.name, functions),), fn)
+    (let fn=<y, x> in (arg -> fn[1](fn[0](arg)))
+
+    Args:
+      comps: A Python list of computations.
 
-    block = _create_block_to_chained_calls((
+    Returns:
+      A `building_blocks.Block`.
+    """
+    functions = building_blocks.Tuple(comps)
+    functions_name = six.next(self._name_generator)
+    functions_ref = building_blocks.Reference(functions_name,
+                                              functions.type_signature)
+    arg_name = six.next(self._name_generator)
+    arg_type = comps[0].type_signature.parameter
+    arg_ref = building_blocks.Reference(arg_name, arg_type)
+    arg = arg_ref
+    for index, _ in enumerate(comps):
+      fn_sel = building_blocks.Selection(functions_ref, index=index)
+      call = building_blocks.Call(fn_sel, arg)
+      arg = call
+    fn = building_blocks.Lambda(arg_ref.name, arg_ref.type_signature, call)
+    return building_blocks.Block(((functions_ref.name, functions),), fn)
+
+  def transform(self, comp):
+    """Returns a new transformed computation or `comp`."""
+    if not self.should_transform(comp):
+      return comp, False
+    block = self._create_block_to_chained_calls((
         comp.argument[1].argument[0],
         comp.argument[0],
     ))
-    arg = computation_building_blocks.Tuple([
+    arg = building_blocks.Tuple([
         block,
         comp.argument[1].argument[1],
     ])
     intrinsic_type = computation_types.FunctionType(
         arg.type_signature, comp.function.type_signature.result)
-    intrinsic = computation_building_blocks.Intrinsic(comp.function.uri,
-                                                      intrinsic_type)
-    transformed_comp = computation_building_blocks.Call(intrinsic, arg)
-    return transformed_comp, True
+    intrinsic = building_blocks.Intrinsic(comp.function.uri, intrinsic_type)
+    comp = building_blocks.Call(intrinsic, arg)
+    return comp, True
 
-  return transformation_utils.transform_postorder(comp, _transform)
 
+def merge_chained_federated_maps_or_applys(comp):
+  """Merges chained federated maps or federated apply into one structure."""
+  return _apply_transforms(comp, MergeChainedFederatedMapsOrApplys(comp))
 
-def merge_tuple_intrinsics(comp, uri):
-  r"""Merges all the tuples of intrinsics in `comp` into one intrinsic.
 
-  This transform traverses `comp` postorder, matches the following pattern, and
-  replaces the following computation containing a tuple of called intrinsics all
-  represeting the same operation:
+class MergeTupleIntrinsics(transformation_utils.TransformSpec):
+  r"""Merges a tuple of called intrinsics into one called intrinsic.
+
+  This transform matches the following pattern, and replaces the following
+  computation containing a tuple of called intrinsics all represeting the same
+  operation:
 
            Tuple
            |
            [Call,                        Call, ...]
            /    \                       /    \
   Intrinsic      Tuple         Intrinsic      Tuple
                  |                            |
@@ -566,113 +705,115 @@
 
   This transformation is implemented to match the following intrinsics:
 
   * intrinsic_defs.FEDERATED_AGGREGATE.uri
   * intrinsic_defs.FEDERATED_APPLY.uri
   * intrinsic_defs.FEDERATED_BROADCAST.uri
   * intrinsic_defs.FEDERATED_MAP.uri
+  """
 
-  Args:
-    comp: The computation building block in which to perform the merges.
-    uri: The URI of the intrinsic to merge.
-
-  Returns:
-    A new computation with the transformation applied or the original `comp`.
+  def __init__(self, comp, uri):
+    """Constructs a new instance.
 
-  Raises:
-    TypeError: If types do not match.
-  """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(uri, six.string_types)
-  expected_uri = (
-      intrinsic_defs.FEDERATED_AGGREGATE.uri,
-      intrinsic_defs.FEDERATED_APPLY.uri,
-      intrinsic_defs.FEDERATED_BROADCAST.uri,
-      intrinsic_defs.FEDERATED_MAP.uri,
-  )
-  if uri not in expected_uri:
-    raise ValueError(
-        'The value of `uri` is expected to be on of {}, found {}'.format(
-            expected_uri, uri))
-  name_generator = computation_constructing_utils.unique_name_generator(comp)
+    Args:
+      comp: The computation building block in which to perform the merges.
+      uri: The URI of the intrinsic to merge.
 
-  def _should_transform(comp):
-    return (isinstance(comp, computation_building_blocks.Tuple) and
-            comp and computation_building_block_utils.is_called_intrinsic(
-                comp[0], uri) and all(
-                    computation_building_block_utils.is_called_intrinsic(
-                        element, comp[0].function.uri) for element in comp))
+    Raises:
+      TypeError: If types do not match.
+      ValueError: If the `uri` has an unexpected value.
+    """
+    super(MergeTupleIntrinsics, self).__init__()
+    py_typecheck.check_type(uri, six.string_types)
+    self._name_generator = building_block_factory.unique_name_generator(comp)
+    expected_uri = (
+        intrinsic_defs.FEDERATED_AGGREGATE.uri,
+        intrinsic_defs.FEDERATED_APPLY.uri,
+        intrinsic_defs.FEDERATED_BROADCAST.uri,
+        intrinsic_defs.FEDERATED_MAP.uri,
+    )
+    if uri not in expected_uri:
+      raise ValueError(
+          'The value of `uri` is expected to be on of {}, found {}'.format(
+              expected_uri, uri))
+    self._uri = uri
+
+  def should_transform(self, comp):
+    return (isinstance(comp, building_blocks.Tuple) and comp and
+            building_block_analysis.is_called_intrinsic(comp[0], self._uri) and
+            all(
+                building_block_analysis.is_called_intrinsic(
+                    element, comp[0].function.uri) for element in comp))
 
-  def _transform_args_with_type(comps, type_signature):
+  def _transform_args_with_type(self, comps, type_signature):
     """Transforms a Python `list` of computations.
 
     Given a computation containing `n` called intrinsics with `m` arguments,
     this function takes a Python `list` of computations `comps` containing the
     `m`-th argument from each computation `n` and creates a new computation
     representing th `m`-th arguments that should be passed to the called
     intrinsic of the transformed computation.
 
     Args:
       comps: A Python list of computations.
       type_signature: The type to use when determining how to transform the
         computations.
 
     Returns:
-      A `computation_building_blocks.Block`.
+      A `building_blocks.Block`.
     """
     if isinstance(type_signature, computation_types.FederatedType):
-      return _transform_args_with_federated_types(comps, type_signature)
+      return self._transform_args_with_federated_types(comps, type_signature)
     elif isinstance(type_signature, computation_types.FunctionType):
-      return _transform_args_with_functional_types(comps, type_signature)
+      return self._transform_args_with_functional_types(comps, type_signature)
     elif isinstance(type_signature, computation_types.AbstractType):
-      return _transform_args_with_abstract_types(comps, type_signature)
+      return self._transform_args_with_abstract_types(comps, type_signature)
     else:
       raise TypeError(
           'Expected a FederatedType, FunctionalType, or an AbstractType, '
           'found: {}'.format(type(type_signature)))
 
-  def _transform_args_with_abstract_types(comps, type_signature):
+  def _transform_args_with_abstract_types(self, comps, type_signature):
     r"""Transforms a Python `list` of computations with abstract types.
 
     Tuple
     |
     [Comp, Comp, ...]
 
     Args:
       comps: A Python list of computations.
       type_signature: The type to use when determining how to transform the
         computations.
 
     Returns:
-      A `computation_building_blocks.Tuple`.
+      A `building_blocks.Tuple`.
     """
     del type_signature  # Unused
-    return computation_building_blocks.Tuple(comps)
+    return building_blocks.Tuple(comps)
 
-  def _transform_args_with_federated_types(comps, type_signature):
+  def _transform_args_with_federated_types(self, comps, type_signature):
     r"""Transforms a Python `list` of computations with federated types.
 
     federated_zip(Tuple)
                   |
                   [Comp, Comp, ...]
 
     Args:
       comps: A Python list of computations.
       type_signature: The type to use when determining how to transform the
         computations.
 
     Returns:
-      A `computation_building_blocks.Block`.
+      A `building_blocks.Block`.
     """
     del type_signature  # Unused
-    values = computation_building_blocks.Tuple(comps)
-    return computation_constructing_utils.create_federated_zip(values)
+    values = building_blocks.Tuple(comps)
+    return building_block_factory.create_federated_zip(values)
 
-  def _transform_args_with_functional_types(comps, type_signature):
+  def _transform_args_with_functional_types(self, comps, type_signature):
     r"""Transforms a Python `list` of computations with functional types.
 
                     Block
                    /     \
          [fn=Tuple]       Lambda(arg)
              |                       \
     [Comp(f1), Comp(f2), ...]         Tuple
@@ -685,101 +826,187 @@
 
     Args:
       comps: a Python list of computations.
       type_signature: The type to use when determining how to transform the
         computations.
 
     Returns:
-      A `computation_building_blocks.Block`.
+      A `building_blocks.Block`.
     """
-    functions = computation_building_blocks.Tuple(comps)
-    fn_name = six.next(name_generator)
-    fn_ref = computation_building_blocks.Reference(fn_name,
-                                                   functions.type_signature)
+    functions = building_blocks.Tuple(comps)
+    fn_name = six.next(self._name_generator)
+    fn_ref = building_blocks.Reference(fn_name, functions.type_signature)
     if isinstance(type_signature.parameter, computation_types.NamedTupleType):
       arg_type = [[] for _ in range(len(type_signature.parameter))]
       for functional_comp in comps:
         named_type_signatures = anonymous_tuple.to_elements(
             functional_comp.type_signature.parameter)
         for index, (_, concrete_type) in enumerate(named_type_signatures):
           arg_type[index].append(concrete_type)
     else:
       arg_type = [e.type_signature.parameter for e in comps]
-    arg_name = six.next(name_generator)
-    arg_ref = computation_building_blocks.Reference(arg_name, arg_type)
+    arg_name = six.next(self._name_generator)
+    arg_ref = building_blocks.Reference(arg_name, arg_type)
     if isinstance(type_signature.parameter, computation_types.NamedTupleType):
-      arg = computation_constructing_utils.create_zip(arg_ref)
+      arg = building_block_factory.create_zip(arg_ref)
     else:
       arg = arg_ref
     elements = []
     for index, functional_comp in enumerate(comps):
-      sel_fn = computation_building_blocks.Selection(fn_ref, index=index)
-      sel_arg = computation_building_blocks.Selection(arg, index=index)
-      call = computation_building_blocks.Call(sel_fn, sel_arg)
+      sel_fn = building_blocks.Selection(fn_ref, index=index)
+      sel_arg = building_blocks.Selection(arg, index=index)
+      call = building_blocks.Call(sel_fn, sel_arg)
       elements.append(call)
-    calls = computation_building_blocks.Tuple(elements)
-    result = computation_building_blocks.Lambda(arg_ref.name,
-                                                arg_ref.type_signature, calls)
-    return computation_building_blocks.Block(((fn_ref.name, functions),),
-                                             result)
+    calls = building_blocks.Tuple(elements)
+    result = building_blocks.Lambda(arg_ref.name, arg_ref.type_signature, calls)
+    return building_blocks.Block(((fn_ref.name, functions),), result)
 
-  def _transform_args(comp, type_signature):
+  def _transform_args(self, comp, type_signature):
     """Transforms the arguments from `comp`.
 
     Given a computation containing a tuple of intrinsics that can be merged,
     this function creates arguments that should be passed to the call of the
     transformed computation.
 
     Args:
       comp: The computation building block in which to perform the transform.
       type_signature: The type to use when determining how to transform the
         computations.
 
     Returns:
-      A `computation_building_blocks.ComputationBuildingBlock` representing the
+      A `building_blocks.ComputationBuildingBlock` representing the
       transformed arguments from `comp`.
     """
     if isinstance(type_signature, computation_types.NamedTupleType):
       comps = [[] for _ in range(len(type_signature))]
-      for _, call in anonymous_tuple.to_elements(comp):
+      for _, call in anonymous_tuple.iter_elements(comp):
         for index, arg in enumerate(call.argument):
           comps[index].append(arg)
       transformed_args = []
       for args, arg_type in zip(comps, type_signature):
-        transformed_arg = _transform_args_with_type(args, arg_type)
+        transformed_arg = self._transform_args_with_type(args, arg_type)
         transformed_args.append(transformed_arg)
-      return computation_building_blocks.Tuple(transformed_args)
+      return building_blocks.Tuple(transformed_args)
     else:
       args = []
-      for _, call in anonymous_tuple.to_elements(comp):
+      for _, call in anonymous_tuple.iter_elements(comp):
         args.append(call.argument)
-      return _transform_args_with_type(args, type_signature)
+      return self._transform_args_with_type(args, type_signature)
 
-  def _transform(comp):
+  def transform(self, comp):
     """Returns a new transformed computation or `comp`."""
-    if not _should_transform(comp):
+    if not self.should_transform(comp):
       return comp, False
-    intrinsic_def = intrinsic_defs.uri_to_intrinsic_def(uri)
-    arg = _transform_args(comp, intrinsic_def.type_signature.parameter)
+    intrinsic_def = intrinsic_defs.uri_to_intrinsic_def(self._uri)
+    arg = self._transform_args(comp, intrinsic_def.type_signature.parameter)
     named_comps = anonymous_tuple.to_elements(comp)
     parameter_type = computation_types.to_type(arg.type_signature)
     type_signature = [call.type_signature.member for _, call in named_comps]
     result_type = computation_types.FederatedType(
         type_signature, intrinsic_def.type_signature.result.placement,
         intrinsic_def.type_signature.result.all_equal)
     intrinsic_type = computation_types.FunctionType(parameter_type, result_type)
-    intrinsic = computation_building_blocks.Intrinsic(uri, intrinsic_type)
-    call = computation_building_blocks.Call(intrinsic, arg)
-    tup = computation_constructing_utils.create_federated_unzip(call)
+    intrinsic = building_blocks.Intrinsic(self._uri, intrinsic_type)
+    call = building_blocks.Call(intrinsic, arg)
+    tup = building_block_factory.create_federated_unzip(call)
     names = [name for name, _ in named_comps]
-    transformed_comp = computation_constructing_utils.create_named_tuple(
-        tup, names)
+    transformed_comp = building_block_factory.create_named_tuple(tup, names)
     return transformed_comp, True
 
-  return transformation_utils.transform_postorder(comp, _transform)
+
+def merge_tuple_intrinsics(comp, uri):
+  r"""Merges tuples of called intrinsics into one called intrinsic."""
+  return _apply_transforms(comp, MergeTupleIntrinsics(comp, uri))
+
+
+def remove_duplicate_computations(comp):
+  r"""Removes duplicated computations from `comp`.
+
+  This transform traverses `comp` postorder and remove duplicated computation
+  building blocks from `comp`. Additionally, Blocks variables whose value is a
+  Reference and References pointing to References are removed.
+
+  Args:
+    comp: The computation building block in which to perform the removals.
+
+  Returns:
+    A new computation with the transformation applied or the original `comp`.
+
+  Raises:
+    TypeError: If types do not match.
+  """
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
+  tree_analysis.check_has_unique_names(comp)
+
+  def _should_transform(comp):
+    """Returns `True` if `comp` should be transformed."""
+    return (isinstance(comp, building_blocks.Block) or
+            isinstance(comp, building_blocks.Reference))
+
+  def _transform(comp, symbol_tree):
+    """Returns a new transformed computation or `comp`."""
+    if not _should_transform(comp):
+      return comp, False
+    if isinstance(comp, building_blocks.Block):
+      variables = []
+      for name, value in comp.locals:
+        symbol_tree.walk_down_one_variable_binding()
+        payload = symbol_tree.get_payload_with_name(name)
+        if (not payload.removed and
+            not isinstance(value, building_blocks.Reference)):
+          variables.append((name, value))
+      if not variables:
+        comp = comp.result
+      else:
+        comp = building_blocks.Block(variables, comp.result)
+      return comp, True
+    elif isinstance(comp, building_blocks.Reference):
+      value = symbol_tree.get_payload_with_name(comp.name).value
+      if value is None:
+        return comp, False
+      while isinstance(value, building_blocks.Reference):
+        new_value = symbol_tree.get_payload_with_name(value.name).value
+        if new_value is None:
+          comp = building_blocks.Reference(value.name, value.type_signature)
+          return comp, True
+        else:
+          value = new_value
+      payloads_with_value = symbol_tree.get_all_payloads_with_value(
+          value, _computations_equal)
+      if payloads_with_value:
+        highest_payload = payloads_with_value[-1]
+        lower_payloads = payloads_with_value[:-1]
+        for payload in lower_payloads:
+          symbol_tree.update_payload_with_name(payload.name)
+        comp = building_blocks.Reference(highest_payload.name,
+                                         highest_payload.value.type_signature)
+        return comp, True
+    return comp, False
+
+  class TrackRemovedReferences(transformation_utils.BoundVariableTracker):
+    """transformation_utils.SymbolTree node for removing References in ASTs."""
+
+    def __init__(self, name, value):
+      super(TrackRemovedReferences, self).__init__(name, value)
+      self._removed = False
+
+    @property
+    def removed(self):
+      return self._removed
+
+    def update(self, value):
+      self._removed = True
+
+    def __str__(self):
+      return 'Name: {}; value: {}; removed: {}'.format(self.name, self.value,
+                                                       self.removed)
+
+  symbol_tree = transformation_utils.SymbolTree(TrackRemovedReferences)
+  return transformation_utils.transform_postorder_with_symbol_bindings(
+      comp, _transform, symbol_tree)
 
 
 def remove_mapped_or_applied_identity(comp):
   r"""Removes all the mapped or applied identity functions in `comp`.
 
   This transform traverses `comp` postorder, matches the following pattern, and
   removes all the mapped or applied identity fucntions by replacing the
@@ -806,46 +1033,43 @@
 
   Returns:
     A new computation with the transformation applied or the original `comp`.
 
   Raises:
     TypeError: If types do not match.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
 
   def _should_transform(comp):
     """Returns `True` if `comp` is a mapped or applied identity function."""
-    if (isinstance(comp, computation_building_blocks.Call) and
-        isinstance(comp.function, computation_building_blocks.Intrinsic) and
+    if (isinstance(comp, building_blocks.Call) and
+        isinstance(comp.function, building_blocks.Intrinsic) and
         comp.function.uri in (
             intrinsic_defs.FEDERATED_MAP.uri,
             intrinsic_defs.FEDERATED_MAP_ALL_EQUAL.uri,
             intrinsic_defs.FEDERATED_APPLY.uri,
             intrinsic_defs.SEQUENCE_MAP.uri,
         )):
       called_function = comp.argument[0]
-      return computation_building_block_utils.is_identity_function(
-          called_function)
+      return building_block_analysis.is_identity_function(called_function)
     return False
 
   def _transform(comp):
     if not _should_transform(comp):
       return comp, False
     transformed_comp = comp.argument[1]
     return transformed_comp, True
 
   return transformation_utils.transform_postorder(comp, _transform)
 
 
-def replace_called_lambda_with_block(comp):
+class ReplaceCalledLambdaWithBlock(transformation_utils.TransformSpec):
   r"""Replaces all the called lambdas in `comp` with a block.
 
-  This transform traverses `comp` postorder, matches the following pattern, and
-  replaces the following computation containing a called lambda:
+  This transform replaces the following computation containing a called lambda:
 
             Call
            /    \
   Lambda(x)      Comp(y)
            \
             Comp(z)
 
@@ -854,138 +1078,69 @@
   with the following computation containing a block:
 
              Block
             /     \
   [x=Comp(y)]       Comp(z)
 
   let x=y in z
-
-  The functional computation `b` and the argument `c` are retained; the other
-  computations are replaced. This transformation is used to facilitate the
-  merging of TFF orchestration logic, in particular to remove unnecessary lambda
-  expressions and as a stepping stone for merging Blocks together.
-
-  Args:
-    comp: The computation building block in which to perform the replacements.
-
-  Returns:
-    A new computation with the transformation applied or the original `comp`.
-
-  Raises:
-    TypeError: If types do not match.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
 
-  def _should_transform(comp):
-    return (isinstance(comp, computation_building_blocks.Call) and
-            isinstance(comp.function, computation_building_blocks.Lambda))
+  def should_transform(self, comp):
+    return (isinstance(comp, building_blocks.Call) and
+            isinstance(comp.function, building_blocks.Lambda))
 
-  def _transform(comp):
-    if not _should_transform(comp):
+  def transform(self, comp):
+    if not self.should_transform(comp):
       return comp, False
-    transformed_comp = computation_building_blocks.Block(
+    transformed_comp = building_blocks.Block(
         [(comp.function.parameter_name, comp.argument)], comp.function.result)
     return transformed_comp, True
 
-  return transformation_utils.transform_postorder(comp, _transform)
-
-
-def replace_intrinsic_with_callable(comp, uri, body, context_stack):
-  """Replaces all the intrinsics with the given `uri` with a callable.
-
-  This transform traverses `comp` postorder and replaces all the intrinsics with
-  the given `uri` with a polymorphic callable that represents the body of the
-  implementation of the intrinsic; i.e., one that given the parameter of the
-  intrinsic constructs the intended result. This will typically be a Python
-  function decorated with `@federated_computation` to make it into a polymorphic
-  callable.
-
-  Args:
-    comp: The computation building block in which to perform the replacements.
-    uri: The URI of the intrinsic to replace.
-    body: A polymorphic callable.
-    context_stack: The context stack to use.
-
-  Returns:
-    A new computation with the transformation applied or the original `comp`.
 
-  Raises:
-    TypeError: If types do not match.
-  """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(uri, six.string_types)
-  py_typecheck.check_type(context_stack, context_stack_base.ContextStack)
-  if not callable(body):
-    raise TypeError('The body of the intrinsic must be a callable.')
-
-  def _should_transform(comp):
-    return (isinstance(comp, computation_building_blocks.Intrinsic) and
-            comp.uri == uri and
-            isinstance(comp.type_signature, computation_types.FunctionType))
-
-  def _transform(comp):
-    if not _should_transform(comp):
-      return comp, False
-    # We need 'wrapped_body' to accept exactly one argument.
-    wrapped_body = lambda x: body(x)  # pylint: disable=unnecessary-lambda
-    transformed_comp = federated_computation_utils.zero_or_one_arg_fn_to_building_block(
-        wrapped_body, 'arg', comp.type_signature.parameter, context_stack, uri)
-    return transformed_comp, True
-
-  return transformation_utils.transform_postorder(comp, _transform)
+def replace_called_lambda_with_block(comp):
+  """Replaces all the called lambdas in `comp` with a block."""
+  return _apply_transforms(comp, ReplaceCalledLambdaWithBlock())
 
 
-def replace_selection_from_tuple_with_element(comp):
+class ReplaceSelectionFromTuple(transformation_utils.TransformSpec):
   r"""Replaces any selection from a tuple with the underlying tuple element.
 
-  Replaces any occurences of:
+  Invocations of `transform` replace any occurences of:
 
   Selection
            \
             Tuple
             |
             [Comp, Comp, ...]
 
   with the appropriate Comp, as determined by the `index` or `name` of the
   `Selection`.
-
-  Args:
-    comp: The computation building block in which to perform the replacements.
-
-  Returns:
-    A possibly modified version of comp, without any occurrences of selections
-    from tuples.
-
-  Raises:
-    TypeError: If `comp` is not an instance of
-      `computation_building_blocks.ComputationBuildingBlock`.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
 
-  def _should_transform(comp):
-    return (isinstance(comp, computation_building_blocks.Selection) and
-            isinstance(comp.source, computation_building_blocks.Tuple))
+  def should_transform(self, comp):
+    return (isinstance(comp, building_blocks.Selection) and
+            isinstance(comp.source, building_blocks.Tuple))
 
-  def _get_index_from_name(selection_name, tuple_type_signature):
+  def _get_index_from_name(self, selection_name, tuple_type_signature):
     named_type_signatures = anonymous_tuple.to_elements(tuple_type_signature)
     return [x[0] for x in named_type_signatures].index(selection_name)
 
-  def _transform(comp):
-    if not _should_transform(comp):
+  def transform(self, comp):
+    if not self.should_transform(comp):
       return comp, False
     if comp.name is not None:
-      index = _get_index_from_name(comp.name, comp.source.type_signature)
+      index = self._get_index_from_name(comp.name, comp.source.type_signature)
     else:
       index = comp.index
     return comp.source[index], True
 
-  return transformation_utils.transform_postorder(comp, _transform)
+
+def replace_selection_from_tuple_with_element(comp):
+  """Replaces any selection from a tuple with the underlying tuple element."""
+  return _apply_transforms(comp, ReplaceSelectionFromTuple())
 
 
 def uniquify_compiled_computation_names(comp):
   """Replaces all the compiled computations names in `comp` with unique names.
 
   This transform traverses `comp` postorder and replaces the name of all the
   comiled computations found in `comp` with a unique name.
@@ -995,26 +1150,24 @@
 
   Returns:
     A new computation with the transformation applied or the original `comp`.
 
   Raises:
     TypeError: If types do not match.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  name_generator = computation_constructing_utils.unique_name_generator(
-      None, prefix='')
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
+  name_generator = building_block_factory.unique_name_generator(None, prefix='')
 
   def _should_transform(comp):
-    return isinstance(comp, computation_building_blocks.CompiledComputation)
+    return isinstance(comp, building_blocks.CompiledComputation)
 
   def _transform(comp):
     if not _should_transform(comp):
       return comp, False
-    transformed_comp = computation_building_blocks.CompiledComputation(
+    transformed_comp = building_blocks.CompiledComputation(
         comp.proto, six.next(name_generator))
     return transformed_comp, True
 
   return transformation_utils.transform_postorder(comp, _transform)
 
 
 def uniquify_reference_names(comp):
@@ -1026,17 +1179,16 @@
   Args:
     comp: The computation building block in which to perform the replacements.
 
   Returns:
     Returns a transformed version of comp inside of which all variable names
       are guaranteed to be unique.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  name_generator = computation_constructing_utils.unique_name_generator(None)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
+  name_generator = building_block_factory.unique_name_generator(None)
 
   class _RenameNode(transformation_utils.BoundVariableTracker):
     """transformation_utils.SymbolTree node for renaming References in ASTs."""
 
     def __init__(self, name, value):
       super(_RenameNode, self).__init__(name, value)
       py_typecheck.check_type(name, str)
@@ -1044,49 +1196,48 @@
 
     def __str__(self):
       return 'Value: {}, name: {}, new_name: {}'.format(self.value, self.name,
                                                         self.new_name)
 
   def _transform(comp, context_tree):
     """Renames References in `comp` to unique names."""
-    if isinstance(comp, computation_building_blocks.Reference):
+    if isinstance(comp, building_blocks.Reference):
       try:
         new_name = context_tree.get_payload_with_name(comp.name).new_name
-        return computation_building_blocks.Reference(new_name,
-                                                     comp.type_signature,
-                                                     comp.context), True
+        return building_blocks.Reference(new_name, comp.type_signature,
+                                         comp.context), True
       except NameError:
         return comp, False
-    elif isinstance(comp, computation_building_blocks.Block):
+    elif isinstance(comp, building_blocks.Block):
       new_locals = []
       for name, val in comp.locals:
         context_tree.walk_down_one_variable_binding()
         new_name = context_tree.get_payload_with_name(name).new_name
         new_locals.append((new_name, val))
-      return computation_building_blocks.Block(new_locals, comp.result), True
-    elif isinstance(comp, computation_building_blocks.Lambda):
+      return building_blocks.Block(new_locals, comp.result), True
+    elif isinstance(comp, building_blocks.Lambda):
       context_tree.walk_down_one_variable_binding()
       new_name = context_tree.get_payload_with_name(
           comp.parameter_name).new_name
-      return computation_building_blocks.Lambda(new_name, comp.parameter_type,
-                                                comp.result), True
+      return building_blocks.Lambda(new_name, comp.parameter_type,
+                                    comp.result), True
     return comp, False
 
   symbol_tree = transformation_utils.SymbolTree(_RenameNode)
   return transformation_utils.transform_postorder_with_symbol_bindings(
       comp, _transform, symbol_tree)
 
 
 class TFParser(object):
   """Callable taking subset of TFF AST constructs to CompiledComputations.
 
   When this function is applied via `transformation_utils.transform_postorder`
   to a TFF AST node satisfying its assumptions,  the tree under this node will
   be reduced to a single instance of
-  `computation_building_blocks.CompiledComputation` representing the same
+  `building_blocks.CompiledComputation` representing the same
   logic.
 
   Notice that this function is designed to be applied to what is essentially
   a subtree of a larger TFF AST; once the processing on a single device has
   been aligned at the AST level, and placement separated from the logic of
   this processing, we should be left with a function wrapped via
   `federated_map` or `federated_apply` to a federated argument. It is this
@@ -1101,15 +1252,15 @@
   3. All compiled computations are called.
   4. No compiled computations have been partially called; we believe this
      should be handled correctly today but we haven't reasoned explicitly about
      this possibility.
   5. The only leaf nodes present under `comp` are compiled computations and
      references to the argument of the top-level lambda which we are hoping to
      replace with a compiled computation. Further, every leaf node which is a
-     reference has as its parent a `computation_building_blocks.Call`, whose
+     reference has as its parent a `building_blocks.Call`, whose
      associated function is a TF graph. This prevents us from needing to
      deal with arbitrary nesting of references and TF graphs, and significantly
      clarifies the reasoning. This can be accomplished by "decorating" the
      appropriate leaves with called identity TF graphs, the construction of
      which is provided by a utility module.
   6. There is only a single lambda binding any references present in the AST,
      and it is placed at the root of the AST to which we apply `TFParser`.
@@ -1122,43 +1273,42 @@
   def __init__(self):
     """Populates the parser library with mutually exclusive options."""
     self._parse_library = [
         compiled_computation_transforms.SelectionFromCalledTensorFlowBlock(),
         compiled_computation_transforms.LambdaWrappingGraph(),
         compiled_computation_transforms.TupleCalledGraphs(),
         compiled_computation_transforms.CalledCompositionOfTensorFlowBlocks(),
+        compiled_computation_transforms.CalledGraphOnReplicatedArg(),
     ]
 
   def __call__(self, comp):
     """Transforms `comp` by checking all elements of the parser library.
 
     This function is roughly performing intermediate-code generation, taking
     TFF and generating TF. Calling this function is essentially checking the
     stack and selecting a semantic action based on its contents, and *only one*
     of these actions should be selected for a given computation.
 
     Notice that since the parser library contains mutually exclusive options,
     it is safe to return early.
 
     Args:
-      comp: The `computation_building_blocks.ComputationBuildingBlock` to check
-        for possibility of reduction according to the parsing library.
+      comp: The `building_blocks.ComputationBuildingBlock` to check for
+        possibility of reduction according to the parsing library.
 
     Returns:
       A tuple whose first element is a possibly transformed version of `comp`,
       and whose second is a Boolean indicating whether or not `comp` was
       transformed. This is in conforming to the conventions of
       `transformation_utils.transform_postorder`.
     """
-    py_typecheck.check_type(
-        comp, computation_building_blocks.ComputationBuildingBlock)
+    py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
     for option in self._parse_library:
       if option.should_transform(comp):
-        transformed, ind = option.transform(comp)
-        return transformed, ind
+        return option.transform(comp)
     return comp, False
 
 
 def insert_called_tf_identity_at_leaves(comp):
   r"""Inserts an identity TF graph called on References under `comp`.
 
   For ease of reasoning about and proving completeness of TFF-to-TF
@@ -1182,191 +1332,155 @@
   and nesting of tuples containing references.
 
   `insert_called_tf_identity_at_leaves` ensures that the pattern above is
   present at the leaves of any portion of the TFF AST which is destined to be
   reduced to TF.
 
   We detect such a destiny by checking for the existence of a
-  `computation_building_blocks.Lambda` whose parameter and result type
+  `building_blocks.Lambda` whose parameter and result type
   can both be bound into TensorFlow. This pattern is enforced here as
   parameter validation on `comp`.
 
   Args:
-    comp: Instance of `computation_building_blocks.Lambda` whose AST we will
-      traverse, replacing appropriate instances of
-      `computation_building_blocks.Reference` with graphs representing thei
-      identity function of the appropriate type called on the same reference.
-      `comp` must declare a parameter and result type which are both able to be
-      stamped in to a TensorFlow graph.
+    comp: Instance of `building_blocks.Lambda` whose AST we will traverse,
+      replacing appropriate instances of `building_blocks.Reference` with graphs
+      representing the identity function of the appropriate type called on the
+      same reference. `comp` must declare a parameter and result type which are
+      both able to be stamped in to a TensorFlow graph.
 
   Returns:
     A possibly modified  version of `comp`, where any references now have a
-    parent of type `computation_building_blocks.Call` with function an instance
-    of `computation_building_blocks.CompiledComputation`.
+    parent of type `building_blocks.Call` with function an instance
+    of `building_blocks.CompiledComputation`.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
 
-  if isinstance(comp, computation_building_blocks.CompiledComputation):
+  if isinstance(comp, building_blocks.CompiledComputation):
     return comp, False
 
-  if not (isinstance(comp, computation_building_blocks.Lambda) and
+  if not (isinstance(comp, building_blocks.Lambda) and
           type_utils.is_tensorflow_compatible_type(comp.result.type_signature)
           and type_utils.is_tensorflow_compatible_type(comp.parameter_type)):
     raise ValueError(
         '`insert_called_tf_identity_at_leaves` should only be '
         'called on instances of '
-        '`computation_building_blocks.Lambda` whose parameter '
+        '`building_blocks.Lambda` whose parameter '
         'and result types can both be stamped into TensorFlow '
         'graphs. You have called in on a {} of type signature {}.'.format(
-            computation_building_blocks.compact_representation(comp),
-            comp.type_signature))
+            comp.compact_representation(), comp.type_signature))
 
   def _should_decorate(comp):
-    return (isinstance(comp, computation_building_blocks.Reference) and
+    return (isinstance(comp, building_blocks.Reference) and
             type_utils.is_tensorflow_compatible_type(comp.type_signature))
 
   def _decorate(comp):
-    identity_function = computation_constructing_utils.create_compiled_identity(
+    identity_function = building_block_factory.create_compiled_identity(
         comp.type_signature)
-    return computation_building_blocks.Call(identity_function, comp)
+    return building_blocks.Call(identity_function, comp)
 
   def _decorate_if_reference_without_graph(comp):
     """Decorates references under `comp` if necessary."""
-    if (isinstance(comp, computation_building_blocks.Tuple) and
+    if (isinstance(comp, building_blocks.Tuple) and
         any(_should_decorate(x) for x in comp)):
       elems = []
-      for x in anonymous_tuple.to_elements(comp):
+      for x in anonymous_tuple.iter_elements(comp):
         if _should_decorate(x[1]):
           elems.append((x[0], _decorate(x[1])))
         else:
           elems.append((x[0], x[1]))
-      return computation_building_blocks.Tuple(elems), True
-    elif (isinstance(comp, computation_building_blocks.Call) and not isinstance(
-        comp.function, computation_building_blocks.CompiledComputation) and
+      return building_blocks.Tuple(elems), True
+    elif (isinstance(comp, building_blocks.Call) and
+          not isinstance(comp.function, building_blocks.CompiledComputation) and
           _should_decorate(comp.argument)):
       arg = _decorate(comp.argument)
-      return computation_building_blocks.Call(comp.function, arg), True
-    elif (isinstance(comp, computation_building_blocks.Selection) and
+      return building_blocks.Call(comp.function, arg), True
+    elif (isinstance(comp, building_blocks.Selection) and
           _should_decorate(comp.source)):
-      return computation_building_blocks.Selection(
+      return building_blocks.Selection(
           _decorate(comp.source), name=comp.name, index=comp.index), True
-    elif (isinstance(comp, computation_building_blocks.Lambda) and
+    elif (isinstance(comp, building_blocks.Lambda) and
           _should_decorate(comp.result)):
-      return computation_building_blocks.Lambda(comp.parameter_name,
-                                                comp.parameter_type,
-                                                _decorate(comp.result)), True
-    elif isinstance(comp, computation_building_blocks.Block) and (
+      return building_blocks.Lambda(comp.parameter_name, comp.parameter_type,
+                                    _decorate(comp.result)), True
+    elif isinstance(comp, building_blocks.Block) and (
         any(_should_decorate(x[1]) for x in comp.locals) or
         _should_decorate(comp.result)):
       new_locals = []
       for x in comp.locals:
         if _should_decorate(x[1]):
           new_locals.append((x[0], _decorate(x[1])))
         else:
           new_locals.append((x[0], x[1]))
       new_result = comp.result
       if _should_decorate(comp.result):
         new_result = _decorate(comp.result)
-      return computation_building_blocks.Block(new_locals, new_result), True
+      return building_blocks.Block(new_locals, new_result), True
     return comp, False
 
   return transformation_utils.transform_postorder(
       comp, _decorate_if_reference_without_graph)
 
 
-def check_has_single_placement(comp, single_placement):
-  """Checks that the AST of `comp` contains only `single_placement`.
-
-  Args:
-    comp: Instance of `computation_building_blocks.ComputationBuildingBlock`.
-    single_placement: Instance of `placement_literals.PlacementLiteral` which
-      should be the only placement present under `comp`.
-
-  Raises:
-    ValueError: If the AST under `comp` contains any
-    `computation_types.FederatedType` other than `single_placement`.
-  """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(single_placement, placement_literals.PlacementLiteral)
-
-  def _check_single_placement(comp):
-    """Checks that the placement in `type_spec` matches `single_placement`."""
-    if (isinstance(comp.type_signature, computation_types.FederatedType) and
-        comp.type_signature.placement != single_placement):
-      raise ValueError(
-          'Comp contains a placement other than {}; '
-          'placement {} on comp {} inside the structure. '.format(
-              single_placement, comp.type_signature.placement,
-              computation_building_blocks.compact_representation(comp)))
-    return comp, False
-
-  transformation_utils.transform_postorder(comp, _check_single_placement)
-
-
 def unwrap_placement(comp):
   """Strips `comp`'s placement, returning a single call to map, apply or value.
 
   For this purpose it is necessary to assume that all processing under `comp`
   is happening at a single placement.
 
   The other assumptions on inputs of `unwrap_placement` are enumerated as
   follows:
 
   1. There is at most one unbound reference under `comp`, which is of federated
      type.
   2. The only intrinsics present here are apply or map, zip,
      and federated_value_at_*.
   3. The type signature of `comp` is federated.
-  4. There are no instances of `computation_building_blocks.Data` of federated
+  4. There are no instances of `building_blocks.Data` of federated
      type under `comp`; how these would be handled by a function such as this
      is not entirely clear.
 
   Under these conditions, `unwrap_placement` will produce a single call to
   federated_map, federated_apply or federated_value, depending on the placement
   and type signature of `comp`. Other than this single map or apply, no
   intrinsics will remain under `comp`.
 
   Args:
-    comp: Instance of `computation_building_blocks.ComputationBuildingBlock`
-      satisfying the assumptions above.
+    comp: Instance of `building_blocks.ComputationBuildingBlock` satisfying the
+      assumptions above.
 
   Returns:
     A modified version of `comp`, whose root is a single called
     intrinsic, and containing no other intrinsics. Equivalent
     to `comp`.
 
   Raises:
     TypeError: If the lone unbound reference under `comp` is not of federated
     type, `comp` itself is not of federated type, or `comp` is not a building
     block.
     ValueError: If we encounter a placement other than the one declared by
     `comp.type_signature`, an intrinsic not present in the whitelist above, or
     `comp` contains more than one unbound reference.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(comp.type_signature, computation_types.FederatedType)
   single_placement = comp.type_signature.placement
 
-  check_has_single_placement(comp, single_placement)
+  tree_analysis.check_has_single_placement(comp, single_placement)
 
-  name_generator = computation_constructing_utils.unique_name_generator(comp)
+  name_generator = building_block_factory.unique_name_generator(comp)
 
   all_unbound_references = get_map_of_unbound_references(comp)
   root_unbound_references = all_unbound_references[comp]
 
   if len(root_unbound_references) > 1:
     raise ValueError(
         '`unwrap_placement` can only handle computations with at most a single '
         'unbound reference; you have passed in the computation {} with {} '
-        'unbound references.'.format(
-            computation_building_blocks.compact_representation(comp),
-            len(root_unbound_references)))
+        'unbound references.'.format(comp.compact_representation(),
+                                     len(root_unbound_references)))
 
   if len(root_unbound_references) == 1:
     unbound_reference_name = root_unbound_references.pop()
   else:
     unbound_reference_name = None
 
   def _rename_unbound_variable(comp, unbound_variable_name):
@@ -1374,16 +1488,16 @@
 
     The unique rename is simply to preserve uniqueness of names if this
     property is present in the argument to `unwrap_placement`, since we will
     eventually be binding a new reference of non-federated type in place
     of this federated unbound reference.
 
     Args:
-      comp: Instance of `computation_building_blocks.ComputationBuildingBlock`
-        with at most a single unbound reference.
+      comp: Instance of `building_blocks.ComputationBuildingBlock` with at most
+        a single unbound reference.
       unbound_variable_name: The name of the lone unbound variable present under
         `comp`.
 
     Returns:
       A tuple, whose first element a is possibly transformed version of `comp`
       with its unbound variable renamed to a name which is globally unique
       within `comp`, and its second element a tuple containing the new name
@@ -1403,34 +1517,31 @@
 
       def update(self, x):
         del x  # Unused
         self.unbound = True
 
     symbol_tree = transformation_utils.SymbolTree(_UnboundVariableIdentifier)
     symbol_tree.ingest_variable_binding(unbound_variable_name, None)
-    symbol_tree.update_payload_tracking_reference(
-        computation_building_blocks.Reference(
-            unbound_variable_name, computation_types.AbstractType('T')))
+    symbol_tree.update_payload_with_name(unbound_variable_name)
 
     def _should_transform(comp, symbol_tree):
-      return (isinstance(comp, computation_building_blocks.Reference) and
+      return (isinstance(comp, building_blocks.Reference) and
               comp.name == unbound_variable_name and
               symbol_tree.get_payload_with_name(comp.name).unbound)
 
     def _rename_unbound_variable(comp, symbol_tree):
       """Updates the nonlocal tracker, and renames the unbound variable."""
       if not _should_transform(comp, symbol_tree):
         return comp, False
       if unbound_reference_name_and_type_pair[0][1] is None:
         name = six.next(name_generator)
         unbound_reference_name_and_type_pair[0] = (name, comp.type_signature)
       else:
         name = unbound_reference_name_and_type_pair[0][0]
-      return computation_building_blocks.Reference(name,
-                                                   comp.type_signature), True
+      return building_blocks.Reference(name, comp.type_signature), True
 
     renamed_comp, _ = transformation_utils.transform_postorder_with_symbol_bindings(
         comp, _rename_unbound_variable, symbol_tree)
     return renamed_comp, unbound_reference_name_and_type_pair[0]
 
   def _remove_placement(comp):
     """Unwraps placement from `comp`.
@@ -1442,82 +1553,81 @@
     handle.
 
     One note on the implementation: the four cases in the internal `_transform`
     switch here exactly case for the building blocks which explicitly take type
     signatures as arguments to their constructors.
 
     Args:
-      comp: Instance of `computation_building_blocks.ComputationBuildingBlock`
-        from which we wish to remove placement.
+      comp: Instance of `building_blocks.ComputationBuildingBlock` from which we
+        wish to remove placement.
 
     Returns:
       A transformed version of comp with its placements removed.
 
     Raises:
       NotImplementedError: In case a node of type
-        `computation_building_blocks.Data` is encountered in the AST, as
+        `building_blocks.Data` is encountered in the AST, as
         handling of data objects is not yet implemented in TFF and so it is
         unclear what this function should do in that case.
     """
 
     def _remove_placement_from_type(type_spec):
       if isinstance(type_spec, computation_types.FederatedType):
         return type_spec.member, True
       else:
         return type_spec, False
 
     def _remove_reference_placement(comp):
       """Unwraps placement from references and updates unbound reference info."""
       new_type, _ = type_utils.transform_type_postorder(
           comp.type_signature, _remove_placement_from_type)
-      return computation_building_blocks.Reference(comp.name, new_type)
+      return building_blocks.Reference(comp.name, new_type)
 
     def _replace_intrinsics_with_functions(comp):
       """Helper to remove intrinsics from the AST."""
       if (comp.uri == intrinsic_defs.FEDERATED_ZIP_AT_SERVER.uri or
           comp.uri == intrinsic_defs.FEDERATED_ZIP_AT_CLIENTS.uri or
           comp.uri == intrinsic_defs.FEDERATED_VALUE_AT_SERVER.uri or
           comp.uri == intrinsic_defs.FEDERATED_VALUE_AT_CLIENTS.uri):
         arg_name = six.next(name_generator)
         arg_type = comp.type_signature.result.member
-        val = computation_building_blocks.Reference(arg_name, arg_type)
-        lam = computation_building_blocks.Lambda(arg_name, arg_type, val)
+        val = building_blocks.Reference(arg_name, arg_type)
+        lam = building_blocks.Lambda(arg_name, arg_type, val)
         return lam
       elif comp.uri not in (intrinsic_defs.FEDERATED_MAP.uri,
                             intrinsic_defs.FEDERATED_MAP_ALL_EQUAL.uri,
                             intrinsic_defs.FEDERATED_APPLY.uri):
         raise ValueError('Disallowed intrinsic: {}'.format(comp))
       arg_name = six.next(name_generator)
-      tuple_ref = computation_building_blocks.Reference(arg_name, [
+      tuple_ref = building_blocks.Reference(arg_name, [
           comp.type_signature.parameter[0],
           comp.type_signature.parameter[1].member,
       ])
-      fn = computation_building_blocks.Selection(tuple_ref, index=0)
-      arg = computation_building_blocks.Selection(tuple_ref, index=1)
-      called_fn = computation_building_blocks.Call(fn, arg)
-      return computation_building_blocks.Lambda(arg_name,
-                                                tuple_ref.type_signature,
-                                                called_fn)
+      fn = building_blocks.Selection(tuple_ref, index=0)
+      arg = building_blocks.Selection(tuple_ref, index=1)
+      called_fn = building_blocks.Call(fn, arg)
+      return building_blocks.Lambda(arg_name, tuple_ref.type_signature,
+                                    called_fn)
 
     def _remove_lambda_placement(comp):
       """Removes placement from Lambda's parameter."""
       new_parameter_type, _ = type_utils.transform_type_postorder(
           comp.parameter_type, _remove_placement_from_type)
-      return computation_building_blocks.Lambda(comp.parameter_name,
-                                                new_parameter_type, comp.result)
+      return building_blocks.Lambda(comp.parameter_name, new_parameter_type,
+                                    comp.result)
 
     def _transform(comp):
       """Dispatches to helpers above."""
-      if isinstance(comp, computation_building_blocks.Reference):
+      if isinstance(comp, building_blocks.Reference):
         return _remove_reference_placement(comp), True
-      elif isinstance(comp, computation_building_blocks.Intrinsic):
+      elif isinstance(comp, building_blocks.Intrinsic):
         return _replace_intrinsics_with_functions(comp), True
-      elif isinstance(comp, computation_building_blocks.Lambda):
+      elif isinstance(comp, building_blocks.Lambda):
         return _remove_lambda_placement(comp), True
-      elif (isinstance(comp, computation_building_blocks.Data) and
+      elif (isinstance(comp, building_blocks.Data) and
             isinstance(comp.type_signature, computation_types.FederatedType)):
         # TODO(b/135126947): Design and implement Data constructs.
         raise NotImplementedError
       return comp, False
 
     return transformation_utils.transform_postorder(comp, _transform)
 
@@ -1535,67 +1645,29 @@
       raise TypeError('The lone unbound reference is not of federated type; '
                       'this is disallowed. '
                       'The unbound type is {}'.format(unbound_reference_type))
 
   placement_removed, _ = _remove_placement(unbound_variable_renamed)
 
   if unbound_reference_name is None:
-    return computation_constructing_utils.create_federated_value(
+    return building_block_factory.create_federated_value(
         placement_removed, single_placement), True
 
-  ref_to_fed_arg = computation_building_blocks.Reference(
-      unbound_reference_name, unbound_reference_type)
+  ref_to_fed_arg = building_blocks.Reference(unbound_reference_name,
+                                             unbound_reference_type)
 
-  lambda_wrapping_placement_removal = computation_building_blocks.Lambda(
+  lambda_wrapping_placement_removal = building_blocks.Lambda(
       new_reference_name, unbound_reference_type.member, placement_removed)
 
-  called_intrinsic = computation_constructing_utils.create_federated_map_or_apply(
+  called_intrinsic = building_block_factory.create_federated_map_or_apply(
       lambda_wrapping_placement_removal, ref_to_fed_arg)
 
   return called_intrinsic, True
 
 
-def replace_all_intrinsics_with_bodies(comp, context_stack):
-  """Iterates over all intrinsic bodies, inlining the intrinsics in `comp`.
-
-  Args:
-    comp: Instance of `computation_building_blocks.ComputationBuildingBlock` in
-      which we wish to replace all intrinsics with their bodies.
-    context_stack: Instance of `context_stack_base.ContextStack`, the context
-      stack to use for the bodies of the intrinsics.
-
-  Returns:
-    Instance of `computation_building_blocks.ComputationBuildingBlock` with all
-    the intrinsics from `intrinsic_bodies.py` inlined with their bodies, along
-    with a Boolean indicating whether there was any inlining in fact done.
-
-  Raises:
-    TypeError: If the types don't match.
-  """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(context_stack, context_stack_base.ContextStack)
-  bodies = intrinsic_bodies.get_intrinsic_bodies(context_stack)
-  transformed = False
-  for uri, body in six.iteritems(bodies):
-    comp, uri_found = replace_intrinsic_with_callable(comp, uri, body,
-                                                      context_stack)
-    transformed = transformed or uri_found
-  return comp, transformed
-
-
-def check_has_unique_names(comp):
-  if not transformation_utils.has_unique_names(comp):
-    raise ValueError(
-        'This transform should only be called after we have uniquified all '
-        '`computation_building_blocks.Reference` names, since we may be moving '
-        'computations with unbound references under constructs which bind '
-        'those references.')
-
-
 def get_map_of_unbound_references(comp):
   """Gets a Python `dict` of the unbound references in `comp`.
 
   Compuations that are equal will have the same collections of unbounded
   references, so it is safe to use `comp` as the key for this `dict` even though
   a given compuation may appear in many positions in the AST.
 
@@ -1603,84 +1675,119 @@
     comp: The computation building block to parse.
 
   Returns:
     A Python `dict` of elements where keys are the compuations in `comp` and
     values are a Python `set` of the names of the unbound references in the
     subtree of that compuation.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
   references = {}
 
   def _update(comp):
     """Updates the Python dict of references."""
-    if isinstance(comp, computation_building_blocks.Reference):
+    if isinstance(comp, building_blocks.Reference):
       references[comp] = set((comp.name,))
-    elif isinstance(comp, computation_building_blocks.Block):
+    elif isinstance(comp, building_blocks.Block):
       references[comp] = set()
       names = []
       for name, variable in comp.locals:
         elements = references[variable]
         references[comp].update([e for e in elements if e not in names])
         names.append(name)
       elements = references[comp.result]
       references[comp].update([e for e in elements if e not in names])
-    elif isinstance(comp, computation_building_blocks.Call):
+    elif isinstance(comp, building_blocks.Call):
       elements = references[comp.function]
       if comp.argument is not None:
         elements.update(references[comp.argument])
       references[comp] = elements
-    elif isinstance(comp, computation_building_blocks.Lambda):
+    elif isinstance(comp, building_blocks.Lambda):
       elements = references[comp.result]
       references[comp] = set([e for e in elements if e != comp.parameter_name])
-    elif isinstance(comp, computation_building_blocks.Selection):
+    elif isinstance(comp, building_blocks.Selection):
       references[comp] = references[comp.source]
-    elif isinstance(comp, computation_building_blocks.Tuple):
+    elif isinstance(comp, building_blocks.Tuple):
       elements = [references[e] for e in comp]
       references[comp] = set(itertools.chain.from_iterable(elements))
     else:
       references[comp] = set()
     return comp, False
 
   transformation_utils.transform_postorder(comp, _update)
   return references
 
 
-def check_intrinsics_whitelisted_for_reduction(comp):
-  """Checks whitelist of intrinsics reducible to aggregate or broadcast.
+def _computations_equal(comp_1, comp_2):
+  """Returns `True` if the computations are equal.
+
+  If you pass objects other than instances of
+  `building_blocks.ComputationBuildingBlock` this function will
+  return `False`. Structurally equaivalent computations with different variable
+  names are not considered to be equal.
+
+  NOTE: This function could be quite expensive if you do not
+  `extract_computations` first. Extracting all comptations reduces the equality
+  of two computations in most cases to an identity check. One notable exception
+  to this is `CompiledComputation` for which equality is delegated to the proto
+  object.
 
   Args:
-    comp: Instance of `computation_building_blocks.ComputationBuildingBlock` to
-      check for presence of intrinsics not currently immediately reducible to
-      `FEDERATED_AGGREGATE` or `FEDERATED_BROADCAST`, or local processing.
+    comp_1: A `building_blocks.ComputationBuildingBlock` to test.
+    comp_2: A `building_blocks.ComputationBuildingBlock` to test.
 
   Raises:
-    ValueError: If we encounter an intrinsic under `comp` that is not
-    whitelisted as currently reducible.
+    TypeError: If `comp_1` or `comp_2` is not an instance of
+      `building_blocks.ComputationBuildingBlock`.
+    NotImplementedError: If `comp_1` and `comp_2` are an unexpected subclass of
+      `building_blocks.ComputationBuildingBlock`.
   """
-  # TODO(b/135930668): Factor this and other non-transforms (e.g.
-  # `check_has_unique_names` out of this file into a structure specified for
-  # static analysis of ASTs.
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  uri_whitelist = (
-      intrinsic_defs.FEDERATED_AGGREGATE.uri,
-      intrinsic_defs.FEDERATED_APPLY.uri,
-      intrinsic_defs.FEDERATED_BROADCAST.uri,
-      intrinsic_defs.FEDERATED_MAP.uri,
-      intrinsic_defs.FEDERATED_MAP_ALL_EQUAL.uri,
-      intrinsic_defs.FEDERATED_VALUE_AT_CLIENTS.uri,
-      intrinsic_defs.FEDERATED_VALUE_AT_SERVER.uri,
-      intrinsic_defs.FEDERATED_ZIP_AT_SERVER.uri,
-      intrinsic_defs.FEDERATED_ZIP_AT_CLIENTS.uri,
-  )
-
-  def _check_whitelisted(comp):
-    if isinstance(comp, computation_building_blocks.Intrinsic
-                 ) and comp.uri not in uri_whitelist:
-      raise ValueError(
-          'Encountered an Intrinsic not currently reducible to aggregate or '
-          'broadcast, the intrinsic {}'.format(
-              computation_building_blocks.compact_representation(comp)))
-    return comp, False
-
-  transformation_utils.transform_postorder(comp, _check_whitelisted)
+  py_typecheck.check_type(comp_1, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp_2, building_blocks.ComputationBuildingBlock)
+  if comp_1 is comp_2:
+    return True
+  # The unidiomatic-typecheck is intentional, for the purposes of equality this
+  # function requires that the types are identical and that a subclass will not
+  # be equal to it's baseclass.
+  if type(comp_1) != type(comp_2):  # pylint: disable=unidiomatic-typecheck
+    return False
+  if comp_1.type_signature != comp_2.type_signature:
+    return False
+  if isinstance(comp_1, building_blocks.Block):
+    if not _computations_equal(comp_1.result, comp_2.result):
+      return False
+    if len(comp_1.locals) != len(comp_2.locals):
+      return False
+    for (name_1, value_1), (name_2, value_2) in zip(comp_1.locals,
+                                                    comp_2.locals):
+      if name_1 != name_2 or not _computations_equal(value_1, value_2):
+        return False
+    return True
+  elif isinstance(comp_1, building_blocks.Call):
+    return (_computations_equal(comp_1.function, comp_2.function) and
+            (comp_1.argument is None and comp_2.argument is None or
+             _computations_equal(comp_1.argument, comp_2.argument)))
+  elif isinstance(comp_1, building_blocks.CompiledComputation):
+    return comp_1.proto == comp_2.proto
+  elif isinstance(comp_1, building_blocks.Data):
+    return comp_1.uri == comp_2.uri
+  elif isinstance(comp_1, building_blocks.Intrinsic):
+    return comp_1.uri == comp_2.uri
+  elif isinstance(comp_1, building_blocks.Lambda):
+    return (comp_1.parameter_name == comp_2.parameter_name and
+            comp_1.parameter_type == comp_2.parameter_type and
+            _computations_equal(comp_1.result, comp_2.result))
+  elif isinstance(comp_1, building_blocks.Placement):
+    return comp_1.uri == comp_2.uri
+  elif isinstance(comp_1, building_blocks.Reference):
+    return comp_1.name == comp_2.name
+  elif isinstance(comp_1, building_blocks.Selection):
+    return (_computations_equal(comp_1.source, comp_2.source) and
+            comp_1.name == comp_2.name and comp_1.index == comp_2.index)
+  elif isinstance(comp_1, building_blocks.Tuple):
+    # The element names are checked as part of the `type_signature`.
+    if len(comp_1) != len(comp_2):
+      return False
+    for element_1, element_2 in zip(comp_1, comp_2):
+      if not _computations_equal(element_1, element_2):
+        return False
+    return True
+  raise NotImplementedError('Unexpected type found: {}.'.format(type(comp_1)))
```

## tensorflow_federated/python/core/impl/transforming_executor.py

```diff
@@ -12,18 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """An executor that transforms computations prior to executing them."""
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import py_typecheck
-from tensorflow_federated.python.core.impl import computation_building_blocks
 from tensorflow_federated.python.core.impl import computation_impl
 from tensorflow_federated.python.core.impl import executor_base
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import building_blocks
 
 
 class TransformingExecutor(executor_base.Executor):
   """This executor transforms computations prior to executing them.
 
   This executor only performs transformations. All other aspects of execution
   are delegated to the underlying target executor.
@@ -52,21 +52,18 @@
   async def create_value(self, value, type_spec=None):
     if isinstance(value, computation_impl.ComputationImpl):
       return await self.create_value(
           computation_impl.ComputationImpl.get_proto(value),
           type_utils.reconcile_value_with_type_spec(value, type_spec))
     elif isinstance(value, pb.Computation):
       return await self.create_value(
-          computation_building_blocks.ComputationBuildingBlock.from_proto(
-              value), type_spec)
-    elif isinstance(value,
-                    computation_building_blocks.ComputationBuildingBlock):
+          building_blocks.ComputationBuildingBlock.from_proto(value), type_spec)
+    elif isinstance(value, building_blocks.ComputationBuildingBlock):
       value = self._transformation_fn(value)
-      py_typecheck.check_type(
-          value, computation_building_blocks.ComputationBuildingBlock)
+      py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
       return await self._target_executor.create_value(value.proto, type_spec)
     else:
       return await self._target_executor.create_value(value, type_spec)
 
   async def create_call(self, comp, arg=None):
     return await self._target_executor.create_call(comp, arg)
```

## tensorflow_federated/python/core/impl/type_utils.py

```diff
@@ -25,16 +25,15 @@
 from six.moves import range
 import tensorflow as tf
 
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.api import typed_object
-from tensorflow_federated.python.core.api import value_base
-from tensorflow_federated.python.core.impl import placement_literals
+from tensorflow_federated.python.core.impl.compiler import placement_literals
 
 
 def infer_type(arg):
   """Infers the TFF type of the argument (a `computation_types.Type` instance).
 
   WARNING: This function is only partially implemented.
 
@@ -64,15 +63,15 @@
     return computation_types.SequenceType(
         tf_dtypes_and_shapes_to_type(
             tf.compat.v1.data.get_output_types(arg),
             tf.compat.v1.data.get_output_shapes(arg)))
   elif isinstance(arg, anonymous_tuple.AnonymousTuple):
     return computation_types.NamedTupleType([
         (k, infer_type(v)) if k else infer_type(v)
-        for k, v in anonymous_tuple.to_elements(arg)
+        for k, v in anonymous_tuple.iter_elements(arg)
     ])
   elif py_typecheck.is_attrs(arg):
     items = attr.asdict(
         arg, dict_factory=collections.OrderedDict, recurse=False)
     return computation_types.NamedTupleTypeWithPyContainerType(
         [(k, infer_type(v)) for k, v in six.iteritems(items)], type(arg))
   elif py_typecheck.is_named_tuple(arg):
@@ -116,15 +115,15 @@
         # TODO(b/113112885): Find something more lightweight we could use here.
         tensor_proto = tf.make_tensor_proto(arg)
         return computation_types.TensorType(
             tf.DType(tensor_proto.dtype),
             tf.TensorShape(tensor_proto.tensor_shape))
       except TypeError as err:
         raise TypeError('Could not infer the TFF type of {}: {}'.format(
-            py_typecheck.type_string(type(arg)), str(err)))
+            py_typecheck.type_string(type(arg)), err))
 
 
 def to_canonical_value(value):
   """Converts a Python object to a canonical TFF value for a given type.
 
   Args:
     value: The object to convert.
@@ -160,15 +159,15 @@
   """
   type_spec = computation_types.to_type(type_spec)
   py_typecheck.check_type(type_spec, computation_types.Type)
   val_type = infer_type(val)
   if not is_assignable_from(type_spec, val_type):
     raise TypeError(
         'Expected TFF type {}, which is not assignable from {}.'.format(
-            str(type_spec), str(val_type)))
+            type_spec, val_type))
 
 
 def tf_dtypes_and_shapes_to_type(dtypes, shapes):
   """Returns computation_types.Type for the given TF (dtypes, shapes) tuple.
 
   The returned dtypes and shapes match those used by `tf.data.Dataset`s to
   indicate the type and shape of their elements. They can be used, e.g., as
@@ -221,15 +220,15 @@
   elif isinstance(dtypes, (list, tuple)):
     return computation_types.NamedTupleTypeWithPyContainerType([
         tf_dtypes_and_shapes_to_type(dtypes_elem, shapes[idx])
         for idx, dtypes_elem in enumerate(dtypes)
     ], type(dtypes))
   else:
     raise TypeError('Unrecognized: dtypes {}, shapes {}.'.format(
-        str(dtypes), str(shapes)))
+        dtypes, shapes))
 
 
 def type_to_tf_dtypes_and_shapes(type_spec):
   """Returns nested structures of tensor dtypes and shapes for a given TFF type.
 
   The returned dtypes and shapes match those used by `tf.data.Dataset`s to
   indicate the type and shape of their elements. They can be used, e.g., as
@@ -252,27 +251,30 @@
       tuples and tensors, or if any of the elements in named tuples are unnamed.
   """
   type_spec = computation_types.to_type(type_spec)
   if isinstance(type_spec, computation_types.TensorType):
     return (type_spec.dtype, type_spec.shape)
   elif isinstance(type_spec, computation_types.NamedTupleType):
     elements = anonymous_tuple.to_elements(type_spec)
-    if elements[0][0] is not None:
+    if not elements:
+      output_dtypes = []
+      output_shapes = []
+    elif elements[0][0] is not None:
       output_dtypes = collections.OrderedDict()
       output_shapes = collections.OrderedDict()
       for e in elements:
         element_name = e[0]
         element_spec = e[1]
         if element_name is None:
           raise ValueError(
               'When a sequence appears as a part of a parameter to a section '
               'of TensorFlow code, in the type signature of elements of that '
               'sequence all named tuples must have their elements explicitly '
               'named, and this does not appear to be the case in {}.'.format(
-                  str(type_spec)))
+                  type_spec))
         element_output = type_to_tf_dtypes_and_shapes(element_spec)
         output_dtypes[element_name] = element_output[0]
         output_shapes[element_name] = element_output[1]
     else:
       output_dtypes = []
       output_shapes = []
       for e in elements:
@@ -280,15 +282,15 @@
         element_spec = e[1]
         if element_name is not None:
           raise ValueError(
               'When a sequence appears as a part of a parameter to a section '
               'of TensorFlow code, in the type signature of elements of that '
               'sequence all named tuples must have their elements explicitly '
               'named, and this does not appear to be the case in {}.'.format(
-                  str(type_spec)))
+                  type_spec))
         element_output = type_to_tf_dtypes_and_shapes(element_spec)
         output_dtypes.append(element_output[0])
         output_shapes.append(element_output[1])
     if isinstance(type_spec,
                   computation_types.NamedTupleTypeWithPyContainerType):
       container_type = computation_types.NamedTupleTypeWithPyContainerType.get_container_type(
           type_spec)
@@ -350,16 +352,15 @@
 
   Raises:
     ValueError: if the `type_spec` is composed of something other than named
       tuples and tensors, or if any of the elements in named tuples are unnamed.
   """
   type_spec = computation_types.to_type(type_spec)
   if isinstance(type_spec, computation_types.TensorType):
-    return tf.data.experimental.TensorStructure(type_spec.dtype,
-                                                type_spec.shape)
+    return tf.TensorSpec(type_spec.shape, type_spec.dtype)
   elif isinstance(type_spec, computation_types.NamedTupleType):
     elements = anonymous_tuple.to_elements(type_spec)
     if not elements:
       raise ValueError('Empty tuples are unsupported.')
     element_outputs = [(k, type_to_tf_structure(v)) for k, v in elements]
     named = element_outputs[0][0] is not None
     if not all((e[0] is not None) == named for e in element_outputs):
@@ -428,17 +429,17 @@
   py_typecheck.check_type(name, six.string_types)
   type_spec = computation_types.to_type(type_spec)
   py_typecheck.check_type(type_spec, computation_types.NamedTupleType)
   elements = anonymous_tuple.to_elements(type_spec)
   for elem_name, elem_type in elements:
     if name == elem_name:
       return elem_type
-  raise ValueError('The name \'{}\' of the element does not correspond to '
-                   'any of the names {} in the named tuple type.'.format(
-                       name, str([e[0] for e in elements if e[0]])))
+  raise ValueError('The name \'{}\' of the element does not correspond to any '
+                   'of the names {} in the named tuple type.'.format(
+                       name, [e[0] for e in elements if e[0]]))
 
 
 def preorder_call(given_type, fn, arg):
   """Recursively calls `fn` on the possibly nested structure `given_type`.
 
   Walks the tree in a preorder manner. Updates `arg` on the way down with
   the appropriate information, as defined in `fn`.
@@ -458,15 +459,15 @@
     preorder_call(type_signature.member, fn, arg)
   elif isinstance(type_signature, computation_types.SequenceType):
     preorder_call(type_signature.element, fn, arg)
   elif isinstance(type_signature, computation_types.FunctionType):
     preorder_call(type_signature.parameter, fn, arg)
     preorder_call(type_signature.result, fn, arg)
   elif isinstance(type_signature, computation_types.NamedTupleType):
-    for element in anonymous_tuple.to_elements(type_signature):
+    for element in anonymous_tuple.iter_elements(type_signature):
       preorder_call(element[1], fn, arg)
 
 
 def check_well_formed(type_spec):
   """Checks that `type_spec` represents a well-formed type.
 
   Performs the following checks of well-formedness for `type_spec`:
@@ -719,15 +720,15 @@
                                                         bound_labels, check)
     elif isinstance(type_spec, computation_types.FederatedType):
       return _check_or_get_unbound_abstract_type_labels(type_spec.member,
                                                         bound_labels, check)
     elif isinstance(type_spec, computation_types.NamedTupleType):
       return set().union(*[
           _check_or_get_unbound_abstract_type_labels(v, bound_labels, check)
-          for _, v in anonymous_tuple.to_elements(type_spec)
+          for _, v in anonymous_tuple.iter_elements(type_spec)
       ])
     elif isinstance(type_spec, computation_types.AbstractType):
       if type_spec.label in bound_labels:
         return set()
       elif not check:
         return set([type_spec.label])
       else:
@@ -775,22 +776,25 @@
     `True` iff `type_spec` is sum-compatible, `False` otherwise.
   """
   type_spec = computation_types.to_type(type_spec)
   if isinstance(type_spec, computation_types.TensorType):
     return is_numeric_dtype(type_spec.dtype)
   elif isinstance(type_spec, computation_types.NamedTupleType):
     return all(
-        is_sum_compatible(v) for _, v in anonymous_tuple.to_elements(type_spec))
+        is_sum_compatible(v)
+        for _, v in anonymous_tuple.iter_elements(type_spec))
   elif isinstance(type_spec, computation_types.FederatedType):
     return is_sum_compatible(type_spec.member)
   else:
     return False
 
 
-def check_federated_type(type_spec, member=None, placement=None,
+def check_federated_type(type_spec,
+                         member=None,
+                         placement=None,
                          all_equal=None):
   """Checks that `type_spec` is a federated type with the given parameters.
 
   Args:
     type_spec: The `tff.Type` to check (or something convertible to it).
     member: The expected member type, or `None` if unspecified.
     placement: The desired placement, or `None` if unspecified.
@@ -805,47 +809,24 @@
   py_typecheck.check_type(type_spec, computation_types.FederatedType)
   if member is not None:
     member = computation_types.to_type(member)
     py_typecheck.check_type(member, computation_types.Type)
     check_assignable_from(member, type_spec.member)
   if placement is not None:
     py_typecheck.check_type(placement, placement_literals.PlacementLiteral)
-    if type_spec.placement != placement:
+    if type_spec.placement is not placement:
       raise TypeError(
           'Expected federated type placed at {}, got one placed at {}.'.format(
-              str(placement), str(type_spec.placement)))
+              placement, type_spec.placement))
   if all_equal is not None:
     py_typecheck.check_type(all_equal, bool)
     if type_spec.all_equal != all_equal:
       raise TypeError(
           'Expected federated type with all_equal {}, got one with {}.'.format(
-              str(all_equal), str(type_spec.all_equal)))
-
-
-def check_federated_value_placement(value, placement, label=None):
-  """Checks that `value` is a federated value placed at `placement`.
-
-  Args:
-    value: The value to check, an instance of value_base.Value.
-    placement: The expected placement.
-    label: An optional string label that describes `value`.
-
-  Raises:
-    TypeError: if `value` is not a value_base.Value of a federated type with
-      the expected placement `placement`.
-  """
-  py_typecheck.check_type(value, value_base.Value)
-  py_typecheck.check_type(value.type_signature, computation_types.FederatedType)
-  if label is not None:
-    py_typecheck.check_type(label, six.string_types)
-  if value.type_signature.placement is not placement:
-    raise TypeError('The {} should be placed at {}, but it '
-                    'is placed at {}.'.format(
-                        label if label else 'value', str(placement),
-                        str(value.type_signature.placement)))
+              all_equal, type_spec.all_equal))
 
 
 def is_average_compatible(type_spec):
   """Determines if `type_spec` can be averaged.
 
   Types that are average-compatible are composed of numeric tensor types,
   either floating-point or complex, possibly packaged into nested named tuples,
@@ -859,15 +840,15 @@
   """
   type_spec = computation_types.to_type(type_spec)
   if isinstance(type_spec, computation_types.TensorType):
     return type_spec.dtype.is_floating or type_spec.dtype.is_complex
   elif isinstance(type_spec, computation_types.NamedTupleType):
     return all(
         is_average_compatible(v)
-        for _, v in anonymous_tuple.to_elements(type_spec))
+        for _, v in anonymous_tuple.iter_elements(type_spec))
   elif isinstance(type_spec, computation_types.FederatedType):
     return is_average_compatible(type_spec.member)
   else:
     return False
 
 
 def is_assignable_from(target_type, source_type):
@@ -936,24 +917,24 @@
         target_type.all_equal and not source_type.all_equal):
       return False
     for val in [target_type, source_type]:
       py_typecheck.check_type(val.placement,
                               placement_literals.PlacementLiteral)
     return target_type.placement is source_type.placement
   else:
-    raise TypeError('Unexpected target type {}.'.format(str(target_type)))
+    raise TypeError('Unexpected target type {}.'.format(target_type))
 
 
 def check_assignable_from(target, source):
   target = computation_types.to_type(target)
   source = computation_types.to_type(source)
   if not is_assignable_from(target, source):
     raise TypeError(
         'The target type {} is not assignable from source type {}.'.format(
-            str(target), str(source)))
+            target, source))
 
 
 def are_equivalent_types(type1, type2):
   """Determines whether `type1` and `type2` are equivalent.
 
   We define equivaence in this context as both types being assignable from
   one-another.
@@ -1120,16 +1101,16 @@
   """
   py_typecheck.check_type(type_with_abstract_elements, computation_types.Type)
   py_typecheck.check_type(type_with_concrete_elements, computation_types.Type)
 
   if type_tree_contains_types(type_with_concrete_elements,
                               computation_types.AbstractType):
     raise TypeError(
-        '`type_with_concrete_elements` must contain no abstract types. You have passed {}'
-        .format(type_with_concrete_elements))
+        '`type_with_concrete_elements` must contain no abstract types. You '
+        'have passed {}'.format(type_with_concrete_elements))
 
   bound_abstract_types = {}
   type_error_string = ('Structural mismatch encountered while concretizing '
                        'abstract types. The structure of {} does not match the '
                        'structure of {}').format(type_with_abstract_elements,
                                                  type_with_concrete_elements)
 
@@ -1184,16 +1165,16 @@
         raise TypeError(type_error_string)
       new_member = _concretize_abstract_types(abstract_type_spec.member,
                                               concrete_type_spec.member)
       return computation_types.FederatedType(new_member,
                                              abstract_type_spec.placement,
                                              abstract_type_spec.all_equal)
     else:
-      raise TypeError('Unexpected abstract typespec {}.'.format(
-          str(abstract_type_spec)))
+      raise TypeError(
+          'Unexpected abstract typespec {}.'.format(abstract_type_spec))
 
   concretized_abstract_type = _concretize_abstract_types(
       type_with_abstract_elements, type_with_concrete_elements)
 
   return are_equivalent_types(concretized_abstract_type,
                               type_with_concrete_elements)
 
@@ -1245,15 +1226,15 @@
       type_signature = computation_types.FunctionType(transformed_param,
                                                       transformed_result)
     fn_type_signature, fn_mutated = transform_fn(type_signature)
     return fn_type_signature, fn_mutated or param_mutated or result_mutated
   elif isinstance(type_signature, computation_types.NamedTupleType):
     elems = []
     elems_mutated = False
-    for element in anonymous_tuple.to_elements(type_signature):
+    for element in anonymous_tuple.iter_elements(type_signature):
       transformed_element, element_mutated = transform_type_postorder(
           element[1], transform_fn)
       elems_mutated = elems_mutated or element_mutated
       elems.append((element[0], transformed_element))
     if elems_mutated:
       if isinstance(type_signature,
                     computation_types.NamedTupleTypeWithPyContainerType):
@@ -1329,15 +1310,15 @@
     return value_type
   else:
     type_spec = computation_types.to_type(type_spec)
     if are_equivalent_types(value_type, type_spec):
       return type_spec
     else:
       raise TypeError('Expected a value of type {}, found {}.'.format(
-          str(type_spec), str(value_type)))
+          type_spec, value_type))
 
 
 def get_function_type(type_spec):
   """Constructs a functional type signature for `type_spec`.
 
   Given `type_spec` that is `T`, a functional type signature may be either `T`
   itelf if it is a function, or `( -> T)` otherwise. This allows types from
@@ -1404,18 +1385,18 @@
   Raises:
     TypeError: If the check fails.
   """
   type_spec = computation_types.to_type(type_spec)
   py_typecheck.check_not_none(type_spec)
   py_typecheck.check_type(type_spec, computation_types.NamedTupleType)
   if len(type_spec) != 2:
-    raise TypeError('Expected a 2-tuple, found {}.'.format(str(type_spec)))
-  for _, v in anonymous_tuple.to_elements(type_spec):
+    raise TypeError('Expected a 2-tuple, found {}.'.format(type_spec))
+  for _, v in anonymous_tuple.iter_elements(type_spec):
     check_federated_type(v, None, placement_literals.CLIENTS, False)
     if not is_average_compatible(v.member):
       raise TypeError(
-          'Expected average-compatible args, got {} from argument of '
-          'type {}.'.format(str(v.member), str(type_spec)))
+          'Expected average-compatible args, got {} from argument of type {}.'
+          .format(v.member, type_spec))
   w_type = type_spec[1].member
   py_typecheck.check_type(w_type, computation_types.TensorType)
   if w_type.shape.ndims != 0:
-    raise TypeError('Expected scalar weight, got {}.'.format(str(w_type)))
+    raise TypeError('Expected scalar weight, got {}.'.format(w_type))
```

## tensorflow_federated/python/core/impl/value_impl.py

```diff
@@ -27,41 +27,39 @@
 import tensorflow as tf
 
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_base
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.api import value_base
-from tensorflow_federated.python.core.impl import computation_building_blocks
-from tensorflow_federated.python.core.impl import computation_constructing_utils
 from tensorflow_federated.python.core.impl import computation_impl
 from tensorflow_federated.python.core.impl import context_stack_base
-from tensorflow_federated.python.core.impl import dtype_utils
-from tensorflow_federated.python.core.impl import function_utils
-from tensorflow_federated.python.core.impl import graph_utils
-from tensorflow_federated.python.core.impl import intrinsic_defs
-from tensorflow_federated.python.core.impl import placement_literals
 from tensorflow_federated.python.core.impl import tensorflow_serialization
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import building_block_factory
+from tensorflow_federated.python.core.impl.compiler import building_blocks
+from tensorflow_federated.python.core.impl.compiler import intrinsic_defs
+from tensorflow_federated.python.core.impl.compiler import placement_literals
+from tensorflow_federated.python.core.impl.utils import function_utils
+from tensorflow_federated.python.core.impl.utils import tensorflow_utils
 
 
 @six.add_metaclass(abc.ABCMeta)
 class ValueImpl(value_base.Value):
   """A generic base class for values that appear in TFF computations."""
 
   def __init__(self, comp, context_stack):
     """Constructs a value of the given type.
 
     Args:
-      comp: An instance of computation_building_blocks.ComputationBuildingBlock
-        that contains the logic that computes this value.
+      comp: An instance of building_blocks.ComputationBuildingBlock that
+        contains the logic that computes this value.
       context_stack: The context stack to use.
     """
-    py_typecheck.check_type(
-        comp, computation_building_blocks.ComputationBuildingBlock)
+    py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
     py_typecheck.check_type(context_stack, context_stack_base.ContextStack)
     super(ValueImpl, self).__setattr__('_comp', comp)
     super(ValueImpl, self).__setattr__('_context_stack', context_stack)
 
   @property
   def type_signature(self):
     return self._comp.type_signature
@@ -82,100 +80,98 @@
   def __str__(self):
     return str(self._comp)
 
   def __dir__(self):
     if not isinstance(self._comp.type_signature,
                       computation_types.NamedTupleType):
       raise TypeError(
-          'Operator dir() is only suppored for named tuples, but the object '
-          'on which it has been invoked is of type {}.'.format(
-              str(self._comp.type_signature)))
+          'Operator dir() is only suppored for named tuples, but the object on '
+          'which it has been invoked is of type {}.'.format(
+              self._comp.type_signature))
     return dir(self._comp.type_signature)
 
   def __getattr__(self, name):
     py_typecheck.check_type(name, six.string_types)
     if (isinstance(self._comp.type_signature, computation_types.FederatedType)
         and isinstance(self._comp.type_signature.member,
                        computation_types.NamedTupleType)):
       return ValueImpl(
-          computation_constructing_utils.create_federated_getattr_call(
+          building_block_factory.create_federated_getattr_call(
               self._comp, name), self._context_stack)
     elif not isinstance(self._comp.type_signature,
                         computation_types.NamedTupleType):
       raise TypeError(
           'Operator getattr() is only supported for named tuples, but the '
           'object on which it has been invoked is of type {}.'.format(
-              str(self._comp.type_signature)))
+              self._comp.type_signature))
     if name not in dir(self._comp.type_signature):
       raise AttributeError(
           'There is no such attribute as \'{}\' in this tuple.'.format(name))
-    if isinstance(self._comp, computation_building_blocks.Tuple):
+    if isinstance(self._comp, building_blocks.Tuple):
       return ValueImpl(getattr(self._comp, name), self._context_stack)
     return ValueImpl(
-        computation_building_blocks.Selection(self._comp, name=name),
-        self._context_stack)
+        building_blocks.Selection(self._comp, name=name), self._context_stack)
 
   def __setattr__(self, name, value):
     py_typecheck.check_type(name, six.string_types)
     value_comp = ValueImpl.get_comp(to_value(value, None, self._context_stack))
     if isinstance(self._comp.type_signature,
                   computation_types.FederatedType) and isinstance(
                       self._comp.type_signature.member,
                       computation_types.NamedTupleType):
-      new_comp = computation_constructing_utils.create_federated_setattr_call(
+      new_comp = building_block_factory.create_federated_setattr_call(
           self._comp, name, value_comp)
       super(ValueImpl, self).__setattr__('_comp', new_comp)
       return
     elif not isinstance(self._comp.type_signature,
                         computation_types.NamedTupleType):
       raise TypeError(
           'Operator setattr() is only supported for named tuples, but the '
           'object on which it has been invoked is of type {}.'.format(
-              str(self._comp.type_signature)))
-    named_tuple_setattr_lambda = computation_constructing_utils.create_named_tuple_setattr_lambda(
+              self._comp.type_signature))
+    named_tuple_setattr_lambda = building_block_factory.create_named_tuple_setattr_lambda(
         self._comp.type_signature, name, value_comp)
-    new_comp = computation_building_blocks.Call(named_tuple_setattr_lambda,
-                                                self._comp)
+    new_comp = building_blocks.Call(named_tuple_setattr_lambda, self._comp)
     super(ValueImpl, self).__setattr__('_comp', new_comp)
 
   def __len__(self):
     type_signature = self._comp.type_signature
     if isinstance(type_signature, computation_types.FederatedType):
       type_signature = type_signature.member
     if not isinstance(type_signature, computation_types.NamedTupleType):
       raise TypeError(
           'Operator len() is only supported for (possibly federated) named '
-          'tuples, but the object on which it has been invoked is of type '
-          '{}.'.format(str(self._comp.type_signature)))
+          'tuples, but the object on which it has been invoked is of type {}.'
+          .format(self._comp.type_signature))
     return len(type_signature)
 
   def __getitem__(self, key):
     py_typecheck.check_type(key, (int, slice))
     if (isinstance(self._comp.type_signature, computation_types.FederatedType)
         and isinstance(self._comp.type_signature.member,
                        computation_types.NamedTupleType)):
       return ValueImpl(
-          computation_constructing_utils.create_federated_getitem_call(
-              self._comp, key), self._context_stack)
+          building_block_factory.create_federated_getitem_call(self._comp, key),
+          self._context_stack)
     if not isinstance(self._comp.type_signature,
                       computation_types.NamedTupleType):
       raise TypeError(
           'Operator getitem() is only supported for named tuples, but the '
           'object on which it has been invoked is of type {}.'.format(
-              str(self._comp.type_signature)))
+              self._comp.type_signature))
     elem_length = len(self._comp.type_signature)
     if isinstance(key, int):
       if key < 0 or key >= elem_length:
         raise IndexError(
             'The index of the selected element {} is out of range.'.format(key))
-      if isinstance(self._comp, computation_building_blocks.Tuple):
+      if isinstance(self._comp, building_blocks.Tuple):
         return ValueImpl(self._comp[key], self._context_stack)
       else:
         return ValueImpl(
-            computation_building_blocks.Selection(self._comp, index=key),
+            building_blocks.Selection(self._comp, index=key),
             self._context_stack)
     elif isinstance(key, slice):
       index_range = range(*key.indices(elem_length))
       if not index_range:
         raise IndexError('Attempted to slice 0 elements, which is not '
                          'currently supported.')
       return to_value([self[k] for k in index_range], None, self._context_stack)
@@ -183,50 +179,48 @@
   def __iter__(self):
     type_signature = self._comp.type_signature
     if isinstance(type_signature, computation_types.FederatedType):
       type_signature = type_signature.member
     if not isinstance(type_signature, computation_types.NamedTupleType):
       raise TypeError(
           'Operator iter() is only supported for (possibly federated) named '
-          'tuples, but the object on which it has been invoked is of type '
-          '{}.'.format(str(self._comp.type_signature)))
+          'tuples, but the object on which it has been invoked is of type {}.'
+          .format(self._comp.type_signature))
     for index in range(len(type_signature)):
       yield self[index]
 
   def __call__(self, *args, **kwargs):
     if not isinstance(self._comp.type_signature,
                       computation_types.FunctionType):
       raise SyntaxError(
-          'Function-like invocation is only supported for values of '
-          'functional types, but the value being invoked is of type '
-          '{} that does not support invocation.'.format(
-              str(self._comp.type_signature)))
+          'Function-like invocation is only supported for values of functional '
+          'types, but the value being invoked is of type {} that does not '
+          'support invocation.'.format(self._comp.type_signature))
     if args or kwargs:
       args = [to_value(x, None, self._context_stack) for x in args]
       kwargs = {
           k: to_value(v, None, self._context_stack)
           for k, v in six.iteritems(kwargs)
       }
       arg = function_utils.pack_args(self._comp.type_signature.parameter, args,
                                      kwargs, self._context_stack.current)
       arg = ValueImpl.get_comp(to_value(arg, None, self._context_stack))
     else:
       arg = None
-    return ValueImpl(
-        computation_building_blocks.Call(self._comp, arg), self._context_stack)
+    return ValueImpl(building_blocks.Call(self._comp, arg), self._context_stack)
 
   def __add__(self, other):
     other = to_value(other, None, self._context_stack)
     if not type_utils.are_equivalent_types(self.type_signature,
                                            other.type_signature):
-      raise TypeError('Cannot add {} and {}.'.format(
-          str(self.type_signature), str(other.type_signature)))
+      raise TypeError('Cannot add {} and {}.'.format(self.type_signature,
+                                                     other.type_signature))
     return ValueImpl(
-        computation_building_blocks.Call(
-            computation_building_blocks.Intrinsic(
+        building_blocks.Call(
+            building_blocks.Intrinsic(
                 intrinsic_defs.GENERIC_PLUS.uri,
                 computation_types.FunctionType(
                     [self.type_signature, self.type_signature],
                     self.type_signature)),
             ValueImpl.get_comp(
                 to_value([self, other], None, self._context_stack))),
         self._context_stack)
@@ -242,16 +236,16 @@
 
   Returns:
     An instance of `value_base.Value`.
   """
   py_typecheck.check_type(context_stack, context_stack_base.ContextStack)
   tf_comp, _ = tensorflow_serialization.serialize_py_fn_as_tf_computation(
       lambda: tf.constant(const), None, context_stack)
-  compiled_comp = computation_building_blocks.CompiledComputation(tf_comp)
-  called_comp = computation_building_blocks.Call(compiled_comp)
+  compiled_comp = building_blocks.CompiledComputation(tf_comp)
+  called_comp = building_blocks.Call(compiled_comp)
   return ValueImpl(called_comp, context_stack)
 
 
 def _wrap_sequence_as_value(elements, element_type, context_stack):
   """Wraps `elements` as a TFF sequence with elements of type `element_type`.
 
   Args:
@@ -273,27 +267,26 @@
   # Checks that the types of all the individual elements are compatible with the
   # requested type of the sequence as a while.
   for elem in elements:
     elem_type = type_utils.infer_type(elem)
     if not type_utils.is_assignable_from(element_type, elem_type):
       raise TypeError(
           'Expected all sequence elements to be {}, found {}.'.format(
-              str(element_type), str(elem_type)))
+              element_type, elem_type))
 
   # Defines a no-arg function that builds a `tf.data.Dataset` from the elements.
   def _create_dataset_from_elements():
-    return graph_utils.make_data_set_from_elements(
+    return tensorflow_utils.make_data_set_from_elements(
         tf.compat.v1.get_default_graph(), elements, element_type)
 
   # Wraps the dataset as a value backed by a no-argument TensorFlow computation.
   tf_comp, _ = tensorflow_serialization.serialize_py_fn_as_tf_computation(
       _create_dataset_from_elements, None, context_stack)
   return ValueImpl(
-      computation_building_blocks.Call(
-          computation_building_blocks.CompiledComputation(tf_comp)),
+      building_blocks.Call(building_blocks.CompiledComputation(tf_comp)),
       context_stack)
 
 
 def to_value(arg, type_spec, context_stack):
   """Converts the argument into an instance of `tff.Value`.
 
   The types of non-`tff.Value` arguments that are currently convertible to
@@ -328,54 +321,53 @@
   """
   py_typecheck.check_type(context_stack, context_stack_base.ContextStack)
   if type_spec is not None:
     type_spec = computation_types.to_type(type_spec)
     type_utils.check_well_formed(type_spec)
   if isinstance(arg, ValueImpl):
     result = arg
-  elif isinstance(arg, computation_building_blocks.ComputationBuildingBlock):
+  elif isinstance(arg, building_blocks.ComputationBuildingBlock):
     result = ValueImpl(arg, context_stack)
   elif isinstance(arg, placement_literals.PlacementLiteral):
-    result = ValueImpl(
-        computation_building_blocks.Placement(arg), context_stack)
+    result = ValueImpl(building_blocks.Placement(arg), context_stack)
   elif isinstance(arg, computation_base.Computation):
     result = ValueImpl(
-        computation_building_blocks.CompiledComputation(
+        building_blocks.CompiledComputation(
             computation_impl.ComputationImpl.get_proto(arg)), context_stack)
   elif type_spec is not None and isinstance(type_spec,
                                             computation_types.SequenceType):
     result = _wrap_sequence_as_value(arg, type_spec.element, context_stack)
   elif isinstance(arg, anonymous_tuple.AnonymousTuple):
     result = ValueImpl(
-        computation_building_blocks.Tuple([
+        building_blocks.Tuple([
             (k, ValueImpl.get_comp(to_value(v, None, context_stack)))
-            for k, v in anonymous_tuple.to_elements(arg)
+            for k, v in anonymous_tuple.iter_elements(arg)
         ]), context_stack)
   elif py_typecheck.is_named_tuple(arg):
     result = to_value(arg._asdict(), None, context_stack)
   elif py_typecheck.is_attrs(arg):
     result = to_value(
         attr.asdict(arg, dict_factory=collections.OrderedDict, recurse=False),
         None, context_stack)
   elif isinstance(arg, dict):
     if isinstance(arg, collections.OrderedDict):
       items = six.iteritems(arg)
     else:
       items = sorted(six.iteritems(arg))
-    value = computation_building_blocks.Tuple([
+    value = building_blocks.Tuple([
         (k, ValueImpl.get_comp(to_value(v, None, context_stack)))
         for k, v in items
     ])
     result = ValueImpl(value, context_stack)
   elif isinstance(arg, (tuple, list)):
     result = ValueImpl(
-        computation_building_blocks.Tuple([
+        building_blocks.Tuple([
             ValueImpl.get_comp(to_value(x, None, context_stack)) for x in arg
         ]), context_stack)
-  elif isinstance(arg, dtype_utils.TENSOR_REPRESENTATION_TYPES):
+  elif isinstance(arg, tensorflow_utils.TENSOR_REPRESENTATION_TYPES):
     result = _wrap_constant_as_value(arg, context_stack)
   elif isinstance(arg, (tf.Tensor, tf.Variable)):
     raise TypeError(
         'TensorFlow construct {} has been encountered in a federated '
         'context. TFF does not support mixing TF and federated orchestration '
         'code. Please wrap any TensorFlow constructs with '
         '`tff.tf_computation`.'.format(arg))
@@ -383,11 +375,10 @@
     raise TypeError(
         'Unable to interpret an argument of type {} as a TFF value.'.format(
             py_typecheck.type_string(type(arg))))
   py_typecheck.check_type(result, ValueImpl)
   if (type_spec is not None and
       not type_utils.is_assignable_from(type_spec, result.type_signature)):
     raise TypeError(
-        'The supplied argument maps to TFF type {}, which is incompatible '
-        'with the requested type {}.'.format(
-            str(result.type_signature), str(type_spec)))
+        'The supplied argument maps to TFF type {}, which is incompatible with '
+        'the requested type {}.'.format(result.type_signature, type_spec))
   return result
```

## tensorflow_federated/python/core/impl/value_utils.py

```diff
@@ -14,20 +14,22 @@
 # limitations under the License.
 """Utilities file for functions with TFF `Value`s as inputs and outputs."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
+import six
+
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.api import value_base
-from tensorflow_federated.python.core.impl import computation_building_blocks
 from tensorflow_federated.python.core.impl import value_impl
+from tensorflow_federated.python.core.impl.compiler import building_blocks
 
 
 def get_curried(fn):
   """Returns a curried version of function `fn` that takes a parameter tuple.
 
   For functions `fn` of types <T1,T2,....,Tn> -> U, the result is a function
   of the form T1 -> (T2 -> (T3 -> .... (Tn -> U) ... )).
@@ -45,17 +47,37 @@
   py_typecheck.check_type(fn, value_base.Value)
   py_typecheck.check_type(fn.type_signature, computation_types.FunctionType)
   py_typecheck.check_type(fn.type_signature.parameter,
                           computation_types.NamedTupleType)
   param_elements = anonymous_tuple.to_elements(fn.type_signature.parameter)
   references = []
   for idx, (_, elem_type) in enumerate(param_elements):
-    references.append(
-        computation_building_blocks.Reference('arg{}'.format(idx), elem_type))
-  result = computation_building_blocks.Call(
-      value_impl.ValueImpl.get_comp(fn),
-      computation_building_blocks.Tuple(references))
+    references.append(building_blocks.Reference('arg{}'.format(idx), elem_type))
+  result = building_blocks.Call(
+      value_impl.ValueImpl.get_comp(fn), building_blocks.Tuple(references))
   for ref in references[::-1]:
-    result = computation_building_blocks.Lambda(ref.name, ref.type_signature,
-                                                result)
+    result = building_blocks.Lambda(ref.name, ref.type_signature, result)
   return value_impl.ValueImpl(result,
                               value_impl.ValueImpl.get_context_stack(fn))
+
+
+def check_federated_value_placement(value, placement, label=None):
+  """Checks that `value` is a federated value placed at `placement`.
+
+  Args:
+    value: The value to check, an instance of value_base.Value.
+    placement: The expected placement.
+    label: An optional string label that describes `value`.
+
+  Raises:
+    TypeError: if `value` is not a value_base.Value of a federated type with
+      the expected placement `placement`.
+  """
+  py_typecheck.check_type(value, value_base.Value)
+  py_typecheck.check_type(value.type_signature, computation_types.FederatedType)
+  if label is not None:
+    py_typecheck.check_type(label, six.string_types)
+  if value.type_signature.placement is not placement:
+    raise TypeError(
+        'The {} should be placed at {}, but it is placed at {}.'.format(
+            label if label else 'value', placement,
+            value.type_signature.placement))
```

## tensorflow_federated/python/core/utils/__init__.py

```diff
@@ -24,25 +24,33 @@
 from __future__ import division
 from __future__ import print_function
 
 from tensorflow_federated.python.core.utils.computation_utils import IterativeProcess
 from tensorflow_federated.python.core.utils.computation_utils import StatefulAggregateFn
 from tensorflow_federated.python.core.utils.computation_utils import StatefulBroadcastFn
 from tensorflow_federated.python.core.utils.computation_utils import update_state
+from tensorflow_federated.python.core.utils.differential_privacy import build_dp_aggregate
+from tensorflow_federated.python.core.utils.encoding_utils import build_encoded_broadcast
+from tensorflow_federated.python.core.utils.encoding_utils import build_encoded_mean
+from tensorflow_federated.python.core.utils.encoding_utils import build_encoded_sum
 from tensorflow_federated.python.core.utils.federated_aggregations import federated_max
 from tensorflow_federated.python.core.utils.federated_aggregations import federated_min
 from tensorflow_federated.python.core.utils.tf_computation_utils import assign
-from tensorflow_federated.python.core.utils.tf_computation_utils import get_variables
+from tensorflow_federated.python.core.utils.tf_computation_utils import create_variables
 from tensorflow_federated.python.core.utils.tf_computation_utils import identity
 
 # Used by doc generation script.
 _allowed_symbols = [
     "StatefulAggregateFn",
     "StatefulBroadcastFn",
     "IterativeProcess",
     "assign",
+    "build_dp_aggregate",
+    "build_encoded_broadcast",
+    "build_encoded_mean",
+    "build_encoded_sum",
     "federated_max",
     "federated_min",
-    "get_variables",
+    "create_variables",
     "identity",
     "update_state",
 ]
```

## tensorflow_federated/python/core/utils/computation_utils.py

```diff
@@ -66,16 +66,16 @@
   def __init__(self, initialize_fn, next_fn):
     """Creates the StatefulFn.
 
     Args:
       initialize_fn: A no-arg function that returns a Python container which can
         be converted to a `tff.Value`, placed on the `tff.SERVER`, and passed as
         the first argument of `__call__`. This may be called in vanilla
-        TensorFlow code, typically wrapped as a `tff.tf_compuatation`, as part
-        of the initialization of a larger state object.
+        TensorFlow code, typically wrapped as a `tff.tf_computation`, as part of
+        the initialization of a larger state object.
       next_fn: A function matching the signature of `__call__`, see below.
     """
     py_typecheck.check_callable(initialize_fn)
     py_typecheck.check_callable(next_fn)
     self._initialize_fn = initialize_fn
     self._next_fn = next_fn
 
@@ -115,16 +115,16 @@
 
   def __call__(self, state, value, weight=None):
     """Performs an aggregate of `value@CLIENTS`, producing `value@SERVER`.
 
     The aggregation is optionally parameterized by `weight@CLIENTS`.
 
     This is a function intended to (only) be invoked in the context
-    of a `tff.federated_computation`. It shold be compatible with the
-    TFF type signature
+    of a `tff.federated_computation`. It should be compatible with the
+    TFF type signature.
 
     ```
     (state@SERVER, value@CLIENTS, weight@CLIENTS) ->
          (state@SERVER, aggregate@SERVER).
     ```
 
     Args:
@@ -258,44 +258,43 @@
 
     Raises:
       TypeError: `initialize_fn` and `next_fn` are not compatible function
         types.
     """
     py_typecheck.check_type(initialize_fn, tff.Computation)
     if initialize_fn.type_signature.parameter is not None:
-      raise TypeError('initialize_fn must be a no-arg tff.Computation, '
-                      'but found parameter ' +
-                      str(initialize_fn.type_signature))
+      raise TypeError(
+          'initialize_fn must be a no-arg tff.Computation, but found parameter '
+          '{}'.format(initialize_fn.type_signature))
     initialize_result_type = initialize_fn.type_signature.result
 
     py_typecheck.check_type(next_fn, tff.Computation)
     if isinstance(next_fn.type_signature.parameter, tff.NamedTupleType):
       next_first_param_type = next_fn.type_signature.parameter[0]
     else:
       next_first_param_type = next_fn.type_signature.parameter
     if initialize_result_type != next_first_param_type:
       raise TypeError('The return type of initialize_fn should match the '
                       'first parameter of next_fn, but found\n'
-                      'initialize_fn.type_signature.result={}\n'
-                      'next_fn.type_signature.parameter[0]={}'.format(
+                      'initialize_fn.type_signature.result=\n{}\n'
+                      'next_fn.type_signature.parameter[0]=\n{}'.format(
                           initialize_result_type, next_first_param_type))
 
     next_result_type = next_fn.type_signature.result
     if next_first_param_type != next_result_type:
       # This might be multiple output next_fn, check if the first argument might
-      # be the state. If still not the right type, raise and error.
+      # be the state. If still not the right type, raise an error.
       if isinstance(next_result_type, tff.NamedTupleType):
         next_result_type = next_result_type[0]
       if next_first_param_type != next_result_type:
         raise TypeError('The return type of next_fn should match the '
                         'first parameter, but found\n'
-                        'next_fn.type_signature.parameter[0]={}\n'
-                        'next_fn.type_signature.result={}'.format(
-                            next_first_param_type,
-                            next_fn.type_signature.result))
+                        'next_fn.type_signature.parameter[0]=\n{}\n'
+                        'actual next_result_type=\n{}'.format(
+                            next_first_param_type, next_result_type))
     self._initialize_fn = initialize_fn
     self._next_fn = next_fn
 
   @property
   def initialize(self):
     """A no-arg `tff.Computation` that returns the initial state."""
     return self._initialize_fn
```

## tensorflow_federated/python/core/utils/tf_computation_utils.py

```diff
@@ -22,50 +22,63 @@
 import tensorflow as tf
 
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
 
 
-def get_variables(name, type_spec, **kwargs):
+def create_variables(name, type_spec, **kwargs):
   """Creates a set of variables that matches the given `type_spec`.
 
+  Unlike `tf.get_variables`, this method will always create new variables,
+  and will not retrieve variables previously created with the same name.
+
   Args:
     name: The common name to use for the scope in which all of the variables are
       to be created.
     type_spec: An instance of `tff.Type` or something convertible to it. The
       type signature may only be composed of tensor types and named tuples,
       possibly nested.
-    **kwargs: Additional keyword args to pass to `tf.get_variable` calls.
+    **kwargs: Additional keyword args to pass to `tf.Variable` construction.
 
   Returns:
     Either a single variable when invoked with a tensor TFF type, or a nested
     structure of variables created in the appropriately-named variable scopes
     made up of anonymous tuples if invoked with a named tuple TFF type.
 
   Raises:
     TypeError: if `type_spec` is not a type signature composed of tensor and
       named tuple TFF types.
   """
   py_typecheck.check_type(name, six.string_types)
   type_spec = computation_types.to_type(type_spec)
   py_typecheck.check_type(type_spec, computation_types.Type)
   if isinstance(type_spec, computation_types.TensorType):
-    return tf.get_variable(
-        name, dtype=type_spec.dtype, shape=type_spec.shape, **kwargs)
+    return tf.Variable(
+        initial_value=tf.zeros(dtype=type_spec.dtype, shape=type_spec.shape),
+        name=name,
+        **kwargs)
   elif isinstance(type_spec, computation_types.NamedTupleType):
-    with tf.variable_scope(name):
-      return anonymous_tuple.AnonymousTuple([
-          (k, get_variables(k if k is not None else str(i), v, **kwargs))
-          for i, (k, v) in enumerate(anonymous_tuple.to_elements(type_spec))
-      ])
+
+    def _scoped_name(var_name, index):
+      if var_name is None:
+        var_name = str(index)
+      if name:
+        return '{}/{}'.format(name, var_name)
+      else:
+        return var_name
+
+    return anonymous_tuple.AnonymousTuple([
+        (k, create_variables(_scoped_name(k, i), v, **kwargs))
+        for i, (k, v) in enumerate(anonymous_tuple.to_elements(type_spec))
+    ])
   else:
     raise TypeError(
         'Expected a TFF type signature composed of tensors and named tuples, '
-        'found {}.'.format(str(type_spec)))
+        'found {}.'.format(type_spec))
 
 
 def assign(target, source):
   """Creates an op that assigns `target` from `source`.
 
   This utility function provides the exact same behavior as
   `tf.Variable.assign`, but it generalizes to a wider class of objects,
@@ -115,15 +128,15 @@
   Raises:
     TypeError: If types mismatch.
   """
 
   def _mapping_fn(x):
     if not tf.is_tensor(x):
       raise TypeError('Expected a tensor, found {}.'.format(
-          str(py_typecheck.type_string(type(x)))))
+          py_typecheck.type_string(type(x))))
     if hasattr(x, 'read_value'):
       x = x.read_value()
     return tf.identity(x)
 
   # TODO(b/113112108): Extend this to containers of mixed types.
   if isinstance(source, anonymous_tuple.AnonymousTuple):
     return anonymous_tuple.map_structure(_mapping_fn, source)
```

## tensorflow_federated/python/learning/federated_averaging.py

```diff
@@ -74,15 +74,18 @@
     tf.nest.map_structure(lambda a, b: a.assign(b), model.weights,
                           initial_weights)
 
     @tf.function
     def reduce_fn(num_examples_sum, batch):
       """Runs `tff.learning.Model.train_on_batch` on local client batch."""
       output = model.train_on_batch(batch)
-      return num_examples_sum + tf.shape(output.predictions)[0]
+      if output.num_examples is None:
+        return num_examples_sum + tf.shape(output.predictions)[0]
+      else:
+        return num_examples_sum + output.num_examples
 
     num_examples_sum = dataset.reduce(
         initial_state=tf.constant(0), reduce_func=reduce_fn)
 
     weights_delta = tf.nest.map_structure(tf.subtract, model.weights.trainable,
                                           initial_weights.trainable)
     aggregated_outputs = model.report_local_outputs()
```

## tensorflow_federated/python/learning/keras_utils.py

```diff
@@ -47,15 +47,15 @@
   def model_fn():
     return tff.learning.from_keras_model(keras_model)
 
   fed_avg = tff.learning.build_federated_averaging_process(model_fn, ...)
   state = fed_avg.initialize()
   state = fed_avg.next(state, ...)
   ...
-  tff.learning.assign_weights_to_keras_model(state.model, keras_model)
+  tff.learning.assign_weights_to_keras_model(keras_model, state.model)
   ```
 
   Args:
     keras_model: A `tf.keras.models.Model` instance to assign weights to.
     tff_weights: A TFF value representing the weights of a model.
 
   Raises:
@@ -190,23 +190,23 @@
     A `tff.learning.Model`.
 
   Raises:
     TypeError: If `keras_model` is not an instance of `tf.keras.Model`.
     ValueError: If `keras_model` was *not* compiled.
   """
   py_typecheck.check_type(keras_model, tf.keras.Model)
+  # Optimizer attribute is only set after calling tf.keras.Model.compile().
+  if not keras_model.optimizer:
+    raise ValueError('`keras_model` must be compiled. Use from_keras_model() '
+                     'instead.')
   dummy_tensors = _preprocess_dummy_batch(dummy_batch)
   # NOTE: A sub-classed tf.keras.Model does not produce the compiled metrics
   # until the model has been called on input. The work-around is to call
   # Model.test_on_batch() once before asking for metrics.
   keras_model.test_on_batch(**dummy_tensors)
-  # Optimizer attribute is only set after calling tf.keras.Model.compile().
-  if not hasattr(keras_model, 'optimizer'):
-    raise ValueError('`keras_model` must be compiled. Use from_keras_model() '
-                     'instead.')
   return model_utils.enhance(_TrainableKerasModel(keras_model, dummy_tensors))
 
 
 def federated_aggregate_keras_metric(metric_type, metric_config,
                                      federated_variables):
   """Aggregates variables a keras metric placed at CLIENTS to SERVER.
 
@@ -245,15 +245,15 @@
 
   @tff.tf_computation(member_type, member_type)
   def merge(a, b):
     return tf.nest.map_structure(tf.add, a, b)
 
   @tff.tf_computation(member_type)
   def report(accumulators):
-    """Insert `accumulators` back into the kera metric to obtain result."""
+    """Insert `accumulators` back into the keras metric to obtain result."""
     # NOTE: the following call requires that `metric_type` have a no argument
     # __init__ method, which will restrict the types of metrics that can be
     # used. This is somewhat limiting, but the pattern to use default arguments
     # and export the values in `get_config()` (see
     # `tf.keras.metrics.TopKCategoricalAccuracy`) works well.
     keras_metric = None
     try:
@@ -430,15 +430,18 @@
 
     else:
       batch_loss = None
 
     for metric in self.get_metrics():
       metric.update_state(y_true=y_true, y_pred=predictions)
 
-    return model_lib.BatchOutput(loss=batch_loss, predictions=predictions)
+    return model_lib.BatchOutput(
+        loss=batch_loss,
+        predictions=predictions,
+        num_examples=tf.shape(inputs)[0])
 
   @tf.function
   def forward_pass(self, batch_input, training=True):
     return self._forward_pass(batch_input, training=training)
 
   @tf.function
   def report_local_outputs(self):
```

## tensorflow_federated/python/learning/model.py

```diff
@@ -21,23 +21,25 @@
 import abc
 import collections
 
 import six
 
 
 class BatchOutput(
-    collections.namedtuple('BatchOutput', ['loss', 'predictions'])):
+    collections.namedtuple('BatchOutput',
+                           ['loss', 'predictions', 'num_examples'])):
   """A structure that holds the output of a `tff.learning.Model`.
 
   NOTE: All fields are optional (may be None).
 
   -   `loss`: The scalar mean loss on the examples in the batch. If the model
       has multiple losses, it is the sum of all the individual losses.
   -   `predictions`: Tensor of predictions on the examples. The first dimension
       must be the same size (the size of the batch).
+  -   `num_examples`: Number of examples seen in the batch.
   """
   __slots__ = ()
 
 
 @six.add_metaclass(abc.ABCMeta)
 class Model(object):
   """Represents a model for use in TensorFlow Federated.
```

## tensorflow_federated/python/learning/framework/__init__.py

```diff
@@ -14,24 +14,33 @@
 # limitations under the License.
 """The public API for contributors who develop federated learning algorithms."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
+from tensorflow_federated.python.learning.framework.encoding_utils import build_encoded_broadcast_from_model
+from tensorflow_federated.python.learning.framework.encoding_utils import build_encoded_mean_from_model
+from tensorflow_federated.python.learning.framework.encoding_utils import build_encoded_sum_from_model
 from tensorflow_federated.python.learning.framework.optimizer_utils import build_model_delta_optimizer_process
+from tensorflow_federated.python.learning.framework.optimizer_utils import build_stateless_broadcaster
 from tensorflow_federated.python.learning.framework.optimizer_utils import ClientDeltaFn
 from tensorflow_federated.python.learning.framework.optimizer_utils import ClientOutput
-
+from tensorflow_federated.python.learning.model_utils import enhance
 from tensorflow_federated.python.learning.model_utils import EnhancedModel
 from tensorflow_federated.python.learning.model_utils import EnhancedTrainableModel
 from tensorflow_federated.python.learning.model_utils import ModelWeights
 
 # Used by doc generation script.
 _allowed_symbols = [
-    "build_model_delta_optimizer_process",
     "ClientDeltaFn",
     "ClientOutput",
     "EnhancedModel",
     "EnhancedTrainableModel",
     "ModelWeights",
+    "build_encoded_broadcast_from_model",
+    "build_encoded_mean_from_model",
+    "build_encoded_sum_from_model",
+    "build_model_delta_optimizer_process",
+    "build_stateless_broadcaster",
+    "enhance",
 ]
```

## tensorflow_federated/python/simulation/__init__.py

```diff
@@ -14,23 +14,41 @@
 # limitations under the License.
 """The public API for experimenters running federated learning simulations."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
+import six
+
 from tensorflow_federated.python.simulation import datasets
+from tensorflow_federated.python.simulation import models
 from tensorflow_federated.python.simulation.client_data import ClientData
 from tensorflow_federated.python.simulation.file_per_user_client_data import FilePerUserClientData
 from tensorflow_federated.python.simulation.from_tensor_slices_client_data import FromTensorSlicesClientData
 from tensorflow_federated.python.simulation.hdf5_client_data import HDF5ClientData
 from tensorflow_federated.python.simulation.transforming_client_data import TransformingClientData
 
+# High-performance simulation components currently only available in Python 3,
+# and dependent on targets are are not currently included in the open-source
+# build rule.
+# TODO(b/134543154): Modify the OSS build rule to conditionally include these
+# new targets if possible.
+if six.PY3:
+  # pylint: disable=g-import-not-at-top,undefined-variable
+  try:
+    from tensorflow_federated.python.simulation.server_utils import run_server
+  except ModuleNotFoundError:
+    pass
+  # pylint: enable=g-import-not-at-top,undefined-variable
+
 # Used by doc generation script.
 _allowed_symbols = [
     "ClientData",
     "FilePerUserClientData",
     "FromTensorSlicesClientData",
     "HDF5ClientData",
     "TransformingClientData",
     "datasets",
+    "models",
+    "run_server",
 ]
```

## tensorflow_federated/python/simulation/client_data.py

```diff
@@ -26,14 +26,15 @@
 from __future__ import print_function
 
 import abc
 import numpy as np
 
 import six
 import tensorflow as tf
+from tensorflow_federated.python.common_libs import py_typecheck
 
 
 @six.add_metaclass(abc.ABCMeta)
 class ClientData(object):
   """Object to hold a dataset and a mapping of clients to examples."""
 
   @abc.abstractproperty
@@ -49,14 +50,42 @@
       client_id: The string client_id for the desired client.
 
     Returns:
       A `tf.data.Dataset` object.
     """
     pass
 
+  @abc.abstractproperty
+  def output_types(self):
+    """Returns the type of each component of an element of the client datasets.
+
+    Any `tf.data.Dataset` constructed by this class is expected have matching
+    `output_types` properties when accessed via
+    `tf.compat.v1.data.get_output_types(dataset)`.
+
+    Returns:
+      A nested structure of `tf.DType` objects corresponding to each component
+      of an element of the client datasets.
+    """
+    pass
+
+  @abc.abstractproperty
+  def output_shapes(self):
+    """Returns the shape of each component of an element of the client datasets.
+
+    Any `tf.data.Dataset` constructed by this class is expected to have matching
+    `output_shapes` properties when accessed via
+    `tf.compat.v1.data.get_output_shapes(dataset)`.
+
+    Returns:
+      A nested structure of `tf.TensorShape` objects corresponding to each
+      component of an element of the client datasets.
+    """
+    pass
+
   def create_tf_dataset_from_all_clients(self, seed=None):
     """Creates a new `tf.data.Dataset` containing _all_ client examples.
 
     NOTE: the returned `tf.data.Dataset` is not serializable and runnable on
     other devices, as it uses `tf.py_func` internally.
 
     Currently, the implementation produces a dataset that contains
@@ -80,32 +109,76 @@
       for client_id in client_ids:
         for example in self.create_tf_dataset_for_client(client_id):
           yield example
 
     return tf.data.Dataset.from_generator(_generator, self.output_types,
                                           self.output_shapes)
 
-  @abc.abstractproperty
-  def output_types(self):
-    """Returns the type of each component of an element of the client datasets.
+  def preprocess(self, preprocess_fn):
+    """Applies `preprocess_fn` to each client's data."""
+    py_typecheck.check_callable(preprocess_fn)
+
+    def get_dataset(client_id):
+      return preprocess_fn(self.create_tf_dataset_for_client(client_id))
+
+    return ConcreteClientData(self.client_ids, get_dataset)
+
+  @classmethod
+  def from_clients_and_fn(cls, client_ids, create_tf_dataset_for_client_fn):
+    """Constructs a `ClientData` based on the given function.
 
-    Any `tf.data.Dataset` constructed by this class is expected have matching
-    `tf.data.Dataset.output_types` properties.
+    Args:
+      client_ids: A non-empty list of client_ids which are valid inputs to the
+        create_tf_dataset_for_client_fn.
+      create_tf_dataset_for_client_fn: A function that takes a client_id from
+        the above list, and returns a `tf.data.Dataset`.
 
     Returns:
-      A nested structure of `tf.DType` objects corresponding to each component
-      of an element of the client datasets.
+      A `ClientData`.
     """
-    pass
+    return ConcreteClientData(client_ids, create_tf_dataset_for_client_fn)
 
-  @abc.abstractproperty
-  def output_shapes(self):
-    """Returns the shape of each component of an element of the client datasets.
 
-    Any `tf.data.Dataset` constructed by this class is expected to have matching
-    `tf.data.Dataset.output_shapes` properties.
+class ConcreteClientData(ClientData):
+  """A generic `ClientData` object.
 
-    Returns:
-      A nested structure of `tf.TensorShape` objects corresponding to each
-      component of an element of the client datasets.
+  This is a simple implementation of client_data, where Datasets are specified
+  as a function from client_id to Dataset.
+
+  The `ConcreteClientData.preprocess` classmethod is provided as a utility
+  used to wrap another `ClientData` with an additional preprocessing function.
+  """
+
+  def __init__(self, client_ids, create_tf_dataset_for_client_fn):
+    """Arguments correspond to the corresponding members of `ClientData`.
+
+    Args:
+      client_ids: A non-empty list of client_ids.
+      create_tf_dataset_for_client_fn: A function that takes a client_id from
+        the above list, and returns a `tf.data.Dataset`.
     """
-    pass
+    py_typecheck.check_type(client_ids, list)
+    py_typecheck.check_callable(create_tf_dataset_for_client_fn)
+    if not client_ids:
+      raise ValueError('At least one client_id is required.')
+
+    self._client_ids = client_ids
+    self._create_tf_dataset_for_client_fn = create_tf_dataset_for_client_fn
+
+    example_dataset = create_tf_dataset_for_client_fn(client_ids[0])
+    self._output_types = tf.compat.v1.data.get_output_types(example_dataset)
+    self._output_shapes = tf.compat.v1.data.get_output_shapes(example_dataset)
+
+  @property
+  def client_ids(self):
+    return self._client_ids
+
+  def create_tf_dataset_for_client(self, client_id):
+    return self._create_tf_dataset_for_client_fn(client_id)
+
+  @property
+  def output_types(self):
+    return self._output_types
+
+  @property
+  def output_shapes(self):
+    return self._output_shapes
```

## tensorflow_federated/python/simulation/file_per_user_client_data.py

```diff
@@ -48,26 +48,27 @@
     py_typecheck.check_callable(create_tf_dataset_fn)
     self._client_ids = sorted(client_ids)
     self._create_tf_dataset_fn = create_tf_dataset_fn
 
     g = tf.Graph()
     with g.as_default():
       tf_dataset = self._create_tf_dataset_fn(self._client_ids[0])
-      self._output_types = tf_dataset.output_types
-      self._output_shapes = tf_dataset.output_shapes
+      self._output_types = tf.compat.v1.data.get_output_types(tf_dataset)
+      self._output_shapes = tf.compat.v1.data.get_output_shapes(tf_dataset)
 
   @property
   def client_ids(self):
     return self._client_ids
 
   def create_tf_dataset_for_client(self, client_id):
     tf_dataset = self._create_tf_dataset_fn(client_id)
-    tensor_utils.check_nested_equal(tf_dataset.output_types, self._output_types)
-    tensor_utils.check_nested_equal(tf_dataset.output_shapes,
-                                    self._output_shapes)
+    tensor_utils.check_nested_equal(
+        tf.compat.v1.data.get_output_types(tf_dataset), self._output_types)
+    tensor_utils.check_nested_equal(
+        tf.compat.v1.data.get_output_shapes(tf_dataset), self._output_shapes)
     return tf_dataset
 
   @property
   def output_types(self):
     return self._output_types
 
   @property
```

## tensorflow_federated/python/simulation/from_tensor_slices_client_data.py

```diff
@@ -38,16 +38,16 @@
 
     Raises:
       ValueError: If a client with no data is found.
     """
     py_typecheck.check_type(tensor_slices_dict, dict)
     self._tensor_slices_dict = tensor_slices_dict
     example_dataset = self.create_tf_dataset_for_client(self.client_ids[0])
-    self._output_types = example_dataset.output_types
-    self._output_shapes = example_dataset.output_shapes
+    self._output_types = tf.compat.v1.data.get_output_types(example_dataset)
+    self._output_shapes = tf.compat.v1.data.get_output_shapes(example_dataset)
 
   @property
   def client_ids(self):
     return list(self._tensor_slices_dict.keys())
 
   def create_tf_dataset_for_client(self, client_id):
     tensor_slices = self._tensor_slices_dict[client_id]
```

## tensorflow_federated/python/simulation/hdf5_client_data.py

```diff
@@ -57,32 +57,33 @@
         list(self._h5_file[HDF5ClientData._EXAMPLES_GROUP].keys()))
 
     # Get the types and shapes from the first client. We do it once during
     # initialization so we can get both properties in one go.
     g = tf.Graph()
     with g.as_default():
       tf_dataset = self._create_dataset(self._client_ids[0])
-      self._output_types = tf_dataset.output_types
-      self._output_shapes = tf_dataset.output_shapes
+      self._output_types = tf.compat.v1.data.get_output_types(tf_dataset)
+      self._output_shapes = tf.compat.v1.data.get_output_shapes(tf_dataset)
 
   def _create_dataset(self, client_id):
     return tf.data.Dataset.from_tensor_slices(
-        collections.OrderedDict(
-            six.iteritems(
-                self._h5_file[HDF5ClientData._EXAMPLES_GROUP][client_id])))
+        collections.OrderedDict((name, ds.value) for name, ds in sorted(
+            six.iteritems(self._h5_file[HDF5ClientData._EXAMPLES_GROUP]
+                          [client_id]))))
 
   @property
   def client_ids(self):
     return self._client_ids
 
   def create_tf_dataset_for_client(self, client_id):
     tf_dataset = self._create_dataset(client_id)
-    tensor_utils.check_nested_equal(tf_dataset.output_types, self._output_types)
-    tensor_utils.check_nested_equal(tf_dataset.output_shapes,
-                                    self._output_shapes)
+    tensor_utils.check_nested_equal(
+        tf.compat.v1.data.get_output_types(tf_dataset), self._output_types)
+    tensor_utils.check_nested_equal(
+        tf.compat.v1.data.get_output_shapes(tf_dataset), self._output_shapes)
     return tf_dataset
 
   @property
   def output_types(self):
     return self._output_types
 
   @property
```

## tensorflow_federated/python/simulation/datasets/__init__.py

```diff
@@ -16,13 +16,21 @@
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 from tensorflow_federated.python.simulation.datasets import emnist
 from tensorflow_federated.python.simulation.datasets import shakespeare
+from tensorflow_federated.python.simulation.datasets import stackoverflow
+from tensorflow_federated.python.simulation.datasets.dataset_utils import build_dataset_mixture
+from tensorflow_federated.python.simulation.datasets.dataset_utils import build_single_label_dataset
+from tensorflow_federated.python.simulation.datasets.dataset_utils import build_synthethic_iid_datasets
 
 # Used by doc generation script.
 _allowed_symbols = [
+    "build_dataset_mixture",
+    "build_single_label_dataset",
+    "build_synthethic_iid_datasets",
     "emnist",
     "shakespeare",
+    "stackoverflow",
 ]
```

## tensorflow_federated/python/tensorflow_libs/tensor_utils.py

```diff
@@ -133,38 +133,15 @@
   if not tf.is_tensor(tensor):
     raise TypeError('Expected a tensor, found "{}".'.format(
         py_typecheck.type_string(type(tensor))))
   return (hasattr(tensor, 'get_shape') and
           all(dim == 1 for dim in tensor.get_shape()))
 
 
-def metrics_sum(values, name=None):
-  """A function like tf.metrics.mean, but for a simple sum.
-
-  Args:
-    values: A rank-1 tensor to be summed.
-    name: Optional name for the op.
-
-  Returns:
-    A tuple of:
-      sum: A variable holding the current sum of all 'values' seen so far.
-      update_op: An opt to run on each minibatch.
-  """
-  with tf.variable_scope(name, 'metrics_sum', (values,)):
-    sum_var = tf.get_variable(
-        'sum', [],
-        values.dtype,
-        initializer=tf.zeros_initializer,
-        collections=[tf.GraphKeys.LOCAL_VARIABLES],
-        trainable=False)
-    update_op = sum_var.assign_add(tf.reduce_sum(values))
-    return sum_var, update_op
-
-
-def same_dimension(x, y):
+def _same_dimension(x, y):
   """Determines if two `tf.Dimension`s are the same.
 
   Args:
     x: a `tf.Dimension` object.
     y: a `tf.Dimension` object.
 
   Returns:
@@ -181,17 +158,17 @@
   """Determines if two `tf.TensorShape`s are the same.
 
   Args:
     x: a `tf.TensorShape` object.
     y: a `tf.TensorShape` object.
 
   Returns:
-    True iff `x` and `y` are either both _unknonw_ shapes (e.g.
+    True iff `x` and `y` are either both _unknown_ shapes (e.g.
     `tf.TensorShape(None)`) or have each dimension the same.
   """
   if x.ndims != y.ndims:
     return False
   if x.dims is None:
     return y.dims is None
   else:
     return y.dims is not None and all(
-        same_dimension(a, b) for a, b in zip(x.dims, y.dims))
+        _same_dimension(a, b) for a, b in zip(x.dims, y.dims))
```

## Comparing `tensorflow_federated/python/core/impl/computation_building_blocks.py` & `tensorflow_federated/python/core/impl/compiler/building_blocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 """Classes representing various kinds of computations in a deserialized form."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import abc
-import enum
+import enum  # pylint: disable=g-bad-import-order
 import zlib
 
 import six
 from six.moves import zip
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
 from tensorflow_federated.python.core.api import typed_object
-from tensorflow_federated.python.core.impl import intrinsic_defs
-from tensorflow_federated.python.core.impl import placement_literals
-from tensorflow_federated.python.core.impl import type_serialization
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import intrinsic_defs
+from tensorflow_federated.python.core.impl.compiler import placement_literals
+from tensorflow_federated.python.core.impl.compiler import type_serialization
 
 
 def _check_computation_oneof(computation_proto, expected_computation_oneof):
   py_typecheck.check_type(computation_proto, pb.Computation)
   computation_oneof = computation_proto.WhichOneof('computation')
   if computation_oneof != expected_computation_oneof:
     raise TypeError('Expected a {} computation, found {}.'.format(
@@ -82,15 +82,15 @@
       deserialized = deserializer(computation_proto)
       type_spec = type_serialization.deserialize_type(computation_proto.type)
       if not type_utils.are_equivalent_types(deserialized.type_signature,
                                              type_spec):
         raise ValueError(
             'The type {} derived from the computation structure does not '
             'match the type {} declared in its signature'.format(
-                str(deserialized.type_signature), str(type_spec)))
+                deserialized.type_signature, type_spec))
       return deserialized
     else:
       raise NotImplementedError(
           'Deserialization for computations of type {} has not been '
           'implemented yet.'.format(computation_oneof))
 
   def __init__(self, type_spec):
@@ -104,14 +104,26 @@
     type_utils.check_well_formed(type_signature)
     self._type_signature = type_signature
 
   @property
   def type_signature(self):
     return self._type_signature
 
+  def compact_representation(self):
+    """Returns the compact string representation of this building block."""
+    return _string_representation(self, formatted=False)
+
+  def formatted_representation(self):
+    """Returns the formatted string representation of this building block."""
+    return _string_representation(self, formatted=True)
+
+  def structural_representation(self):
+    """Returns the structural string representation of this building block."""
+    return _structural_representation(self)
+
   @abc.abstractproperty
   def proto(self):
     """Returns a serialized form of this object as a pb.Computation instance."""
     raise NotImplementedError
 
   # TODO(b/113112885): Add memoization after identifying a suitable externally
   # available standard library that works in Python 2/3.
@@ -119,15 +131,15 @@
   @abc.abstractmethod
   def __repr__(self):
     """Returns a full-form representation of this computation building block."""
     raise NotImplementedError
 
   def __str__(self):
     """Returns a concise representation of this computation building block."""
-    return compact_representation(self)
+    return self.compact_representation()
 
 
 class Reference(ComputationBuildingBlock):
   """A reference to a name defined earlier in TFF's internal language.
 
   Names are defined by lambda expressions (which have formal named parameters),
   and block structures (which can have one or more locals). The reference
@@ -178,17 +190,17 @@
     return self._name
 
   @property
   def context(self):
     return self._context
 
   def __repr__(self):
-    return 'Reference(\'{}\', {}{})'.format(
-        self._name, repr(self.type_signature),
-        ', {}'.format(repr(self._context)) if self._context is not None else '')
+    return 'Reference(\'{}\', {!r}{})'.format(
+        self._name, self.type_signature,
+        ', {!r}'.format(self._context) if self._context is not None else '')
 
 
 class Selection(ComputationBuildingBlock):
   """A selection by name or index from a tuple-typed value in TFF's language.
 
   The concise syntax for selections is `foo.bar` (selecting a named `bar` from
   the value of expression `foo`), and `foo[n]` (selecting element at index `n`
@@ -203,15 +215,15 @@
     selection_oneof = computation_proto.selection.WhichOneof('selection')
     if selection_oneof == 'name':
       return cls(selection, name=str(computation_proto.selection.name))
     elif selection_oneof == 'index':
       return cls(selection, index=computation_proto.selection.index)
     else:
       raise ValueError('Unknown selection type \'{}\' in {}.'.format(
-          selection_oneof, str(computation_proto)))
+          selection_oneof, computation_proto))
 
   def __init__(self, source, name=None, index=None):
     """A selection from 'source' by a string or numeric 'name_or_index'.
 
     Exactly one of 'name' or 'index' must be specified (not None).
 
     Args:
@@ -234,15 +246,15 @@
           'Cannot simultaneously specify a name and an index, choose one.')
     py_typecheck.check_type(source, ComputationBuildingBlock)
     self._source = source
     source_type = self._source.type_signature
     if not isinstance(source_type, computation_types.NamedTupleType):
       raise TypeError(
           'Expected the source of selection to be a TFF named tuple, '
-          'instead found it to be of type {}.'.format(str(source_type)))
+          'instead found it to be of type {}.'.format(source_type))
     if name is not None:
       py_typecheck.check_type(name, six.string_types)
       if not name:
         raise ValueError('The name of the selected element cannot be empty.')
       else:
         # Normalize, in case we are dealing with a Unicode type or some such.
         name = str(name)
@@ -258,15 +270,16 @@
         super(Selection, self).__init__(elements[index][1])
         self._name = None
         self._index = index
       else:
         raise ValueError(
             'The index of the selected element {} does not fit into the '
             'valid range 0..{} determined by the source type '
-            'signature.'.format(index, str(len(elements) - 1)))
+            'signature.'.format(index,
+                                len(elements) - 1))
 
   @property
   def proto(self):
     if self._name is not None:
       selection = pb.Selection(source=self._source.proto, name=self._name)
     else:
       selection = pb.Selection(source=self._source.proto, index=self._index)
@@ -284,18 +297,17 @@
 
   @property
   def index(self):
     return self._index
 
   def __repr__(self):
     if self._name is not None:
-      return 'Selection({}, name={})'.format(
-          repr(self._source), '\'{}\''.format(self._name))
+      return 'Selection({!r}, name=\'{}\')'.format(self._source, self._name)
     else:
-      return 'Selection({}, index={})'.format(repr(self._source), self._index)
+      return 'Selection({!r}, index={})'.format(self._source, self._index)
 
 
 class Tuple(ComputationBuildingBlock, anonymous_tuple.AnonymousTuple):
   """A tuple with named or unnamed elements in TFF's internal language.
 
   The concise notation for tuples is `<name_1=value_1, ...., name_n=value_n>`
   for tuples with named elements, `<value_1, ..., value_n>` for tuples with
@@ -336,43 +348,47 @@
         return (None, e)
       elif py_typecheck.is_name_value_pair(
           e, name_required=False, value_type=ComputationBuildingBlock):
         if e[0] is not None and not e[0]:
           raise ValueError('Unexpected tuple element with empty string name.')
         return (e[0], e[1])
       else:
-        raise TypeError('Unexpected tuple element: {}.'.format(str(e)))
+        raise TypeError('Unexpected tuple element: {}.'.format(e))
 
     elements = [_map_element(e) for e in elements]
     ComputationBuildingBlock.__init__(
         self,
         computation_types.NamedTupleType([
             ((e[0], e[1].type_signature) if e[0] else e[1].type_signature)
             for e in elements
         ]))
     anonymous_tuple.AnonymousTuple.__init__(self, elements)
 
   @property
   def proto(self):
     elements = []
-    for k, v in anonymous_tuple.to_elements(self):
+    for k, v in anonymous_tuple.iter_elements(self):
       if k is not None:
         element = pb.Tuple.Element(name=k, value=v.proto)
       else:
         element = pb.Tuple.Element(value=v.proto)
       elements.append(element)
     return pb.Computation(
         type=type_serialization.serialize_type(self.type_signature),
         tuple=pb.Tuple(element=elements))
 
   def __repr__(self):
+
+    def _element_repr(element):
+      name, value = element
+      name_repr = '\'{}\''.format(name) if name is not None else 'None'
+      return '({}, {!r})'.format(name_repr, value)
+
     return 'Tuple([{}])'.format(', '.join(
-        '({}, {})'.format('\'{}\''.format(e[0]) if e[0] is not None else 'None',
-                          repr(e[1]))
-        for e in anonymous_tuple.to_elements(self)))
+        _element_repr(e) for e in anonymous_tuple.iter_elements(self)))
 
 
 class Call(ComputationBuildingBlock):
   """A representation of a function invocation in TFF's internal language.
 
   The call construct takes an argument tuple with two elements, the first being
   the function to invoke (represented as a computation with a functional result
@@ -407,27 +423,26 @@
     """
     py_typecheck.check_type(fn, ComputationBuildingBlock)
     if arg is not None:
       py_typecheck.check_type(arg, ComputationBuildingBlock)
     if not isinstance(fn.type_signature, computation_types.FunctionType):
       raise TypeError('Expected fn to be of a functional type, '
                       'but found that its type is {}.'.format(
-                          str(fn.type_signature)))
+                          fn.type_signature))
     if fn.type_signature.parameter is not None:
       if arg is None:
         raise TypeError('The invoked function expects an argument of type {}, '
                         'but got None instead.'.format(
-                            str(fn.type_signature.parameter)))
+                            fn.type_signature.parameter))
       if not type_utils.is_assignable_from(fn.type_signature.parameter,
                                            arg.type_signature):
         raise TypeError(
             'The parameter of the invoked function is expected to be of '
             'type {}, but the supplied argument is of an incompatible '
-            'type {}.'.format(
-                str(fn.type_signature.parameter), str(arg.type_signature)))
+            'type {}.'.format(fn.type_signature.parameter, arg.type_signature))
     elif arg is not None:
       raise TypeError(
           'The invoked function does not expect any parameters, but got '
           'an argument of type {}.'.format(py_typecheck.type_string(type(arg))))
     super(Call, self).__init__(fn.type_signature.result)
     # By now, this condition should hold, so we only double-check in debug mode.
     assert (arg is not None) == (fn.type_signature.parameter is not None)
@@ -450,17 +465,17 @@
 
   @property
   def argument(self):
     return self._argument
 
   def __repr__(self):
     if self._argument is not None:
-      return 'Call({}, {})'.format(repr(self._function), repr(self._argument))
+      return 'Call({!r}, {!r})'.format(self._function, self._argument)
     else:
-      return 'Call({})'.format(repr(self._function))
+      return 'Call({!r})'.format(self._function)
 
 
 class Lambda(ComputationBuildingBlock):
   """A representation of a lambda expression in TFF's internal language.
 
   A lambda expression consists of a string formal parameter name, and a result
   expression that can contain references by name to that formal parameter. A
@@ -525,17 +540,17 @@
     return self._parameter_type
 
   @property
   def result(self):
     return self._result
 
   def __repr__(self):
-    return ('Lambda(\'{}\', {}, {})'.format(self._parameter_name,
-                                            repr(self._parameter_type),
-                                            repr(self._result)))
+    return 'Lambda(\'{}\', {!r}, {!r})'.format(self._parameter_name,
+                                               self._parameter_type,
+                                               self._result)
 
 
 class Block(ComputationBuildingBlock):
   """A representation of a block of code in TFF's internal language.
 
   A block is a syntactic structure that consists of a sequence of local name
   bindings followed by a result. The bindings are interpreted sequentially,
@@ -600,16 +615,15 @@
     updated_locals = []
     for index, element in enumerate(local_symbols):
       if (not isinstance(element, tuple) or (len(element) != 2) or
           not isinstance(element[0], six.string_types)):
         raise TypeError(
             'Expected the locals to be a list of 2-element tuples with string '
             'name as their first element, but this is not the case for the '
-            'local at position {} in the sequence: {}.'.format(
-                index, str(element)))
+            'local at position {} in the sequence: {}.'.format(index, element))
       name = element[0]
       value = element[1]
       py_typecheck.check_type(value, ComputationBuildingBlock)
       updated_locals.append((name, value))
     py_typecheck.check_type(result, ComputationBuildingBlock)
     super(Block, self).__init__(result.type_signature)
     self._locals = updated_locals
@@ -633,17 +647,17 @@
     return list(self._locals)
 
   @property
   def result(self):
     return self._result
 
   def __repr__(self):
-    return ('Block([{}], {})'.format(
-        ', '.join('(\'{}\', {})'.format(k, repr(v)) for k, v in self._locals),
-        repr(self._result)))
+    return 'Block([{}], {!r})'.format(
+        ', '.join('(\'{}\', {!r})'.format(k, v) for k, v in self._locals),
+        self._result)
 
 
 class Intrinsic(ComputationBuildingBlock):
   """A representation of an intrinsic in TFF's internal language.
 
   An instrinsic is a symbol known to the TFF's compiler pipeline, represended
   a a known URI. It generally appears in expressions with a concrete type,
@@ -694,15 +708,15 @@
         intrinsic=pb.Intrinsic(uri=self._uri))
 
   @property
   def uri(self):
     return self._uri
 
   def __repr__(self):
-    return 'Intrinsic(\'{}\', {})'.format(self._uri, repr(self.type_signature))
+    return 'Intrinsic(\'{}\', {!r})'.format(self._uri, self.type_signature)
 
 
 class Data(ComputationBuildingBlock):
   """A representation of data (an input pipeline).
 
   This class does not deal with parsing data URIs and verifying correctness,
   it is only a container. Parsing and type analysis are a responsibility
@@ -744,15 +758,15 @@
         data=pb.Data(uri=self._uri))
 
   @property
   def uri(self):
     return self._uri
 
   def __repr__(self):
-    return 'Data(\'{}\', {})'.format(self._uri, repr(self.type_signature))
+    return 'Data(\'{}\', {!r})'.format(self._uri, self.type_signature)
 
 
 class CompiledComputation(ComputationBuildingBlock):
   """A representation of a fully constructed and serialized computation.
 
   A compile comutation is one that has not been parsed into constituents, and
   is simply represented as an embedded `Computation` protocol buffer. Whereas
@@ -790,16 +804,16 @@
     return self._proto
 
   @property
   def name(self):
     return self._name
 
   def __repr__(self):
-    return 'CompiledComputation({}, {})'.format(self._name,
-                                                repr(self.type_signature))
+    return 'CompiledComputation(\'{}\', {!r})'.format(self._name,
+                                                      self.type_signature)
 
 
 class Placement(ComputationBuildingBlock):
   """A representation of a placement literal in TFF's internal language.
 
   Currently this can only be `tff.SERVER` or `tff.CLIENTS`.
   """
@@ -837,32 +851,14 @@
   def uri(self):
     return self._literal.uri
 
   def __repr__(self):
     return 'Placement(\'{}\')'.format(self.uri)
 
 
-def compact_representation(comp):
-  """Returns the compact string representation of the given `comp`.
-
-  Args:
-    comp: An instance of a TFF `ComputationBuildingBlock`.
-  """
-  return _string_representation(comp, formatted=False)
-
-
-def formatted_representation(comp):
-  """Returns the formatted string representation of the given `comp`.
-
-  Args:
-    comp: An instance of a TFF `ComputationBuildingBlock`.
-  """
-  return _string_representation(comp, formatted=True)
-
-
 def _string_representation(comp, formatted):
   """Returns the string representation of a `ComputationBuildingBlock`.
 
   This functions creates a `list` of strings representing the given `comp`;
   combines the strings in either a formatted or un-formatted representation; and
   returns the resulting string represetnation.
 
@@ -992,15 +988,15 @@
   lines = [line.rstrip() for line in lines]
   if formatted:
     return '\n'.join(lines)
   else:
     return ''.join(lines)
 
 
-def structural_representation(comp):
+def _structural_representation(comp):
   """Returns the structural string representation of the given `comp`.
 
   This functions creates and returns a string representing the structure of the
   abstract syntax tree for the given `comp`.
 
   Args:
     comp: An instance of a `ComputationBuildingBlock`.
```

## Comparing `tensorflow_federated/python/core/impl/computation_constructing_utils.py` & `tensorflow_federated/python/core/impl/compiler/building_block_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 import tensorflow as tf
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.common_libs import serialization_utils
 from tensorflow_federated.python.core.api import computation_types
-from tensorflow_federated.python.core.impl import computation_building_blocks
-from tensorflow_federated.python.core.impl import graph_utils
-from tensorflow_federated.python.core.impl import intrinsic_defs
-from tensorflow_federated.python.core.impl import placement_literals
-from tensorflow_federated.python.core.impl import transformation_utils
-from tensorflow_federated.python.core.impl import type_serialization
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import building_blocks
+from tensorflow_federated.python.core.impl.compiler import intrinsic_defs
+from tensorflow_federated.python.core.impl.compiler import placement_literals
+from tensorflow_federated.python.core.impl.compiler import transformation_utils
+from tensorflow_federated.python.core.impl.compiler import type_serialization
+from tensorflow_federated.python.core.impl.utils import tensorflow_utils
 
 
 def unique_name_generator(comp, prefix='_var'):
   """Yields a new unique name that does not exist in `comp`.
 
   Args:
     comp: The compuation building block to use as a reference.
@@ -61,45 +61,45 @@
     index += 1
 
 
 def create_compiled_empty_tuple():
   """Returns called graph representing the empty tuple.
 
   Returns:
-    An instance of `computation_building_blocks.Call`, calling a noarg function
+    An instance of `building_blocks.Call`, calling a noarg function
     which returns an empty tuple. This function is an instance of
-    `computation_building_blocks.CompiledComputation`.
+    `building_blocks.CompiledComputation`.
   """
   with tf.Graph().as_default() as graph:
-    result_type, result_binding = graph_utils.capture_result_from_graph([],
-                                                                        graph)
+    result_type, result_binding = tensorflow_utils.capture_result_from_graph(
+        [], graph)
 
   function_type = computation_types.FunctionType(None, result_type)
   serialized_function_type = type_serialization.serialize_type(function_type)
 
   proto = pb.Computation(
       type=serialized_function_type,
       tensorflow=pb.TensorFlow(
           graph_def=serialization_utils.pack_graph_def(graph.as_graph_def()),
           parameter=None,
           result=result_binding))
 
-  return computation_building_blocks.Call(
-      computation_building_blocks.CompiledComputation(proto), None)
+  return building_blocks.Call(building_blocks.CompiledComputation(proto), None)
 
 
-def create_compiled_identity(type_signature):
+def create_compiled_identity(type_signature, name=None):
   """Creates CompiledComputation representing identity function.
 
   Args:
     type_signature: Argument convertible to instance of `computation_types.Type`
       via `computation_types.to_type`.
+    name: An optional string name to use as the name of the computation.
 
   Returns:
-    An instance of `computation_building_blocks.CompiledComputation`
+    An instance of `building_blocks.CompiledComputation`
     representing the identity function taking an argument of type
     `type_signature` and returning the same value.
 
   Raises:
     TypeError: If `type_signature` contains any types which cannot appear in
       TensorFlow bindings.
   """
@@ -107,30 +107,27 @@
   py_typecheck.check_type(type_spec, computation_types.Type)
   if not type_utils.is_tensorflow_compatible_type(type_spec):
     raise TypeError(
         'Can only construct a TF block with types which only contain tensor, '
         'sequence or tuple types; you have tried to construct a TF block with '
         'parameter of type {}'.format(type_spec))
   with tf.Graph().as_default() as graph:
-    parameter_value, parameter_binding = graph_utils.stamp_parameter_in_graph(
+    parameter_value, parameter_binding = tensorflow_utils.stamp_parameter_in_graph(
         'x', type_spec, graph)
-    result_type, result_binding = graph_utils.capture_result_from_graph(
+    result_type, result_binding = tensorflow_utils.capture_result_from_graph(
         parameter_value, graph)
-
   function_type = computation_types.FunctionType(type_spec, result_type)
   serialized_function_type = type_serialization.serialize_type(function_type)
-
   proto = pb.Computation(
       type=serialized_function_type,
       tensorflow=pb.TensorFlow(
           graph_def=serialization_utils.pack_graph_def(graph.as_graph_def()),
           parameter=parameter_binding,
           result=result_binding))
-
-  return computation_building_blocks.CompiledComputation(proto)
+  return building_blocks.CompiledComputation(proto, name)
 
 
 def create_tensorflow_constant(type_spec, scalar_value):
   """Creates called graph returning constant `scalar_value` of type `type_spec`.
 
   `scalar_value` must be a scalar, and cannot be a float if any of the tensor
   leaves of `type_spec` contain an integer data type. `type_spec` must contain
@@ -139,17 +136,17 @@
   Args:
     type_spec: Value convertible to `computation_types.Type` via
       `computation_types.to_type`, and whose resulting type tree can only
       contain named tuples and tensors.
     scalar_value: Scalar value to place in all the tensor leaves of `type_spec`.
 
   Returns:
-    An instance of `computation_building_blocks.Call`, whose argument is `None`
+    An instance of `building_blocks.Call`, whose argument is `None`
     and whose function is a noarg
-    `computation_building_blocks.CompiledComputation` which returns the
+    `building_blocks.CompiledComputation` which returns the
     specified `scalar_value` packed into a TFF structure of type `type_spec.
 
   Raises:
     TypeError: If the type assumptions above are violated.
   """
   type_spec = computation_types.to_type(type_spec)
   py_typecheck.check_type(type_spec, computation_types.Type)
@@ -185,49 +182,49 @@
     """Packs `scalar_value` into `type_spec` recursively."""
     if isinstance(type_spec, computation_types.TensorType):
       type_spec.shape.assert_is_fully_defined()
       result = tf.constant(
           scalar_value, dtype=type_spec.dtype, shape=type_spec.shape)
     else:
       elements = []
-      for _, type_element in anonymous_tuple.to_elements(type_spec):
+      for _, type_element in anonymous_tuple.iter_elements(type_spec):
         elements.append(_create_result_tensor(type_element, scalar_value))
       result = elements
     return result
 
   with tf.Graph().as_default() as graph:
     result = _create_result_tensor(type_spec, scalar_value)
-  _, result_binding = graph_utils.capture_result_from_graph(result, graph)
+  _, result_binding = tensorflow_utils.capture_result_from_graph(result, graph)
 
   function_type = computation_types.FunctionType(None, type_spec)
   serialized_function_type = type_serialization.serialize_type(function_type)
 
   proto = pb.Computation(
       type=serialized_function_type,
       tensorflow=pb.TensorFlow(
           graph_def=serialization_utils.pack_graph_def(graph.as_graph_def()),
           parameter=None,
           result=result_binding))
 
-  noarg_constant_fn = computation_building_blocks.CompiledComputation(proto)
-  return computation_building_blocks.Call(noarg_constant_fn, None)
+  noarg_constant_fn = building_blocks.CompiledComputation(proto)
+  return building_blocks.Call(noarg_constant_fn, None)
 
 
 def create_compiled_input_replication(type_signature, n_replicas):
   """Creates a compiled computation which replicates its argument.
 
   Args:
     type_signature: Value convertible to `computation_types.Type` via
       `computation_types.to_type`. The type of the parameter of the constructed
       computation.
     n_replicas: Integer, the number of times the argument is intended to be
       replicated.
 
   Returns:
-    An instance of `computation_building_blocks.CompiledComputation` encoding
+    An instance of `building_blocks.CompiledComputation` encoding
     a function taking a single argument fo type `type_signature` and returning
     `n_replicas` identical copies of this argument.
 
   Raises:
     TypeError: If `type_signature` contains any types which cannot appear in
       TensorFlow bindings, or if `n_replicas` is not an integer.
   """
@@ -236,44 +233,44 @@
   if not type_utils.is_tensorflow_compatible_type(type_spec):
     raise TypeError(
         'Can only construct a TF block with types which only contain tensor, '
         'sequence or tuple types; you have tried to construct a TF block with '
         'parameter of type {}'.format(type_spec))
   py_typecheck.check_type(n_replicas, int)
   with tf.Graph().as_default() as graph:
-    parameter_value, parameter_binding = graph_utils.stamp_parameter_in_graph(
+    parameter_value, parameter_binding = tensorflow_utils.stamp_parameter_in_graph(
         'x', type_spec, graph)
     result = [parameter_value] * n_replicas
-    result_type, result_binding = graph_utils.capture_result_from_graph(
+    result_type, result_binding = tensorflow_utils.capture_result_from_graph(
         result, graph)
 
   function_type = computation_types.FunctionType(type_spec, result_type)
   serialized_function_type = type_serialization.serialize_type(function_type)
 
   proto = pb.Computation(
       type=serialized_function_type,
       tensorflow=pb.TensorFlow(
           graph_def=serialization_utils.pack_graph_def(graph.as_graph_def()),
           parameter=parameter_binding,
           result=result_binding))
 
-  return computation_building_blocks.CompiledComputation(proto)
+  return building_blocks.CompiledComputation(proto)
 
 
 def create_tensorflow_to_broadcast_scalar(scalar_type, new_shape):
   """Creates TF function broadcasting scalar to shape `new_shape`.
 
   Args:
     scalar_type: Instance of `tf.DType`, the type of the scalar we are looking
       to broadcast.
     new_shape: Instance of `tf.TensorShape`, the shape we wish to broadcast to.
       Must be fully defined.
 
   Returns:
-    Instance of `computation_building_blocks.CompiledComputation` representing
+    Instance of `building_blocks.CompiledComputation` representing
     a function declaring a scalar parameter of dtype `scalar_type`, and
     returning a tensor of this same dtype and shape `new_shape`, with the same
     value in each entry as its scalar argument.
 
   Raises:
     TypeError: If the types of the arguments do not match the declared arg
     types.
@@ -289,32 +286,32 @@
   # revisit the pattern.
   py_typecheck.check_type(scalar_type, tf.DType)
   py_typecheck.check_type(new_shape, tf.TensorShape)
   new_shape.assert_is_fully_defined()
   tensor_spec = computation_types.TensorType(scalar_type, shape=())
 
   with tf.Graph().as_default() as graph:
-    parameter_value, parameter_binding = graph_utils.stamp_parameter_in_graph(
+    parameter_value, parameter_binding = tensorflow_utils.stamp_parameter_in_graph(
         'x', tensor_spec, graph)
     result = tf.broadcast_to(parameter_value, new_shape)
-    result_type, result_binding = graph_utils.capture_result_from_graph(
+    result_type, result_binding = tensorflow_utils.capture_result_from_graph(
         result, graph)
 
   function_type = computation_types.FunctionType(
       computation_types.TensorType(dtype=scalar_type, shape=()), result_type)
   serialized_function_type = type_serialization.serialize_type(function_type)
 
   proto = pb.Computation(
       type=serialized_function_type,
       tensorflow=pb.TensorFlow(
           graph_def=serialization_utils.pack_graph_def(graph.as_graph_def()),
           parameter=parameter_binding,
           result=result_binding))
 
-  return computation_building_blocks.CompiledComputation(proto)
+  return building_blocks.CompiledComputation(proto)
 
 
 def create_tensorflow_binary_operator(operand_type, operator):
   """Creates a TensorFlow computation for the binary `operator`.
 
   For `T` the `operand_type`, the type signature of the constructed operator
   will be `(<T,T> -> U)`, where `U` is the result of applying `operator` to
@@ -335,15 +332,15 @@
   Args:
     operand_type: The type of argument to the constructed binary operator. Must
       be convertible to `computation_types.Type`.
     operator: Callable taking two arguments specifying the operation to encode.
       For example, `tf.add`, `tf.multiply`, `tf.divide`, ...
 
   Returns:
-    Instance of `computation_building_blocks.CompiledComputation` encoding
+    Instance of `building_blocks.CompiledComputation` encoding
     this binary operator.
 
   Raises:
     TypeError: If the type tree of `operand_type` contains any type which is
     incompatible with the TFF generic operators, as checked by
     `type_utils.is_generic_op_compatible_type`, or `operator` is not callable.
   """
@@ -352,30 +349,30 @@
   py_typecheck.check_callable(operator)
   if not type_utils.is_generic_op_compatible_type(operand_type):
     raise TypeError('The type {} contains a type other than '
                     '`computation_types.TensorType` and '
                     '`computation_types.NamedTupleType`; this is disallowed '
                     'in the generic operators.'.format(operand_type))
   with tf.Graph().as_default() as graph:
-    operand_1_value, operand_1_binding = graph_utils.stamp_parameter_in_graph(
+    operand_1_value, operand_1_binding = tensorflow_utils.stamp_parameter_in_graph(
         'x', operand_type, graph)
-    operand_2_value, operand_2_binding = graph_utils.stamp_parameter_in_graph(
+    operand_2_value, operand_2_binding = tensorflow_utils.stamp_parameter_in_graph(
         'y', operand_type, graph)
 
     if isinstance(operand_type, computation_types.TensorType):
       result_value = operator(operand_1_value, operand_2_value)
     elif isinstance(operand_type, computation_types.NamedTupleType):
       result_value = anonymous_tuple.map_structure(operator, operand_1_value,
                                                    operand_2_value)
     else:
       raise TypeError('Operand type {} cannot be used in generic operations. '
                       'The whitelist in '
                       '`type_utils.is_generic_op_compatible_type` has allowed '
                       'it to pass, and should be updated.'.format(operand_type))
-    result_type, result_binding = graph_utils.capture_result_from_graph(
+    result_type, result_binding = tensorflow_utils.capture_result_from_graph(
         result_value, graph)
 
   function_type = computation_types.FunctionType(
       computation_types.NamedTupleType([operand_type, operand_type]),
       result_type)
   serialized_function_type = type_serialization.serialize_type(function_type)
 
@@ -386,154 +383,146 @@
   proto = pb.Computation(
       type=serialized_function_type,
       tensorflow=pb.TensorFlow(
           graph_def=serialization_utils.pack_graph_def(graph.as_graph_def()),
           parameter=parameter_binding,
           result=result_binding))
 
-  return computation_building_blocks.CompiledComputation(proto)
+  return building_blocks.CompiledComputation(proto)
 
 
 def create_federated_getitem_call(arg, idx):
   """Creates computation building block passing getitem to federated value.
 
   Args:
-    arg: Instance of `computation_building_blocks.ComputationBuildingBlock` of
+    arg: Instance of `building_blocks.ComputationBuildingBlock` of
       `computation_types.FederatedType` with member of type
       `computation_types.NamedTupleType` from which we wish to pick out item
       `idx`.
     idx: Index, instance of `int` or `slice` used to address the
       `computation_types.NamedTupleType` underlying `arg`.
 
   Returns:
-    Returns a `computation_building_blocks.Call` with type signature
+    Returns a `building_blocks.Call` with type signature
     `computation_types.FederatedType` of same placement as `arg`, the result
     of applying or mapping the appropriate `__getitem__` function, as defined
     by `idx`.
   """
-  py_typecheck.check_type(arg,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(arg, building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(idx, (int, slice))
   py_typecheck.check_type(arg.type_signature, computation_types.FederatedType)
   py_typecheck.check_type(arg.type_signature.member,
                           computation_types.NamedTupleType)
   getitem_comp = create_federated_getitem_comp(arg, idx)
   return create_federated_map_or_apply(getitem_comp, arg)
 
 
 def create_federated_getattr_call(arg, name):
   """Creates computation building block passing getattr to federated value.
 
   Args:
-    arg: Instance of `computation_building_blocks.ComputationBuildingBlock` of
+    arg: Instance of `building_blocks.ComputationBuildingBlock` of
       `computation_types.FederatedType` with member of type
       `computation_types.NamedTupleType` from which we wish to pick out item
       `name`.
     name: String name to address the `computation_types.NamedTupleType`
       underlying `arg`.
 
   Returns:
-    Returns a `computation_building_blocks.Call` with type signature
+    Returns a `building_blocks.Call` with type signature
     `computation_types.FederatedType` of same placement as `arg`,
     the result of applying or mapping the appropriate `__getattr__` function,
     as defined by `name`.
   """
-  py_typecheck.check_type(arg,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(arg, building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(name, six.string_types)
   py_typecheck.check_type(arg.type_signature, computation_types.FederatedType)
   py_typecheck.check_type(arg.type_signature.member,
                           computation_types.NamedTupleType)
   getattr_comp = create_federated_getattr_comp(arg, name)
   return create_federated_map_or_apply(getattr_comp, arg)
 
 
 def create_federated_setattr_call(federated_comp, name, value_comp):
   """Returns building block for `setattr(name, value_comp)` on `federated_comp`.
 
   Creates an appropriate communication intrinsic (either `federated_map` or
-  `federated_apply`) as well as a `computation_building_blocks.Lambda`
+  `federated_apply`) as well as a `building_blocks.Lambda`
   representing setting the `name` attribute of `federated_comp`'s `member` to
   `value_comp`, and stitches these together in a call.
 
   Notice that `federated_comp`'s `member` must actually define a `name`
   attribute; this is enforced to avoid the need to worry about theplacement of a
   previously undefined name.
 
   Args:
-    federated_comp: Instance of
-      `computation_building_blocks.ComputationBuildingBlock` of type
-      `computation_types.FederatedType`, with member of type
+    federated_comp: Instance of `building_blocks.ComputationBuildingBlock` of
+      type `computation_types.FederatedType`, with member of type
       `computation_types.NamedTupleType` whose attribute `name` we wish to set
       to `value_comp`.
     name: String name of the attribute we wish to overwrite in `federated_comp`.
-    value_comp: Instance of
-      `computation_building_blocks.ComputationBuildingBlock`, the value to
-      assign to `federated_comp`'s `member`'s `name` attribute.
+    value_comp: Instance of `building_blocks.ComputationBuildingBlock`, the
+      value to assign to `federated_comp`'s `member`'s `name` attribute.
 
   Returns:
-    Instance of `computation_building_blocks.ComputationBuildingBlock`
+    Instance of `building_blocks.ComputationBuildingBlock`
     representing `federated_comp` with its `member`'s `name` attribute set to
     `value`.
   """
   py_typecheck.check_type(federated_comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+                          building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(name, six.string_types)
-  py_typecheck.check_type(value_comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value_comp, building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(federated_comp.type_signature,
                           computation_types.FederatedType)
   py_typecheck.check_type(federated_comp.type_signature.member,
                           computation_types.NamedTupleType)
   named_tuple_type_signature = federated_comp.type_signature.member
   setattr_lambda = create_named_tuple_setattr_lambda(named_tuple_type_signature,
                                                      name, value_comp)
   return create_federated_map_or_apply(setattr_lambda, federated_comp)
 
 
 def create_named_tuple_setattr_lambda(named_tuple_signature, name, value_comp):
   """Creates a building block for replacing one attribute in a named tuple.
 
-  Returns an instance of `computation_building_blocks.Lambda` which takes an
+  Returns an instance of `building_blocks.Lambda` which takes an
   argument of type `computation_types.NamedTupleType` and returns a
-  `computation_building_blocks.Tuple` which contains all the same elements as
+  `building_blocks.Tuple` which contains all the same elements as
   the argument, except the attribute `name` now has value `value_comp`. The
   Lambda constructed is the analogue of Python's `setattr` for the concrete
   type `named_tuple_signature`.
 
   Args:
     named_tuple_signature: Instance of `computation_types.NamedTupleType`, the
-      type of the argument to the constructed
-      `computation_building_blocks.Lambda`.
+      type of the argument to the constructed `building_blocks.Lambda`.
     name: String name of the attribute in the `named_tuple_signature` to replace
       with `value_comp`. Must be present as a name in `named_tuple_signature;
       otherwise we will raise an `AttributeError`.
-    value_comp: Instance of
-      `computation_building_blocks.ComputationBuildingBlock`, the value to place
-      as attribute `name` in the argument of the returned function.
+    value_comp: Instance of `building_blocks.ComputationBuildingBlock`, the
+      value to place as attribute `name` in the argument of the returned
+      function.
 
   Returns:
-    An instance of `computation_building_blocks.Block` of functional type
+    An instance of `building_blocks.Block` of functional type
     representing setting attribute `name` to value `value_comp` in its argument
     of type `named_tuple_signature`.
 
   Raises:
     TypeError: If the types of the arguments don't match the assumptions above.
     AttributeError: If `name` is not present as a named element in
       `named_tuple_signature`
   """
   py_typecheck.check_type(named_tuple_signature,
                           computation_types.NamedTupleType)
   py_typecheck.check_type(name, six.string_types)
-  py_typecheck.check_type(value_comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  value_comp_placeholder = computation_building_blocks.Reference(
-      'value_comp_placeholder', value_comp.type_signature)
-  lambda_arg = computation_building_blocks.Reference('lambda_arg',
-                                                     named_tuple_signature)
+  py_typecheck.check_type(value_comp, building_blocks.ComputationBuildingBlock)
+  value_comp_placeholder = building_blocks.Reference('value_comp_placeholder',
+                                                     value_comp.type_signature)
+  lambda_arg = building_blocks.Reference('lambda_arg', named_tuple_signature)
   if name not in dir(named_tuple_signature):
     raise AttributeError(
         'There is no such attribute as \'{}\' in this federated tuple. '
         'TFF does not allow for assigning to a nonexistent attribute. '
         'If you want to assign to \'{}\', you must create a new named tuple '
         'containing this attribute.'.format(name, name))
   elements = []
@@ -543,103 +532,95 @@
       if not type_utils.is_assignable_from(element_type,
                                            value_comp.type_signature):
         raise TypeError(
             '`setattr` has attempted to set element {} of type {} with incompatible type {}'
             .format(key, element_type, value_comp.type_signature))
       elements.append((key, value_comp_placeholder))
     else:
-      elements.append(
-          (key, computation_building_blocks.Selection(lambda_arg, index=idx)))
-  return_tuple = computation_building_blocks.Tuple(elements)
-  lambda_to_return = computation_building_blocks.Lambda(lambda_arg.name,
-                                                        named_tuple_signature,
-                                                        return_tuple)
+      elements.append((key, building_blocks.Selection(lambda_arg, index=idx)))
+  return_tuple = building_blocks.Tuple(elements)
+  lambda_to_return = building_blocks.Lambda(lambda_arg.name,
+                                            named_tuple_signature, return_tuple)
   symbols = ((value_comp_placeholder.name, value_comp),)
-  return computation_building_blocks.Block(symbols, lambda_to_return)
+  return building_blocks.Block(symbols, lambda_to_return)
 
 
 def create_federated_getattr_comp(comp, name):
   """Function to construct computation for `federated_apply` of `__getattr__`.
 
-  Creates a `computation_building_blocks.ComputationBuildingBlock`
+  Creates a `building_blocks.ComputationBuildingBlock`
   which selects `name` from its argument, of type `comp.type_signature.member`,
   an instance of `computation_types.NamedTupleType`.
 
   Args:
-    comp: Instance of `computation_building_blocks.ComputationBuildingBlock`
-      with type signature `computation_types.FederatedType` whose `member`
-      attribute is of type `computation_types.NamedTupleType`.
+    comp: Instance of `building_blocks.ComputationBuildingBlock` with type
+      signature `computation_types.FederatedType` whose `member` attribute is of
+      type `computation_types.NamedTupleType`.
     name: String name of attribute to grab.
 
   Returns:
-    Instance of `computation_building_blocks.Lambda` which grabs attribute
+    Instance of `building_blocks.Lambda` which grabs attribute
       according to `name` of its argument.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(comp.type_signature, computation_types.FederatedType)
   py_typecheck.check_type(comp.type_signature.member,
                           computation_types.NamedTupleType)
   py_typecheck.check_type(name, six.string_types)
   element_names = [
-      x for x, _ in anonymous_tuple.to_elements(comp.type_signature.member)
+      x for x, _ in anonymous_tuple.iter_elements(comp.type_signature.member)
   ]
   if name not in element_names:
-    raise ValueError('The federated value {} has no element of name {}'.format(
-        comp, name))
-  apply_input = computation_building_blocks.Reference(
-      'x', comp.type_signature.member)
-  selected = computation_building_blocks.Selection(apply_input, name=name)
-  apply_lambda = computation_building_blocks.Lambda('x',
-                                                    apply_input.type_signature,
-                                                    selected)
+    raise ValueError(
+        'The federated value has no element of name `{}`. Value: {}'.format(
+            name, comp.formatted_representation()))
+  apply_input = building_blocks.Reference('x', comp.type_signature.member)
+  selected = building_blocks.Selection(apply_input, name=name)
+  apply_lambda = building_blocks.Lambda('x', apply_input.type_signature,
+                                        selected)
   return apply_lambda
 
 
 def create_federated_getitem_comp(comp, key):
   """Function to construct computation for `federated_apply` of `__getitem__`.
 
-  Creates a `computation_building_blocks.ComputationBuildingBlock`
+  Creates a `building_blocks.ComputationBuildingBlock`
   which selects `key` from its argument, of type `comp.type_signature.member`,
   of type `computation_types.NamedTupleType`.
 
   Args:
-    comp: Instance of `computation_building_blocks.ComputationBuildingBlock`
-      with type signature `computation_types.FederatedType` whose `member`
-      attribute is of type `computation_types.NamedTupleType`.
+    comp: Instance of `building_blocks.ComputationBuildingBlock` with type
+      signature `computation_types.FederatedType` whose `member` attribute is of
+      type `computation_types.NamedTupleType`.
     key: Instance of `int` or `slice`, key used to grab elements from the member
       of `comp`. implementation of slicing for `ValueImpl` objects with
       `type_signature` `computation_types.NamedTupleType`.
 
   Returns:
-    Instance of `computation_building_blocks.Lambda` which grabs slice
+    Instance of `building_blocks.Lambda` which grabs slice
       according to `key` of its argument.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(comp.type_signature, computation_types.FederatedType)
   py_typecheck.check_type(comp.type_signature.member,
                           computation_types.NamedTupleType)
   py_typecheck.check_type(key, (int, slice))
-  apply_input = computation_building_blocks.Reference(
-      'x', comp.type_signature.member)
+  apply_input = building_blocks.Reference('x', comp.type_signature.member)
   if isinstance(key, int):
-    selected = computation_building_blocks.Selection(apply_input, index=key)
+    selected = building_blocks.Selection(apply_input, index=key)
   else:
     elems = anonymous_tuple.to_elements(comp.type_signature.member)
     index_range = range(*key.indices(len(elems)))
     elem_list = []
     for k in index_range:
       elem_list.append(
-          (elems[k][0],
-           computation_building_blocks.Selection(apply_input, index=k)))
-    selected = computation_building_blocks.Tuple(elem_list)
-  apply_lambda = computation_building_blocks.Lambda('x',
-                                                    apply_input.type_signature,
-                                                    selected)
+          (elems[k][0], building_blocks.Selection(apply_input, index=k)))
+    selected = building_blocks.Tuple(elem_list)
+  apply_lambda = building_blocks.Lambda('x', apply_input.type_signature,
+                                        selected)
   return apply_lambda
 
 
 def create_computation_appending(comp1, comp2):
   r"""Returns a block appending `comp2` to `comp1`.
 
                 Block
@@ -649,299 +630,277 @@
     [Comp, Comp]      [Sel(0), ...,  Sel(0),   Sel(1)]
                              \             \         \
                               Sel(0)        Sel(n)    Ref(comps)
                                     \             \
                                      Ref(comps)    Ref(comps)
 
   Args:
-    comp1: A `computation_building_blocks.ComputationBuildingBlock` with a
-      `type_signature` of type `computation_type.NamedTupleType`.
-    comp2: A `computation_building_blocks.ComputationBuildingBlock` or a named
-      computation (a tuple pair of name, computation) representing a single
-      element of an `anonymous_tuple.AnonymousTuple`.
+    comp1: A `building_blocks.ComputationBuildingBlock` with a `type_signature`
+      of type `computation_type.NamedTupleType`.
+    comp2: A `building_blocks.ComputationBuildingBlock` or a named computation
+      (a tuple pair of name, computation) representing a single element of an
+      `anonymous_tuple.AnonymousTuple`.
 
   Returns:
-    A `computation_building_blocks.Block`.
+    A `building_blocks.Block`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(comp1,
-                          computation_building_blocks.ComputationBuildingBlock)
-  if isinstance(comp2, computation_building_blocks.ComputationBuildingBlock):
+  py_typecheck.check_type(comp1, building_blocks.ComputationBuildingBlock)
+  if isinstance(comp2, building_blocks.ComputationBuildingBlock):
     name2 = None
   elif py_typecheck.is_name_value_pair(
       comp2,
       name_required=False,
-      value_type=computation_building_blocks.ComputationBuildingBlock):
+      value_type=building_blocks.ComputationBuildingBlock):
     name2, comp2 = comp2
   else:
     raise TypeError('Unexpected tuple element: {}.'.format(comp2))
-  comps = computation_building_blocks.Tuple((comp1, comp2))
-  ref = computation_building_blocks.Reference('comps', comps.type_signature)
-  sel_0 = computation_building_blocks.Selection(ref, index=0)
+  comps = building_blocks.Tuple((comp1, comp2))
+  ref = building_blocks.Reference('comps', comps.type_signature)
+  sel_0 = building_blocks.Selection(ref, index=0)
   elements = []
   named_type_signatures = anonymous_tuple.to_elements(comp1.type_signature)
   for index, (name, _) in enumerate(named_type_signatures):
-    sel = computation_building_blocks.Selection(sel_0, index=index)
+    sel = building_blocks.Selection(sel_0, index=index)
     elements.append((name, sel))
-  sel_1 = computation_building_blocks.Selection(ref, index=1)
+  sel_1 = building_blocks.Selection(ref, index=1)
   elements.append((name2, sel_1))
-  result = computation_building_blocks.Tuple(elements)
+  result = building_blocks.Tuple(elements)
   symbols = ((ref.name, comps),)
-  return computation_building_blocks.Block(symbols, result)
+  return building_blocks.Block(symbols, result)
 
 
 def create_federated_aggregate(value, zero, accumulate, merge, report):
   r"""Creates a called federated aggregate.
 
             Call
            /    \
   Intrinsic      Tuple
                  |
                  [Comp, Comp, Comp, Comp, Comp]
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the value.
-    zero: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      initial value.
-    accumulate: A `computation_building_blocks.ComputationBuildingBlock` to use
-      as the accumulate function.
-    merge: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the merge function.
-    report: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the report function.
+    value: A `building_blocks.ComputationBuildingBlock` to use as the value.
+    zero: A `building_blocks.ComputationBuildingBlock` to use as the initial
+      value.
+    accumulate: A `building_blocks.ComputationBuildingBlock` to use as the
+      accumulate function.
+    merge: A `building_blocks.ComputationBuildingBlock` to use as the merge
+      function.
+    report: A `building_blocks.ComputationBuildingBlock` to use as the report
+      function.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(zero,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(accumulate,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(merge,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(report,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(zero, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(accumulate, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(merge, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(report, building_blocks.ComputationBuildingBlock)
+  # Its okay if the first argument of accumulate is assignable from the zero,
+  # without being the exact type. This occurs when accumulate has a type like
+  # (<int32[?], int32> -> int32[?]) but zero is int32[0].
+  zero_arg_type = accumulate.type_signature.parameter[0]
+  type_utils.check_assignable_from(zero_arg_type, zero.type_signature)
   result_type = computation_types.FederatedType(report.type_signature.result,
                                                 placement_literals.SERVER)
+
   intrinsic_type = computation_types.FunctionType((
       type_utils.to_non_all_equal(value.type_signature),
-      zero.type_signature,
+      zero_arg_type,
       accumulate.type_signature,
       merge.type_signature,
       report.type_signature,
   ), result_type)
-  intrinsic = computation_building_blocks.Intrinsic(
-      intrinsic_defs.FEDERATED_AGGREGATE.uri, intrinsic_type)
-  values = computation_building_blocks.Tuple(
-      (value, zero, accumulate, merge, report))
-  return computation_building_blocks.Call(intrinsic, values)
+  intrinsic = building_blocks.Intrinsic(intrinsic_defs.FEDERATED_AGGREGATE.uri,
+                                        intrinsic_type)
+  values = building_blocks.Tuple((value, zero, accumulate, merge, report))
+  return building_blocks.Call(intrinsic, values)
 
 
 def create_federated_apply(fn, arg):
   r"""Creates a called federated apply.
 
             Call
            /    \
   Intrinsic      Tuple
                  |
                  [Comp, Comp]
 
   Args:
-    fn: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      function.
-    arg: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      argument.
+    fn: A `building_blocks.ComputationBuildingBlock` to use as the function.
+    arg: A `building_blocks.ComputationBuildingBlock` to use as the argument.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(fn,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(arg,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(fn, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(arg, building_blocks.ComputationBuildingBlock)
   result_type = computation_types.FederatedType(fn.type_signature.result,
                                                 placement_literals.SERVER)
   intrinsic_type = computation_types.FunctionType(
       (fn.type_signature, arg.type_signature), result_type)
-  intrinsic = computation_building_blocks.Intrinsic(
-      intrinsic_defs.FEDERATED_APPLY.uri, intrinsic_type)
-  values = computation_building_blocks.Tuple((fn, arg))
-  return computation_building_blocks.Call(intrinsic, values)
+  intrinsic = building_blocks.Intrinsic(intrinsic_defs.FEDERATED_APPLY.uri,
+                                        intrinsic_type)
+  values = building_blocks.Tuple((fn, arg))
+  return building_blocks.Call(intrinsic, values)
 
 
 def create_federated_broadcast(value):
   r"""Creates a called federated broadcast.
 
             Call
            /    \
   Intrinsic      Comp
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the value.
+    value: A `building_blocks.ComputationBuildingBlock` to use as the value.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   result_type = computation_types.FederatedType(
       value.type_signature.member, placement_literals.CLIENTS, all_equal=True)
   intrinsic_type = computation_types.FunctionType(value.type_signature,
                                                   result_type)
-  intrinsic = computation_building_blocks.Intrinsic(
-      intrinsic_defs.FEDERATED_BROADCAST.uri, intrinsic_type)
-  return computation_building_blocks.Call(intrinsic, value)
+  intrinsic = building_blocks.Intrinsic(intrinsic_defs.FEDERATED_BROADCAST.uri,
+                                        intrinsic_type)
+  return building_blocks.Call(intrinsic, value)
 
 
 def create_federated_collect(value):
   r"""Creates a called federated collect.
 
             Call
            /    \
   Intrinsic      Comp
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the value.
+    value: A `building_blocks.ComputationBuildingBlock` to use as the value.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   type_signature = computation_types.SequenceType(value.type_signature.member)
   result_type = computation_types.FederatedType(type_signature,
                                                 placement_literals.SERVER)
-  intrinsic_type = computation_types.FunctionType(value.type_signature,
-                                                  result_type)
-  intrinsic = computation_building_blocks.Intrinsic(
-      intrinsic_defs.FEDERATED_COLLECT.uri, intrinsic_type)
-  return computation_building_blocks.Call(intrinsic, value)
+  intrinsic_type = computation_types.FunctionType(
+      type_utils.to_non_all_equal(value.type_signature), result_type)
+  intrinsic = building_blocks.Intrinsic(intrinsic_defs.FEDERATED_COLLECT.uri,
+                                        intrinsic_type)
+  return building_blocks.Call(intrinsic, value)
 
 
 def create_federated_map(fn, arg):
   r"""Creates a called federated map.
 
             Call
            /    \
   Intrinsic      Tuple
                  |
                  [Comp, Comp]
 
   Args:
-    fn: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      function.
-    arg: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      argument.
+    fn: A `building_blocks.ComputationBuildingBlock` to use as the function.
+    arg: A `building_blocks.ComputationBuildingBlock` to use as the argument.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(fn,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(arg,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(fn, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(arg, building_blocks.ComputationBuildingBlock)
   parameter_type = computation_types.FederatedType(arg.type_signature.member,
                                                    placement_literals.CLIENTS)
   result_type = computation_types.FederatedType(fn.type_signature.result,
                                                 placement_literals.CLIENTS)
   intrinsic_type = computation_types.FunctionType(
       (fn.type_signature, parameter_type), result_type)
-  intrinsic = computation_building_blocks.Intrinsic(
-      intrinsic_defs.FEDERATED_MAP.uri, intrinsic_type)
-  values = computation_building_blocks.Tuple((fn, arg))
-  return computation_building_blocks.Call(intrinsic, values)
+  intrinsic = building_blocks.Intrinsic(intrinsic_defs.FEDERATED_MAP.uri,
+                                        intrinsic_type)
+  values = building_blocks.Tuple((fn, arg))
+  return building_blocks.Call(intrinsic, values)
 
 
 def create_federated_map_all_equal(fn, arg):
   r"""Creates a called federated map of equal values.
 
             Call
            /    \
   Intrinsic      Tuple
                  |
                  [Comp, Comp]
 
   NOTE: The `fn` is required to be deterministic and therefore should contain no
-  `computation_building_blocks.CompiledComputations`.
+  `building_blocks.CompiledComputations`.
 
   Args:
-    fn: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      function.
-    arg: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      argument.
+    fn: A `building_blocks.ComputationBuildingBlock` to use as the function.
+    arg: A `building_blocks.ComputationBuildingBlock` to use as the argument.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(fn,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(arg,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(fn, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(arg, building_blocks.ComputationBuildingBlock)
   parameter_type = computation_types.FederatedType(
       arg.type_signature.member, placement_literals.CLIENTS, all_equal=True)
   result_type = computation_types.FederatedType(
       fn.type_signature.result, placement_literals.CLIENTS, all_equal=True)
   intrinsic_type = computation_types.FunctionType(
       (fn.type_signature, parameter_type), result_type)
-  intrinsic = computation_building_blocks.Intrinsic(
+  intrinsic = building_blocks.Intrinsic(
       intrinsic_defs.FEDERATED_MAP_ALL_EQUAL.uri, intrinsic_type)
-  values = computation_building_blocks.Tuple((fn, arg))
-  return computation_building_blocks.Call(intrinsic, values)
+  values = building_blocks.Tuple((fn, arg))
+  return building_blocks.Call(intrinsic, values)
 
 
 def create_federated_map_or_apply(fn, arg):
   r"""Creates a called federated map or apply depending on `arg`s placement.
 
             Call
            /    \
   Intrinsic      Tuple
                  |
                  [Comp, Comp]
 
   Args:
-    fn: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      function.
-    arg: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      argument.
+    fn: A `building_blocks.ComputationBuildingBlock` to use as the function.
+    arg: A `building_blocks.ComputationBuildingBlock` to use as the argument.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(fn,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(arg,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(fn, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(arg, building_blocks.ComputationBuildingBlock)
   if arg.type_signature.placement is placement_literals.CLIENTS:
     if arg.type_signature.all_equal:
       return create_federated_map_all_equal(fn, arg)
     else:
       return create_federated_map(fn, arg)
   elif arg.type_signature.placement is placement_literals.SERVER:
     return create_federated_apply(fn, arg)
@@ -956,115 +915,106 @@
             Call
            /    \
   Intrinsic      Tuple
                  |
                  [Comp, Comp]
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the value.
-    weight: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the weight or `None`.
+    value: A `building_blocks.ComputationBuildingBlock` to use as the value.
+    weight: A `building_blocks.ComputationBuildingBlock` to use as the weight or
+      `None`.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   if weight is not None:
-    py_typecheck.check_type(
-        weight, computation_building_blocks.ComputationBuildingBlock)
+    py_typecheck.check_type(weight, building_blocks.ComputationBuildingBlock)
   result_type = computation_types.FederatedType(value.type_signature.member,
                                                 placement_literals.SERVER)
   if weight is not None:
     intrinsic_type = computation_types.FunctionType(
-        (value.type_signature, weight.type_signature), result_type)
-    intrinsic = computation_building_blocks.Intrinsic(
+        (type_utils.to_non_all_equal(value.type_signature),
+         type_utils.to_non_all_equal(weight.type_signature)), result_type)
+    intrinsic = building_blocks.Intrinsic(
         intrinsic_defs.FEDERATED_WEIGHTED_MEAN.uri, intrinsic_type)
-    values = computation_building_blocks.Tuple((value, weight))
-    return computation_building_blocks.Call(intrinsic, values)
+    values = building_blocks.Tuple((value, weight))
+    return building_blocks.Call(intrinsic, values)
   else:
-    intrinsic_type = computation_types.FunctionType(value.type_signature,
-                                                    result_type)
-    intrinsic = computation_building_blocks.Intrinsic(
-        intrinsic_defs.FEDERATED_MEAN.uri, intrinsic_type)
-    return computation_building_blocks.Call(intrinsic, value)
+    intrinsic_type = computation_types.FunctionType(
+        type_utils.to_non_all_equal(value.type_signature), result_type)
+    intrinsic = building_blocks.Intrinsic(intrinsic_defs.FEDERATED_MEAN.uri,
+                                          intrinsic_type)
+    return building_blocks.Call(intrinsic, value)
 
 
 def create_federated_reduce(value, zero, op):
   r"""Creates a called federated reduce.
 
             Call
            /    \
   Intrinsic      Tuple
                  |
                  [Comp, Comp, Comp]
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the value.
-    zero: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      initial value.
-    op: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      op function.
+    value: A `building_blocks.ComputationBuildingBlock` to use as the value.
+    zero: A `building_blocks.ComputationBuildingBlock` to use as the initial
+      value.
+    op: A `building_blocks.ComputationBuildingBlock` to use as the op function.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(zero,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(op,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(zero, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(op, building_blocks.ComputationBuildingBlock)
   result_type = computation_types.FederatedType(op.type_signature.result,
                                                 placement_literals.SERVER)
   intrinsic_type = computation_types.FunctionType((
       type_utils.to_non_all_equal(value.type_signature),
       zero.type_signature,
       op.type_signature,
   ), result_type)
-  intrinsic = computation_building_blocks.Intrinsic(
-      intrinsic_defs.FEDERATED_REDUCE.uri, intrinsic_type)
-  values = computation_building_blocks.Tuple((value, zero, op))
-  return computation_building_blocks.Call(intrinsic, values)
+  intrinsic = building_blocks.Intrinsic(intrinsic_defs.FEDERATED_REDUCE.uri,
+                                        intrinsic_type)
+  values = building_blocks.Tuple((value, zero, op))
+  return building_blocks.Call(intrinsic, values)
 
 
 def create_federated_sum(value):
   r"""Creates a called federated sum.
 
             Call
            /    \
   Intrinsic      Comp
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the value.
+    value: A `building_blocks.ComputationBuildingBlock` to use as the value.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   result_type = computation_types.FederatedType(value.type_signature.member,
                                                 placement_literals.SERVER)
   intrinsic_type = computation_types.FunctionType(
       type_utils.to_non_all_equal(value.type_signature), result_type)
-  intrinsic = computation_building_blocks.Intrinsic(
-      intrinsic_defs.FEDERATED_SUM.uri, intrinsic_type)
-  return computation_building_blocks.Call(intrinsic, value)
+  intrinsic = building_blocks.Intrinsic(intrinsic_defs.FEDERATED_SUM.uri,
+                                        intrinsic_type)
+  return building_blocks.Call(intrinsic, value)
 
 
 def create_federated_unzip(value):
   r"""Creates a tuple of called federated maps or applies.
 
                 Block
                /     \
@@ -1080,79 +1030,74 @@
                                    \                            \
                                     Ref(arg)                     Ref(arg)
 
   This function returns a tuple of federated values given a `value` with a
   federated tuple type signature.
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` with a
-      `type_signature` of type `computation_types.NamedTupleType` containing at
-      least one element.
+    value: A `building_blocks.ComputationBuildingBlock` with a `type_signature`
+      of type `computation_types.NamedTupleType` containing at least one
+      element.
 
   Returns:
-    A `computation_building_blocks.Block`.
+    A `building_blocks.Block`.
 
   Raises:
     TypeError: If any of the types do not match.
     ValueError: If `value` does not contain any elements.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   named_type_signatures = anonymous_tuple.to_elements(
       value.type_signature.member)
   length = len(named_type_signatures)
   if length == 0:
     raise ValueError('federated_zip is only supported on non-empty tuples.')
-  value_ref = computation_building_blocks.Reference('value',
-                                                    value.type_signature)
+  value_ref = building_blocks.Reference('value', value.type_signature)
   elements = []
-  fn_ref = computation_building_blocks.Reference('arg', named_type_signatures)
+  fn_ref = building_blocks.Reference('arg', named_type_signatures)
   for index, (name, _) in enumerate(named_type_signatures):
-    sel = computation_building_blocks.Selection(fn_ref, index=index)
-    fn = computation_building_blocks.Lambda(fn_ref.name, fn_ref.type_signature,
-                                            sel)
+    sel = building_blocks.Selection(fn_ref, index=index)
+    fn = building_blocks.Lambda(fn_ref.name, fn_ref.type_signature, sel)
     intrinsic = create_federated_map_or_apply(fn, value_ref)
     elements.append((name, intrinsic))
-  result = computation_building_blocks.Tuple(elements)
+  result = building_blocks.Tuple(elements)
   symbols = ((value_ref.name, value),)
-  return computation_building_blocks.Block(symbols, result)
+  return building_blocks.Block(symbols, result)
 
 
 def create_federated_value(value, placement):
   r"""Creates a called federated value.
 
             Call
            /    \
   Intrinsic      Comp
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the value.
+    value: A `building_blocks.ComputationBuildingBlock` to use as the value.
     placement: A `placement_literals.PlacementLiteral` to use as the placement.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   if placement is placement_literals.CLIENTS:
     uri = intrinsic_defs.FEDERATED_VALUE_AT_CLIENTS.uri
   elif placement is placement_literals.SERVER:
     uri = intrinsic_defs.FEDERATED_VALUE_AT_SERVER.uri
   else:
     raise TypeError('Unsupported placement {}.'.format(placement))
   result_type = computation_types.FederatedType(
       value.type_signature, placement, all_equal=True)
   intrinsic_type = computation_types.FunctionType(value.type_signature,
                                                   result_type)
-  intrinsic = computation_building_blocks.Intrinsic(uri, intrinsic_type)
-  return computation_building_blocks.Call(intrinsic, value)
+  intrinsic = building_blocks.Intrinsic(uri, intrinsic_type)
+  return building_blocks.Call(intrinsic, value)
 
 
 def create_federated_zip(value):
   r"""Creates a called federated zip.
 
             Call
            /    \
@@ -1160,55 +1105,121 @@
                  |
                  [Comp, Comp]
 
   This function returns a federated tuple given a `value` with a tuple of
   federated values type signature.
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` with a
-      `type_signature` of type `computation_types.NamedTupleType` containing at
-      least one element.
+    value: A `building_blocks.ComputationBuildingBlock` with a `type_signature`
+      of type `computation_types.NamedTupleType` containing at least one
+      element.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
     ValueError: If `value` does not contain any elements.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   named_type_signatures = anonymous_tuple.to_elements(value.type_signature)
   names_to_add = [name for name, _ in named_type_signatures]
   length = len(named_type_signatures)
   if length == 0:
     raise ValueError('federated_zip is only supported on non-empty tuples.')
   first_name, first_type_signature = named_type_signatures[0]
   if first_type_signature.placement == placement_literals.CLIENTS:
     map_fn = create_federated_map
   elif first_type_signature.placement == placement_literals.SERVER:
     map_fn = create_federated_apply
   else:
     raise TypeError('Unsupported placement {}.'.format(
         first_type_signature.placement))
   if length == 1:
-    ref = computation_building_blocks.Reference('arg',
-                                                first_type_signature.member)
-    values = computation_building_blocks.Tuple(((first_name, ref),))
-    fn = computation_building_blocks.Lambda(ref.name, ref.type_signature,
-                                            values)
-    sel = computation_building_blocks.Selection(value, index=0)
+    ref = building_blocks.Reference('arg', first_type_signature.member)
+    values = building_blocks.Tuple(((first_name, ref),))
+    fn = building_blocks.Lambda(ref.name, ref.type_signature, values)
+    sel = building_blocks.Selection(value, index=0)
     return map_fn(fn, sel)
   else:
     zipped_args = _create_chain_zipped_values(value)
     append_fn = _create_fn_to_append_chain_zipped_values(value)
     unnamed_zip = map_fn(append_fn, zipped_args)
     return create_named_federated_tuple(unnamed_zip, names_to_add)
 
 
+def create_generic_constant(type_spec, scalar_value):
+  """Creates constant for a combination of federated, tuple and tensor types.
+
+  Args:
+    type_spec: Instance of `computation_types.Type` containing only federated,
+      tuple or tensor types for which we wish to construct a generic constant.
+      May also be something convertible to a `computation_types.Type` via
+      `computation_types.to_type`.
+    scalar_value: The scalar value we wish this constant to have.
+
+  Returns:
+    Instance of `building_blocks.ComputationBuildingBlock`
+    representing `scalar_value` packed into `type_spec`.
+
+  Raises:
+    TypeError: If types don't match their specification in the args section.
+      Notice validation of consistency of `type_spec` with `scalar_value` is not
+      the rsponsibility of this function.
+  """
+  type_spec = computation_types.to_type(type_spec)
+  py_typecheck.check_type(type_spec, computation_types.Type)
+  inferred_scalar_value_type = type_utils.infer_type(scalar_value)
+  if (not isinstance(inferred_scalar_value_type, computation_types.TensorType)
+      or inferred_scalar_value_type.shape != tf.TensorShape(())):
+    raise TypeError(
+        'Must pass a scalar value to `create_generic_constant`; encountered a '
+        'value {}'.format(scalar_value))
+  if not type_utils.type_tree_contains_only(type_spec, (
+      computation_types.FederatedType,
+      computation_types.NamedTupleType,
+      computation_types.TensorType,
+  )):
+    raise TypeError
+  if type_utils.type_tree_contains_only(type_spec, (
+      computation_types.NamedTupleType,
+      computation_types.TensorType,
+  )):
+    return create_tensorflow_constant(type_spec, scalar_value)
+  elif isinstance(type_spec, computation_types.FederatedType):
+    unplaced_zero = create_tensorflow_constant(type_spec.member, scalar_value)
+    if type_spec.placement == placement_literals.CLIENTS:
+      placement_federated_type = computation_types.FederatedType(
+          type_spec.member, type_spec.placement, all_equal=True)
+      placement_fn_type = computation_types.FunctionType(
+          type_spec.member, placement_federated_type)
+      placement_function = building_blocks.Intrinsic(
+          intrinsic_defs.FEDERATED_VALUE_AT_CLIENTS.uri, placement_fn_type)
+    elif type_spec.placement == placement_literals.SERVER:
+      placement_federated_type = computation_types.FederatedType(
+          type_spec.member, type_spec.placement, all_equal=True)
+      placement_fn_type = computation_types.FunctionType(
+          type_spec.member, placement_federated_type)
+      placement_function = building_blocks.Intrinsic(
+          intrinsic_defs.FEDERATED_VALUE_AT_SERVER.uri, placement_fn_type)
+    return building_blocks.Call(placement_function, unplaced_zero)
+  elif isinstance(type_spec, computation_types.NamedTupleType):
+    elements = []
+    for k in range(len(type_spec)):
+      elements.append(create_generic_constant(type_spec[k], scalar_value))
+    names = [name for name, _ in anonymous_tuple.iter_elements(type_spec)]
+    packed_elements = building_blocks.Tuple(elements)
+    named_tuple = create_named_tuple(packed_elements, names)
+    return named_tuple
+  else:
+    raise ValueError(
+        'The type_spec {} has slipped through all our '
+        'generic constant cases, and failed to raise.'.format(type_spec))
+
+
 def _create_chain_zipped_values(value):
   r"""Creates a chain of called federated zip with two values.
 
                 Block--------
                /             \
   [value=Tuple]               Call
          |                   /    \
@@ -1230,42 +1241,41 @@
   system is an element of the type proper. That is, a named tuple type of
   length 2 is a different type than a named tuple type of length 3, they are
   not simply items with the same type and different values, as would be the
   case if you were thinking of these as Python `list`s. It may be better to
   think of named tuple types in TFF as more like `struct`s.
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` with a
-      `type_signature` of type `computation_types.NamedTupleType` containing at
-      least two elements.
+    value: A `building_blocks.ComputationBuildingBlock` with a `type_signature`
+      of type `computation_types.NamedTupleType` containing at least two
+      elements.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
     ValueError: If `value` does not contain at least two elements.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   named_type_signatures = anonymous_tuple.to_elements(value.type_signature)
   length = len(named_type_signatures)
   if length < 2:
     raise ValueError(
         'Expected a value with at least two elements, received {} elements.'
         .format(named_type_signatures))
-  ref = computation_building_blocks.Reference('value', value.type_signature)
+  ref = building_blocks.Reference('value', value.type_signature)
   symbols = ((ref.name, value),)
-  sel_0 = computation_building_blocks.Selection(ref, index=0)
+  sel_0 = building_blocks.Selection(ref, index=0)
   result = sel_0
   for i in range(1, length):
-    sel = computation_building_blocks.Selection(ref, index=i)
-    values = computation_building_blocks.Tuple((result, sel))
+    sel = building_blocks.Selection(ref, index=i)
+    values = building_blocks.Tuple((result, sel))
     result = create_zip_two_values(values)
-  return computation_building_blocks.Block(symbols, result)
+  return building_blocks.Block(symbols, result)
 
 
 def create_zip_two_values(value):
   r"""Creates a called federated zip with two values.
 
             Call
            /    \
@@ -1278,27 +1288,26 @@
   underlying federated zip intrinsic, `<T@P,U@P>-><T,U>@P`. Keeping names
   here would violate this type signature. The names are cached at a higher
   level than this function, and appended to the resulting tuple in a single
   call to `federated_map` or `federated_apply` before the resulting structure
   is sent back to the caller.
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` with a
-      `type_signature` of type `computation_types.NamedTupleType` containing
-      exactly two elements.
+    value: A `building_blocks.ComputationBuildingBlock` with a `type_signature`
+      of type `computation_types.NamedTupleType` containing exactly two
+      elements.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
     ValueError: If `value` does not contain exactly two elements.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   named_type_signatures = anonymous_tuple.to_elements(value.type_signature)
   length = len(named_type_signatures)
   if length != 2:
     raise ValueError(
         'Expected a value with exactly two elements, received {} elements.'
         .format(named_type_signatures))
   placement = value[0].type_signature.placement
@@ -1316,16 +1325,16 @@
                                                      placement, all_equal)
     elements.append((None, federated_type))
   parameter_type = computation_types.NamedTupleType(elements)
   result_type = computation_types.FederatedType(
       [(None, e.member) for _, e in named_type_signatures], placement,
       all_equal)
   intrinsic_type = computation_types.FunctionType(parameter_type, result_type)
-  intrinsic = computation_building_blocks.Intrinsic(uri, intrinsic_type)
-  return computation_building_blocks.Call(intrinsic, value)
+  intrinsic = building_blocks.Intrinsic(uri, intrinsic_type)
+  return building_blocks.Call(intrinsic, value)
 
 
 def _create_fn_to_append_chain_zipped_values(value):
   r"""Creates a function to append a chain of zipped values.
 
   Lambda(arg3)
             \
@@ -1344,263 +1353,247 @@
                                Ref(arg1)
 
   Note that this function will not respect any names it is passed; names
   for tuples will be cached at a higher level than this function and added back
   in a single call to federated map or federated apply.
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` with a
-      `type_signature` of type `computation_types.NamedTupleType` containing at
-      least two elements.
+    value: A `building_blocks.ComputationBuildingBlock` with a `type_signature`
+      of type `computation_types.NamedTupleType` containing at least two
+      elements.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   named_type_signatures = anonymous_tuple.to_elements(value.type_signature)
   length = len(named_type_signatures)
   if length < 2:
     raise ValueError(
         'Expected a value with at least two elements, received {} elements.'
         .format(named_type_signatures))
   _, first_type_signature = named_type_signatures[0]
   _, second_type_signature = named_type_signatures[1]
   ref_type = computation_types.NamedTupleType((
       first_type_signature.member,
       second_type_signature.member,
   ))
-  ref = computation_building_blocks.Reference('arg', ref_type)
-  fn = computation_building_blocks.Lambda(ref.name, ref.type_signature, ref)
+  ref = building_blocks.Reference('arg', ref_type)
+  fn = building_blocks.Lambda(ref.name, ref.type_signature, ref)
   for _, type_signature in named_type_signatures[2:]:
     ref_type = computation_types.NamedTupleType((
         fn.type_signature.parameter,
         type_signature.member,
     ))
-    ref = computation_building_blocks.Reference('arg', ref_type)
-    sel_0 = computation_building_blocks.Selection(ref, index=0)
-    call = computation_building_blocks.Call(fn, sel_0)
-    sel_1 = computation_building_blocks.Selection(ref, index=1)
+    ref = building_blocks.Reference('arg', ref_type)
+    sel_0 = building_blocks.Selection(ref, index=0)
+    call = building_blocks.Call(fn, sel_0)
+    sel_1 = building_blocks.Selection(ref, index=1)
     result = create_computation_appending(call, sel_1)
-    fn = computation_building_blocks.Lambda(ref.name, ref.type_signature,
-                                            result)
+    fn = building_blocks.Lambda(ref.name, ref.type_signature, result)
   return fn
 
 
 def create_sequence_map(fn, arg):
   r"""Creates a called sequence map.
 
             Call
            /    \
   Intrinsic      Tuple
                  |
                  [Comp, Comp]
 
   Args:
-    fn: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      function.
-    arg: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      argument.
+    fn: A `building_blocks.ComputationBuildingBlock` to use as the function.
+    arg: A `building_blocks.ComputationBuildingBlock` to use as the argument.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(fn,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(arg,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(fn, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(arg, building_blocks.ComputationBuildingBlock)
   result_type = computation_types.SequenceType(fn.type_signature.result)
   intrinsic_type = computation_types.FunctionType(
       (fn.type_signature, arg.type_signature), result_type)
-  intrinsic = computation_building_blocks.Intrinsic(
-      intrinsic_defs.SEQUENCE_MAP.uri, intrinsic_type)
-  values = computation_building_blocks.Tuple((fn, arg))
-  return computation_building_blocks.Call(intrinsic, values)
+  intrinsic = building_blocks.Intrinsic(intrinsic_defs.SEQUENCE_MAP.uri,
+                                        intrinsic_type)
+  values = building_blocks.Tuple((fn, arg))
+  return building_blocks.Call(intrinsic, values)
 
 
 def create_sequence_reduce(value, zero, op):
   r"""Creates a called sequence reduce.
 
             Call
            /    \
   Intrinsic      Tuple
                  |
                  [Comp, Comp, Comp]
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the value.
-    zero: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      initial value.
-    op: A `computation_building_blocks.ComputationBuildingBlock` to use as the
-      op function.
+    value: A `building_blocks.ComputationBuildingBlock` to use as the value.
+    zero: A `building_blocks.ComputationBuildingBlock` to use as the initial
+      value.
+    op: A `building_blocks.ComputationBuildingBlock` to use as the op function.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(zero,
-                          computation_building_blocks.ComputationBuildingBlock)
-  py_typecheck.check_type(op,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(zero, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(op, building_blocks.ComputationBuildingBlock)
   intrinsic_type = computation_types.FunctionType((
       value.type_signature,
       zero.type_signature,
       op.type_signature,
   ), op.type_signature.result)
-  intrinsic = computation_building_blocks.Intrinsic(
-      intrinsic_defs.SEQUENCE_REDUCE.uri, intrinsic_type)
-  values = computation_building_blocks.Tuple((value, zero, op))
-  return computation_building_blocks.Call(intrinsic, values)
+  intrinsic = building_blocks.Intrinsic(intrinsic_defs.SEQUENCE_REDUCE.uri,
+                                        intrinsic_type)
+  values = building_blocks.Tuple((value, zero, op))
+  return building_blocks.Call(intrinsic, values)
 
 
 def create_sequence_sum(value):
   r"""Creates a called sequence sum.
 
             Call
            /    \
   Intrinsic      Comp
 
   Args:
-    value: A `computation_building_blocks.ComputationBuildingBlock` to use as
-      the value.
+    value: A `building_blocks.ComputationBuildingBlock` to use as the value.
 
   Returns:
-    A `computation_building_blocks.Call`.
+    A `building_blocks.Call`.
 
   Raises:
     TypeError: If any of the types do not match.
   """
-  py_typecheck.check_type(value,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
   intrinsic_type = computation_types.FunctionType(value.type_signature,
                                                   value.type_signature.element)
-  intrinsic = computation_building_blocks.Intrinsic(
-      intrinsic_defs.SEQUENCE_SUM.uri, intrinsic_type)
-  return computation_building_blocks.Call(intrinsic, value)
+  intrinsic = building_blocks.Intrinsic(intrinsic_defs.SEQUENCE_SUM.uri,
+                                        intrinsic_type)
+  return building_blocks.Call(intrinsic, value)
 
 
 def _create_naming_function(tuple_type_to_name, names_to_add):
   """Private function to construct lambda naming a given tuple type.
 
   Args:
     tuple_type_to_name: Instance of `computation_types.NamedTupleType`, the type
       of the argument which we wish to name.
     names_to_add: Python `list` or `tuple`, the names we wish to give to
       `tuple_type_to_name`.
 
   Returns:
-    An instance of `computation_building_blocks.Lambda` representing a function
+    An instance of `building_blocks.Lambda` representing a function
     which will take an argument of type `tuple_type_to_name` and return a tuple
     with the same elements, but with names in `names_to_add` attached.
 
   Raises:
     ValueError: If `tuple_type_to_name` and `names_to_add` have different
     lengths.
   """
   py_typecheck.check_type(tuple_type_to_name, computation_types.NamedTupleType)
   if len(names_to_add) != len(tuple_type_to_name):
     raise ValueError(
         'Number of elements in `names_to_add` must match number of element in '
         'the named tuple type `tuple_type_to_name`; here, `names_to_add` has '
         '{} elements and `tuple_type_to_name` has {}.'.format(
             len(names_to_add), len(tuple_type_to_name)))
-  naming_lambda_arg = computation_building_blocks.Reference(
-      'x', tuple_type_to_name)
+  naming_lambda_arg = building_blocks.Reference('x', tuple_type_to_name)
 
   def _create_tuple_element(i):
     return (names_to_add[i],
-            computation_building_blocks.Selection(naming_lambda_arg, index=i))
+            building_blocks.Selection(naming_lambda_arg, index=i))
 
-  named_result = computation_building_blocks.Tuple(
+  named_result = building_blocks.Tuple(
       [_create_tuple_element(k) for k in range(len(names_to_add))])
-  return computation_building_blocks.Lambda('x',
-                                            naming_lambda_arg.type_signature,
-                                            named_result)
+  return building_blocks.Lambda('x', naming_lambda_arg.type_signature,
+                                named_result)
 
 
 def create_named_federated_tuple(tuple_to_name, names_to_add):
   """Name tuple elements with names in `names_to_add`.
 
   Certain intrinsics, e.g. `federated_zip`, only accept unnamed tuples as
   arguments, and can only produce unnamed tuples as their outputs. This is not
   necessarily desirable behavior, as it necessitates dropping any names that
   exist before the zip. This function is intended to provide a general remedy
   for this shortcoming, so that a tuple can be renamed after it is passed
   through any function which drops its names.
 
   Args:
-    tuple_to_name: Instance of
-      `computation_building_blocks.ComputationBuildingBlock` of type
-      `computation_types.FederatedType` with `computation_types.NamedTupleType`
-      member, to populate with names from `names_to_add`.
+    tuple_to_name: Instance of `building_blocks.ComputationBuildingBlock` of
+      type `computation_types.FederatedType` with
+      `computation_types.NamedTupleType` member, to populate with names from
+      `names_to_add`.
     names_to_add: Python `tuple` or `list` containing instances of type `str` or
       `None`, the names to give to `tuple_to_name`.
 
   Returns:
-    An instance of `computation_building_blocks.ComputationBuildingBlock`
+    An instance of `building_blocks.ComputationBuildingBlock`
     representing a federated tuple with the same elements as `tuple_to_name`
     but with the names from `names_to_add` attached to the type
     signature. Notice that if these names are already present in
     `tuple_to_name`, `create_naming_function` represents the identity.
 
   Raises:
     TypeError: If the types do not match the description above.
   """
   py_typecheck.check_type(names_to_add, (list, tuple))
   element_types_to_accept = six.string_types + (type(None),)
   if not all(isinstance(x, element_types_to_accept) for x in names_to_add):
     raise TypeError('`names_to_add` must contain only instances of `str` or '
                     'NoneType; you have passed in {}'.format(names_to_add))
   py_typecheck.check_type(tuple_to_name,
-                          computation_building_blocks.ComputationBuildingBlock)
+                          building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(tuple_to_name.type_signature,
                           computation_types.FederatedType)
 
   naming_fn = _create_naming_function(tuple_to_name.type_signature.member,
                                       names_to_add)
   return create_federated_map_or_apply(naming_fn, tuple_to_name)
 
 
 def create_named_tuple(comp, names):
   """Creates a computation that applies `names` to `comp`.
 
   Args:
-    comp: A `computation_building_blocks.ComputationBuildingBlock` with a
-      `type_signature` of type `computation_types.NamedTupleType`.
+    comp: A `building_blocks.ComputationBuildingBlock` with a `type_signature`
+      of type `computation_types.NamedTupleType`.
     names: Python `tuple` or `list` containing instances of type `str` or
       `None`, the names to apply to `comp`.
 
   Returns:
-    A `computation_building_blocks.ComputationBuildingBlock` representing a
+    A `building_blocks.ComputationBuildingBlock` representing a
     tuple with the elements from `comp` and the names from `names` attached to
     the `type_signature` of those elements.
 
   Raises:
     TypeError: If the types do not match.
   """
   py_typecheck.check_type(names, (list, tuple))
   if not all(isinstance(x, (six.string_types, type(None))) for x in names):
     raise TypeError('Expected `names` containing only instances of `str` or '
                     '`None`, found {}'.format(names))
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(comp.type_signature, computation_types.NamedTupleType)
   fn = _create_naming_function(comp.type_signature, names)
-  return computation_building_blocks.Call(fn, comp)
+  return building_blocks.Call(fn, comp)
 
 
 def create_zip(comp):
   r"""Returns a computation which zips `comp`.
 
   Returns the following computation where `x` is `comp` unless `comp` is a
   Reference, in which case the Reference is inlined and the Tuple is returned.
@@ -1621,41 +1614,181 @@
   it would be possible for the resulting type signature to contain a Tuple where
   two elements have the same name and this is not allowed. It is left up to the
   caller to descide if and where to add the names back.
 
   Args:
     comp: The computation building block in which to perform the merges.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(comp.type_signature, computation_types.NamedTupleType)
   named_type_signatures = anonymous_tuple.to_elements(comp.type_signature)
   _, first_type_signature = named_type_signatures[0]
   py_typecheck.check_type(first_type_signature,
                           computation_types.NamedTupleType)
   length = len(first_type_signature)
   for _, type_signature in named_type_signatures:
     py_typecheck.check_type(type_signature, computation_types.NamedTupleType)
     if len(type_signature) != length:
       raise TypeError(
           'Expected a NamedTupleType containing NamedTupleTypes with the same '
           'length, found: {}'.format(comp.type_signature))
-  if not isinstance(comp, computation_building_blocks.Reference):
+  if not isinstance(comp, building_blocks.Reference):
     name_generator = unique_name_generator(comp)
     name = six.next(name_generator)
-    ref = computation_building_blocks.Reference(name, comp.type_signature)
+    ref = building_blocks.Reference(name, comp.type_signature)
   else:
     ref = comp
   rows = []
   for column in range(len(first_type_signature)):
     columns = []
     for row in range(len(named_type_signatures)):
-      sel_row = computation_building_blocks.Selection(ref, index=row)
-      sel_column = computation_building_blocks.Selection(sel_row, index=column)
+      sel_row = building_blocks.Selection(ref, index=row)
+      sel_column = building_blocks.Selection(sel_row, index=column)
       columns.append(sel_column)
-    tup = computation_building_blocks.Tuple(columns)
+    tup = building_blocks.Tuple(columns)
     rows.append(tup)
-  tup = computation_building_blocks.Tuple(rows)
-  if not isinstance(comp, computation_building_blocks.Reference):
-    return computation_building_blocks.Block(((ref.name, comp),), tup)
+  tup = building_blocks.Tuple(rows)
+  if not isinstance(comp, building_blocks.Reference):
+    return building_blocks.Block(((ref.name, comp),), tup)
   else:
     return tup
+
+
+def _check_generic_operator_type(type_spec):
+  """Checks that `type_spec` can be the signature of args to a generic op."""
+  if not type_utils.type_tree_contains_only(type_spec, (
+      computation_types.FederatedType,
+      computation_types.NamedTupleType,
+      computation_types.TensorType,
+  )):
+    raise TypeError(
+        'Generic operators are only implemented for arguments both containing '
+        'only federated, tuple and tensor types; you have passed an argument '
+        'of type {} '.format(type_spec))
+  if not (isinstance(type_spec, computation_types.NamedTupleType) and
+          len(type_spec) == 2):
+    raise TypeError(
+        'We are trying to construct a generic operator declaring argument that '
+        'is not a two-tuple, the type {}.'.format(type_spec))
+  if not type_utils.is_binary_op_with_upcast_compatible_pair(
+      type_spec[0], type_spec[1]):
+    raise TypeError(
+        'The two-tuple you have passed in is incompatible with upcasted '
+        'binary operators. You have passed the tuple type {}, which fails the '
+        'check that the two members of the tuple are either the same type, or '
+        'the second is a scalar with the same dtype as the leaves of the '
+        'first. See `type_utils.is_binary_op_with_upcast_compatible_pair` for '
+        'more details.'.format(type_spec))
+
+
+def create_binary_operator_with_upcast(type_signature, operator):
+  """Creates lambda upcasting its argument and applying `operator`.
+
+  The concept of upcasting is explained further in the docstring for
+  `apply_binary_operator_with_upcast`.
+
+  Notice that since we are constructing a function here, e.g. for the body
+  of an intrinsic, the function we are constructing must be reducible to
+  TensorFlow. Therefore `type_signature` can only have named tuple or tensor
+  type elements; that is, we cannot handle federated types here in a generic
+  way.
+
+  Args:
+    type_signature: Value convertible to `computation_types.NamedTupleType`,
+      with two elements, both of the same type or the second able to be upcast
+      to the first, as explained in `apply_binary_operator_with_upcast`, and
+      both containing only tuples and tensors in their type tree.
+    operator: Callable defining the operator.
+
+  Returns:
+    A `building_blocks.Lambda` encapsulating a function which
+    upcasts the second element of its argument and applies the binary
+    operator.
+  """
+  py_typecheck.check_callable(operator)
+  type_signature = computation_types.to_type(type_signature)
+  _check_generic_operator_type(type_signature)
+  ref_to_arg = building_blocks.Reference('binary_operator_arg', type_signature)
+
+  def _pack_into_type(to_pack, type_spec):
+    """Pack Tensor value `to_pack` into the nested structure `type_spec`."""
+    if isinstance(type_spec, computation_types.NamedTupleType):
+      elems = anonymous_tuple.to_elements(type_spec)
+      packed_elems = [(elem_name, _pack_into_type(to_pack, elem_type))
+                      for elem_name, elem_type in elems]
+      return building_blocks.Tuple(packed_elems)
+    elif isinstance(type_spec, computation_types.TensorType):
+      expand_fn = create_tensorflow_to_broadcast_scalar(
+          to_pack.type_signature.dtype, type_spec.shape)
+      return building_blocks.Call(expand_fn, to_pack)
+
+  y_ref = building_blocks.Selection(ref_to_arg, index=1)
+  first_arg = building_blocks.Selection(ref_to_arg, index=0)
+
+  if type_utils.are_equivalent_types(first_arg.type_signature,
+                                     y_ref.type_signature):
+    second_arg = y_ref
+  else:
+    second_arg = _pack_into_type(y_ref, first_arg.type_signature)
+
+  fn = create_tensorflow_binary_operator(first_arg.type_signature, operator)
+  packed = building_blocks.Tuple([first_arg, second_arg])
+  operated = building_blocks.Call(fn, packed)
+  lambda_encapsulating_op = building_blocks.Lambda(ref_to_arg.name,
+                                                   ref_to_arg.type_signature,
+                                                   operated)
+  return lambda_encapsulating_op
+
+
+def apply_binary_operator_with_upcast(arg, operator):
+  """Constructs result of applying `operator` to `arg` upcasting if appropriate.
+
+  Notice `arg` here must be of federated type, with a named tuple member of
+  length 2, or a named tuple type of length 2. If the named tuple type of `arg`
+  satisfies certain conditions (that is, there is only a single tensor dtype in
+  the first element of `arg`, and the second element represents a scalar of
+  this dtype), the second element will be upcast to match the first. Here this
+  means it will be pushed into a nested structure matching the structure of the
+  first element of `arg`. For example, it makes perfect sense to divide a model
+  of type `<a=float32[784],b=float32[10]>` by a scalar of type `float32`, but
+  the binary operator constructors we have implemented only take arguments of
+  type `<T, T>`. Therefore in this case we would broadcast the `float` argument
+  to the `tuple` type, before constructing a biary operator which divides
+  pointwise.
+
+  Args:
+    arg: `building_blocks.ComputationBuildingBlock` of federated type whose
+      `member` attribute is a named tuple type of length 2, or named tuple type
+      of length 2.
+    operator: Callable representing binary operator to apply to the 2-tuple
+      represented by the federated `arg`.
+
+  Returns:
+    Instance of `building_blocks.ComputationBuildingBlock`
+    encapsulating the result of formally applying `operator` to
+    `arg[0], `arg[1]`, upcasting `arg[1]` in the condition described above.
+
+  Raises:
+    TypeError: If the types don't match.
+  """
+  py_typecheck.check_type(arg, building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_callable(operator)
+  if isinstance(arg.type_signature, computation_types.FederatedType):
+    py_typecheck.check_type(arg.type_signature.member,
+                            computation_types.NamedTupleType)
+    tuple_type = arg.type_signature.member
+  elif isinstance(arg.type_signature, computation_types.NamedTupleType):
+    tuple_type = arg.type_signature
+  else:
+    raise TypeError(
+        'Generic binary operators are only implemented for federated tuple and '
+        'unplaced tuples; you have passed {}.'.format(arg.type_signature))
+
+  lambda_encapsulating_op = create_binary_operator_with_upcast(
+      tuple_type, operator)
+
+  if isinstance(arg.type_signature, computation_types.FederatedType):
+    called = create_federated_map_or_apply(lambda_encapsulating_op, arg)
+  else:
+    called = building_blocks.Call(lambda_encapsulating_op, arg)
+
+  return called
```

## Comparing `tensorflow_federated/python/core/impl/dtype_utils.py` & `tensorflow_federated/python/simulation/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,27 +8,19 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Representations of Tensor types."""
+"""Models for running Federated Learning experiments in simulation."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-import numpy as np
+import tensorflow_federated.python.simulation.models.mnist
 
-TENSOR_REPRESENTATION_TYPES = (
-    # Python native types
-    str,
-    int,
-    float,
-    bool,
-    bytes,
-
-    # Numpy data types
-    np.generic,
-    np.ndarray,
-)
+# Used by doc generation script.
+_allowed_symbols = [
+    "mnist",
+]
```

## Comparing `tensorflow_federated/python/core/impl/function_utils.py` & `tensorflow_federated/python/core/impl/utils/function_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import inspect
 import types
 
+import attr
 import six
 from six.moves import range
 
 from tensorflow.python.framework import function
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_base
@@ -62,54 +63,90 @@
           function._DefinedFunction,  # pylint: disable=protected-access
           function._OverloadedFunction  # pylint: disable=protected-access
       )) or (
           # TODO(b/113112885): Add (cleaner) support for tf.Function and
           'def_function.Function' in py_typecheck.type_string(type(fn)))
 
 
+@attr.s(slots=True, frozen=True)
+class SimpleArgSpec(object):
+  """A simple container class that mimics the deprecated `inspect.ArgSpec`."""
+  args = attr.ib()
+  varargs = attr.ib()
+  keywords = attr.ib()
+  defaults = attr.ib()
+
+
 def get_argspec(fn):
-  """Returns the inspect.ArgSpec structure for the given function/defun `fn`.
+  """Returns the `SimpleArgSpec` structure for the given function.
 
   Args:
-    fn: The Python function or defun to analyze.
+    fn: The Python function or Tensorflow function to analyze.
 
   Returns:
-    The corresponding instance of inspect.ArgSpec.
+    A `SimpleArgSpec`.
 
   Raises:
     TypeError: if the argument is not of a supported type.
   """
+
+  def _getargspec(fn):
+    """Get the argspec depending on the version of Python being used."""
+    if six.PY2:
+      argspec = inspect.getargspec(fn)  # pylint: disable=deprecated-method
+      return SimpleArgSpec(*argspec)
+    else:
+      signature = inspect.signature(fn)
+      args = []
+      varargs = None
+      keywords = None
+      defaults = None
+      for param in signature.parameters.values():
+        if param.kind == inspect.Parameter.VAR_KEYWORD:
+          keywords = param.name
+        elif param.kind == inspect.Parameter.VAR_POSITIONAL:
+          varargs = param.name
+        else:
+          args.append(param.name)
+        if param.default != inspect.Parameter.empty:
+          if defaults is None:
+            defaults = [param.default]
+          else:
+            defaults.append(param.default)
+      return SimpleArgSpec(args, varargs, keywords,
+                           tuple(defaults) if defaults else None)
+
   if isinstance(fn, types.FunctionType):
-    return inspect.getargspec(fn)  # pylint: disable=deprecated-method
+    return _getargspec(fn)
   elif is_defun(fn):
-    return inspect.getargspec(fn.python_function)  # pylint: disable=deprecated-method
+    return _getargspec(fn.python_function)
   else:
     raise TypeError('Expected a Python function or a defun, found {}.'.format(
         py_typecheck.type_string(type(fn))))
 
 
 def get_callargs_for_argspec(argspec, *args, **kwargs):
-  """Similar to inspect.getcallargs(), but accepts inspect.ArgSpec instead.
+  """Similar to `inspect.getcallargs()`, but accepts SimpleArgSpec instead.
 
-  This function allows getcallargs() capability to be used with defuns and
+  This function allows `getcallargs()` capability to be used with defuns and
   other types of callables that aren't Python functions.
 
   Args:
-    argspec: An instance of inspect.ArgSpec to assign arguments to.
+    argspec: An instance of SimpleArgSpec to assign arguments to.
     *args: Positional arguments.
     **kwargs: Keyword-based arguments.
 
   Returns:
-    The same type of result as what inspect.getcallargs() returns.
+    The same type of result as what `inspect.getcallargs()` returns.
 
   Raises:
     TypeError: if the arguments are of the wrong types, or if the 'args' and
       'kwargs' combo is not compatible with 'argspec'.
   """
-  py_typecheck.check_type(argspec, inspect.ArgSpec)
+  py_typecheck.check_type(argspec, SimpleArgSpec)
   result = {}
   num_specargs = len(argspec.args) if argspec.args else 0
   num_defaults = len(argspec.defaults) if argspec.defaults else 0
   num_specargs_without_defaults = num_specargs - num_defaults
   if len(args) > num_specargs and not argspec.varargs:
     raise TypeError(
         'Too many positional arguments for the call: expected at most {}, '
@@ -138,15 +175,15 @@
   return result
 
 
 def is_argspec_compatible_with_types(argspec, *args, **kwargs):
   """Determines if functions matching 'argspec' accept given 'args'/'kwargs'.
 
   Args:
-    argspec: An instance of inspect.ArgSpec to verify agains the arguments.
+    argspec: An instance of `SimpleArgSpec` to verify agains the arguments.
     *args: Zero or more positional arguments, all of which must be instances of
       computation_types.Type or something convertible to it by
       computation_types.to_type().
     **kwargs: Zero or more keyword arguments, all of which must be instances of
       computation_types.Type or something convertible to it by
       computation_types.to_type().
 
@@ -225,15 +262,15 @@
   Returns:
     A pair (args, kwargs) containing tuple elements from 'tuple_with_args'.
 
   Raises:
     TypeError: if 'tuple_with_args' is of a wrong type.
   """
   if not is_argument_tuple(tuple_with_args):
-    raise TypeError('Not an argument tuple: {}.'.format(str(tuple_with_args)))
+    raise TypeError('Not an argument tuple: {}.'.format(tuple_with_args))
   if isinstance(tuple_with_args, anonymous_tuple.AnonymousTuple):
     elements = anonymous_tuple.to_elements(tuple_with_args)
   elif isinstance(tuple_with_args, value_base.Value):
     elements = []
     for index, (name, _) in enumerate(
         anonymous_tuple.to_elements(tuple_with_args.type_signature)):
       if name is not None:
@@ -288,17 +325,17 @@
     return anonymous_tuple.AnonymousTuple([(None, arg) for arg in args] +
                                           list(six.iteritems(kwargs)))
   else:
     py_typecheck.check_type(type_spec, computation_types.NamedTupleType)
     py_typecheck.check_type(context, context_base.Context)
     if not is_argument_tuple(type_spec):
       raise TypeError(
-          'Parameter type {} does not have a structure of an argument '
-          'tuple, and cannot be populated from multiple positional and '
-          'keyword arguments'.format(str(type_spec)))
+          'Parameter type {} does not have a structure of an argument tuple, '
+          'and cannot be populated from multiple positional and keyword '
+          'arguments'.format(type_spec))
     else:
       result_elements = []
       positions_used = set()
       keywords_used = set()
       for index, (name, elem_type) in enumerate(
           anonymous_tuple.to_elements(type_spec)):
         if index < len(args):
@@ -357,35 +394,35 @@
     else:
       return None
   else:
     parameter_type = computation_types.to_type(parameter_type)
     if not args and not kwargs:
       raise TypeError(
           'Declared a parameter of type {}, but got no arguments.'.format(
-              str(parameter_type)))
+              parameter_type))
     else:
       single_positional_arg = (len(args) == 1) and not kwargs
       if not isinstance(parameter_type, computation_types.NamedTupleType):
         # If not a named tuple type, a single positional argument is the only
         # supported call style.
         if not single_positional_arg:
           raise TypeError(
               'Parameter type {} is compatible only with a single positional '
               'argument, but found {} positional and {} keyword args.'.format(
-                  str(parameter_type), len(args), len(kwargs)))
+                  parameter_type, len(args), len(kwargs)))
         else:
           arg = args[0]
       elif single_positional_arg:
         arg = args[0]
       elif not is_argument_tuple(parameter_type):
         raise TypeError(
             'Parameter type {} does not have a structure of an argument '
             'tuple, and cannot be populated from multiple positional and '
             'keyword arguments; please construct a tuple before the '
-            'call.'.format(str(parameter_type)))
+            'call.'.format(parameter_type))
       else:
         arg = pack_args_into_anonymous_tuple(args, kwargs, parameter_type,
                                              context)
       return context.ingest(arg, parameter_type)
 
 
 def infer_unpack_needed(fn, parameter_type, should_unpack=None):
@@ -399,55 +436,54 @@
       value should be returned. If either unpacking or packing could work, and
       should_unpack is not None, then should_unpack is returned.
 
   Returns:
     A `bool` indicating whether or not to unpack.
   """
   if should_unpack not in [True, False, None]:
-    raise TypeError('The unpack argument has an unexpected value {}.'.format(
-        repr(should_unpack)))
+    raise TypeError('The unpack argument has an unexpected value {!r}.'.format(
+        should_unpack))
   unpack = should_unpack  # Default return value.
   argspec = get_argspec(fn)
 
   if parameter_type is None:
     if is_argspec_compatible_with_types(argspec):
       if should_unpack:
         raise ValueError('Requested unpacking of a no-arg function.')
       return False
     else:
       raise TypeError(
           'The argspec {} of the supplied function cannot be interpreted as a '
-          'body of a no-parameter computation.'.format(str(argspec)))
+          'body of a no-parameter computation.'.format(argspec))
 
   unpack_required = not is_argspec_compatible_with_types(
       argspec, parameter_type)
   # Boolean identity comparison becaue unpack can have a non-boolean value.
   if unpack_required and should_unpack is False:  # pylint: disable=g-bool-id-comparison
     raise TypeError(
-        'The supplied function with argspec {} cannot accept a value of '
-        'type {} as a single argument.'.format(
-            str(argspec), str(parameter_type)))
+        'The supplied function with argspec {} cannot accept a value of type '
+        '{} as a single argument.'.format(argspec, parameter_type))
   if is_argument_tuple(parameter_type):
     arg_types, kwarg_types = unpack_args_from_tuple(parameter_type)
     unpack_possible = is_argspec_compatible_with_types(argspec, *arg_types,
                                                        **kwarg_types)
   else:
     unpack_possible = False
   # Boolean identity comparison becaue unpack can have a non-boolean value.
   if not unpack_possible and should_unpack is True:  # pylint: disable=g-bool-id-comparison
     raise TypeError(
-        'The supplied function with argspec {} cannot accept a value of '
-        'type {} as multiple positional and/or keyword arguments. '
-        'That is, the argument cannot be unpacked, but unpacking '
-        'was requested.'.format(str(argspec), str(parameter_type)))
+        'The supplied function with argspec {} cannot accept a value of type '
+        '{} as multiple positional and/or keyword arguments. That is, the '
+        'argument cannot be unpacked, but unpacking was requested.'.format(
+            argspec, parameter_type))
   if unpack_required and not unpack_possible:
     raise TypeError(
-        'The supplied function with argspec {} cannot accept a value of '
-        'type {} as either a single argument or multiple positional and/or '
-        'keyword arguments.'.format(str(argspec), str(parameter_type)))
+        'The supplied function with argspec {} cannot accept a value of type '
+        '{} as either a single argument or multiple positional and/or keyword '
+        'arguments.'.format(argspec, parameter_type))
   if not unpack_required and unpack_possible and should_unpack is None:
     # The supplied function could accept a value as either a single argument,
     # or as multiple positional and/or keyword arguments, and the caller did
     # not specify any preference, leaving ambiguity in how to handle the
     # mapping. We resolve the ambiguity by defaulting to capturing the entire
     # argument, as that's the behavior suggested as expected by the users.
     unpack = False
@@ -507,27 +543,27 @@
   Raises:
     TypeError: if arguments to this call are of the wrong types, or if the
       supplied 'parameter_type' is not compatible with `fn`.
   """
   # TODO(b/113112885): Revisit whether the 3-way 'unpack' knob is sufficient
   # for our needs, or more options are needed.
   if unpack not in [True, False, None]:
-    raise TypeError('The unpack argument has an unexpected value {}.'.format(
-        repr(unpack)))
+    raise TypeError(
+        'The unpack argument has an unexpected value {!r}.'.format(unpack))
   argspec = get_argspec(fn)
   parameter_type = computation_types.to_type(parameter_type)
   if parameter_type is None:
     if is_argspec_compatible_with_types(argspec):
       # Deliberate wrapping to isolate the caller from `fn`, e.g., to prevent
       # the caller from mistakenly specifying args that match fn's defaults.
       return lambda: fn()  # pylint: disable=unnecessary-lambda
     else:
       raise TypeError(
           'The argspec {} of the supplied function cannot be interpreted as a '
-          'body of a no-parameter computation.'.format(str(argspec)))
+          'body of a no-parameter computation.'.format(argspec))
   else:
     if infer_unpack_needed(fn, parameter_type, unpack):
       arg_types, kwarg_types = unpack_args_from_tuple(parameter_type)
 
       def _unpack_and_call(fn, arg_types, kwarg_types, arg):
         """An interceptor function that unpacks 'arg' before calling `fn`.
 
@@ -551,29 +587,29 @@
         py_typecheck.check_type(
             arg, (anonymous_tuple.AnonymousTuple, value_base.Value))
         args = []
         for idx, expected_type in enumerate(arg_types):
           element_value = arg[idx]
           actual_type = type_utils.infer_type(element_value)
           if not type_utils.is_assignable_from(expected_type, actual_type):
-            raise TypeError('Expected element at position {} to be '
-                            'of type {}, found {}.'.format(
-                                idx, str(expected_type), str(actual_type)))
+            raise TypeError(
+                'Expected element at position {} to be of type {}, found {}.'
+                .format(idx, expected_type, actual_type))
           if isinstance(element_value, anonymous_tuple.AnonymousTuple):
             element_value = type_utils.convert_to_py_container(
                 element_value, expected_type)
           args.append(element_value)
         kwargs = {}
         for name, expected_type in six.iteritems(kwarg_types):
           element_value = getattr(arg, name)
           actual_type = type_utils.infer_type(element_value)
           if not type_utils.is_assignable_from(expected_type, actual_type):
-            raise TypeError('Expected element named {} to be '
-                            'of type {}, found {}.'.format(
-                                name, str(expected_type), str(actual_type)))
+            raise TypeError(
+                'Expected element named {} to be of type {}, found {}.'.format(
+                    name, expected_type, actual_type))
           if type_utils.is_anon_tuple_with_py_container(element_value,
                                                         expected_type):
             element_value = type_utils.convert_to_py_container(
                 element_value, expected_type)
           kwargs[name] = element_value
         return fn(*args, **kwargs)
 
@@ -586,15 +622,15 @@
     else:
       # An interceptor function that verifies the actual parameter before it
       # forwards the call as a last-minute check.
       def _call(fn, parameter_type, arg):
         arg_type = type_utils.infer_type(arg)
         if not type_utils.is_assignable_from(parameter_type, arg_type):
           raise TypeError('Expected an argument of type {}, found {}.'.format(
-              str(parameter_type), str(arg_type)))
+              parameter_type, arg_type))
         if type_utils.is_anon_tuple_with_py_container(arg, parameter_type):
           arg = type_utils.convert_to_py_container(arg, parameter_type)
         return fn(arg)
 
       # TODO(b/132888123): Consider other options to avoid possible bugs here.
       try:
         (fn, parameter_type)
@@ -672,11 +708,11 @@
     if not concrete_fn:
       concrete_fn = self._concrete_function_factory(arg_type)
       py_typecheck.check_type(concrete_fn, ConcreteFunction,
                               'concrete function')
       if concrete_fn.type_signature.parameter != arg_type:
         raise TypeError(
             'Expected a concrete function that takes parameter {}, got one '
-            'that takes {}.'.format(
-                str(arg_type), str(concrete_fn.type_signature.parameter)))
+            'that takes {}.'.format(arg_type,
+                                    concrete_fn.type_signature.parameter))
       self._concrete_function_cache[key] = concrete_fn
     return concrete_fn(packed_arg)
```

## Comparing `tensorflow_federated/python/core/impl/graph_utils.py` & `tensorflow_federated/python/core/impl/utils/tensorflow_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,40 +9,50 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utilities for interacting with and manipulating TensorFlow graphs."""
-# TODO(b/132704092): Rename graph_utils.py to tensorflow_utils.py
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import collections
 import functools
 import itertools
-import logging
 
 import attr
 import numpy as np
 import six
 from six.moves import range
 from six.moves import zip
 import tensorflow as tf
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
-from tensorflow_federated.python.core.api import typed_object
-from tensorflow_federated.python.core.impl import dtype_utils
-from tensorflow_federated.python.core.impl import function_utils
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.utils import function_utils
+
+
+TENSOR_REPRESENTATION_TYPES = (
+    # Python native types
+    str,
+    int,
+    float,
+    bool,
+    bytes,
+
+    # Numpy data types
+    np.generic,
+    np.ndarray,
+)
 
 
 class UniqueNameFn(object):
   """Callable which generates names that are unique across calls."""
 
   # TODO(b/133329320): Perhaps use a more general solution here.
 
@@ -115,45 +125,46 @@
           tensor=pb.TensorFlow.TensorBinding(tensor_name=name))
       return (tf_spec, binding)
     elif isinstance(parameter_type, computation_types.NamedTupleType):
       element_typespec_pairs = []
       element_bindings = []
       have_names = False
       have_nones = False
-      for e_name, e_type in anonymous_tuple.to_elements(parameter_type):
+      for e_name, e_type in anonymous_tuple.iter_elements(parameter_type):
         if e_name is None:
           have_nones = True
         else:
           have_names = True
         name = '_'.join([n for n in [parameter_name, e_name] if n])
         e_typespec, e_binding = _get_one_typespec_and_binding(
             name if name else None, e_type)
         element_typespec_pairs.append((e_name, e_typespec))
         element_bindings.append(e_binding)
       # For a given argument or kwarg, we shouldn't have both:
       if (have_names and have_nones):
         raise ValueError(
-            'A mix of named and unnamed entries are not supported inside '
-            'a nested structure representing a single argument in a call '
-            'to a TensorFlow or Python function.\n' + str(parameter_type))
+            'A mix of named and unnamed entries are not supported inside a '
+            'nested structure representing a single argument in a call to a '
+            'TensorFlow or Python function.\n{}'.format(parameter_type))
       tf_typespec = anonymous_tuple.AnonymousTuple(element_typespec_pairs)
       return (tf_typespec,
               pb.TensorFlow.Binding(
                   tuple=pb.TensorFlow.NamedTupleBinding(
                       element=element_bindings)))
     elif isinstance(parameter_type, computation_types.SequenceType):
       raise NotImplementedError('Sequence iputs not yet supported for TF 2.0.')
     else:
-      raise ValueError('Parameter type component {} cannot be converted '
-                       'to a TensorSpec'.format(repr(parameter_type)))
+      raise ValueError(
+          'Parameter type component {!r} cannot be converted to a TensorSpec'
+          .format(parameter_type))
 
   def get_arg_name(i):
     name = arg_names[i]
     if not isinstance(name, six.string_types):
-      raise ValueError('arg_names must be strings, but got' + str(name))
+      raise ValueError('arg_names must be strings, but got: {}'.format(name))
     return name
 
   # Main logic --- process arg_types and kwarg_types:
   arg_typespecs = []
   kwarg_typespecs = {}
   bindings = []
   for i, arg_type in enumerate(arg_types):
@@ -329,15 +340,15 @@
     # call time by function_utils.wrap_as_zero_or_one_arg_callable.
     if not parameter_type:
       # Stamps dummy element to "populate" graph, as TensorFlow does not support
       # empty graphs.
       dummy_tensor = tf.no_op()
     element_name_value_pairs = []
     element_bindings = []
-    for e in anonymous_tuple.to_elements(parameter_type):
+    for e in anonymous_tuple.iter_elements(parameter_type):
       e_val, e_binding = stamp_parameter_in_graph(
           '{}_{}'.format(parameter_name, e[0]), e[1], graph)
       element_name_value_pairs.append((e[0], e_val))
       element_bindings.append(e_binding)
     return (anonymous_tuple.AnonymousTuple(element_name_value_pairs),
             pb.TensorFlow.Binding(
                 tuple=pb.TensorFlow.NamedTupleBinding(
@@ -349,100 +360,20 @@
                                             parameter_type.element)
     return (ds,
             pb.TensorFlow.Binding(
                 sequence=pb.TensorFlow.SequenceBinding(
                     variant_tensor_name=variant_tensor.name)))
   else:
     raise ValueError(
-        'Parameter type component {} cannot be stamped into a TensorFlow '
-        'graph.'.format(repr(parameter_type)))
-
-
-class OneShotDataset(typed_object.TypedObject):
-  """A factory of `tf.data.Dataset`-like objects based on a no-argument lambda.
-
-  This factory supports the same methods as the data sets constructed by the
-  lambda. Upon invocation, it constructs a new data set by invoking the lambda,
-  then forwards the call to that data set. A new data set is created per call.
-  """
-
-  # TODO(b/129956296): Eventually delete this deprecated class.
+        'Parameter type component {!r} cannot be stamped into a TensorFlow '
+        'graph.'.format(parameter_type))
 
-  def __init__(self, fn, element_type):
-    """Constructs this factory from `fn`.
 
-    Args:
-      fn: A no-argument callable that creates instances of `tf.data.Dataset`.
-      element_type: The type of elements.
-    """
-    # TODO(b/131426323) Possibly reuse TensorFlow's @deprecation.deprecated()
-    # here if possible.
-    logging.warning('OneShotDataset is deprecated.')
-    py_typecheck.check_type(element_type, computation_types.Type)
-    self._type_signature = computation_types.SequenceType(element_type)
-    self._fn = fn
-
-  @property
-  def type_signature(self):
-    """Returns the TFF type of this object (an instance of `tff.Type`)."""
-    return self._type_signature
-
-  def __getattr__(self, name):
-    return getattr(self._fn(), name)
-
-
-# TODO(b/129956296): Eventually delete this deprecated declaration.
 DATASET_REPRESENTATION_TYPES = (tf.data.Dataset, tf.compat.v1.data.Dataset,
-                                tf.compat.v2.data.Dataset, OneShotDataset)
-
-
-def make_dataset_from_string_handle(handle, type_spec):
-  """Constructs a `tf.data.Dataset` from a string handle tensor and type spec.
-
-  Args:
-    handle: The tensor that represents the string handle.
-    type_spec: The type spec of elements of the data set, either an instance of
-      `types.Type` or something convertible to it.
-
-  Returns:
-    A corresponding instance of `tf.data.Dataset`.
-  """
-  # TODO(b/129956296): Eventually delete this deprecated code path.
-
-  type_spec = computation_types.to_type(type_spec)
-  tf_dtypes, shapes = type_utils.type_to_tf_dtypes_and_shapes(type_spec)
-
-  def make(handle=handle, tf_dtypes=tf_dtypes, shapes=shapes):
-    """An embedded no-argument function that constructs the data set on-demand.
-
-    This is invoked by `OneShotDataset` on each access to the data set argument
-    passed to the body of the TF computation to ensure that the iterators and
-    tje map are constructed in the appropriate context (e.g., in a defun).
-
-    Args:
-      handle: Captured from the local (above).
-      tf_dtypes: Captured from the local (above).
-      shapes: Captured from the local (above).
-
-    Returns:
-      An instance of `tf.data.Dataset`.
-    """
-    with handle.graph.as_default():
-      it = tf.data.Iterator.from_string_handle(handle, tf_dtypes, shapes)
-      # In order to convert an iterator into something that looks like a data
-      # set, we create a dummy data set that consists of an infinite sequence
-      # of zeroes, and filter it through a map function that invokes
-      # 'it.get_next()' for each of those zeroes.
-      # TODO(b/113112108): Possibly replace this with something more canonical
-      # if and when we can find adequate support for abstractly defined data
-      # sets (at the moment of this writing it does not appear to exist yet).
-      return tf.data.Dataset.range(1).repeat().map(lambda _: it.get_next())
-
-  # NOTE: To revert to the old behavior, simply invoke `make()` here directly.
-  return OneShotDataset(make, type_spec)
+                                tf.compat.v2.data.Dataset)
 
 
 def make_dataset_from_variant_tensor(variant_tensor, type_spec):
   """Constructs a `tf.data.Dataset` from a variant tensor and type spec.
 
   Args:
     variant_tensor: The variant tensor that represents the dataset.
@@ -458,15 +389,15 @@
   if not tf.is_tensor(variant_tensor):
     raise TypeError(
         'Expected `variant_tensor` to be a tensor, found {}.'.format(
             py_typecheck.type_string(type(variant_tensor))))
   if variant_tensor.dtype != tf.variant:
     raise TypeError(
         'Expected `variant_tensor` to be of a variant type, found {}.'.format(
-            str(variant_tensor.dtype)))
+            variant_tensor.dtype))
   return tf.data.experimental.from_variant(
       variant_tensor,
       structure=(type_utils.type_to_tf_structure(
           computation_types.to_type(type_spec))))
 
 
 def capture_result_from_graph(result, graph):
@@ -500,15 +431,15 @@
         tuple=pb.TensorFlow.NamedTupleBinding(
             element=[e[2] for e in element_name_type_binding_triples]))
     return type_spec, binding
 
   # TODO(b/113112885): The emerging extensions for serializing SavedModels may
   # end up introducing similar concepts of bindings, etc., we should look here
   # into the possibility of reusing some of that code when it's available.
-  if isinstance(result, dtype_utils.TENSOR_REPRESENTATION_TYPES):
+  if isinstance(result, TENSOR_REPRESENTATION_TYPES):
     with graph.as_default():
       result = tf.constant(result)
   if tf.is_tensor(result):
     if hasattr(result, 'read_value'):
       # We have a tf.Variable-like result, get a proper tensor to fetch.
       with graph.as_default():
         result = result.read_value()
@@ -568,24 +499,14 @@
     element_type = type_utils.tf_dtypes_and_shapes_to_type(
         tf.compat.v1.data.get_output_types(result),
         tf.compat.v1.data.get_output_shapes(result))
     return (computation_types.SequenceType(element_type),
             pb.TensorFlow.Binding(
                 sequence=pb.TensorFlow.SequenceBinding(
                     variant_tensor_name=variant_tensor.name)))
-  elif isinstance(result, OneShotDataset):
-    # TODO(b/129956296): Eventually delete this deprecated code path.
-    element_type = type_utils.tf_dtypes_and_shapes_to_type(
-        tf.compat.v1.data.get_output_types(result),
-        tf.compat.v1.data.get_output_shapes(result))
-    handle_name = result.make_one_shot_iterator().string_handle().name
-    return (computation_types.SequenceType(element_type),
-            pb.TensorFlow.Binding(
-                sequence=pb.TensorFlow.SequenceBinding(
-                    iterator_string_handle_name=handle_name)))
   else:
     raise TypeError('Cannot capture a result of an unsupported type {}.'.format(
         py_typecheck.type_string(type(result))))
 
 
 def compute_map_from_bindings(source, target):
   """Computes a dictionary for renaming tensors from a matching bindings pair.
@@ -618,21 +539,15 @@
                                      str(target.tensor.tensor_name))])
   elif source_oneof == 'sequence':
     sequence_oneof = source.sequence.WhichOneof('binding')
     if target.sequence.WhichOneof('binding') != sequence_oneof:
       raise ValueError(
           'Source and target sequence bindings mismatch: {} vs. {}'.format(
               sequence_oneof, target.sequence.WhichOneof('binding')))
-    if sequence_oneof == 'iterator_string_handle_name':
-      # TODO(b/129956296): Eventually delete this deprecated code path.
-      return collections.OrderedDict([
-          (str(source.sequence.iterator_string_handle_name),
-           str(target.sequence.iterator_string_handle_name))
-      ])
-    elif sequence_oneof == 'variant_tensor_name':
+    if sequence_oneof == 'variant_tensor_name':
       return collections.OrderedDict([
           (str(source.sequence.variant_tensor_name),
            str(target.sequence.variant_tensor_name)),
       ])
     else:
       raise ValueError('Unsupported sequence binding {}'.format(sequence_oneof))
   elif source_oneof == 'tuple':
@@ -661,18 +576,15 @@
   """
   py_typecheck.check_type(binding, pb.TensorFlow.Binding)
   binding_oneof = binding.WhichOneof('binding')
   if binding_oneof == 'tensor':
     return [str(binding.tensor.tensor_name)]
   elif binding_oneof == 'sequence':
     sequence_oneof = binding.sequence.WhichOneof('binding')
-    if sequence_oneof == 'iterator_string_handle_name':
-      # TODO(b/129956296): Eventually delete this deprecated code path.
-      return [str(binding.sequence.iterator_string_handle_name)]
-    elif sequence_oneof == 'variant_tensor_name':
+    if sequence_oneof == 'variant_tensor_name':
       return [str(binding.sequence.variant_tensor_name)]
     else:
       raise ValueError('Unsupported sequence binding {}'.format(sequence_oneof))
   elif binding_oneof == 'tuple':
     return list(
         itertools.chain.from_iterable([
             extract_tensor_names_from_binding(e) for e in binding.tuple.element
@@ -756,27 +668,23 @@
       return container_type(result_elements)
   elif isinstance(type_spec, computation_types.SequenceType):
     if binding_oneof != 'sequence':
       raise ValueError(
           'Expected a sequence binding, found {}.'.format(binding_oneof))
     else:
       sequence_oneof = binding.sequence.WhichOneof('binding')
-      if sequence_oneof == 'iterator_string_handle_name':
-        # TODO(b/129956296): Eventually delete this deprecated code path.
-        handle = output_map[binding.sequence.iterator_string_handle_name]
-        return make_dataset_from_string_handle(handle, type_spec.element)
-      elif sequence_oneof == 'variant_tensor_name':
+      if sequence_oneof == 'variant_tensor_name':
         variant_tensor = output_map[binding.sequence.variant_tensor_name]
         return make_dataset_from_variant_tensor(variant_tensor,
                                                 type_spec.element)
       else:
         raise ValueError(
             'Unsupported sequence binding \'{}\'.'.format(sequence_oneof))
   else:
-    raise ValueError('Unsupported type \'{}\'.'.format(str(type_spec)))
+    raise ValueError('Unsupported type \'{}\'.'.format(type_spec))
 
 
 def nested_structures_equal(x, y):
   """Determines if nested structures `x` and `y` are equal.
 
   Args:
     x: A nested structure.
@@ -826,19 +734,19 @@
     elif all(k is None for k, _ in elements):
       return tuple([
           make_empty_list_structure_for_element_type_spec(v)
           for _, v in elements
       ])
     else:
       raise TypeError(
-          'Expected a named tuple type with either all elements named '
-          'or all unnamed, got {}.'.format(str(type_spec)))
+          'Expected a named tuple type with either all elements named or all '
+          'unnamed, got {}.'.format(type_spec))
   else:
-    raise TypeError('Expected a tensor or named tuple type, found {}.'.format(
-        str(type_spec)))
+    raise TypeError(
+        'Expected a tensor or named tuple type, found {}.'.format(type_spec))
 
 
 def _make_dummy_element_for_type_spec(type_spec):
   """Creates ndarray of zeros corresponding to `type_spec`.
 
   Returns a list containing this ndarray, whose type is *compatible* with, not
   necessarily equal to, `type_spec`. This is due to the fact that some
@@ -869,16 +777,16 @@
   elif isinstance(type_spec, computation_types.NamedTupleType):
     elements = anonymous_tuple.to_elements(type_spec)
     elem_list = []
     for _, elem_type in elements:
       elem_list.append(_make_dummy_element_for_type_spec(elem_type))
     return elem_list
   else:
-    raise TypeError('Expected a tensor or named tuple type, found {}.'.format(
-        str(type_spec)))
+    raise TypeError(
+        'Expected a tensor or named tuple type, found {}.'.format(type_spec))
 
 
 def append_to_list_structure_for_element_type_spec(structure, value, type_spec):
   """Adds an element `value` to a nested `structure` of lists for `type_spec`.
 
   This function appends tensor-level constituents of an element `value` to the
   lists created by `make_empty_list_structure_for_element_type_spec`. The
@@ -907,56 +815,56 @@
     elements = anonymous_tuple.to_elements(value)
     if all(k is not None for k, _ in elements):
       value = collections.OrderedDict(elements)
     elif all(k is None for k, _ in elements):
       value = tuple([v for _, v in elements])
     else:
       raise TypeError(
-          'Expected an anonymous tuple to either have all elements named '
-          'or all unnamed, got {}.'.format(str(value)))
+          'Expected an anonymous tuple to either have all elements named or '
+          'all unnamed, got {}.'.format(value))
   if isinstance(type_spec, computation_types.TensorType):
     py_typecheck.check_type(structure, list)
     structure.append(value)
   elif isinstance(type_spec, computation_types.NamedTupleType):
     elements = anonymous_tuple.to_elements(type_spec)
     if isinstance(structure, collections.OrderedDict):
       if py_typecheck.is_named_tuple(value):
         value = value._asdict()
       if isinstance(value, dict):
         if set(value.keys()) != set(k for k, _ in elements):
           raise TypeError('Value {} does not match type {}.'.format(
-              str(value), str(type_spec)))
+              value, type_spec))
         for elem_name, elem_type in elements:
           append_to_list_structure_for_element_type_spec(
               structure[elem_name], value[elem_name], elem_type)
       elif isinstance(value, (list, tuple)):
         if len(value) != len(elements):
           raise TypeError('Value {} does not match type {}.'.format(
-              str(value), str(type_spec)))
+              value, type_spec))
         for idx, (elem_name, elem_type) in enumerate(elements):
           append_to_list_structure_for_element_type_spec(
               structure[elem_name], value[idx], elem_type)
       else:
         raise TypeError('Unexpected type of value {} for TFF type {}.'.format(
-            py_typecheck.type_string(type(value)), str(type_spec)))
+            py_typecheck.type_string(type(value)), type_spec))
     elif isinstance(structure, tuple):
       py_typecheck.check_type(value, (list, tuple))
       if len(value) != len(elements):
         raise TypeError('Value {} does not match type {}.'.format(
-            str(value), str(type_spec)))
+            value, type_spec))
       for idx, (_, elem_type) in enumerate(elements):
         append_to_list_structure_for_element_type_spec(structure[idx],
                                                        value[idx], elem_type)
     else:
       raise TypeError(
           'Invalid nested structure, unexpected container type {}.'.format(
               py_typecheck.type_string(type(structure))))
   else:
-    raise TypeError('Expected a tensor or named tuple type, found {}.'.format(
-        str(type_spec)))
+    raise TypeError(
+        'Expected a tensor or named tuple type, found {}.'.format(type_spec))
 
 
 def to_tensor_slices_from_list_structure_for_element_type_spec(
     structure, type_spec):
   """Converts `structure` for use with `tf.data.Dataset.from_tensor_slices`.
 
   This function wraps lists in the leaves of `structure` with `np.array()` for
@@ -1001,16 +909,16 @@
         to_return.append(elem_val)
       return tuple(to_return)
     else:
       raise TypeError(
           'Invalid nested structure, unexpected container type {}.'.format(
               py_typecheck.type_string(type(structure))))
   else:
-    raise TypeError('Expected a tensor or named tuple type, found {}.'.format(
-        str(type_spec)))
+    raise TypeError(
+        'Expected a tensor or named tuple type, found {}.'.format(type_spec))
 
 
 def make_data_set_from_elements(graph, elements, element_type):
   """Creates a `tf.data.Dataset` in `graph` from explicitly listed `elements`.
 
   NOTE: The underlying implementation attempts to use the
   `tf.data.Dataset.from_tensor_slices() method to build the data set quickly,
@@ -1082,15 +990,15 @@
     ds_element_type = type_utils.tf_dtypes_and_shapes_to_type(
         tf.compat.v1.data.get_output_types(ds),
         tf.compat.v1.data.get_output_shapes(ds))
     if not type_utils.is_assignable_from(element_type, ds_element_type):
       raise TypeError(
           'Failure during data set construction, expected elements of type {}, '
           'but the constructed data set has elements of type {}.'.format(
-              str(element_type), str(ds_element_type)))
+              element_type, ds_element_type))
     return ds
 
   if graph is not None:
     with graph.as_default():
       return _work()
   else:
     return _work()
@@ -1144,15 +1052,15 @@
                                                output_types, output_shapes)
           dummy_elem = _make_dummy_element_for_type_spec(zipped_elems)
           dataset_tensors = [dummy_elem]
         dataset_results[idx] = dataset_tensors
       elif tf.is_tensor(v):
         flat_tensors.append(v)
       else:
-        raise ValueError('Unsupported value type {}.'.format(str(v)))
+        raise ValueError('Unsupported value type {}.'.format(v))
     flat_computed_tensors = sess.run(flat_tensors)
     flattened_results = _interleave_dataset_results_and_tensors(
         dataset_results, flat_computed_tensors)
 
     def _to_unicode(v):
       if six.PY3 and isinstance(v, bytes):
         return v.decode('utf-8')
@@ -1244,7 +1152,72 @@
   new_graph_def.CopyFrom(graph_def)
   for new_node in new_graph_def.node:
     if new_node.name not in deps:
       node_inputs = set(new_node.input)
       if init_op_control_dep not in node_inputs:
         new_node.input.extend([init_op_control_dep])
   return new_graph_def
+
+
+def coerce_dataset_elements_to_tff_type_spec(dataset, element_type):
+  """Map the elements of a dataset to a specified type.
+
+  This is used to coerce a `tf.data.Dataset` that may have lost the ordering
+  of dictionary keys back into a `collections.OrderedDict` (required by TFF).
+
+  Args:
+    dataset: a `tf.data.Dataset` instance.
+    element_type: a `tff.Type` specifying the type of the elements of `dataset`.
+      Must be a `tff.TensorType` or `tff.NamedTupleType`.
+
+  Returns:
+    A `tf.data.Dataset` whose output types are compatible with
+    `element_type`.
+
+  Raises:
+    ValueError: if the elements of `dataset` cannot be coerced into
+      `element_type`.
+  """
+  py_typecheck.check_type(dataset, DATASET_REPRESENTATION_TYPES)
+  py_typecheck.check_type(element_type, computation_types.Type)
+
+  if isinstance(element_type, computation_types.TensorType):
+    return dataset
+
+  # This is a similar to `reference_executor.to_representation_for_type`,
+  # look for opportunities to consolidate?
+  def _to_representative_value(type_spec, elements):
+    """Convert to a container to a type understood by TF and TFF."""
+    if isinstance(type_spec, computation_types.TensorType):
+      return elements
+    elif isinstance(type_spec, computation_types.NamedTupleType):
+      field_types = anonymous_tuple.to_elements(type_spec)
+      is_all_named = all([name is not None for name, _ in field_types])
+      if is_all_named:
+        if py_typecheck.is_named_tuple(elements):
+          values = [(name, _to_representative_value(field_type, e))
+                    for (name, field_type), e in zip(field_types, elements)]
+          return type(elements)(**values)
+        else:
+          values = [(name, _to_representative_value(field_type, elements[name]))
+                    for name, field_type in field_types]
+          return collections.OrderedDict(values)
+      else:
+        return tuple(
+            _to_representative_value(t, e) for t, e in zip(type_spec, elements))
+    else:
+      raise ValueError(
+          'Coercing a dataset with elements of expected type {!s}, '
+          'produced a value with incompatible type `{!s}. Value: '
+          '{!s}'.format(type_spec, type(elements), elements))
+
+  # tf.data.Dataset of tuples will unwrap the tuple in the `map()` call, so we
+  # must pass a function taking *args. However, if the call was originally only
+  # a single tuple, it is now "double wrapped" and must be unwrapped before
+  # traversing.
+  def _unwrap_args(*args):
+    if len(args) == 1:
+      return _to_representative_value(element_type, args[0])
+    else:
+      return _to_representative_value(element_type, args)
+
+  return dataset.map(_unwrap_args)
```

## Comparing `tensorflow_federated/python/core/impl/intrinsic_defs.py` & `tensorflow_federated/python/core/impl/compiler/intrinsic_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from __future__ import division
 from __future__ import print_function
 
 import six
 
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
-from tensorflow_federated.python.core.impl import type_constructors
+from tensorflow_federated.python.core.impl.compiler import type_factory
 
 _intrinsic_registry = {}
 
 
 class IntrinsicDef(object):
   """Represents the definition of an intrinsic.
 
@@ -183,111 +183,104 @@
 # Actual implementations might vary.
 #
 # Type signature: <{T}@CLIENTS,U,(<U,T>->U),(<U,U>->U),(U->R)> -> R@SERVER
 FEDERATED_AGGREGATE = IntrinsicDef(
     'FEDERATED_AGGREGATE', 'federated_aggregate',
     computation_types.FunctionType(
         parameter=[
-            type_constructors.at_clients(computation_types.AbstractType('T')),
+            type_factory.at_clients(computation_types.AbstractType('T')),
             computation_types.AbstractType('U'),
-            type_constructors.reduction_op(
+            type_factory.reduction_op(
                 computation_types.AbstractType('U'),
                 computation_types.AbstractType('T')),
-            type_constructors.binary_op(computation_types.AbstractType('U')),
+            type_factory.binary_op(computation_types.AbstractType('U')),
             computation_types.FunctionType(
                 computation_types.AbstractType('U'),
                 computation_types.AbstractType('R'))
         ],
-        result=type_constructors.at_server(
-            computation_types.AbstractType('R'))))
+        result=type_factory.at_server(computation_types.AbstractType('R'))))
 
 # Applies a given function to a value on the server.
 #
 # Type signature: <(T->U),T@SERVER> -> U@SERVER
 FEDERATED_APPLY = IntrinsicDef(
     'FEDERATED_APPLY', 'federated_apply',
     computation_types.FunctionType(
         parameter=[
             computation_types.FunctionType(
                 computation_types.AbstractType('T'),
                 computation_types.AbstractType('U')),
-            type_constructors.at_server(computation_types.AbstractType('T')),
+            type_factory.at_server(computation_types.AbstractType('T')),
         ],
-        result=type_constructors.at_server(
-            computation_types.AbstractType('U'))))
+        result=type_factory.at_server(computation_types.AbstractType('U'))))
 
 # Broadcasts a server item to all clients.
 #
 # Type signature: T@SERVER -> T@CLIENTS
 FEDERATED_BROADCAST = IntrinsicDef(
     'FEDERATED_BROADCAST', 'federated_broadcast',
     computation_types.FunctionType(
-        parameter=type_constructors.at_server(
-            computation_types.AbstractType('T')),
-        result=type_constructors.at_clients(
+        parameter=type_factory.at_server(computation_types.AbstractType('T')),
+        result=type_factory.at_clients(
             computation_types.AbstractType('T'), all_equal=True)))
 
 # Materializes client items as a sequence on the server.
 #
 # Type signature: {T}@CLIENTS -> T*@SERVER
 FEDERATED_COLLECT = IntrinsicDef(
     'FEDERATED_COLLECT', 'federated_collect',
     computation_types.FunctionType(
-        parameter=type_constructors.at_clients(
-            computation_types.AbstractType('T')),
-        result=type_constructors.at_server(
+        parameter=type_factory.at_clients(computation_types.AbstractType('T')),
+        result=type_factory.at_server(
             computation_types.SequenceType(
                 computation_types.AbstractType('T')))))
 
 # Maps member constituents of a client value pointwise using a given mapping
 # function that operates independently on each client.
 #
 # Type signature: <(T->U),{T}@CLIENTS> -> {U}@CLIENTS
 FEDERATED_MAP = IntrinsicDef(
     'FEDERATED_MAP', 'federated_map',
     computation_types.FunctionType(
         parameter=[
             computation_types.FunctionType(
                 computation_types.AbstractType('T'),
                 computation_types.AbstractType('U')),
-            type_constructors.at_clients(computation_types.AbstractType('T')),
+            type_factory.at_clients(computation_types.AbstractType('T')),
         ],
-        result=type_constructors.at_clients(
-            computation_types.AbstractType('U'))))
+        result=type_factory.at_clients(computation_types.AbstractType('U'))))
 
 # Maps member constituents of a client all equal value pointwise using a given
 # mapping function that operates independently on each client, as a result of
 # this independence, the value is only garunteed to be all equal if the function
 # is deterministic.
 #
 # Type signature: <(T->U),T@CLIENTS> -> U@CLIENTS
 FEDERATED_MAP_ALL_EQUAL = IntrinsicDef(
     'FEDERATED_MAP_ALL_EQUAL', 'federated_map_all_equal',
     computation_types.FunctionType(
         parameter=[
             computation_types.FunctionType(
                 computation_types.AbstractType('T'),
                 computation_types.AbstractType('U')),
-            type_constructors.at_clients(
+            type_factory.at_clients(
                 computation_types.AbstractType('T'), all_equal=True),
         ],
-        result=type_constructors.at_clients(
+        result=type_factory.at_clients(
             computation_types.AbstractType('U'), all_equal=True)))
 
 # Computes a simple (equally weighted) mean of client items. Only supported
 # for numeric tensor types, or composite structures made up of numeric types.
 #
 # Type signature: {T}@CLIENTS -> T@SERVER
 FEDERATED_MEAN = IntrinsicDef(
     'FEDERATED_MEAN', 'federated_mean',
     computation_types.FunctionType(
-        parameter=type_constructors.at_clients(
-            computation_types.AbstractType('T')),
-        result=type_constructors.at_server(
-            computation_types.AbstractType('T'))))
+        parameter=type_factory.at_clients(computation_types.AbstractType('T')),
+        result=type_factory.at_server(computation_types.AbstractType('T'))))
 
 # Reduces a set of member constituents of a client value using a given 'zero' in
 # the algebra (i.e., the result of reducing an empty set) and a given reduction
 # operator with the signature U,T->U that incorporates a single T-typed element
 # into a U-typed result of partial reduction. In the special case of T = U, this
 # corresponds to the classical notion of reduction of a set using a commutative
 # associative binary operator. The generalized reduction operator (with T != U)
@@ -295,54 +288,50 @@
 # in any order.
 #
 # Type signature: <{T}@CLIENTS,U,(<U,T>->U)> -> U@SERVER
 FEDERATED_REDUCE = IntrinsicDef(
     'FEDERATED_REDUCE', 'federated_reduce',
     computation_types.FunctionType(
         parameter=[
-            type_constructors.at_clients(computation_types.AbstractType('T')),
+            type_factory.at_clients(computation_types.AbstractType('T')),
             computation_types.AbstractType('U'),
-            type_constructors.reduction_op(
+            type_factory.reduction_op(
                 computation_types.AbstractType('U'),
                 computation_types.AbstractType('T'))
         ],
-        result=type_constructors.at_server(
-            computation_types.AbstractType('U'))))
+        result=type_factory.at_server(computation_types.AbstractType('U'))))
 
 # Computes the sum of client values on the server. Only supported for numeric
 # types, or nested structures made up of numeric computation_types.
 #
 # Type signature: {T}@CLIENTS -> T@SERVER
 FEDERATED_SUM = IntrinsicDef(
     'FEDERATED_SUM', 'federated_sum',
     computation_types.FunctionType(
-        parameter=type_constructors.at_clients(
-            computation_types.AbstractType('T')),
-        result=type_constructors.at_server(
-            computation_types.AbstractType('T'))))
+        parameter=type_factory.at_clients(computation_types.AbstractType('T')),
+        result=type_factory.at_server(computation_types.AbstractType('T'))))
 
 # Places a value at the clients.
 #
 # Type signature: T -> T@CLIENTS
 FEDERATED_VALUE_AT_CLIENTS = IntrinsicDef(
     'FEDERATED_VALUE_AT_CLIENTS', 'federated_value_at_clients',
     computation_types.FunctionType(
         parameter=computation_types.AbstractType('T'),
-        result=type_constructors.at_clients(
+        result=type_factory.at_clients(
             computation_types.AbstractType('T'), True)))
 
 # Places a value at the server.
 #
 # Type signature: T -> T@SERVER
 FEDERATED_VALUE_AT_SERVER = IntrinsicDef(
     'FEDERATED_VALUE_AT_SERVER', 'federated_value_at_server',
     computation_types.FunctionType(
         parameter=computation_types.AbstractType('T'),
-        result=type_constructors.at_server(
-            computation_types.AbstractType('T'))))
+        result=type_factory.at_server(computation_types.AbstractType('T'))))
 
 # Computes a weighted mean of client items. Only supported for numeric tensor
 # types, or composite structures made up of numeric types. Weights must be
 # simple scalar numeric (integer or floating point, not complex) tensor types.
 # The types of weights and values must be compatible, i.e., multiplying and
 # dividing member constituents of the value by weights should yield results of
 # the same type as the type of these member constituents being weighted. Thus,
@@ -351,43 +340,42 @@
 # injected, where appropriate, by the compiler before invoking this intrinsic.
 #
 # Type signature: <{T}@CLIENTS,{U}@CLIENTS> -> T@SERVER
 FEDERATED_WEIGHTED_MEAN = IntrinsicDef(
     'FEDERATED_WEIGHTED_MEAN', 'federated_weighted_mean',
     computation_types.FunctionType(
         parameter=[
-            type_constructors.at_clients(computation_types.AbstractType('T')),
-            type_constructors.at_clients(computation_types.AbstractType('U'))
+            type_factory.at_clients(computation_types.AbstractType('T')),
+            type_factory.at_clients(computation_types.AbstractType('U'))
         ],
-        result=type_constructors.at_server(
-            computation_types.AbstractType('T'))))
+        result=type_factory.at_server(computation_types.AbstractType('T'))))
 
 # Zips a tuple of two federated types into a federated tuple.
 #
 # Type signature: <{T}@CLIENTS,{U}@CLIENTS> -> {<T,U>}@CLIENTS
 FEDERATED_ZIP_AT_CLIENTS = IntrinsicDef(
     'FEDERATED_ZIP_AT_CLIENTS', 'federated_zip_at_clients',
     computation_types.FunctionType(
         parameter=[
-            type_constructors.at_clients(computation_types.AbstractType('T')),
-            type_constructors.at_clients(computation_types.AbstractType('U'))
+            type_factory.at_clients(computation_types.AbstractType('T')),
+            type_factory.at_clients(computation_types.AbstractType('U'))
         ],
-        result=type_constructors.at_clients([
+        result=type_factory.at_clients([
             computation_types.AbstractType('T'),
             computation_types.AbstractType('U')
         ])))
 # Type signature: <T@SERVER,U@SERVER> -> <T,U>@SERVER
 FEDERATED_ZIP_AT_SERVER = IntrinsicDef(
     'FEDERATED_ZIP_AT_SERVER', 'federated_zip_at_server',
     computation_types.FunctionType(
         parameter=[
-            type_constructors.at_server(computation_types.AbstractType('T')),
-            type_constructors.at_server(computation_types.AbstractType('U'))
+            type_factory.at_server(computation_types.AbstractType('T')),
+            type_factory.at_server(computation_types.AbstractType('U'))
         ],
-        result=type_constructors.at_server([
+        result=type_factory.at_server([
             computation_types.AbstractType('T'),
             computation_types.AbstractType('U')
         ])))
 
 # TODO(b/122728050): Define GENERIC_DIVIDE, GENERIC_MULTIPLY, and GENERIC_ONE
 # to support intrinsic reductions (see the uses in intrinsic_bodies.py for
 # the motivation and usage in support of which we need to define semantics).
@@ -398,15 +386,15 @@
 # maybe even functions (although it's unclear if such generality is desirable).
 #
 # TODO(b/113123410): Define the range of supported computation_types.
 #
 # Type signature: <T,T> -> T
 GENERIC_PLUS = IntrinsicDef(
     'GENERIC_PLUS', 'generic_plus',
-    type_constructors.binary_op(computation_types.AbstractType('T')))
+    type_factory.binary_op(computation_types.AbstractType('T')))
 
 # Performs pointwise TensorFlow division on its arguments.
 # The type signature of generic divide is determined by TensorFlow's set of
 # implicit type equations. For example, dividing `int32` by `int32` in TF
 # generates a tensor of type `float64`. There is therefore more structure than
 # is suggested by the type signature `<T,T> -> U`.
 # Type signature: <T,T> -> U
@@ -459,15 +447,15 @@
 # Type signature: <T*,U,(<U,T>->U)> -> U
 SEQUENCE_REDUCE = IntrinsicDef(
     'SEQUENCE_REDUCE', 'sequence_reduce',
     computation_types.FunctionType(
         parameter=[
             computation_types.SequenceType(computation_types.AbstractType('T')),
             computation_types.AbstractType('U'),
-            type_constructors.reduction_op(
+            type_factory.reduction_op(
                 computation_types.AbstractType('U'),
                 computation_types.AbstractType('T'))
         ],
         result=computation_types.AbstractType('U')))
 
 # Computes the sum of values in a sequence. Only supported for numeric types
 # or nested structures made up of numeric types.
```

## Comparing `tensorflow_federated/python/core/impl/placement_literals.py` & `tensorflow_federated/python/core/impl/compiler/placement_literals.py`

 * *Files identical despite different names*

## Comparing `tensorflow_federated/python/core/impl/transformation_utils.py` & `tensorflow_federated/python/core/impl/compiler/transformation_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,22 +17,23 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import abc
 import collections
 import itertools
+import operator
 
 import six
 from six.moves import zip
 
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
-from tensorflow_federated.python.core.impl import computation_building_blocks
 from tensorflow_federated.python.core.impl import type_utils
+from tensorflow_federated.python.core.impl.compiler import building_blocks
 
 
 def transform_postorder(comp, transform):
   """Traverses `comp` recursively postorder and replaces its constituents.
 
   For each element of `comp` viewed as an expression tree, the transformation
   `transform` is applied first to building blocks it is parameterized by, then
@@ -65,68 +66,67 @@
     transformed and `False` if it was not.
 
   Raises:
     TypeError: If the arguments are of the wrong computation_types.
     NotImplementedError: If the argument is a kind of computation building block
       that is currently not recognized.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
-  if isinstance(
-      comp,
-      (computation_building_blocks.CompiledComputation,
-       computation_building_blocks.Data, computation_building_blocks.Intrinsic,
-       computation_building_blocks.Placement,
-       computation_building_blocks.Reference)):
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
+  if isinstance(comp, (
+      building_blocks.CompiledComputation,
+      building_blocks.Data,
+      building_blocks.Intrinsic,
+      building_blocks.Placement,
+      building_blocks.Reference,
+  )):
     return transform(comp)
-  elif isinstance(comp, computation_building_blocks.Selection):
+  elif isinstance(comp, building_blocks.Selection):
     source, source_modified = transform_postorder(comp.source, transform)
     if source_modified:
-      comp = computation_building_blocks.Selection(source, comp.name,
-                                                   comp.index)
+      comp = building_blocks.Selection(source, comp.name, comp.index)
     comp, comp_modified = transform(comp)
     return comp, comp_modified or source_modified
-  elif isinstance(comp, computation_building_blocks.Tuple):
+  elif isinstance(comp, building_blocks.Tuple):
     elements = []
     elements_modified = False
-    for key, value in anonymous_tuple.to_elements(comp):
+    for key, value in anonymous_tuple.iter_elements(comp):
       value, value_modified = transform_postorder(value, transform)
       elements.append((key, value))
       elements_modified = elements_modified or value_modified
     if elements_modified:
-      comp = computation_building_blocks.Tuple(elements)
+      comp = building_blocks.Tuple(elements)
     comp, comp_modified = transform(comp)
     return comp, comp_modified or elements_modified
-  elif isinstance(comp, computation_building_blocks.Call):
+  elif isinstance(comp, building_blocks.Call):
     fn, fn_modified = transform_postorder(comp.function, transform)
     if comp.argument is not None:
       arg, arg_modified = transform_postorder(comp.argument, transform)
     else:
       arg, arg_modified = (None, False)
     if fn_modified or arg_modified:
-      comp = computation_building_blocks.Call(fn, arg)
+      comp = building_blocks.Call(fn, arg)
     comp, comp_modified = transform(comp)
     return comp, comp_modified or fn_modified or arg_modified
-  elif isinstance(comp, computation_building_blocks.Lambda):
+  elif isinstance(comp, building_blocks.Lambda):
     result, result_modified = transform_postorder(comp.result, transform)
     if result_modified:
-      comp = computation_building_blocks.Lambda(comp.parameter_name,
-                                                comp.parameter_type, result)
+      comp = building_blocks.Lambda(comp.parameter_name, comp.parameter_type,
+                                    result)
     comp, comp_modified = transform(comp)
     return comp, comp_modified or result_modified
-  elif isinstance(comp, computation_building_blocks.Block):
+  elif isinstance(comp, building_blocks.Block):
     variables = []
     variables_modified = False
     for key, value in comp.locals:
       value, value_modified = transform_postorder(value, transform)
       variables.append((key, value))
       variables_modified = variables_modified or value_modified
     result, result_modified = transform_postorder(comp.result, transform)
     if variables_modified or result_modified:
-      comp = computation_building_blocks.Block(variables, result)
+      comp = building_blocks.Block(variables, result)
     comp, comp_modified = transform(comp)
     return comp, comp_modified or variables_modified or result_modified
   else:
     raise NotImplementedError(
         'Unrecognized computation building block: {}'.format(str(comp)))
 
 
@@ -148,71 +148,68 @@
   not 'from node to node'.
 
   One important fact to note: there are recursion invariants that
   `transform_postorder_with_symbol_bindings` uses the `SymbolTree` data
   structure to enforce. In particular, within a `transform` call the following
   invariants hold:
 
-    * `symbol_tree.update_payload_tracking_reference` with an argument `ref` of
-      type `Reference` will call `update` on the `BoundVariableTracker` in
-      `symbol_tree` which tracks the value of `ref` active in the current
-      lexical scope. Will raise a `NameError` if none exists.
-
-    * `symbol_tree.get_payload_with_name` with a string argument `name`
-       will return the `BoundVariableTracker` instance from `symbol_tree`
-      which corresponds to the computation bound to the variable `name` in
-      the current lexical scope. Will raise a `NameError` if none exists.
+  *  `symbol_tree.update_payload_with_name` with an argument `name` will call
+     `update` on the `BoundVariableTracker` in `symbol_tree` which tracks the
+     value of `ref` active in the current lexical scope. Will raise a
+     `NameError` if none exists.
+
+  *  `symbol_tree.get_payload_with_name` with a string argument `name` will
+     return the `BoundVariableTracker` instance from `symbol_tree` which
+     corresponds to the computation bound to the variable `name` in the current
+     lexical scope. Will raise a `NameError` if none exists.
 
   These recursion invariants are enforced by the framework, and should be
   relied on when designing new transformations that depend on variable
   bindings.
 
   Args:
-    comp: Instance of `computation_building_blocks.ComputationBuildingBlock` to
-      read information from or transform.
+    comp: Instance of `building_blocks.ComputationBuildingBlock` to read
+      information from or transform.
     transform: Python function accepting `comp` and `symbol_tree` arguments and
       returning `transformed_comp`.
     symbol_tree: Instance of `SymbolTree`, the data structure into which we may
       read information about variable bindings, and from which we may read.
 
   Returns:
     Returns a possibly modified version of `comp`, an instance
-    of `computation_building_blocks.ComputationBuildingBlock`, along with a
+    of `building_blocks.ComputationBuildingBlock`, along with a
     Boolean with the value `True` if `comp` was transformed and `False` if it
     was not.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
   py_typecheck.check_type(symbol_tree, SymbolTree)
   if not callable(transform):
     raise TypeError('Argument `transform` to '
                     '`transform_postorder_with_symbol_bindings` must '
                     'be callable.')
   identifier_seq = itertools.count(start=1)
 
   def _transform_postorder_with_symbol_bindings_switch(comp, transform_fn,
                                                        ctxt_tree,
                                                        identifier_sequence):
     """Recursive helper function delegated to after binding comp_id sequence."""
-    if isinstance(comp, (computation_building_blocks.CompiledComputation,
-                         computation_building_blocks.Data,
-                         computation_building_blocks.Intrinsic,
-                         computation_building_blocks.Placement,
-                         computation_building_blocks.Reference)):
+    if isinstance(comp, (building_blocks.CompiledComputation,
+                         building_blocks.Data, building_blocks.Intrinsic,
+                         building_blocks.Placement, building_blocks.Reference)):
       return _traverse_leaf(comp, transform_fn, ctxt_tree, identifier_sequence)
-    elif isinstance(comp, computation_building_blocks.Selection):
+    elif isinstance(comp, building_blocks.Selection):
       return _traverse_selection(comp, transform, ctxt_tree,
                                  identifier_sequence)
-    elif isinstance(comp, computation_building_blocks.Tuple):
+    elif isinstance(comp, building_blocks.Tuple):
       return _traverse_tuple(comp, transform, ctxt_tree, identifier_sequence)
-    elif isinstance(comp, computation_building_blocks.Call):
+    elif isinstance(comp, building_blocks.Call):
       return _traverse_call(comp, transform, ctxt_tree, identifier_sequence)
-    elif isinstance(comp, computation_building_blocks.Lambda):
+    elif isinstance(comp, building_blocks.Lambda):
       return _traverse_lambda(comp, transform, ctxt_tree, identifier_sequence)
-    elif isinstance(comp, computation_building_blocks.Block):
+    elif isinstance(comp, building_blocks.Block):
       return _traverse_block(comp, transform, ctxt_tree, identifier_sequence)
     else:
       raise NotImplementedError(
           'Unrecognized computation building block: {}'.format(str(comp)))
 
   def _traverse_leaf(comp, transform, context_tree, identifier_seq):
     """Helper function holding traversal logic for leaf nodes."""
@@ -221,60 +218,59 @@
 
   def _traverse_selection(comp, transform, context_tree, identifier_seq):
     """Helper function holding traversal logic for selection nodes."""
     _ = six.next(identifier_seq)
     source, source_modified = _transform_postorder_with_symbol_bindings_switch(
         comp.source, transform, context_tree, identifier_seq)
     if source_modified:
-      comp = computation_building_blocks.Selection(source, comp.name,
-                                                   comp.index)
+      comp = building_blocks.Selection(source, comp.name, comp.index)
     comp, comp_modified = transform(comp, context_tree)
     return comp, comp_modified or source_modified
 
   def _traverse_tuple(comp, transform, context_tree, identifier_seq):
     """Helper function holding traversal logic for tuple nodes."""
     _ = six.next(identifier_seq)
     elements = []
     elements_modified = False
-    for key, value in anonymous_tuple.to_elements(comp):
+    for key, value in anonymous_tuple.iter_elements(comp):
       value, value_modified = _transform_postorder_with_symbol_bindings_switch(
           value, transform, context_tree, identifier_seq)
       elements.append((key, value))
       elements_modified = elements_modified or value_modified
     if elements_modified:
-      comp = computation_building_blocks.Tuple(elements)
+      comp = building_blocks.Tuple(elements)
     comp, comp_modified = transform(comp, context_tree)
     return comp, comp_modified or elements_modified
 
   def _traverse_call(comp, transform, context_tree, identifier_seq):
     """Helper function holding traversal logic for call nodes."""
     _ = six.next(identifier_seq)
     fn, fn_modified = _transform_postorder_with_symbol_bindings_switch(
         comp.function, transform, context_tree, identifier_seq)
     if comp.argument is not None:
       arg, arg_modified = _transform_postorder_with_symbol_bindings_switch(
           comp.argument, transform, context_tree, identifier_seq)
     else:
       arg, arg_modified = (None, False)
     if fn_modified or arg_modified:
-      comp = computation_building_blocks.Call(fn, arg)
+      comp = building_blocks.Call(fn, arg)
     comp, comp_modified = transform(comp, context_tree)
     return comp, comp_modified or fn_modified or arg_modified
 
   def _traverse_lambda(comp, transform, context_tree, identifier_seq):
     """Helper function holding traversal logic for lambda nodes."""
     comp_id = six.next(identifier_seq)
     context_tree.drop_scope_down(comp_id)
     context_tree.ingest_variable_binding(name=comp.parameter_name, value=None)
     result, result_modified = _transform_postorder_with_symbol_bindings_switch(
         comp.result, transform, context_tree, identifier_seq)
     context_tree.walk_to_scope_beginning()
     if result_modified:
-      comp = computation_building_blocks.Lambda(comp.parameter_name,
-                                                comp.parameter_type, result)
+      comp = building_blocks.Lambda(comp.parameter_name, comp.parameter_type,
+                                    result)
     comp, comp_modified = transform(comp, context_tree)
     context_tree.pop_scope_up()
     return comp, comp_modified or result_modified
 
   def _traverse_block(comp, transform, context_tree, identifier_seq):
     """Helper function holding traversal logic for block nodes."""
     comp_id = six.next(identifier_seq)
@@ -287,15 +283,15 @@
       context_tree.ingest_variable_binding(name=key, value=value)
       variables.append((key, value))
       variables_modified = variables_modified or value_modified
     result, result_modified = _transform_postorder_with_symbol_bindings_switch(
         comp.result, transform, context_tree, identifier_seq)
     context_tree.walk_to_scope_beginning()
     if variables_modified or result_modified:
-      comp = computation_building_blocks.Block(variables, result)
+      comp = building_blocks.Block(variables, result)
     comp, comp_modified = transform(comp, context_tree)
     context_tree.pop_scope_up()
     return comp, comp_modified or variables_modified or result_modified
 
   return _transform_postorder_with_symbol_bindings_switch(
       comp, transform, symbol_tree, identifier_seq)
 
@@ -355,46 +351,68 @@
         return comp.payload
       if comp.older_sibling is not None:
         comp = comp.older_sibling
       elif comp.parent is not None:
         comp = comp.parent
     raise NameError('Name {} is not available in {}'.format(name, self))
 
-  def update_payload_tracking_reference(self, ref):
-    """Calls `update` if it finds its Reference arg among the available symbols.
+  def get_all_payloads_with_value(self, value, equal_fn=None):
+    """Returns all the payloads whose `value` attribute is equal to `value`.
+
+    Args:
+      value: The value to test.
+      equal_fn: The optional function to use to determine equality, if `None` is
+        specified `operator.is_` is used.
+    """
+    payloads = []
+    if equal_fn is None:
+      equal_fn = operator.is_
+    comp = self.active_node
+    while comp.parent is not None or comp.older_sibling is not None:
+      if comp.payload.value is not None and equal_fn(value, comp.payload.value):
+        payloads.append(comp.payload)
+      if comp.older_sibling is not None:
+        comp = comp.older_sibling
+      elif comp.parent is not None:
+        comp = comp.parent
+    return payloads
+
+  def update_payload_with_name(self, name):
+    """Calls `update` if `name` is found among the available symbols.
 
     If there is no such available symbol, simply does nothing.
 
     Args:
-      ref: Instance of `computation_building_blocks.Reference`; generally, this
-        is the variable a walker has encountered in a TFF AST, and which it is
-        relying on `SymbolTable` to address correctly.
+      name: A string; generally, this is the variable a walker has encountered
+        in a TFF AST, and which it is relying on `SymbolTable` to address
+        correctly.
 
     Raises:
-      NameError: If `ref` is not found among the bound names currently
+      ValueError: If `name` is not found among the bound names currently
         available in `self`.
     """
-    py_typecheck.check_type(ref, computation_building_blocks.Reference)
+    py_typecheck.check_type(name, six.string_types)
     comp = self.active_node
     while comp.parent is not None or comp.older_sibling is not None:
-      if ref.name == comp.payload.name:
-        comp.payload.update(ref)
+      if name == comp.payload.name:
+        comp.payload.update(name)
         return
       if comp.older_sibling is not None:
         comp = comp.older_sibling
       elif comp.parent is not None:
         comp = comp.parent
-    raise NameError('The reference {} is not available in {}'.format(ref, self))
+    raise ValueError('The name \'{}\' is not available in \'{}\'.'.format(
+        name, self))
 
   def walk_to_scope_beginning(self):
     """Walks `active_node` back to the sentinel node beginning current scope.
 
     `walk_to_scope_beginning` resolves the issue of scope at a node which
     introduces scope in the following manner: each of these nodes (for instance,
-    a `computation_building_blocks.Lambda`) corresponds to a sentinel value of
+    a `building_blocks.Lambda`) corresponds to a sentinel value of
     the `_BeginScopePointer` class, ensuring that these nodes do not have access
     to
     scope that is technically not available to them. That is, we conceptualize
     the node corresponding to `(x -> x)` as existing in the scope outside of the
     binding of `x`, and therefore is unable to reference `x`. However, these
     nodes can walk down their variable declarations via
     `walk_down_one_variable_binding` in order to inspect these declarations and
@@ -417,27 +435,27 @@
       raise ValueError('You have tried to pop out of the highest level in this '
                        '`SymbolTree`.')
 
   def drop_scope_down(self, comp_id):
     """Constructs a new scope level for `self`.
 
     Scope levels in `SymbolTree` correspond to scope-introducing nodes in TFF
-    ASTs; that is, either `computation_building_blocks.Block` or
-    `computation_building_blocks.Lambda` nodes. Inside of these levels,
+    ASTs; that is, either `building_blocks.Block` or
+    `building_blocks.Lambda` nodes. Inside of these levels,
     variables are bound in sequence. The implementer of a transformation
     function needing to interact with scope should never need to explicitly walk
     the scope levels `drop_scope_down` constructs; `drop_scope_down` is simply
     provided
     for ease of exposing to a traversal function.
 
     Args:
       comp_id: Integer representing a unique key for the
-        `computation_building_blocks.ComputationBuildingBlock` which is defines
-        this scope. Used to differentiate between scopes which both branch from
-        the same point in the tree.
+        `building_blocks.ComputationBuildingBlock` which is defines this scope.
+        Used to differentiate between scopes which both branch from the same
+        point in the tree.
     """
     py_typecheck.check_type(comp_id, int)
     if self.active_node.children.get(comp_id) is None:
       node = SequentialBindingNode(_BeginScopePointer())
       self._add_child(comp_id, node)
       self._move_to_child(comp_id)
     else:
@@ -474,30 +492,28 @@
     initialized. If there is an existing node, `ingest_variable_binding` checks
     that this node has the correct `payload.name`, and overwrites its
     `payload.value` with the `value` argument.
 
     Args:
       name: The string name of the `CompTracker` instance we are constructing or
         updating.
-      value: Instance of `computation_building_blocks.ComputationBuildingBlock`
-        or `None`, as in the `value` to pass to symbol tree's node payload
-        constructor.
+      value: Instance of `building_blocks.ComputationBuildingBlock` or `None`,
+        as in the `value` to pass to symbol tree's node payload constructor.
 
     Raises:
       ValueError: If we are passed a name-mode pair such that a
         preexisting node in the symbol tree bears this relationship with
         the active node, but has a different name. This is an indication
         that either a transformation has failed to happen in the symbol tree
         or that we have a symbol tree instance that does not match the
         computation we are currently processing.
     """
     py_typecheck.check_type(name, six.string_types)
     if value is not None:
-      py_typecheck.check_type(
-          value, computation_building_blocks.ComputationBuildingBlock)
+      py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
     node = SequentialBindingNode(self.payload_type(name=name, value=value))
     if self.active_node.younger_sibling is None:
       self._add_younger_sibling(node)
       self.walk_down_one_variable_binding()
     else:
       if self.active_node.younger_sibling.payload.name != name:
         raise ValueError(
@@ -662,15 +678,15 @@
   Parent-child relationships represent relationships between levels of the AST,
   meaning, moving through an AST node which defines a variable scope in preorder
   corresponds to moving from a `SequentialBindingNode` to one of its children,
   and moving through such a node postorder corresponds to moving from a
   `SequentialBindingNode` to its parent.
 
   Sibling-sibling relationships are particular to sequential binding of
-  variables in `computation_building_blocks.Block` constructs; binding
+  variables in `building_blocks.Block` constructs; binding
   a new variable in such a construct corresponds to moving from a
   `SequentialBindingNode` to its (unique) younger sibling.
   """
 
   def __init__(self, payload):
     """Initializes `SequentialBindingNode`.
 
@@ -724,15 +740,15 @@
     py_typecheck.check_type(node, SequentialBindingNode)
     self._older_sibling = node
 
   def set_younger_sibling(self, node):
     """Sets the younger sibling scope of `self` to `node`.
 
     This corresponds to binding a new variable in a
-    `computation_building_blocks.Block` construct.
+    `building_blocks.Block` construct.
 
     This method should not be assumed to be efficient.
 
     Args:
       node: Instance of `SequentialBindingNode` representing this new binding.
     """
     py_typecheck.check_type(node, SequentialBindingNode)
@@ -781,24 +797,23 @@
     `BoundVariableTracker` represents a variable binding in a TFF AST;
     no more information is avaiable to it than the `name`-`value` pair
     being bound together.
 
     Args:
       name: String name of variable to be bound.
       value: Value to bind to this name. Can be instance of
-        `computation_building_blocks.ComputationBuildingBlock` if this
+        `building_blocks.ComputationBuildingBlock` if this
         `BoundVariableTracker` represents a concrete binding to a variable (e.g.
         in a block locals declaration), or `None`, if this
         `BoundVariableTracker` represents merely a variable declaration (e.g. in
         a lambda).
     """
     py_typecheck.check_type(name, six.string_types)
     if value is not None:
-      py_typecheck.check_type(
-          value, computation_building_blocks.ComputationBuildingBlock)
+      py_typecheck.check_type(value, building_blocks.ComputationBuildingBlock)
     self.name = name
     self.value = value
 
   def update(self, value=None):
     """Defines the way information is read into this node.
 
     Defaults to no-op.
@@ -812,29 +827,27 @@
   def __str__(self):
     """Abstract string method required as context tree will delegate."""
     pass
 
   def __eq__(self, other):
     """Base class equality checks names and values equal."""
     # TODO(b/130890785): Delegate value-checking to
-    # `computation_building_blocks.ComputationBuildingBlock`.
+    # `building_blocks.ComputationBuildingBlock`.
     if self is other:
       return True
     if not isinstance(other, BoundVariableTracker):
       return NotImplemented
     if self.name != other.name:
       return False
-    if (isinstance(self.value,
-                   computation_building_blocks.ComputationBuildingBlock) and
-        isinstance(other.value,
-                   computation_building_blocks.ComputationBuildingBlock)):
-      return (computation_building_blocks.compact_representation(
-          self.value) == computation_building_blocks.compact_representation(
-              other.value) and type_utils.are_equivalent_types(
-                  self.value.type_signature, other.value.type_signature))
+    if (isinstance(self.value, building_blocks.ComputationBuildingBlock) and
+        isinstance(other.value, building_blocks.ComputationBuildingBlock)):
+      return (self.value.compact_representation() ==
+              other.value.compact_representation() and
+              type_utils.are_equivalent_types(self.value.type_signature,
+                                              other.value.type_signature))
     return self.value is other.value
 
   def __ne__(self, other):
     """Implementing __ne__ to enforce in Python2 the Python3 standard."""
     return not self == other
 
 
@@ -897,16 +910,16 @@
   """Data container to track number References to a variable in an AST.
 
 
   Attributes:
     name: The string name representing the variable whose binding is represented
       by an instance of `ReferenceCounter`.
     value: The value bound to `name`. Can be an instance of
-      `computation_building_blocks.ComputationBuildingBlock` or None if this
-      binding is simply a placeholder, e.g. in a Lambda.
+      `building_blocks.ComputationBuildingBlock` or None if this binding is
+      simply a placeholder, e.g. in a Lambda.
     count: An integer tracking how many times the variable an instance of
       `ReferenceCounter` represents is referenced in a TFF AST.
   """
 
   def __init__(self, name, value):
     super(ReferenceCounter, self).__init__(name, value)
     self.count = 0
@@ -932,98 +945,101 @@
     return self.count == other.count
 
 
 def get_count_of_references_to_variables(comp):
   """Returns `SymbolTree` counting references to each bound variable in `comp`.
 
   Args:
-    comp: Instance of `computation_building_blocks.ComputationBuildingBlock`
-      representing the root of the AST for which we want to read total reference
-      counts by context.
+    comp: Instance of `building_blocks.ComputationBuildingBlock` representing
+      the root of the AST for which we want to read total reference counts by
+      context.
 
   Returns:
-    An instance of `SymbolTree` representing root of context tree
-    populated with `transformation_utils.ReferenceCounter`s which
-    contain the number of times each variable bound by a
-    `computation_building_blocks.Lambda`
-    or `computation_building_blocks.Block` are referenced in their computation's
-    body.
+    An instance of `SymbolTree` representing root of context tree populated with
+    `ReferenceCounter`s which contain the number of times each variable bound by
+    a `building_blocks.Lambda` or `building_blocks.Block` are referenced in
+    their computation's body.
   """
 
   reference_counter = SymbolTree(ReferenceCounter)
 
   def _should_transform(comp, context_tree):
     del context_tree  # Unused
-    return isinstance(comp, computation_building_blocks.Reference)
+    return isinstance(comp, building_blocks.Reference)
 
   def transform_fn(comp, context_tree):
     if _should_transform(comp, context_tree):
-      context_tree.update_payload_tracking_reference(comp)
+      context_tree.update_payload_with_name(comp.name)
     return comp, False
 
   transform_postorder_with_symbol_bindings(comp, transform_fn,
                                            reference_counter)
   return reference_counter
 
 
 def get_unique_names(comp):
   """Returns the unique names in `comp`."""
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
   names = set()
 
   def _update(comp):
-    if isinstance(comp, computation_building_blocks.Block):
+    if isinstance(comp, building_blocks.Block):
       names.update([name for name, _ in comp.locals])
-    elif isinstance(comp, computation_building_blocks.Lambda):
+    elif isinstance(comp, building_blocks.Lambda):
       names.add(comp.parameter_name)
     return comp, False
 
   transform_postorder(comp, _update)
   return names
 
 
 def has_unique_names(comp):
   """Checks that each variable of `comp` is bound at most once.
 
   Args:
-    comp: Instance of `computation_building_blocks.ComputationBuildingBlock`.
+    comp: Instance of `building_blocks.ComputationBuildingBlock`.
 
   Returns:
     `True` if and only if every variable bound under `comp` uses a unique name.
     Returns `False` if this condition fails.
   """
-  py_typecheck.check_type(comp,
-                          computation_building_blocks.ComputationBuildingBlock)
+  py_typecheck.check_type(comp, building_blocks.ComputationBuildingBlock)
   names = set()
   # TODO(b/129791812): Cleanup Python 2 and 3 compatibility
   unique = [True]
 
   def _transform(comp):
     """Binds any names to external `names` set."""
     if unique[0]:
-      if isinstance(comp, computation_building_blocks.Block):
+      if isinstance(comp, building_blocks.Block):
         for name, _ in comp.locals:
           if name in names:
             unique[0] = False
           names.add(name)
-      elif isinstance(comp, computation_building_blocks.Lambda):
+      elif isinstance(comp, building_blocks.Lambda):
         if comp.parameter_name in names:
           unique[0] = False
         names.add(comp.parameter_name)
     return comp, False
 
   transform_postorder(comp, _transform)
   return unique[0]
 
 
 @six.add_metaclass(abc.ABCMeta)
 class TransformSpec(object):
   """"Base class to express the should_transform/transform interface."""
 
+  def __init__(self, global_transform=False):
+    self._global_transform = global_transform
+
+  @property
+  def global_transform(self):
+    return self._global_transform
+
   @abc.abstractmethod
   def should_transform(self, comp):
     pass
 
   @abc.abstractmethod
   def transform(self, comp):
     pass
```

## Comparing `tensorflow_federated/python/core/impl/type_constructors.py` & `tensorflow_federated/python/core/impl/compiler/type_factory.py`

 * *Files identical despite different names*

## Comparing `tensorflow_federated/python/core/impl/type_serialization.py` & `tensorflow_federated/python/core/impl/compiler/type_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import tensorflow as tf
 
 from tensorflow_federated.proto.v0 import computation_pb2 as pb
 from tensorflow_federated.python.common_libs import anonymous_tuple
 from tensorflow_federated.python.common_libs import py_typecheck
 from tensorflow_federated.python.core.api import computation_types
-from tensorflow_federated.python.core.impl import placement_literals
+from tensorflow_federated.python.core.impl.compiler import placement_literals
 
 
 def _to_tensor_type_proto(tensor_type):
   py_typecheck.check_type(tensor_type, computation_types.TensorType)
   shape = tensor_type.shape
   if shape.dims is None:
     dims = None
@@ -80,15 +80,15 @@
   elif isinstance(target, computation_types.SequenceType):
     return pb.Type(
         sequence=pb.SequenceType(element=serialize_type(target.element)))
   elif isinstance(target, computation_types.NamedTupleType):
     return pb.Type(
         tuple=pb.NamedTupleType(element=[
             pb.NamedTupleType.Element(name=e[0], value=serialize_type(e[1]))
-            for e in anonymous_tuple.to_elements(target)
+            for e in anonymous_tuple.iter_elements(target)
         ]))
   elif isinstance(target, computation_types.FunctionType):
     return pb.Type(
         function=pb.FunctionType(
             parameter=serialize_type(target.parameter),
             result=serialize_type(target.result)))
   elif isinstance(target, computation_types.PlacementType):
```

## Comparing `tensorflow_federated/python/examples/__init__.py` & `tensorflow_federated/python/core/impl/compiler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Lint as: python3
-# Copyright 2018, The TensorFlow Federated Authors.
+# Copyright 2019, The TensorFlow Federated Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

## Comparing `tensorflow_federated/python/examples/mnist/__init__.py` & `tensorflow_federated/python/core/backends/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-# Lint as: python3
-# Copyright 2019, The TensorFlow Federated Authors.
+# Lint as: python2
+# Copyright 2018, The TensorFlow Federated Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Example code for use with variants of the MNIST data set."""
+"""This directory contains code for interfacing custom types of backends."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-from tensorflow_federated.python.examples.mnist.models import create_simple_keras_model
-from tensorflow_federated.python.examples.mnist.models import keras_dataset_from_emnist
+from tensorflow_federated.python.core.backends import mapreduce
+
+# Used by doc generation script.
+_allowed_symbols = [
+    "mapreduce",
+]
```

## Comparing `tensorflow_federated/python/examples/mnist/models.py` & `tensorflow_federated/python/simulation/models/mnist.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,51 +18,65 @@
 from __future__ import division
 from __future__ import print_function
 
 import collections
 
 import tensorflow as tf
 
-import tensorflow_federated as tff
+
+class _NumExamplesCounter(tf.keras.metrics.Sum):
+  """A `tf.keras.metrics.Metric` that counts the number of examples seen."""
+
+  def __init__(self, name='num_examples', dtype=tf.int64):  # pylint: disable=useless-super-delegation
+    super(_NumExamplesCounter, self).__init__(name, dtype)
+
+  def update_state(self, y_true, y_pred, sample_weight=None):
+    return super(_NumExamplesCounter,
+                 self).update_state(tf.shape(y_pred)[0], sample_weight)
 
 
 def create_simple_keras_model(learning_rate=0.1):
   """Returns an instance of `tf.Keras.Model` with just one dense layer.
 
   Args:
     learning_rate: The learning rate to use with the SGD optimizer.
 
   Returns:
     An instance of `tf.Keras.Model`.
   """
   model = tf.keras.models.Sequential([
       tf.keras.layers.Flatten(input_shape=(784,)),
-      tf.keras.layers.Dense(10, tf.nn.softmax, kernel_initializer='zeros')
+      tf.keras.layers.Dense(10, tf.nn.softmax, kernel_initializer='zeros'),
   ])
 
   model.compile(
       loss=tf.keras.losses.SparseCategoricalCrossentropy(),
       optimizer=tf.keras.optimizers.SGD(learning_rate),
-      metrics=[tf.keras.metrics.SparseCategoricalAccuracy()])
+      metrics=[
+          tf.keras.metrics.SparseCategoricalAccuracy(),
+          _NumExamplesCounter(),
+      ])
   return model
 
 
 def keras_dataset_from_emnist(dataset):
   """Converts `dataset` for use with the output of `create_simple_keras_model`.
 
   Args:
     dataset: An instance of `tf.data.Dataset` to read from.
 
   Returns:
     An instance of `tf.data.Dataset` after conversion.
   """
 
   def map_fn(example):
-    return collections.OrderedDict([('x', tf.reshape(example['pixels'], [-1])),
-                                    ('y', example['label'])])
+    return collections.OrderedDict([
+        ('x', tf.reshape(example['pixels'], [-1])),
+        ('y', example['label']),
+    ])
 
   return dataset.map(map_fn)
 
 
 def create_keras_model(compile_model=False):
   """Returns an instance of `tf.keras.Model` for use with the MNIST example.
 
@@ -76,63 +90,40 @@
 
   Returns:
     A `tf.keras.Model`.
   """
   # TODO(b/120157713): Find a way to import this code.
   data_format = 'channels_last'
   input_shape = [28, 28, 1]
-  l = tf.keras.layers
   initializer = tf.keras.initializers.RandomNormal(seed=0)
-  max_pool = l.MaxPooling2D((2, 2), (2, 2),
-                            padding='same',
-                            data_format=data_format)
+  max_pool = tf.keras.layers.MaxPooling2D((2, 2), (2, 2),
+                                          padding='same',
+                                          data_format=data_format)
   model = tf.keras.Sequential([
-      l.Reshape(target_shape=input_shape, input_shape=(28 * 28,)),
-      l.Conv2D(
+      tf.keras.layers.Reshape(target_shape=input_shape, input_shape=(28 * 28,)),
+      tf.keras.layers.Conv2D(
           32,
           5,
           padding='same',
           data_format=data_format,
           activation=tf.nn.relu,
-          kernel_initializer=initializer), max_pool,
-      l.Conv2D(
+          kernel_initializer=initializer),
+      max_pool,
+      tf.keras.layers.Conv2D(
           64,
           5,
           padding='same',
           data_format=data_format,
           activation=tf.nn.relu,
-          kernel_initializer=initializer), max_pool,
-      l.Flatten(),
-      l.Dense(1024, activation=tf.nn.relu, kernel_initializer=initializer),
-      l.Dropout(0.4, seed=1),
-      l.Dense(10, kernel_initializer=initializer)
+          kernel_initializer=initializer),
+      max_pool,
+      tf.keras.layers.Flatten(),
+      tf.keras.layers.Dense(
+          1024, activation=tf.nn.relu, kernel_initializer=initializer),
+      tf.keras.layers.Dropout(0.4, seed=1),
+      tf.keras.layers.Dense(10, kernel_initializer=initializer),
   ])
   if compile_model:
     model.compile(
         loss=tf.keras.losses.SparseCategoricalCrossentropy(),
         optimizer=tf.keras.optimizers.SGD(learning_rate=0.1))
   return model
-
-
-Batch = collections.namedtuple('Batch', ['x', 'y'])  # pylint: disable=invalid-name
-
-
-def create_random_batch():
-  """Returns an instance of `Batch` populated with random tensors."""
-  return Batch(
-      x=tf.random.uniform(tf.TensorShape([1, 784]), dtype=tf.float32),
-      y=tf.constant(1, dtype=tf.int64, shape=[1, 1]))
-
-
-def model_fn():
-  """Constructs the MNIST model wrapped for use with TensorFlow Federated.
-
-  The model constructed by this function can be passed as an argument to
-  `tff.learning.build_federated_averaging_process` to create a federated
-  training process.
-
-  Returns:
-    An instance of `tff.learning.Model` that represents a trainable model.
-  """
-  keras_model = create_keras_model(compile_model=True)
-  dummy_batch = create_random_batch()
-  return tff.learning.from_compiled_keras_model(keras_model, dummy_batch)
```

## Comparing `tensorflow_federated/python/simulation/datasets/emnist/synthetic.py` & `tensorflow_federated/python/simulation/datasets/emnist.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,58 +8,301 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A tiny version of Federated EMNIST, for testing.
-
-The digits were generated programmatically using PIL.
-"""
+"""Libraries for the federated EMNIST dataset for simulation."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import collections
+import hashlib
+import math
+import os.path
+import struct
 
 import numpy as np
-from six.moves import range
+import tensorflow as tf
+import tensorflow_addons.image as tfa_image
 
+from tensorflow_federated.python.common_libs import py_typecheck
+from tensorflow_federated.python.simulation import from_tensor_slices_client_data
+from tensorflow_federated.python.simulation import hdf5_client_data
+from tensorflow_federated.python.simulation import transforming_client_data
+
+
+def load_data(only_digits=True, cache_dir=None):
+  """Loads the Federated EMNIST dataset.
+
+  Downloads and caches the dataset locally. If previously downloaded, tries to
+  load the dataset from cache.
+
+  This dataset is derived from the Leaf repository
+  (https://github.com/TalwalkarLab/leaf) pre-processing of the Extended MNIST
+  dataset, grouping examples by writer. Details about Leaf were published in
+  "LEAF: A Benchmark for Federated Settings" https://arxiv.org/abs/1812.01097.
+
+  *Note*: This dataset does not include some additional preprocessing that
+  MNIST includes, such as size-normalization and centering.
+  In the Federated EMNIST data, the value of 1.0
+  corresponds to the background, and 0.0 corresponds to the color of the digits
+  themselves; this is the *inverse* of some MNIST representations,
+  e.g. in [tensorflow_datasets]
+  (https://github.com/tensorflow/datasets/blob/master/docs/datasets.md#mnist),
+  where 0 corresponds to the background color, and 255 represents the color of
+  the digit.
+
+  Data set sizes:
+
+  *only_digits=True*: 3,383 users, 10 label classes
+
+  -   train: 341,873 examples
+  -   test: 40,832 examples
+
+  *only_digits=False*: 3,400 users, 62 label classes
+
+  -   train: 671,585 examples
+  -   test: 77,483 examples
+
+  Rather than holding out specific users, each user's examples are split across
+  _train_ and _test_ so that all users have at least one example in _train_ and
+  one example in _test_. Writers that had less than 2 examples are excluded from
+  the data set.
+
+  The `tf.data.Datasets` returned by
+  `tff.simulation.ClientData.create_tf_dataset_for_client` will yield
+  `collections.OrderedDict` objects at each iteration, with the following keys
+  and values:
+
+    -   `'pixels'`: a `tf.Tensor` with `dtype=tf.float32` and shape [28, 28],
+        containing the pixels of the handwritten digit, with values in
+        the range [0.0, 1.0].
+    -   `'label'`: a `tf.Tensor` with `dtype=tf.int32` and shape [1], the class
+        label of the corresponding pixels. Labels [0-9] correspond to the digits
+        classes, labels [10-35] correspond to the uppercase classes (e.g., label
+        11 is 'B'), and labels [36-61] correspond to the lowercase classes
+        (e.g., label 37 is 'b').
+
+  Args:
+    only_digits: (Optional) whether to only include examples that are from the
+      digits [0-9] classes. If `False`, includes lower and upper case
+      characters, for a total of 62 class labels.
+    cache_dir: (Optional) directory to cache the downloaded file. If `None`,
+      caches in Keras' default cache directory.
 
-def from_ints(data):
-  data = np.array(data)
-  results = []
-  for img_array in data:
-    img_array = img_array.astype(np.float32) / 9.0
-    results.append(img_array)
-  return results
+  Returns:
+    Tuple of (train, test) where the tuple elements are
+    `tff.simulation.ClientData` objects.
+  """
+  if only_digits:
+    fileprefix = 'fed_emnist_digitsonly'
+    sha256 = '55333deb8546765427c385710ca5e7301e16f4ed8b60c1dc5ae224b42bd5b14b'
+  else:
+    fileprefix = 'fed_emnist'
+    sha256 = 'fe1ed5a502cea3a952eb105920bff8cffb32836b5173cb18a57a32c3606f3ea0'
+
+  filename = fileprefix + '.tar.bz2'
+  path = tf.keras.utils.get_file(
+      filename,
+      origin='https://storage.googleapis.com/tff-datasets-public/' + filename,
+      file_hash=sha256,
+      hash_algorithm='sha256',
+      extract=True,
+      archive_format='tar',
+      cache_dir=cache_dir)
+
+  dir_path = os.path.dirname(path)
+  train_client_data = hdf5_client_data.HDF5ClientData(
+      os.path.join(dir_path, fileprefix + '_train.h5'))
+  test_client_data = hdf5_client_data.HDF5ClientData(
+      os.path.join(dir_path, fileprefix + '_test.h5'))
+
+  return train_client_data, test_client_data
+
+
+def get_synthetic(num_clients=2):
+  """Quickly returns a small synthetic dataset, useful for unit tests, etc.
+
+  Each client produced has exactly 10 examples, one of each digit. The images
+  are derived from a fixed set of hard-coded images, and transformed using
+  `tff.simulation.datasets.emnist.infinite_emnist` to produce the desired
+  number of clients.
+
+  Args:
+    num_clients: The number of synthetic clients to generate.
+
+  Returns:
+     A `tff.simulation.ClientData` object that matches the characteristics
+     (other than size) of those provided by
+     `tff.simulation.datasets.emnist.load_data`.
+  """
+  return get_infinite(
+      # Base ClientData with one client
+      from_tensor_slices_client_data.FromTensorSlicesClientData(
+          {'synthetic': _get_synthetic_digits_data()}),
+      num_pseudo_clients=num_clients)
+
+
+def _compile_transform(angle=0,
+                       shear=0,
+                       scale_x=1,
+                       scale_y=1,
+                       translation_x=0,
+                       translation_y=0):
+  """Compiles affine transform parameters into single projective transform.
+
+  The transformations are performed in the following order: rotation, shearing,
+  scaling, and translation.
+
+  Args:
+    angle: The angle of counter-clockwise rotation, in degrees.
+    shear: The amount of shear. Precisely, shear*x is added to the y coordinate
+      after centering.
+    scale_x: The amount to scale in the x-axis.
+    scale_y: The amount to scale in the y-axis.
+    translation_x: The number of pixels to translate in the x-axis.
+    translation_y: The number of pixels to translate in the y-axis.
+
+  Returns:
+    A length 8 tensor representing the composed transform.
+  """
+  angle = math.radians(angle)
+  size = 28
+
+  # angles_to_projective_transforms performs rotations around center of image.
+  rotation = tfa_image.transform_ops.angles_to_projective_transforms(
+      angle, size, size)
+
+  # shearing and scaling require centering and decentering.
+  half = (size - 1) / 2.0
+  center = tfa_image.translate_ops.translations_to_projective_transforms(
+      [-half, -half])
+  shear = [1., 0., 0., -shear, 1., 0., 0., 0.]
+  scaling = [1. / scale_x, 0., 0., 0., 1. / scale_y, 0., 0., 0.]
+  decenter = tfa_image.translate_ops.translations_to_projective_transforms(
+      [half, half])
+
+  translation = tfa_image.translate_ops.translations_to_projective_transforms(
+      [translation_x, translation_y])
+  return tfa_image.transform_ops.compose_transforms(
+      transforms=[rotation, center, shear, scaling, decenter, translation])
+
+
+def _make_transform_fn(raw_client_id, index):
+  """Generates a pseudorandom affine transform based on the client_id and index.
+
+  If the index is 0, `None` is returned so no transform is applied by the
+  transforming_client_data.
+
+  Args:
+    raw_client_id: The raw client_id.
+    index: The index of the pseudo-client.
+
+  Returns:
+    The transformed data.
+  """
+  if index == 0:
+    return None
+
+  py_typecheck.check_type(raw_client_id, str)
+  # To be python2 compatible, we need to use struct.unpack() to convert bytes to
+  # int. (In python3, the int.from_bytes() method could be used instead.)
+  _, _, _, stable_hash_of_client_id = struct.unpack(
+      '>IIII',
+      hashlib.md5(raw_client_id.encode()).digest())
+  np.random.seed((stable_hash_of_client_id + index) % (2**32))
+
+  def random_scale(min_val):
+    b = math.log(min_val)
+    return math.exp(np.random.uniform(b, -b))
+
+  transform = _compile_transform(
+      angle=np.random.uniform(-20, 20),
+      shear=np.random.uniform(-0.2, 0.2),
+      scale_x=random_scale(0.8),
+      scale_y=random_scale(0.8),
+      translation_x=np.random.uniform(-5, 5),
+      translation_y=np.random.uniform(-5, 5))
+
+  def _transform_fn(data):
+    """Applies a random transform to the pixels."""
+    # EMNIST background is 1.0 but tfa_image.transform assumes 0.0, so invert.
+    pixels = 1.0 - data['pixels']
+
+    pixels = tfa_image.transform(pixels, transform, 'BILINEAR')
+
+    # num_bits=9 actually yields 256 unique values.
+    pixels = tf.quantization.quantize_and_dequantize(
+        pixels, 0.0, 1.0, num_bits=9, range_given=True)
+
+    data['pixels'] = 1.0 - pixels
+    return data
+
+  return _transform_fn
+
+
+def get_infinite(emnist_client_data, num_pseudo_clients):
+  """Converts a Federated EMNIST dataset into an Infinite Federated EMNIST set.
+
+  Infinite Federated EMNIST expands each writer from the EMNIST dataset into
+  some number of pseudo-clients each of whose characters are the same but apply
+  a fixed random affine transformation to the original user's characters. The
+  distribution over affine transformation is approximately equivalent to the one
+  described at https://www.cs.toronto.edu/~tijmen/affNIST/. It applies the
+  following transformations in this order:
+
+    1. A random rotation chosen uniformly between -20 and 20 degrees.
+    2. A random shearing adding between -0.2 to 0.2 of the x coordinate to the
+       y coordinate (after centering).
+    3. A random scaling between 0.8 and 1.25 (sampled log uniformly).
+    4. A random translation between -5 and 5 pixels in both the x and y axes.
+
+  Args:
+    emnist_client_data: The `tff.simulation.ClientData` to convert.
+    num_pseudo_clients: How many pseudo-clients to generate for each real
+      client. Each pseudo-client is formed by applying a given random affine
+      transformation to the characters written by a given real user. The first
+      pseudo-client for a given user applies the identity transformation, so the
+      original users are always included.
+
+  Returns:
+    An expanded `tff.simulation.ClientData`.
+  """
+  num_client_ids = len(emnist_client_data.client_ids)
+
+  return transforming_client_data.TransformingClientData(
+      raw_client_data=emnist_client_data,
+      make_transform_fn=_make_transform_fn,
+      num_transformed_clients=(num_client_ids * num_pseudo_clients))
 
 
-def get_data():
+def _get_synthetic_digits_data():
   """Returns a dictionary suitable for `tf.data.Dataset.from_tensor_slices`.
 
   Returns:
     A dictionary that matches the structure of the data produced by
     `tff.simulation.datasets.emnist.load_data`, with keys `pixels` and `label`.
   """
-  data = np.array(DIGITS_DATA)
+  data = np.array(_SYNTHETIC_DIGITS_DATA)
   img_list = []
   for img_array in data:
     img_array = img_array.astype(np.float32) / 9.0
     img_list.append(img_array)
   assert len(img_list) == 10
   return collections.OrderedDict([('pixels', img_list),
                                   ('label', list(range(10)))])
 
 
 # pyformat: disable
 # pylint: disable=bad-continuation,bad-whitespace
-DIGITS_DATA = [
+_SYNTHETIC_DIGITS_DATA = [
    [[9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9],
     [9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9],
     [9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9],
     [9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9],
     [9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9],
     [9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9],
     [9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9],
```

## Comparing `tensorflow_federated/python/simulation/datasets/shakespeare/load_data.py` & `tensorflow_federated/python/simulation/datasets/shakespeare.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Libraries for the Shakesepare dataset for federated learning simulation."""
+"""Libraries for the Shakespeare dataset for federated learning simulation."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import os.path
```

## Comparing `tensorflow_federated-0.7.0.dist-info/METADATA` & `tensorflow_federated-0.9.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-federated
-Version: 0.7.0
+Version: 0.9.0
 Summary: TensorFlow Federated is an open-source federated learning framework.
 Home-page: http://tensorflow.org/federated
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Download-URL: https://github.com/tensorflow/federated/tags
 Keywords: tensorflow federated machine learning
@@ -23,21 +23,27 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/plain
+Requires-Dist: absl-py (~=0.7)
 Requires-Dist: attrs (~=18.2)
+Requires-Dist: cachetools (~=3.1.1)
+Requires-Dist: enum34 (~=1.1)
+Requires-Dist: grpcio (~=1.22.0)
 Requires-Dist: h5py (~=2.6)
 Requires-Dist: numpy (~=1.14)
+Requires-Dist: portpicker (~=1.3.1)
 Requires-Dist: six (~=1.10)
+Requires-Dist: tensorflow-model-optimization (~=0.1.3)
+Requires-Dist: tensorflow-privacy (~=0.1.0)
 Requires-Dist: tf-nightly
-Requires-Dist: grpcio (~=1.8.0)
-Requires-Dist: portpicker
+Requires-Dist: tfa-nightly
 
 TensorFlow Federated (TFF) is an open-source framework for machine learning and
 other computations on decentralized data. TFF has been developed to facilitate
 open research and experimentation with Federated Learning (FL), an approach to
 machine learning where a shared global model is trained across many
 participating clients that keep their training data locally. For example, FL has
 been used to train prediction models for mobile keyboards without uploading
```

## Comparing `tensorflow_federated-0.7.0.dist-info/RECORD` & `tensorflow_federated-0.9.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,121 @@
-tensorflow_federated/__init__.py,sha256=LyA5ZxH-OvnDvdP8k-XX-jaXOqT-Aap4o1qjIJ1fYVU,4056
+tensorflow_federated/__init__.py,sha256=CDave0RAfjXc5BXvOEi2o4WdPu17q-HQhZwxnvwucsQ,4218
+tensorflow_federated/version.py,sha256=8pnlyU12-VQB3S2HK6nBS1Tq_nAlgFs_8ft4a82hCwk,787
 tensorflow_federated/proto/__init__.py,sha256=anWWDQNP86PB8Dq84zcV1Tppw_Qslk-4IwSP4DRcQK0,618
 tensorflow_federated/proto/v0/__init__.py,sha256=anWWDQNP86PB8Dq84zcV1Tppw_Qslk-4IwSP4DRcQK0,618
-tensorflow_federated/proto/v0/computation_pb2.py,sha256=tShe2yO74jAZQ9FU4f3ehMebi_QdK6OQuTg90xiUzpk,66868
-tensorflow_federated/proto/v0/computation_pb2_grpc.py,sha256=s9KvvTKGqObFxOBLz6ktRK2g4c8yLiOXt7p2M71egTM,83
-tensorflow_federated/proto/v0/executor_pb2.py,sha256=QKEd5l9toJ5jj1ItdPXQ3BkQarfIWd2lipJIfJEE2cU,31793
-tensorflow_federated/proto/v0/executor_pb2_grpc.py,sha256=jx547iKkMCZuIMzt74qwiqJ14FPUq0wiEQruiBFws54,7042
+tensorflow_federated/proto/v0/computation_pb2.py,sha256=l3saMPhd8Lj2e_SEIDxxEGMgcPE-r3mAeEv5gE3e_Bo,65974
+tensorflow_federated/proto/v0/executor_pb2.py,sha256=WANWfPDdxds6ru-wyXnyEc_6DWClRQoRhXnku9nfI8s,47745
+tensorflow_federated/proto/v0/executor_pb2_grpc.py,sha256=_jsCXe_QG3ZqAE3JTylNMZuju3_cP2j3_0lTvooFREE,7996
 tensorflow_federated/python/__init__.py,sha256=PuAd8tRBzvtTxsmkCavfROwpPrfnt2fW7XJRN2d1c40,618
 tensorflow_federated/python/common_libs/__init__.py,sha256=FeYbWP7LhXKaDsGLx5MR2VQQNMPrYNx6z8heLIkEKtI,699
-tensorflow_federated/python/common_libs/anonymous_tuple.py,sha256=SB8ZDiWTftDf3MoMidAfoQqRGRqebsDHLYe-Vlwpo-w,14346
-tensorflow_federated/python/common_libs/py_typecheck.py,sha256=mV-0CIbOesd89fIEZSQDRPaMdJG4yVTmN3waoW_9XqU,7347
-tensorflow_federated/python/common_libs/serialization_utils.py,sha256=pm5_FtRuz7Ol9eHvx3jWLy7znhW7METB2n7DCcuViIU,2013
-tensorflow_federated/python/core/__init__.py,sha256=Krfz4pe85ilW44LT1a7DOfXSS786xed2XhpYafT1WnQ,3120
+tensorflow_federated/python/common_libs/anonymous_tuple.py,sha256=nfPFu0BbPUToy9uxZI2n285bsC8WMq4yKg9uQo9vY1E,16820
+tensorflow_federated/python/common_libs/py_typecheck.py,sha256=LI-Ce4cwkPkM8h5IJDDSfRePRPl1gX2caJJvz1KA41o,7751
+tensorflow_federated/python/common_libs/serialization_utils.py,sha256=fWc9N11UWjrtCztizFkqTShWMkPyvWGpz1FVImnafI8,2872
+tensorflow_federated/python/core/__init__.py,sha256=XkuKHHzApHNhtkKx03WVCXkepTgR31rjbfRnVvVw3uc,3174
 tensorflow_federated/python/core/api/__init__.py,sha256=WIssZTE6JwXf7NM8RBsthopKxi_KqBpmlnNSdn_xzzU,2879
 tensorflow_federated/python/core/api/computation_base.py,sha256=iofXmeWsXjTmvVewEAJmd_O0AJ4C-YoqCO3uTW99DCg,1434
-tensorflow_federated/python/core/api/computation_types.py,sha256=fOiMTpLtIMq3yIOaPC48NumQ4xK6h91FGY2X3B3nODw,20387
+tensorflow_federated/python/core/api/computation_types.py,sha256=Jwj9oNEkaBEf3gnOPlHSHI_E0DK5PKBXJ0LChs1NV04,20539
 tensorflow_federated/python/core/api/computations.py,sha256=xMRWj544KrPSV0VBdSpa4mM78SubkRcQh5yAm3_A2Qc,8441
-tensorflow_federated/python/core/api/intrinsics.py,sha256=y5sVAQLWy4s3G28V_5cIlG2ARXdHliglBTdHqGLsZ7Y,16053
-tensorflow_federated/python/core/api/placements.py,sha256=WKQ4qYrSPuHMTlDfJL3Y2OhM_2GInxgxB2D6mRr9kko,1091
+tensorflow_federated/python/core/api/intrinsics.py,sha256=sXQiLfKaUWmW-CgkRmh_dtDqo9wpnA3Bd3pp4TRSAfA,16171
+tensorflow_federated/python/core/api/placements.py,sha256=PkcWtp7nJqL4-qB_EkXfL_hz_JH0Ele5XP6qNCxtTbY,1100
 tensorflow_federated/python/core/api/typed_object.py,sha256=4jz3AAE9VS60N3iM768uvVWxlNgEOSUpR0aUq6ZgnZY,1127
 tensorflow_federated/python/core/api/value_base.py,sha256=MOXburVRTmAgeiETv65T_LGvK4LJdNF-HZSejCdmiJw,2977
 tensorflow_federated/python/core/api/values.py,sha256=8eOO3D7S_OZv14MHoMl3xuMb2oFyrji29Zift6buxTw,3047
-tensorflow_federated/python/core/framework/__init__.py,sha256=UkgdPP5UipfkrQKgqgPxlpIFrjjtynVOFm2gU0bwfAM,7452
+tensorflow_federated/python/core/backends/__init__.py,sha256=SndV8HFWnRxZrRf1gBdpNddkj1ULBoDcsR50u4xTMLQ,944
+tensorflow_federated/python/core/backends/mapreduce/__init__.py,sha256=1Y0wIu4xx8jH3mwBhATN4oxvb-etX8F-_tE6uRfwDJs,2003
+tensorflow_federated/python/core/backends/mapreduce/canonical_form.py,sha256=nzKn-pT_h8o5cvl9W1q8CMvL8nBVukEzUfNcRStuGrU,19822
+tensorflow_federated/python/core/backends/mapreduce/canonical_form_utils.py,sha256=mlCZD6Oi7whEAfUR2ux2kii6VKs1ZwpZFnjT5x9bp5w,32232
+tensorflow_federated/python/core/backends/mapreduce/transformations.py,sha256=lgbAHaAnb8OoPtuJ5_XftbCvyKOOEQgHi8577smrc_I,52094
+tensorflow_federated/python/core/framework/__init__.py,sha256=GBYRO0BFjHCCTiW-mYceVkRqfwWMVeMMeqZs0EmmZz8,7937
 tensorflow_federated/python/core/impl/__init__.py,sha256=_oxRNbqrDcBIqLAx8I_lWPUKmSLQAjssXgUrdBlI9uo,694
-tensorflow_federated/python/core/impl/compiled_computation_transforms.py,sha256=XsCZ27S-RBNpVU4MUpVShe_BZZO5jsIlQpXCeolVdBc,53517
-tensorflow_federated/python/core/impl/compiler_pipeline.py,sha256=bSGlDsyv4hYU8jksdN64D74ZGaCp5rQJOHybcVpCQsM,3738
-tensorflow_federated/python/core/impl/computation_building_block_utils.py,sha256=DsKKcLtqHI4ht7c8mfK4tvDnZ2H-vyiEPifA-9zTTUk,1790
-tensorflow_federated/python/core/impl/computation_building_blocks.py,sha256=ZsiFQo16rey7QgGxH1Wwl2Xslz8_3ay8INteUSllZ1k,51156
-tensorflow_federated/python/core/impl/computation_constructing_utils.py,sha256=wBjz_zSd4gis-WXj8_9wmStUTNQo_FnNLM5UocCDTJM,68812
-tensorflow_federated/python/core/impl/computation_impl.py,sha256=P6F2ALKnTC1IEWFkR7LmLJHgXgwgJxFDXacVUzaaeO8,3569
-tensorflow_federated/python/core/impl/computation_wrapper.py,sha256=CYc_WBlHU_YpsIOYHnUNuFvoQcfj89dJkR-e2myCcjg,18681
-tensorflow_federated/python/core/impl/computation_wrapper_instances.py,sha256=daaG-gOlqvcRJj0miXgDvhf1_rvIP3eiZ4-irJkYr8k,4103
-tensorflow_federated/python/core/impl/concurrent_executor.py,sha256=u0cXLdsmLyvDQsvIeRdF2p4NTi7XsIX1ijlgctnG2II,2676
+tensorflow_federated/python/core/impl/caching_executor.py,sha256=Ej-kBOOQ4qO6VqptbT_UId_4GllVKi89aRuviDSDAGw,13050
+tensorflow_federated/python/core/impl/compiled_computation_transforms.py,sha256=S8ICBxUvaMtcCO1ybKZf_KpJax8klyBeWR6CtJhp96k,53456
+tensorflow_federated/python/core/impl/compiler_pipeline.py,sha256=zHNfKaN03C2VxZNZSXyXI5yVWOfZWqgCi8ChKuFXFkU,4129
+tensorflow_federated/python/core/impl/composite_executor.py,sha256=FhlO-F6C7MwkX7EUBAN3P0Z-RvCvDHur-q7iidKpWR8,24425
+tensorflow_federated/python/core/impl/computation_impl.py,sha256=v3kMx2R7VPSjjWaJL2AnAgHxJwQTfg1abg6St8cA-MU,3584
+tensorflow_federated/python/core/impl/computation_wrapper.py,sha256=UwwG1dALoYFTvuRxT8-DoJIdKA_ely8eyX1RfImP790,18687
+tensorflow_federated/python/core/impl/computation_wrapper_instances.py,sha256=Ingd_B8g1JTuqJRpEfSVWrwYUxDcJMK2lcIoJxw-MlU,4094
+tensorflow_federated/python/core/impl/concurrent_executor.py,sha256=p9_C14mLhr-XI7f0Zam0uNPT_5WqhYJQgZHJzKgw_9U,2761
 tensorflow_federated/python/core/impl/context_base.py,sha256=61hygV9_v2p5ucihCkZA17Mtm9uCd-SQ1-FiUiJRFvw,3656
 tensorflow_federated/python/core/impl/context_stack_base.py,sha256=ycJWudpAHAE9B0ZH07XtSu6e2PzerJFfHCwgq3mhG5A,1853
 tensorflow_federated/python/core/impl/context_stack_impl.py,sha256=FWMiwhjCvGy7Em7aTr2c1S8k48r7aqWwyWPbYtvldbo,2458
-tensorflow_federated/python/core/impl/dtype_utils.py,sha256=2H0ju4OLW7l64CtV2yg4NPl7_bpKPqLdyk_fATO-J5M,954
-tensorflow_federated/python/core/impl/eager_executor.py,sha256=nxdy1556hyvo8pK7VrSzIhWP9-6ayYZ4DYd7utHVrpQ,18424
-tensorflow_federated/python/core/impl/execution_context.py,sha256=scbtki8vv95U0bEKOeugS2yvVn17srrlKuC6JRvHz3k,4421
+tensorflow_federated/python/core/impl/eager_executor.py,sha256=tuG1AFa2pLFZnohNmmmdZUxO2leV7Mj-tOvzMc500m8,18657
+tensorflow_federated/python/core/impl/execution_context.py,sha256=9nijRHVVXtgTd5ProEZFNiC1btxFKztNwfGMRST0WVY,5923
 tensorflow_federated/python/core/impl/executor_base.py,sha256=wDOvOgiH_QzcMmHgleiJgejIq7uQE1IZFvedpFazyi4,3960
-tensorflow_federated/python/core/impl/executor_service.py,sha256=weAuCl6sqEJqpWCwKpGYzT43Qu63sgVAoIDCUU78BN8,8354
-tensorflow_federated/python/core/impl/executor_service_utils.py,sha256=H9G4PrjDFLkZFhHQZ5qwVmCqurCNzU-UDaNtuw-V7gY,8047
-tensorflow_federated/python/core/impl/executor_stacks.py,sha256=QXlKUWFz-a8QR8oLEhwQdBnrkEdO9svZ5K70ZfYeCwo,2159
+tensorflow_federated/python/core/impl/executor_service.py,sha256=ubOvEYOd6Qu_yWWrgXZa2lGhWF9noimY23KbdBE6jPM,9352
+tensorflow_federated/python/core/impl/executor_service_utils.py,sha256=maiS9PUg8U7Z4yBwb4Gl8IQ7K-l9Obn9nJ3lAnFjIXA,12722
+tensorflow_federated/python/core/impl/executor_stacks.py,sha256=LOP77iAivKaa-ljczCoh18YCi5f1wAap7kJA8hSkYdQ,7945
+tensorflow_federated/python/core/impl/executor_utils.py,sha256=2S_aMlBGrfVh8uzyMmO2-D-M4ehOSYeGA_32Qob7Iz0,11102
 tensorflow_federated/python/core/impl/executor_value_base.py,sha256=HBlnYILGQDKWtlJD_iwbd0nsuG4DpWHOvwTU_qurSos,1549
-tensorflow_federated/python/core/impl/federated_computation_context.py,sha256=XWZAfQrBibOAuaZTjYpfatZLDHYz_ZyZ8yLPic1nYRU,3461
-tensorflow_federated/python/core/impl/federated_computation_utils.py,sha256=ZleAyl2_PMPrl7l_X3PY9mPi0ry65LEoHjOE4iXDo5E,3825
-tensorflow_federated/python/core/impl/federated_executor.py,sha256=MCoNZIfPB2xHvWSU5gsdM7pMjTMSMwKLyRZB6AjAe7g,32327
-tensorflow_federated/python/core/impl/function_utils.py,sha256=7POsZ8B5e2hQFw5GQF7BZ9fgCfF-KYiQcuUyeYNhHt4,28783
-tensorflow_federated/python/core/impl/graph_utils.py,sha256=Yr3wPTq5qRuTIjYNRmpRjT6ensvSB5DZrVMtOLnwSPU,54128
-tensorflow_federated/python/core/impl/intrinsic_bodies.py,sha256=h0JWHAbCr27hX-ZHe9qQK5yQl5rlL8EC_fuQSB9iF2k,13656
-tensorflow_federated/python/core/impl/intrinsic_defs.py,sha256=BvjXO7177xudioSzldm2JhsjbQ8kIzmL8dGz5G_rn58,19970
-tensorflow_federated/python/core/impl/intrinsic_factory.py,sha256=i3eZTQnV7NBJVHElEnKZZ2pGbGZRxcLbfs1MHVDC7uY,26457
-tensorflow_federated/python/core/impl/intrinsic_reductions.py,sha256=VyIZBIirPZsO8bo8CWIKXryTMyHC8OjAa4aZjHQD2qs,2327
-tensorflow_federated/python/core/impl/intrinsic_utils.py,sha256=wwLhwT4Zk2jGKeXcStOrqTuXF3rP9cmDNF7JeZQ2FWE,12435
-tensorflow_federated/python/core/impl/lambda_executor.py,sha256=zhMjwYanv77ji2KFmxrh35yU_deBZnQpRfGvPDAQ51s,18827
-tensorflow_federated/python/core/impl/placement_literals.py,sha256=zJbzGPMFYTijGmb115ajMNArPebtk2O7oNk5-hZUU8o,2525
-tensorflow_federated/python/core/impl/reference_executor.py,sha256=dMFJFyqtKFzpghsCAMhAC99z1fkksgHVuLuNC6L5g5w,51963
-tensorflow_federated/python/core/impl/remote_executor.py,sha256=sk8q1Sm20ASJN1CtYqv-RnVzkR3_o05j6gOUJ8SGvCM,5044
-tensorflow_federated/python/core/impl/set_default_executor.py,sha256=J1Oh_m5lXjskH23h7COJd7KJZsCZv8o9qVN1zDcXwX4,1519
-tensorflow_federated/python/core/impl/tensorflow_deserialization.py,sha256=8S1Ri_lDIE2KeM3qUykd0fVzmGv9LGbGxxTlu-kbXm4,6154
-tensorflow_federated/python/core/impl/tensorflow_serialization.py,sha256=HRW2vvZ9TDROBJ6xzrRFZiLtWNMwnnXm4aEOgTMJNkA,14775
+tensorflow_federated/python/core/impl/federated_computation_context.py,sha256=jFZ1niW-bsJlVBuZSjmxwsnWfU6f9g8rmx2zyLWTeR0,3446
+tensorflow_federated/python/core/impl/federated_computation_utils.py,sha256=-9mX9vlT2impplEmG7YYwbVRZnEnaOAuvpsD9u2qlYs,3959
+tensorflow_federated/python/core/impl/federated_executor.py,sha256=qgKWc5TnuWOv8p1BzmcqMsaMacKWEO2T72lrsJE9FTc,29494
+tensorflow_federated/python/core/impl/intrinsic_bodies.py,sha256=fXf_efqQI5YyNp3QiBrIbvtFSfRDvPiTBlYQ2Nqdu4o,14247
+tensorflow_federated/python/core/impl/intrinsic_factory.py,sha256=adhxJaPCXzwxXMKuoB4lxxgtk48h9tXwZu2MPIoQu0g,26662
+tensorflow_federated/python/core/impl/intrinsic_reductions.py,sha256=IweQJukhBEfwNO4pkWvdjaGHv6ZrFkpRnv3RwI7GbzU,2262
+tensorflow_federated/python/core/impl/lambda_executor.py,sha256=C3eLvoGJOL85ZqcNTkivSkP_1--UbJ-r2l8LS84PXnU,18841
+tensorflow_federated/python/core/impl/reference_executor.py,sha256=KDaEeK4t4IKy46VfquG7sDsxpyfMqXfMdJM1YIyXlDI,50372
+tensorflow_federated/python/core/impl/remote_executor.py,sha256=kXiY5e37iYAJjXbVei_8ILc3pe3rVke5ndyz79WpPMI,10769
+tensorflow_federated/python/core/impl/runtime_utils.py,sha256=TinhQHyEe1geCmak2PqjIPgT5j0xgS7C8BDRZ9YJyUw,3617
+tensorflow_federated/python/core/impl/set_default_executor.py,sha256=IXTgUjww7T2ALCQFN8KXblIr83rxnCc-bBbg1Ve4uHA,1910
+tensorflow_federated/python/core/impl/tensorflow_deserialization.py,sha256=97erOkjXKnzrjTTB2XuJ7Uf2Hi1dAovQT9RGXXTybQg,6218
+tensorflow_federated/python/core/impl/tensorflow_serialization.py,sha256=tplqdziki0VsHBSG2Uanvzh1kIfCGMv4cp2A2d1-Zw4,18601
 tensorflow_federated/python/core/impl/tf_computation_context.py,sha256=-aJ54xYrwyTJ67owizZ_9ZupKu0-6wJrcr2mx-v6EgE,2177
-tensorflow_federated/python/core/impl/transformation_utils.py,sha256=aNz0x94YfeGm_BqlDkKWQ_x69kUnnLyjsQKOHmxmR6U,41804
-tensorflow_federated/python/core/impl/transformations.py,sha256=qffOp_K-jRCIqK1usVGT92Y7IvTlktABzbXACISr07Q,69203
-tensorflow_federated/python/core/impl/transforming_executor.py,sha256=6nUVZPdMdV41hAQ-mwBaawMe-GwAnPnLgTiP3Eb9PZs,3568
-tensorflow_federated/python/core/impl/type_constructors.py,sha256=cG_kWoMXahcgBgxL6BO94HXO9-wdx0ohSIfOQ0p-Kw8,3399
-tensorflow_federated/python/core/impl/type_serialization.py,sha256=ElKFBNQZQ0PfsPzzgHtxm7ecYGL5Kn3bGcUtSWTMLdg,6574
-tensorflow_federated/python/core/impl/type_utils.py,sha256=SVI-7drWbg9GIOBY1cegmw4AQH5tSJQISGyzry5oas8,59467
-tensorflow_federated/python/core/impl/value_impl.py,sha256=OraZWxXUIenrvLkSAmYSihu4IdUK2ETjKeXcfWQppY8,17373
-tensorflow_federated/python/core/impl/value_utils.py,sha256=NA7gnT4o3_ifmDTH7qtr99-ONjilqBE6ldKhs-UJrjY,2653
-tensorflow_federated/python/core/utils/__init__.py,sha256=3i6O-t2gEaMJQV3ZHNkigKwQX-nZsstzNn8WIFdFtfA,2143
-tensorflow_federated/python/core/utils/computation_utils.py,sha256=FskjukHxylbIaWn4jTYwW8WMsVE8rlTIPQJPeCP_ReM,11655
+tensorflow_federated/python/core/impl/transformations.py,sha256=vk--I67JH4RMIrYjRmbS8EiVx8UxHFxbU4PH0HffwaA,71861
+tensorflow_federated/python/core/impl/transforming_executor.py,sha256=Z-Su5mS9yAYaD_DjgSREXRJKS0JleN4zIqIqh8Rp9s4,3483
+tensorflow_federated/python/core/impl/type_utils.py,sha256=R7_VrW5rxci5z1R70Nd75rY7hMadddu5l2K8exUFvZU,58436
+tensorflow_federated/python/core/impl/value_impl.py,sha256=EDuykaMn2QnzZuPmU4Q1vWua6WE5zT-UoN4Kqa20xS4,16930
+tensorflow_federated/python/core/impl/value_transformations.py,sha256=KckRjtKbjNeBeoV-vIexHtCCrQlWY0MA9j4DfRB4HB0,4388
+tensorflow_federated/python/core/impl/value_utils.py,sha256=WiSZBdr40v5pcmupknOJlsqhljQeWWz8HRbmxxl36Xg,3451
+tensorflow_federated/python/core/impl/compiler/__init__.py,sha256=anWWDQNP86PB8Dq84zcV1Tppw_Qslk-4IwSP4DRcQK0,618
+tensorflow_federated/python/core/impl/compiler/building_block_analysis.py,sha256=qbofTITmA9zsud379FS88lpNZTob9t-Mz3cctZGgRIc,3367
+tensorflow_federated/python/core/impl/compiler/building_block_factory.py,sha256=hI233Xh2sSGeclIbH7Mewl9fFjLpUXOCi7RF9kqDFBQ,75043
+tensorflow_federated/python/core/impl/compiler/building_blocks.py,sha256=_d8UfiMQ6klXrhohQM5LIrIqBZuW5C5UnXrIn4_LYpY,51222
+tensorflow_federated/python/core/impl/compiler/intrinsic_defs.py,sha256=QQ0iPK2Q_D1igXDvIdtIOFa6PdZA3fQlqdaa5ACSY84,19648
+tensorflow_federated/python/core/impl/compiler/placement_literals.py,sha256=zJbzGPMFYTijGmb115ajMNArPebtk2O7oNk5-hZUU8o,2525
+tensorflow_federated/python/core/impl/compiler/proto_transformations.py,sha256=YUzg82EkYTz8qlyBsCP2leSNRnx_-zXRFxjKLSNqTRA,3070
+tensorflow_federated/python/core/impl/compiler/transformation_utils.py,sha256=5XQTJR7U5Mg3R1ED_Urfmu6YhOARcSn2b-dk5Rga7DU,41536
+tensorflow_federated/python/core/impl/compiler/tree_analysis.py,sha256=irfz-6J4O_GpVZr-7BEZfe08mjAbN9EYKSWuS8BSYp8,11927
+tensorflow_federated/python/core/impl/compiler/type_factory.py,sha256=cG_kWoMXahcgBgxL6BO94HXO9-wdx0ohSIfOQ0p-Kw8,3399
+tensorflow_federated/python/core/impl/compiler/type_serialization.py,sha256=O8LPWVjyw4J5RZP2b_aZK5bc9jAGVO9ns8c_ROld6n8,6585
+tensorflow_federated/python/core/impl/utils/__init__.py,sha256=anWWDQNP86PB8Dq84zcV1Tppw_Qslk-4IwSP4DRcQK0,618
+tensorflow_federated/python/core/impl/utils/function_utils.py,sha256=VbwJ7zF5huvCFmz3YExVbCy2hcroZe8tWIUVWfFJIFE,29687
+tensorflow_federated/python/core/impl/utils/tensorflow_utils.py,sha256=VbyBNn-hASuwvHhDNjtGNpVKIqXqV0ojxUiYukmq3vw,52057
+tensorflow_federated/python/core/utils/__init__.py,sha256=49JnrTDKFhp4qroFoAZswhrfKM3y5QZP9rk1KO_Ab5c,2607
+tensorflow_federated/python/core/utils/computation_utils.py,sha256=Y49f0Z4bl6TsBiRSuGwaJKAwJrfgZuowm1VcHM7_7OY,11596
+tensorflow_federated/python/core/utils/differential_privacy.py,sha256=ovVXgn3xZ1p64ZUj3hc67KSh7KXh7QcpyjN-aBMcRFM,7337
+tensorflow_federated/python/core/utils/encoding_utils.py,sha256=YuHukbcE9w3yuKq_jQhF_H2UVBh5bV2Jp3G7vgV6hyk,18192
 tensorflow_federated/python/core/utils/federated_aggregations.py,sha256=uIssLKdju5QZGAnM3pmawyV7ZSPnof0bZwbWeseyxuY,5076
-tensorflow_federated/python/core/utils/tf_computation_utils.py,sha256=YChtafd4qVoCWLv5xFkaLO2Qw82iEKaQm7C-EEzjFCk,5122
-tensorflow_federated/python/examples/__init__.py,sha256=PuAd8tRBzvtTxsmkCavfROwpPrfnt2fW7XJRN2d1c40,618
-tensorflow_federated/python/examples/mnist/__init__.py,sha256=bgdrG-zJnphZWMaR4xUS8GAHy_K5gVtlCWPSnL8mLmA,969
-tensorflow_federated/python/examples/mnist/models.py,sha256=JJEPeJ9N6Px0v8S6nPVDS5CU-V3EAH7N2Z4W6nClhtU,4464
+tensorflow_federated/python/core/utils/tf_computation_utils.py,sha256=Snc0wJTQvWanKnr1Rzp_PyiIpu0X-fKNfLUkhplZVbQ,5452
 tensorflow_federated/python/learning/__init__.py,sha256=KZhBGxc-H024YA1cpM1zB3JtS8qHlUb7dSsIKgRw8lM,2084
-tensorflow_federated/python/learning/federated_averaging.py,sha256=q-GPih9Bsmxxk1IKFNWY47FJ7hhxwr9zaJc2lHoabcU,6929
+tensorflow_federated/python/learning/federated_averaging.py,sha256=23yihPUcyfXf2lkIS6cmMQqHUXA0Ggn41dH7sCM94CU,7035
 tensorflow_federated/python/learning/federated_evaluation.py,sha256=9ajHu6vrppwqAACC4QINSZBuqdkY4RYOZfQKKu7SGyA,3125
 tensorflow_federated/python/learning/federated_sgd.py,sha256=VpRC4v_4DT-OBy9sh2c0fbSnh-Ef-ZamRkH9k1Vs9L0,8002
-tensorflow_federated/python/learning/keras_utils.py,sha256=sjxJeAQn0jBTht9ipz3v31KiGkWbCoL_kgWKM7K9Eso,19168
-tensorflow_federated/python/learning/model.py,sha256=CvXWjCRdkhy3LW20dGlhCUIM6ISL0UitCJguPebVe8M,8542
+tensorflow_federated/python/learning/keras_utils.py,sha256=j0RAaazdUdztgS3cv8XJOWO2YxJ5elPEODrOKmXfsno,19216
+tensorflow_federated/python/learning/model.py,sha256=27ZZXum3FD6AEZSnbr-JjFdFTf6ZVsYZLPoNJglv8jI,8645
 tensorflow_federated/python/learning/model_utils.py,sha256=-EvbX83E9-bidrL7-zGtGfXoScOif-x5SYITrxnhkyk,6303
-tensorflow_federated/python/learning/framework/__init__.py,sha256=17lb88HVAnlb7NxwbFSRN1ymvdjFsqMqvEZaP2inJTI,1544
+tensorflow_federated/python/learning/framework/__init__.py,sha256=G8MA2I5IS6cIXASLcy-UhXeSY1hR44Ojs6TUyne6XMc,2196
+tensorflow_federated/python/learning/framework/encoding_utils.py,sha256=DwF9HeCjztf1p-J6asVZGGkxkZy1SXvlKcBO0B1vDCA,4814
 tensorflow_federated/python/learning/framework/optimizer_utils.py,sha256=xfxBsNLSNBle-xsxPQQzvfU-ZgBXdXeziX9f-a8CW6A,18608
-tensorflow_federated/python/simulation/__init__.py,sha256=Em585KqOUoAx-dAH7HcDviuITXWp7H98itEJ9lrei_g,1538
-tensorflow_federated/python/simulation/client_data.py,sha256=kp5Ml61c15nfqjpkaHK2oF8sS3i3WPweBVL_EmXgibs,3837
-tensorflow_federated/python/simulation/file_per_user_client_data.py,sha256=yzs5dGSC2ff83gbvbi2FFsL6K-0MTtbGZxf_0EWN7cE,3469
-tensorflow_federated/python/simulation/from_tensor_slices_client_data.py,sha256=O-DS8qCW3RyZQCRa46-26joJWxkDZxpfpVyMcnDB0vI,2269
-tensorflow_federated/python/simulation/hdf5_client_data.py,sha256=drYlcpZeWgOMlj6YrVMKekAI6-8XkK4Q8qjPEGtqg3c,3080
+tensorflow_federated/python/simulation/__init__.py,sha256=83ByRAfCvRr2WzvzLyh2gd7zRFsiYlgZ8mPO68RCBhU,2170
+tensorflow_federated/python/simulation/client_data.py,sha256=IXGyVITl_n8yEIoRUx03kM_Waf7FlSkSKnnOvDWFL0M,6416
+tensorflow_federated/python/simulation/file_per_user_client_data.py,sha256=Ig78SG0ghpWH3KvP7JiEavHs8FF04PX8gG_JKp4t_vU,3543
+tensorflow_federated/python/simulation/from_tensor_slices_client_data.py,sha256=L6JdzuAfarqvqMYGXRSxK6dUdUwJDzpW7N1A8WVgk10,2315
+tensorflow_federated/python/simulation/hdf5_client_data.py,sha256=NqDW9QFqcG8uVa9jy27k7gpsYfitLk9wKcOHjg0RS-s,3205
+tensorflow_federated/python/simulation/server_utils.py,sha256=-bQH0eVPv4J6KNLVijzfeyzJ34ckpFYu7ioxZF3-GVQ,2931
 tensorflow_federated/python/simulation/transforming_client_data.py,sha256=CZe2cGV0ahPOzcfZOldt4BM3AzSYt0xR6KvPB2DHy6c,5863
-tensorflow_federated/python/simulation/datasets/__init__.py,sha256=l2VVHtQ0k0P-OacNyS5L7H8hu8mNlM4Acgt9bixPg8w,1031
-tensorflow_federated/python/simulation/datasets/emnist/__init__.py,sha256=oZjJt1tpqEeFNi1mHJKJumpF_q24zZ64t-ZonCsLUsY,1172
-tensorflow_federated/python/simulation/datasets/emnist/load_data.py,sha256=YWG1_Bo7huQBwqOtUh69E44rVoUF-qHko9pobSgQwaI,9992
-tensorflow_federated/python/simulation/datasets/emnist/synthetic.py,sha256=az3Pk2ymkl1cIydCOb5deBIAhoITOQ10cVJBDFpxbgQ,19403
-tensorflow_federated/python/simulation/datasets/shakespeare/__init__.py,sha256=sZoOSE_UBMV0WnQFEXnN_V3kIncQVUKac4GCZqOch2w,960
-tensorflow_federated/python/simulation/datasets/shakespeare/load_data.py,sha256=RdUcDmmw43V_N4nX3ygpQTNn5_TbsrxPBofwmh_zT5Q,3051
+tensorflow_federated/python/simulation/datasets/__init__.py,sha256=QVfS7_CuSr-SEeUfyDqFY23Bug-ve8PtVdLHkwNV6Hw,1527
+tensorflow_federated/python/simulation/datasets/dataset_utils.py,sha256=KyZ-8rnWp-5DXFy4iwSwXaGF4ZJB_I1eWkvT86l5w2k,3725
+tensorflow_federated/python/simulation/datasets/emnist.py,sha256=3mq4izAEVEslWDr0ElwBSuyFc4dez9k4cfyltBGR9TE,29071
+tensorflow_federated/python/simulation/datasets/shakespeare.py,sha256=B6MQJllQ_tXglFG09WOXKYyEx3MHhKkpY7-RT_6TqY0,3051
+tensorflow_federated/python/simulation/datasets/stackoverflow.py,sha256=bnE_PWmnnPtedHgmalNVK7tt63ATYCE-DgYW1CYRXgk,5688
+tensorflow_federated/python/simulation/models/__init__.py,sha256=JkihZlbjIdFHRWIOmL5-KW3E5n3S0M1Ab79vQtHbKiA,929
+tensorflow_federated/python/simulation/models/mnist.py,sha256=8I3eMIj6eDXUBA5cTgReKikANC_aLdFfk6VQvsSqDGU,4228
 tensorflow_federated/python/tensorflow_libs/__init__.py,sha256=PuAd8tRBzvtTxsmkCavfROwpPrfnt2fW7XJRN2d1c40,618
 tensorflow_federated/python/tensorflow_libs/graph_keys.py,sha256=KlGpGJFELGlDMxi8jHaH558NHfmqhMbtzXYm6NXUBh0,1167
 tensorflow_federated/python/tensorflow_libs/graph_merge.py,sha256=-IojaRmNTQ9sfCUuMrTNjk3DOI4skpGcmGLNeOFyKSE,13608
-tensorflow_federated/python/tensorflow_libs/tensor_utils.py,sha256=85nilPwPYYATgQKMnJufzm14LEjJJwloK2JKStYdnRw,5818
-tensorflow_federated-0.7.0.dist-info/METADATA,sha256=r6A32ENYRnSsJNqOgILbWrCU8vca9f5ffr9SGFtxEnI,3214
-tensorflow_federated-0.7.0.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
-tensorflow_federated-0.7.0.dist-info/top_level.txt,sha256=UoTusg-5ICHXomvSyLgvaAielzUm8kchKxID9m8WrJk,21
-tensorflow_federated-0.7.0.dist-info/RECORD,,
+tensorflow_federated/python/tensorflow_libs/nest.py,sha256=-VfkG3r53oOrxkHyq5LH5ffcyWZTNsoxg_TJB_9TSCU,44791
+tensorflow_federated/python/tensorflow_libs/tensor_utils.py,sha256=FN2VuKko19Jn-Rk6y3GvbL-r0QQd4hfYvpFBL86D-c0,5139
+tensorflow_federated-0.9.0.dist-info/METADATA,sha256=Kb_919iqdQRMLk_5Z2eaJl6jda12qL7uE06OUJNmWiE,3448
+tensorflow_federated-0.9.0.dist-info/WHEEL,sha256=8zNYZbwQSXoB9IfXOjPfeNwvAsALAjffgk27FqvCWbo,110
+tensorflow_federated-0.9.0.dist-info/top_level.txt,sha256=UoTusg-5ICHXomvSyLgvaAielzUm8kchKxID9m8WrJk,21
+tensorflow_federated-0.9.0.dist-info/RECORD,,
```

